# Comparing `tmp/socket.d-2.4.12.tar.gz` & `tmp/socket.d-2.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socket.d-2.4.12.tar", last modified: Thu Apr 25 05:57:11 2024, max compression
+gzip compressed data, was "socket.d-2.4.13.tar", last modified: Mon Apr 29 00:56:45 2024, max compression
```

## Comparing `socket.d-2.4.12.tar` & `socket.d-2.4.13.tar`

### file list

```diff
@@ -1,156 +1,157 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.194645 socket.d-2.4.12/
--rw-r--r--   0 noear      (501) staff       (20)      553 2024-04-25 05:57:11.193563 socket.d-2.4.12/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.12/README.md
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-25 05:57:11.194954 socket.d-2.4.12/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      873 2024-04-25 05:32:39.000000 socket.d-2.4.12/setup.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.192385 socket.d-2.4.12/socket.d.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      553 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     5114 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/zip-safe
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.111688 socket.d-2.4.12/socketd/
--rw-r--r--   0 noear      (501) staff       (20)     2710 2024-04-25 05:32:39.000000 socket.d-2.4.12/socketd/SocketD.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.112958 socket.d-2.4.12/socketd/broker/
--rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/broker/BrokerFragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)     3571 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/broker/BrokerListener.py
--rw-r--r--   0 noear      (501) staff       (20)     3124 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/broker/BrokerListenerBase.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/broker/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.115033 socket.d-2.4.12/socketd/cluster/
--rw-r--r--   0 noear      (501) staff       (20)     2757 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/cluster/ClusterClient.py
--rw-r--r--   0 noear      (501) staff       (20)     2654 2024-04-24 03:25:43.000000 socket.d-2.4.12/socketd/cluster/ClusterClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)     1995 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/cluster/LoadBalancer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/cluster/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.115813 socket.d-2.4.12/socketd/exception/
--rw-r--r--   0 noear      (501) staff       (20)      654 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/exception/SocketDExecption.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.116080 socket.d-2.4.12/socketd/transport/
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.128797 socket.d-2.4.12/socketd/transport/client/
--rw-r--r--   0 noear      (501) staff       (20)     1714 2024-04-24 03:25:43.000000 socket.d-2.4.12/socketd/transport/client/Client.py
--rw-r--r--   0 noear      (501) staff       (20)     3584 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd/transport/client/ClientBase.py
--rw-r--r--   0 noear      (501) staff       (20)     6490 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd/transport/client/ClientChannel.py
--rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientConfigHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientConnectHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientConnectorBase.py
--rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientHandshakeResult.py
--rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-24 04:28:16.000000 socket.d-2.4.12/socketd/transport/client/ClientHeartbeatHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     1047 2024-04-24 03:25:43.000000 socket.d-2.4.12/socketd/transport/client/ClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.144586 socket.d-2.4.12/socketd/transport/core/
--rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Asserts.py
--rw-r--r--   0 noear      (501) staff       (20)     2476 2024-04-24 03:33:21.000000 socket.d-2.4.12/socketd/transport/core/Channel.py
--rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/ChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/ChannelInternal.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/ChannelSupporter.py
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/Codec.py
--rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Config.py
--rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Costants.py
--rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Entity.py
--rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/EntityMetas.py
--rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Flags.py
--rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/FragmentAggregator.py
--rw-r--r--   0 noear      (501) staff       (20)      832 2024-04-24 03:33:21.000000 socket.d-2.4.12/socketd/transport/core/FragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Frame.py
--rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Frames.py
--rw-r--r--   0 noear      (501) staff       (20)     2526 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/HandshakeDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      160 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/IdGenerator.py
--rw-r--r--   0 noear      (501) staff       (20)      510 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/Listener.py
--rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Message.py
--rw-r--r--   0 noear      (501) staff       (20)      953 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/Processor.py
--rw-r--r--   0 noear      (501) staff       (20)     1953 2024-04-24 04:28:16.000000 socket.d-2.4.12/socketd/transport/core/Session.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.147704 socket.d-2.4.12/socketd/transport/core/codec/
--rw-r--r--   0 noear      (501) staff       (20)     1346 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/codec/Buffer.py
--rw-r--r--   0 noear      (501) staff       (20)      777 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/codec/ByteBufferCodecReader.py
--rw-r--r--   0 noear      (501) staff       (20)      666 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/codec/ByteBufferCodecWriter.py
--rw-r--r--   0 noear      (501) staff       (20)     4634 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/codec/CodecDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/codec/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.151225 socket.d-2.4.12/socketd/transport/core/entity/
--rw-r--r--   0 noear      (501) staff       (20)     3783 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/entity/EntityDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      800 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/entity/FileEntity.py
--rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/entity/MessageBuilder.py
--rw-r--r--   0 noear      (501) staff       (20)     2045 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/entity/MessageDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/entity/StringEntity.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/entity/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.152976 socket.d-2.4.12/socketd/transport/core/fragment/
--rw-r--r--   0 noear      (501) staff       (20)     2179 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/fragment/FragmentAggregatorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     3371 2024-04-24 03:33:21.000000 socket.d-2.4.12/socketd/transport/core/fragment/FragmentHandlerBase.py
--rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/fragment/FragmentHandlerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/fragment/FragmentHolder.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/fragment/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.156451 socket.d-2.4.12/socketd/transport/core/impl/
--rw-r--r--   0 noear      (501) staff       (20)     2358 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/impl/ChannelBase.py
--rw-r--r--   0 noear      (501) staff       (20)     7281 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd/transport/core/impl/ChannelDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     6565 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd/transport/core/impl/ConfigBase.py
--rw-r--r--   0 noear      (501) staff       (20)     8216 2024-04-25 04:57:58.000000 socket.d-2.4.12/socketd/transport/core/impl/ProcessorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/impl/SessionBase.py
--rw-r--r--   0 noear      (501) staff       (20)     4625 2024-04-24 04:28:16.000000 socket.d-2.4.12/socketd/transport/core/impl/SessionDefault.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/impl/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.160571 socket.d-2.4.12/socketd/transport/core/listener/
--rw-r--r--   0 noear      (501) staff       (20)     2384 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/EventListener.py
--rw-r--r--   0 noear      (501) staff       (20)     1297 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/PathListener.py
--rw-r--r--   0 noear      (501) staff       (20)     1254 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/PipelineListener.py
--rw-r--r--   0 noear      (501) staff       (20)      406 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/RouteSelector.py
--rw-r--r--   0 noear      (501) staff       (20)      559 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/RouteSelectorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      473 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/SimpleListener.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/listener/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.162205 socket.d-2.4.12/socketd/transport/server/
--rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/server/Server.py
--rw-r--r--   0 noear      (501) staff       (20)     2629 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/server/ServerBase.py
--rw-r--r--   0 noear      (501) staff       (20)     1652 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/server/ServerConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/server/ServerProvider.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/server/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.169510 socket.d-2.4.12/socketd/transport/stream/
--rw-r--r--   0 noear      (501) staff       (20)      876 2024-04-24 05:00:55.000000 socket.d-2.4.12/socketd/transport/stream/RequestStream.py
--rw-r--r--   0 noear      (501) staff       (20)      597 2024-04-24 03:00:26.000000 socket.d-2.4.12/socketd/transport/stream/SendStream.py
--rw-r--r--   0 noear      (501) staff       (20)      850 2024-04-24 03:25:43.000000 socket.d-2.4.12/socketd/transport/stream/Stream.py
--rw-r--r--   0 noear      (501) staff       (20)      295 2024-04-24 03:32:44.000000 socket.d-2.4.12/socketd/transport/stream/StreamManger.py
--rw-r--r--   0 noear      (501) staff       (20)     1068 2024-04-24 03:34:35.000000 socket.d-2.4.12/socketd/transport/stream/StreamMangerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      823 2024-04-24 03:25:43.000000 socket.d-2.4.12/socketd/transport/stream/SubscribeStream.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/stream/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.174044 socket.d-2.4.12/socketd/transport/stream/impl/
--rw-r--r--   0 noear      (501) staff       (20)     1855 2024-04-24 09:22:27.000000 socket.d-2.4.12/socketd/transport/stream/impl/RequestStreamImpl.py
--rw-r--r--   0 noear      (501) staff       (20)      734 2024-04-24 02:55:55.000000 socket.d-2.4.12/socketd/transport/stream/impl/SendStreamImpl.py
--rw-r--r--   0 noear      (501) staff       (20)     2381 2024-04-24 09:22:27.000000 socket.d-2.4.12/socketd/transport/stream/impl/StreamBase.py
--rw-r--r--   0 noear      (501) staff       (20)     1279 2024-04-24 04:31:37.000000 socket.d-2.4.12/socketd/transport/stream/impl/SubscribeStreamImpl.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-24 01:56:25.000000 socket.d-2.4.12/socketd/transport/stream/impl/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.178882 socket.d-2.4.12/socketd/utils/
--rw-r--r--   0 noear      (501) staff       (20)     3492 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/utils/AsyncUtils.py
--rw-r--r--   0 noear      (501) staff       (20)     1977 2024-04-24 09:22:27.000000 socket.d-2.4.12/socketd/utils/CompletableFuture.py
--rw-r--r--   0 noear      (501) staff       (20)      267 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/utils/LogConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      216 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/utils/RunUtils.py
--rw-r--r--   0 noear      (501) staff       (20)      665 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/utils/StrUtils.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/utils/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.179927 socket.d-2.4.12/socketd/utils/async_api/
--rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/utils/async_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-24 09:21:46.000000 socket.d-2.4.12/socketd/utils/async_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.181578 socket.d-2.4.12/socketd/utils/sync_api/
--rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/utils/sync_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-24 09:21:55.000000 socket.d-2.4.12/socketd/utils/sync_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.186057 socket.d-2.4.12/socketd_aio_tcp/
--rw-r--r--   0 noear      (501) staff       (20)     4119 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_aio_tcp/TCPAIOServer.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_aio_tcp/TCPStreamIO.py
--rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_aio_tcp/TcpAIOChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_aio_tcp/TcpAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     6563 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_aio_tcp/TcpAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_aio_tcp/TcpAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_aio_tcp/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.188449 socket.d-2.4.12/socketd_websocket/
--rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/WsAioChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/WsAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     3615 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_websocket/WsAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/WsAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     2085 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_websocket/WsAioServer.py
--rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.191752 socket.d-2.4.12/socketd_websocket/impl/
--rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/impl/AIOConnect.py
--rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/impl/AIOServe.py
--rw-r--r--   0 noear      (501) staff       (20)     5966 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_websocket/impl/AIOWebSocketClientImpl.py
--rw-r--r--   0 noear      (501) staff       (20)     4283 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_websocket/impl/AIOWebSocketServerImpl.py
--rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.877551 socket.d-2.4.13/
+-rw-r--r--   0 noear      (501) staff       (20)      553 2024-04-29 00:56:45.876794 socket.d-2.4.13/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.13/README.md
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-29 00:56:45.877736 socket.d-2.4.13/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      873 2024-04-29 00:40:35.000000 socket.d-2.4.13/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.875724 socket.d-2.4.13/socket.d.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      553 2024-04-29 00:56:45.000000 socket.d-2.4.13/socket.d.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     5140 2024-04-29 00:56:45.000000 socket.d-2.4.13/socket.d.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-29 00:56:45.000000 socket.d-2.4.13/socket.d.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-29 00:56:45.000000 socket.d-2.4.13/socket.d.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-29 00:56:45.000000 socket.d-2.4.13/socket.d.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-29 00:56:45.000000 socket.d-2.4.13/socket.d.egg-info/zip-safe
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.792050 socket.d-2.4.13/socketd/
+-rw-r--r--   0 noear      (501) staff       (20)     2711 2024-04-29 00:40:35.000000 socket.d-2.4.13/socketd/SocketD.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.794709 socket.d-2.4.13/socketd/broker/
+-rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/broker/BrokerFragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)     3574 2024-04-28 13:02:14.000000 socket.d-2.4.13/socketd/broker/BrokerListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     3181 2024-04-28 12:41:55.000000 socket.d-2.4.13/socketd/broker/BrokerListenerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/broker/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.797106 socket.d-2.4.13/socketd/cluster/
+-rw-r--r--   0 noear      (501) staff       (20)     2746 2024-04-28 11:41:07.000000 socket.d-2.4.13/socketd/cluster/ClusterClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     2654 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/cluster/ClusterClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)     1995 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/cluster/LoadBalancer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/cluster/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.798141 socket.d-2.4.13/socketd/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      868 2024-04-28 13:38:58.000000 socket.d-2.4.13/socketd/exception/SocketDExecption.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.798581 socket.d-2.4.13/socketd/transport/
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.807402 socket.d-2.4.13/socketd/transport/client/
+-rw-r--r--   0 noear      (501) staff       (20)     1714 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/client/Client.py
+-rw-r--r--   0 noear      (501) staff       (20)     3584 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/client/ClientBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     6554 2024-04-28 23:43:54.000000 socket.d-2.4.13/socketd/transport/client/ClientChannel.py
+-rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/client/ClientConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/client/ClientConfigHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/client/ClientConnectHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/client/ClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/client/ClientConnectorBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/client/ClientHandshakeResult.py
+-rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-24 04:28:16.000000 socket.d-2.4.13/socketd/transport/client/ClientHeartbeatHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/client/ClientProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     1047 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/client/ClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.824126 socket.d-2.4.13/socketd/transport/core/
+-rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/Asserts.py
+-rw-r--r--   0 noear      (501) staff       (20)     2476 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/core/Channel.py
+-rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/ChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/ChannelInternal.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/ChannelSupporter.py
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/Codec.py
+-rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/Config.py
+-rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/Costants.py
+-rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/Entity.py
+-rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/EntityMetas.py
+-rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/Flags.py
+-rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/FragmentAggregator.py
+-rw-r--r--   0 noear      (501) staff       (20)      832 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/core/FragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/Frame.py
+-rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/Frames.py
+-rw-r--r--   0 noear      (501) staff       (20)     2526 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/HandshakeDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      160 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/IdGenerator.py
+-rw-r--r--   0 noear      (501) staff       (20)      510 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/Listener.py
+-rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/Message.py
+-rw-r--r--   0 noear      (501) staff       (20)      953 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/Processor.py
+-rw-r--r--   0 noear      (501) staff       (20)     2025 2024-04-28 12:46:40.000000 socket.d-2.4.13/socketd/transport/core/Session.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.827238 socket.d-2.4.13/socketd/transport/core/codec/
+-rw-r--r--   0 noear      (501) staff       (20)     1346 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/codec/Buffer.py
+-rw-r--r--   0 noear      (501) staff       (20)      777 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/codec/ByteBufferCodecReader.py
+-rw-r--r--   0 noear      (501) staff       (20)      666 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/codec/ByteBufferCodecWriter.py
+-rw-r--r--   0 noear      (501) staff       (20)     4616 2024-04-28 14:08:23.000000 socket.d-2.4.13/socketd/transport/core/codec/CodecDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/codec/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.830396 socket.d-2.4.13/socketd/transport/core/entity/
+-rw-r--r--   0 noear      (501) staff       (20)     3853 2024-04-28 12:41:55.000000 socket.d-2.4.13/socketd/transport/core/entity/EntityDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      800 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/entity/FileEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/entity/MessageBuilder.py
+-rw-r--r--   0 noear      (501) staff       (20)     2162 2024-04-28 13:30:34.000000 socket.d-2.4.13/socketd/transport/core/entity/MessageDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/entity/StringEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/entity/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.833694 socket.d-2.4.13/socketd/transport/core/fragment/
+-rw-r--r--   0 noear      (501) staff       (20)     2236 2024-04-28 12:41:55.000000 socket.d-2.4.13/socketd/transport/core/fragment/FragmentAggregatorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     3371 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/core/fragment/FragmentHandlerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/fragment/FragmentHandlerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/fragment/FragmentHolder.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/fragment/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.839708 socket.d-2.4.13/socketd/transport/core/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     2420 2024-04-28 12:41:55.000000 socket.d-2.4.13/socketd/transport/core/impl/ChannelBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     7317 2024-04-29 00:25:19.000000 socket.d-2.4.13/socketd/transport/core/impl/ChannelDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     6565 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/core/impl/ConfigBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     8362 2024-04-29 00:25:18.000000 socket.d-2.4.13/socketd/transport/core/impl/ProcessorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     1522 2024-04-28 12:48:00.000000 socket.d-2.4.13/socketd/transport/core/impl/SessionBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     4762 2024-04-28 23:43:54.000000 socket.d-2.4.13/socketd/transport/core/impl/SessionDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.843814 socket.d-2.4.13/socketd/transport/core/listener/
+-rw-r--r--   0 noear      (501) staff       (20)     2384 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/listener/EventListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1297 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/listener/PathListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1254 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/listener/PipelineListener.py
+-rw-r--r--   0 noear      (501) staff       (20)      406 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/listener/RouteSelector.py
+-rw-r--r--   0 noear      (501) staff       (20)      606 2024-04-28 12:44:30.000000 socket.d-2.4.13/socketd/transport/core/listener/RouteSelectorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      473 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/core/listener/SimpleListener.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/core/listener/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.847211 socket.d-2.4.13/socketd/transport/server/
+-rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/server/Server.py
+-rw-r--r--   0 noear      (501) staff       (20)     2629 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/server/ServerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     1652 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/transport/server/ServerConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/server/ServerProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/server/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.850863 socket.d-2.4.13/socketd/transport/stream/
+-rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-28 13:24:32.000000 socket.d-2.4.13/socketd/transport/stream/RequestStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      597 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/stream/SendStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      850 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/stream/Stream.py
+-rw-r--r--   0 noear      (501) staff       (20)      295 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/stream/StreamManger.py
+-rw-r--r--   0 noear      (501) staff       (20)     1119 2024-04-28 12:44:30.000000 socket.d-2.4.13/socketd/transport/stream/StreamMangerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      823 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/stream/SubscribeStream.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd/transport/stream/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.854217 socket.d-2.4.13/socketd/transport/stream/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     1855 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/stream/impl/RequestStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)      734 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/stream/impl/SendStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)     2345 2024-04-28 13:22:13.000000 socket.d-2.4.13/socketd/transport/stream/impl/StreamBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     1279 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/stream/impl/SubscribeStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/transport/stream/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.859810 socket.d-2.4.13/socketd/utils/
+-rw-r--r--   0 noear      (501) staff       (20)     3492 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/utils/AsyncUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)     1989 2024-04-28 13:06:13.000000 socket.d-2.4.13/socketd/utils/CompletableFuture.py
+-rw-r--r--   0 noear      (501) staff       (20)      324 2024-04-29 00:23:22.000000 socket.d-2.4.13/socketd/utils/LogConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      191 2024-04-28 12:41:55.000000 socket.d-2.4.13/socketd/utils/MapUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)      216 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/utils/RunUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)      665 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/utils/StrUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-23 03:01:10.000000 socket.d-2.4.13/socketd/utils/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.860984 socket.d-2.4.13/socketd/utils/async_api/
+-rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/utils/async_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/utils/async_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.861935 socket.d-2.4.13/socketd/utils/sync_api/
+-rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/utils/sync_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd/utils/sync_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.866511 socket.d-2.4.13/socketd_aio_tcp/
+-rw-r--r--   0 noear      (501) staff       (20)     4119 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd_aio_tcp/TCPAIOServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_aio_tcp/TCPStreamIO.py
+-rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_aio_tcp/TcpAIOChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_aio_tcp/TcpAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     6563 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd_aio_tcp/TcpAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_aio_tcp/TcpAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_aio_tcp/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.869597 socket.d-2.4.13/socketd_websocket/
+-rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_websocket/WsAioChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_websocket/WsAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     3615 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd_websocket/WsAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_websocket/WsAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     2085 2024-04-25 06:00:37.000000 socket.d-2.4.13/socketd_websocket/WsAioServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_websocket/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 00:56:45.874041 socket.d-2.4.13/socketd_websocket/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_websocket/impl/AIOConnect.py
+-rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_websocket/impl/AIOServe.py
+-rw-r--r--   0 noear      (501) staff       (20)     6031 2024-04-28 23:43:54.000000 socket.d-2.4.13/socketd_websocket/impl/AIOWebSocketClientImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)     4347 2024-04-28 23:43:54.000000 socket.d-2.4.13/socketd_websocket/impl/AIOWebSocketServerImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.13/socketd_websocket/impl/__init__.py
```

### Comparing `socket.d-2.4.12/PKG-INFO` & `socket.d-2.4.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.12
+Version: 2.4.13
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.12/README.md` & `socket.d-2.4.13/README.md`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/setup.py` & `socket.d-2.4.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*_
 from setuptools import setup,find_packages
 
 setup(
     name='socket.d',
-    version='2.4.12',
+    version='2.4.13',
     description='@noear/socket.d python project',
     author='noear,bai',
     url='https://socketd.noear.org/',
     packages=find_packages(exclude=['*test*']),   # 包内不需要引用的文件夹
     install_requires=[                          # 依赖包
         'loguru',
         'websockets'
```

### Comparing `socket.d-2.4.12/socket.d.egg-info/PKG-INFO` & `socket.d-2.4.13/socket.d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.12
+Version: 2.4.13
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.12/socket.d.egg-info/SOURCES.txt` & `socket.d-2.4.13/socket.d.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 socketd/transport/stream/impl/SendStreamImpl.py
 socketd/transport/stream/impl/StreamBase.py
 socketd/transport/stream/impl/SubscribeStreamImpl.py
 socketd/transport/stream/impl/__init__.py
 socketd/utils/AsyncUtils.py
 socketd/utils/CompletableFuture.py
 socketd/utils/LogConfig.py
+socketd/utils/MapUtils.py
 socketd/utils/RunUtils.py
 socketd/utils/StrUtils.py
 socketd/utils/__init__.py
 socketd/utils/async_api/AtomicRefer.py
 socketd/utils/async_api/__init__.py
 socketd/utils/sync_api/AtomicRefer.py
 socketd/utils/sync_api/__init__.py
```

### Comparing `socket.d-2.4.12/socketd/SocketD.py` & `socket.d-2.4.13/socketd/SocketD.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Dict
 
-import socketd.cluster.ClusterClient as ClusterClient
+from socketd.cluster.ClusterClient import ClusterClient
 from socketd.transport.client.ClientConfig import ClientConfig
 from socketd.transport.client.Client import Client
 from socketd.transport.client.ClientProvider import ClientProvider
 from socketd.transport.core.Asserts import Asserts
 from socketd.transport.server.Server import Server
 from socketd.transport.server.ServerConfig import ServerConfig
 from socketd.transport.server.ServerProvider import ServerProvider
 
 from socketd_websocket.WsAioProvider import WsAioProvider
 from socketd_aio_tcp.TcpAioProvider import TcpAioProvider
 
 
 def version() -> str:
-    return "2.4.12"
+    return "2.4.13"
 
 
 def protocol_version() -> str:
     return "1.0"
 
 
 client_factory_map: Dict[str, ClientProvider] = {}
@@ -77,13 +77,13 @@
     if factory is None:
         return None
     else:
         return factory.create_client(config)
 
 
 def create_cluster_client(*urls) -> Client:
-    return ClusterClient(*urls)
+    return ClusterClient(urls)
 
 
 # Initialize the client and server factory maps
 load_factories([WsAioProvider(), TcpAioProvider()], server_factory_map)
 load_factories([WsAioProvider(), TcpAioProvider()], client_factory_map)
```

### Comparing `socket.d-2.4.12/socketd/broker/BrokerListener.py` & `socket.d-2.4.13/socketd/broker/BrokerListener.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,8 @@
             responder.send_and_subscribe(message.event(), message, -1).then_reply(then_reply).then_error(then_error)
             return
 
         responder.send(message.event(), message)
 
     def on_error(self, session: Session, error):
         ...
-        # log.warn("Broker error", error)
+        # log.warning("Broker error", error)
```

### Comparing `socket.d-2.4.12/socketd/broker/BrokerListenerBase.py` & `socket.d-2.4.13/socketd/broker/BrokerListenerBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Dict, List
 from socketd.cluster.LoadBalancer import LoadBalancer
 from socketd.transport.client.ClientSession import ClientSession
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Listener import Listener
 from socketd.transport.core.Message import Message
 from socketd.transport.core.Session import Session
+from socketd.utils.MapUtils import MapUtils
 from socketd.utils.StrUtils import StrUtils
 
 
 # 经纪人监听器基类（实现玩家封闭管理）
 class BrokerListenerBase(Listener, ABC):
     def __init__(self):
         self.__sessionAll: Dict[str, Session] = {}
@@ -75,8 +76,8 @@
     # 移除玩家会话
     def remove_player(self, name: str, session: Session):
         if StrUtils.is_not_empty(name):
             tmp: list[Session] = self.get_player_all(name)
             if tmp is not None:
                 tmp.remove(session)
 
-        self.__sessionAll.pop(session.session_id())
+        MapUtils.remove(self.__sessionAll, session.session_id())
```

### Comparing `socket.d-2.4.12/socketd/cluster/ClusterClient.py` & `socket.d-2.4.13/socketd/cluster/ClusterClient.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import asyncio
-from typing import Optional, List, Awaitable, Any
+from typing import List
 
 from socketd import SocketD
 from socketd.cluster.ClusterClientSession import ClusterClientSession
 from socketd.transport.client.Client import Client, ClientInternal
 from socketd.transport.client.ClientConfigHandler import ClientConfigHandler
 from socketd.transport.client.ClientConnectHandler import ClientConnectHandler
 from socketd.transport.client.ClientSession import ClientSession
 from socketd.transport.core import Listener
 from socketd.transport.core.Session import Session
 from socketd.transport.client.ClientHeartbeatHandler import ClientHeartbeatHandler
 
 
 class ClusterClient(Client):
 
-    def __init__(self, *serverUrls):
-        self.__serverUrls: Optional[tuple[Any, ...]] = serverUrls
+    def __init__(self, serverUrls:tuple[str]):
+        self.__serverUrls:tuple[str] = serverUrls
 
         self.__connectHandler: ClientConnectHandler = None
         self.__heartbeatHandler: ClientHeartbeatHandler = None
         self.__configHandler: ClientConfigHandler = None
 
         self.__listener = None
 
@@ -35,19 +35,19 @@
         self.__configHandler = configHandler
         return self
 
     def listen(self, listener: Listener) -> Client:
         self.__listener = listener
         return self
 
-    def open(self) -> Awaitable[ClientSession]:
-        return self._open_do(False)
+    async def open(self) -> ClientSession:
+        return await self._open_do(False)
 
-    def open_or_throw(self) -> Awaitable[ClientSession]:
-        return self._open_do(True)
+    async def open_or_throw(self) -> ClientSession:
+        return await self._open_do(True)
 
     async def _open_do(self, is_throw):
         sessions: List[Session] = []
         exchangeExecutor = None
         for urls in self.__serverUrls:
             for url in urls.split(","):
                 client: ClientInternal = SocketD.create_client(url)
@@ -65,11 +65,12 @@
                     client.heartbeat_handler(self.__heartbeatHandler)
 
                 if exchangeExecutor is None:
                     exchangeExecutor = client.get_config().get_exchange_executor()
                 else:
                     client.get_config().exchange_executor(exchangeExecutor)
 
-                sessions.extend(await asyncio.gather(*[client.open_or_throw() if is_throw else client.open()]))
+                sesssion = await (client.open_or_throw() if is_throw else client.open())
+                sessions.append(sesssion)
         return ClusterClientSession(sessions)
```

### Comparing `socket.d-2.4.12/socketd/cluster/ClusterClientSession.py` & `socket.d-2.4.13/socketd/cluster/ClusterClientSession.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/cluster/LoadBalancer.py` & `socket.d-2.4.13/socketd/cluster/LoadBalancer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/exception/SocketDExecption.py` & `socket.d-2.4.13/socketd/exception/SocketDExecption.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,27 @@
+from socketd.transport.core.Message import Message
+
+
 class SocketDException(RuntimeError):
 
     def __init__(self, message):
         super().__init__(self)
         self.message = message
 
     def __str__(self):
         return self.message
 
 
 class SocketDAlarmException(SocketDException):
     """ 告警"""
-    pass
+    def __init__(self, alarm:Message):
+        super().__init__(alarm.data_as_string())
+        self.__alarm = alarm
+    def get_alarm(self):
+        return self.__alarm
 
 
 class SocketDChannelException(SocketDException):
     """ 通道"""
     pass
```

### Comparing `socket.d-2.4.12/socketd/transport/client/Client.py` & `socket.d-2.4.13/socketd/transport/client/Client.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/client/ClientBase.py` & `socket.d-2.4.13/socketd/transport/client/ClientBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/client/ClientChannel.py` & `socket.d-2.4.13/socketd/transport/client/ClientChannel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import traceback
 from asyncio import Future
 
 from socketd.exception.SocketDExecption import SocketDException, SocketDChannelException
 from socketd.transport.client.Client import ClientInternal
 from socketd.transport.core.Asserts import Asserts
 from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.Costants import Constants
@@ -36,15 +37,16 @@
         self.init_heartbeat()
 
     def __del__(self):
         try:
             if not self.__heartbeatScheduledFuture.done():
                 self.__heartbeatScheduledFuture.cancel()
         except Exception as e:
-            log.warning(e)
+            e_msg = traceback.format_exc()
+            log.warning(e_msg)
 
     async def __heartbeatScheduled(self) -> None:
         while True:
             await asyncio.sleep(self.__client.get_heartbeat_interval() / 1000)
             await self.heartbeat_handle()
 
     def init_heartbeat(self):
```

### Comparing `socket.d-2.4.12/socketd/transport/client/ClientConfig.py` & `socket.d-2.4.13/socketd/transport/client/ClientConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/client/ClientSession.py` & `socket.d-2.4.13/socketd/transport/client/ClientSession.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/Asserts.py` & `socket.d-2.4.13/socketd/transport/core/Asserts.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/Channel.py` & `socket.d-2.4.13/socketd/transport/core/Channel.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/ChannelAssistant.py` & `socket.d-2.4.13/socketd/transport/core/ChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/ChannelInternal.py` & `socket.d-2.4.13/socketd/transport/core/ChannelInternal.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/ChannelSupporter.py` & `socket.d-2.4.13/socketd/transport/core/ChannelSupporter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/Codec.py` & `socket.d-2.4.13/socketd/transport/core/Codec.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/Config.py` & `socket.d-2.4.13/socketd/transport/core/Config.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/Costants.py` & `socket.d-2.4.13/socketd/transport/core/Costants.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/Entity.py` & `socket.d-2.4.13/socketd/transport/core/Entity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/EntityMetas.py` & `socket.d-2.4.13/socketd/transport/core/EntityMetas.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/Flags.py` & `socket.d-2.4.13/socketd/transport/core/Flags.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/FragmentAggregator.py` & `socket.d-2.4.13/socketd/transport/core/FragmentAggregator.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/FragmentHandler.py` & `socket.d-2.4.13/socketd/transport/core/FragmentHandler.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/Frames.py` & `socket.d-2.4.13/socketd/transport/core/Frames.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/HandshakeDefault.py` & `socket.d-2.4.13/socketd/transport/core/HandshakeDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/Message.py` & `socket.d-2.4.13/socketd/transport/core/Message.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/Processor.py` & `socket.d-2.4.13/socketd/transport/core/Processor.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/Session.py` & `socket.d-2.4.13/socketd/transport/core/Session.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,18 @@
         ...
 
     @abc.abstractmethod
     def attr_has(self, name: str) -> bool:
         ...
 
     @abc.abstractmethod
+    def attr_del(self, name: str):
+        ...
+
+    @abc.abstractmethod
     def attr(self, name: str) -> Union[None, Any]:
         ...
 
     @abc.abstractmethod
     def attr_or_default(self, name: str, defVal: Any) -> Any:
         ...
```

### Comparing `socket.d-2.4.12/socketd/transport/core/codec/Buffer.py` & `socket.d-2.4.13/socketd/transport/core/codec/Buffer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/codec/ByteBufferCodecReader.py` & `socket.d-2.4.13/socketd/transport/core/codec/ByteBufferCodecReader.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/codec/ByteBufferCodecWriter.py` & `socket.d-2.4.13/socketd/transport/core/codec/ByteBufferCodecWriter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/codec/CodecDefault.py` & `socket.d-2.4.13/socketd/transport/core/codec/CodecDefault.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,24 +28,23 @@
             target.flush()
 
             return target
         else:
             # sid
             sidB: bytes = frame.message().sid().encode(self.config.get_charset())
             # event
-            event: bytes = frame.message().event().encode(self.config.get_charset())
+            eventB: bytes = frame.message().event().encode(self.config.get_charset())
             # metaString
             metaStringB: bytes = frame.message().entity().meta_string().encode(self.config.get_charset())
 
-            # length (flag + sid + event + metaString + data + int.bytes + \n*3)
-            len1 = len(sidB) + len(event) + len(
-                metaStringB) + frame.message().entity().data_size() + 1 * 3 + 2 * 4
+            # length (len[int] + flag[int] + sid + event + metaString + data + \n*3)
+            len1 = 4 + 4 + len(sidB) + len(eventB) + len(metaStringB) + frame.message().data_size() + 2 * 3
 
             Asserts.assert_size("sid", len(sidB), Constants.MAX_SIZE_SID)
-            Asserts.assert_size("event", len(event), Constants.MAX_SIZE_EVENT)
+            Asserts.assert_size("event", len(eventB), Constants.MAX_SIZE_EVENT)
             Asserts.assert_size("metaString", len(metaStringB), Constants.MAX_SIZE_META_STRING)
             Asserts.assert_size("data", frame.message().entity().data_size(), Constants.MAX_SIZE_DATA)
 
             target: CodecWriter = writerFactory(len1)
 
             # length
             target.put_int(len1)
@@ -54,15 +53,15 @@
             target.put_int(frame.flag())
 
             # sid
             target.put_bytes(sidB)
             target.put_char(10) #'\n'
 
             # event
-            target.put_bytes(event)
+            target.put_bytes(eventB)
             target.put_char(10)
 
             # metaString
             target.put_bytes(metaStringB)
             target.put_char(10)
 
             # _data
```

### Comparing `socket.d-2.4.12/socketd/transport/core/entity/EntityDefault.py` & `socket.d-2.4.13/socketd/transport/core/entity/EntityDefault.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from io import BytesIO, TextIOWrapper, BufferedReader
 from typing import Any, Optional, BinaryIO
 
 from socketd.transport.core.Entity import Entity
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.EntityMetas import EntityMetas
+from socketd.utils.MapUtils import MapUtils
 
 
 class EntityDefault(Entity):
     def __init__(self):
         self._meta_map: Optional[dict] = None
         self._meta_string = Constants.DEF_META_STRING
         self._meta_stringChanged = False
@@ -62,21 +63,21 @@
                         self._meta_map[kv[0]] = ""
         return self._meta_map
 
     def meta_put(self, name:str, val:str):
         if val:
             self.meta_map()[name] = val
         else:
-            self.meta_map().pop(name)
+            MapUtils.remove(self.meta_map(), name)
 
         self._meta_stringChanged = True
         return self
 
     def meta_del(self, name:str):
-        self.meta_map().pop(name)
+        MapUtils.remove(self.meta_map(), name)
         self._meta_stringChanged = True
         return self
 
     def meta(self, name:str) -> Any:
         return self.meta_map().get(name)
 
     def meta_or_default(self, name:str, default_val:str):
```

### Comparing `socket.d-2.4.12/socketd/transport/core/entity/FileEntity.py` & `socket.d-2.4.13/socketd/transport/core/entity/FileEntity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/entity/MessageBuilder.py` & `socket.d-2.4.13/socketd/transport/core/entity/MessageBuilder.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/entity/MessageDefault.py` & `socket.d-2.4.13/socketd/transport/core/entity/MessageDefault.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,8 +74,11 @@
     def data_size(self) -> int:
         return self._entity.data_size()
 
     def release(self):
         if self._entity:
             self._entity.release()
 
+    def __str__(self):
+        return f"Message(sid='{self._sid}', event='{self._event}', entity='{self._entity}')"
+
```

### Comparing `socket.d-2.4.12/socketd/transport/core/fragment/FragmentAggregatorDefault.py` & `socket.d-2.4.13/socketd/transport/core/fragment/FragmentAggregatorDefault.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from socketd.transport.core.entity.EntityDefault import EntityDefault
 from socketd.transport.core.Frame import Frame
 from socketd.transport.core.Message import MessageInternal
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.FragmentAggregator import FragmentAggregator
 from socketd.exception.SocketDExecption import SocketDException
+from socketd.utils.MapUtils import MapUtils
 
 from .FragmentHolder import FragmentHolder
 from ..entity.MessageBuilder import MessageBuilder
 from socketd.utils.StrUtils import StrUtils
 
 
 class FragmentAggregatorDefault(FragmentAggregator):
@@ -45,15 +46,15 @@
 
         dataBuffer: BytesIO = BytesIO()
 
         for fragment in self.__fragmentHolders:
             dataBuffer.write(fragment.message.data().getvalue())
 
         entity = EntityDefault().meta_map_put(self.__main.meta_map()).data_set(dataBuffer)
-        entity.meta_map().pop(EntityMetas.META_DATA_FRAGMENT_IDX)
+        MapUtils.remove(entity.meta_map(), EntityMetas.META_DATA_FRAGMENT_IDX)
 
         return Frame(self.__main.flag(),
                      MessageBuilder()
                      .flag(self.__main.flag())
                      .sid(self.__main.sid())
                      .event(self.__main.event())
                      .entity(entity)
```

### Comparing `socket.d-2.4.12/socketd/transport/core/fragment/FragmentHandlerBase.py` & `socket.d-2.4.13/socketd/transport/core/fragment/FragmentHandlerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/impl/ChannelBase.py` & `socket.d-2.4.13/socketd/transport/core/impl/ChannelBase.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 from socketd.transport.core.Channel import Channel
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Frames import Frames
 from socketd.transport.core.Config import Config
 from socketd.transport.core.HandshakeDefault import HandshakeInternal
 from socketd.transport.core.Message import Message
+from socketd.utils.MapUtils import MapUtils
 
 
 class ChannelBase(Channel, ABC):
     def __init__(self, config: Config):
         self.config = config
 
         self.handshake: HandshakeInternal = None
-        self.__attachments = {}
+        self.__attachments:dict = {}
 
         self.__lock: threading.Lock = threading.Lock()
         self.__loop: Optional[asyncio.AbstractEventLoop] = None
 
     def __enter__(self):
         return self.__lock.acquire()
 
@@ -41,15 +42,15 @@
         self.__loop = loop
 
     def get_attachment(self, name):
         return self.__attachments.get(name, None)
 
     def put_attachment(self, name, val):
         if val is None:
-            self.__attachments.pop(name)
+            MapUtils.remove(self.__attachments, name)
         else:
             self.__attachments[name] = val
 
     def set_handshake(self, handshake):
         if handshake is not None:
             self.handshake = handshake
```

### Comparing `socket.d-2.4.12/socketd/transport/core/impl/ChannelDefault.py` & `socket.d-2.4.13/socketd/transport/core/impl/ChannelDefault.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import time
+import traceback
 from typing import TypeVar, Optional
 
 from socketd.transport.core import Entity
 from socketd.transport.core.Asserts import Asserts
 from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.ChannelSupporter import ChannelSupporter
 from socketd.transport.core.Message import MessageInternal, Message
@@ -166,16 +167,16 @@
 
             if code > Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING:
                 if self._assistant.is_valid(self._source):
                     # 如果有效且非预关闭，则尝试关闭源
                     await RunUtils.waitTry(self._assistant.close(self._source))
                     log.debug(f"{self.get_config().get_role_name()} channel closed, sessionId={self.get_session().session_id()}")
         except Exception as e:
-            log.warning(f"{self.get_config().get_role_name()} channel close error, "
-                        f"sessionId={self.get_session().session_id()} : {e}")
+            e_msg = traceback.format_exc()
+            log.warning(f"{self.get_config().get_role_name()} channel close error, sessionId={self.get_session().session_id()} \n{e_msg}")
 
         if code > Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING:
             self.on_close_do()
 
 
     def on_close_do(self):
         if self._isCloseNotified == False:
```

### Comparing `socket.d-2.4.12/socketd/transport/core/impl/ConfigBase.py` & `socket.d-2.4.13/socketd/transport/core/impl/ConfigBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/impl/ProcessorDefault.py` & `socket.d-2.4.13/socketd/transport/core/impl/ProcessorDefault.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import traceback
 from abc import ABC
 from typing import Optional
 
 from socketd.exception.SocketDExecption import SocketDAlarmException, SocketDConnectionException
 from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.HandshakeDefault import HandshakeDefault
 from socketd.transport.core.Message import Message
@@ -59,16 +60,15 @@
         else:
             if channel.get_handshake() is None:
                 await channel.close(Constants.CLOSE1002_PROTOCOL_ILLEGAL)
 
                 if frame.flag() == Flags.Close:
                     raise SocketDConnectionException("Connection request was rejected")
 
-                log.warning("{} channel handshake is None, sessionId={}", channel.get_config().get_role_name(),
-                                 channel.get_session().session_id())
+                log.warning(f"{channel.get_config().get_role_name()} channel handshake is None, sessionId={channel.get_session().session_id()}")
                 return
 
             # 更新最后活动时间
             channel.set_live_time_as_now()
 
             try:
                 if frame.flag() == Flags.Ping:
@@ -143,28 +143,30 @@
             self.on_message(channel, frame.message())
 
     def on_open(self, channel: ChannelInternal):
         RunUtils.taskTry(self.on_open_do(channel))
 
     async def on_open_do(self, channel: ChannelInternal):
         try:
-            await self.listener.on_open(channel.get_session())
+            await RunUtils.waitTry(self.listener.on_open(channel.get_session()))
             channel.do_open_future(True, None)
         except Exception as e:
-            log.warning("{} channel listener onOpen error", channel.get_config().get_role_name(), e)
+            e_msg = traceback.format_exc()
+            log.warning(f"{channel.get_config().get_role_name()} channel listener onOpen error \n{e_msg}")
             channel.do_open_future(False, e)
 
     def on_message(self, channel: ChannelInternal, message: Message):
         RunUtils.taskTry(self.on_message_do(channel, message))
 
     async def on_message_do(self, channel: ChannelInternal, message: Message):
         try:
             await self.listener.on_message(channel.get_session(), message)
         except Exception as e:
-            log.warning("{} channel listener onMessage error", channel.get_config().get_role_name(), e)
+            e_msg = traceback.format_exc()
+            log.warning(f"{channel.get_config().get_role_name()} channel listener onMessage error \n{e_msg}")
             self.on_error(channel, e)
 
     def on_close(self, channel: ChannelInternal):
         if channel.is_closed() <= Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING:
             RunUtils.taskTry(self.on_close_internal(channel, Constants.CLOSE2003_DISCONNECTION))
 
     async def on_close_internal(self, channel: ChannelInternal, code: int):
@@ -173,15 +175,16 @@
     def on_error(self, channel: ChannelInternal, error):
         RunUtils.taskTry(self.on_error_internal(channel, error))
 
     async def on_error_internal(self, channel: ChannelInternal, error):
         try:
             await RunUtils.waitTry(self.listener.on_error(channel.get_session(), error))
         except Exception as e:
-            log.warning("{} channel listener onError error", channel.get_config().get_role_name(), e)
+            e_msg = traceback.format_exc()
+            log.warning(f"{channel.get_config().get_role_name()} channel listener onError error \n{e_msg}")
 
     def do_close_notice(self, channel: ChannelInternal):
         RunUtils.taskTry(self.do_close_notice_internal(channel))
 
     async def do_close_notice_internal(self, channel: ChannelInternal):
         try:
             await RunUtils.waitTry(self.listener.on_close(channel.get_session()))
```

### Comparing `socket.d-2.4.12/socketd/transport/core/impl/SessionBase.py` & `socket.d-2.4.13/socketd/transport/core/impl/SessionBase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC
 from typing import Any, Dict
 from socketd.transport.core.Session import Session
 from socketd.transport.core.Channel import Channel
+from socketd.utils.MapUtils import MapUtils
 
 
 class SessionBase(Session, ABC):
     def __init__(self, channel: Channel):
         self._channel = channel
         self._session_id = self.generate_id()
         self._attrMap:Dict[str, Any] = None
@@ -18,14 +19,18 @@
 
     def attr_has(self, name:str) -> bool:
         if self._attrMap is None:
             return False
         else:
             return self._attrMap.__contains__(name)
 
+    def attr_del(self, name: str):
+        if self._attrMap is not None:
+            MapUtils.remove(self._attrMap, name)
+
     def attr(self, name: str) -> Any:
         if self._attrMap is None:
             return None
 
         return self._attrMap.get(name)
 
     def attr_or_default(self, name: str, defVal: Any) -> Any:
```

### Comparing `socket.d-2.4.12/socketd/transport/core/impl/SessionDefault.py` & `socket.d-2.4.13/socketd/transport/core/impl/SessionDefault.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import traceback
 from typing import Optional
 
 from socketd.transport.core.entity.MessageBuilder import MessageBuilder
 from socketd.transport.core.impl.SessionBase import SessionBase
 from socketd.transport.core.Channel import Channel
 from socketd.transport.core.HandshakeDefault import HandshakeDefault
 from socketd.transport.core.Entity import Entity
@@ -10,19 +11,18 @@
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Flags import Flags
 from socketd.transport.stream.RequestStream import RequestStream
 from socketd.transport.stream.SendStream import SendStream
 
 from socketd.transport.stream.SubscribeStream import SubscribeStream
 
-from loguru import logger
-
 from socketd.transport.stream.impl.RequestStreamImpl import RequestStreamImpl
 from socketd.transport.stream.impl.SendStreamImpl import SendStreamImpl
 from socketd.transport.stream.impl.SubscribeStreamImpl import SubscribeStreamImpl
+from socketd.utils.LogConfig import log
 from socketd.utils.RunUtils import RunUtils
 
 
 class SessionDefault(SessionBase):
 
     def __init__(self, channel: Channel):
         super().__init__(channel)
@@ -50,15 +50,18 @@
         message = MessageBuilder().sid(self.generate_id()).event(topic).entity(content).build()
 
         stream: SendStream = SendStreamImpl(message.sid())
         RunUtils.taskTry(self._channel.send(Frame(Flags.Message, message), stream))
         return stream
 
     def send_and_request(self, event: str, content: Entity,
-                               timeout: int = 100) -> RequestStream:
+                               timeout: int|None = 100) -> RequestStream:
+
+        if timeout is None:
+            timeout = 100
 
         if timeout < 100:
             timeout = self._channel.get_config().get_request_timeout() / 1000
         message = MessageBuilder().sid(self.generate_id()).event(event).entity(content).build()
         stream:RequestStream = RequestStreamImpl(message.sid(), timeout)
         RunUtils.taskTry(self._channel.send(Frame(Flags.Request, message), stream))
         return stream
@@ -76,25 +79,26 @@
 
     async def reply_end(self, from_msg: Message, content: Entity):
         message = MessageBuilder().sid(from_msg.sid()).event(from_msg.event()).entity(content).build()
 
         await self._channel.send(Frame(Flags.ReplyEnd, message), None)
 
     async def preclose(self):
-        logger.debug(
+        log.debug(
             f"{self._channel.get_config().get_role_name()} session close starting, sessionId={self.session_id()}")
         if self._channel.is_valid():
             await self._channel.send_close(Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING)
 
     async def close(self):
         if self._channel.is_valid():
             try:
                 await self._channel.send_close(Constants.CLOSE1001_PROTOCOL_CLOSE)
             except Exception as e:
-                logger.warning(f" {self._channel.get_config().get_role_name()} channel send_close error {e}")
+                e_msg = traceback.format_exc()
+                log.warning(f" {self._channel.get_config().get_role_name()} channel send_close error \n{e_msg}")
         await self._channel.close(Constants.CLOSE2009_USER)
 
     def param(self, name: str):
         return self.handshake().param(name)
 
     def path_new(self, path: str):
         self.__path_new = path
```

### Comparing `socket.d-2.4.12/socketd/transport/core/listener/EventListener.py` & `socket.d-2.4.13/socketd/transport/core/listener/EventListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/listener/PathListener.py` & `socket.d-2.4.13/socketd/transport/core/listener/PathListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/core/listener/PipelineListener.py` & `socket.d-2.4.13/socketd/transport/core/listener/PipelineListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/server/Server.py` & `socket.d-2.4.13/socketd/transport/server/Server.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/server/ServerBase.py` & `socket.d-2.4.13/socketd/transport/server/ServerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/server/ServerConfig.py` & `socket.d-2.4.13/socketd/transport/server/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/stream/RequestStream.py` & `socket.d-2.4.13/socketd/transport/stream/SubscribeStream.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 from abc import abstractmethod
 from typing import Callable
-from socketd.transport.stream.Stream import Stream
+
 from socketd.transport.core.Entity import Reply
+from socketd.transport.stream.Stream import Stream
 
 
-class RequestStream(Stream):
+class SubscribeStream(Stream):
     @abstractmethod
-    async def waiter(self) -> Reply:
-        ...
-
-    @abstractmethod
-    def then_error(self, onError: Callable[[Exception], None]) -> 'SendStream':
+    def then_error(self, onError: Callable[[Exception], None]) -> 'SubscribeStream':
         """
         异常发生
         :param onError: 当异常发生时执行的函数，接受一个异常参数
         """
         ...
 
     @abstractmethod
-    def then_progress(self, onProgress: Callable[[bool, int, int], None]) -> 'SendStream':
+    def then_progress(self, onProgress: Callable[[bool, int, int], None]) -> 'SubscribeStream':
         """
         进度发生时
         :param onProgress (isSend, val, max)
         """
         ...
 
     @abstractmethod
-    def then_reply(self, onReply: Callable[[Reply], None]) -> 'SendStream':
+    def then_reply(self, onReply: Callable[[Reply], None]) -> 'SubscribeStream':
         """
         答复发生时
         """
         ...
-
```

### Comparing `socket.d-2.4.12/socketd/transport/stream/SendStream.py` & `socket.d-2.4.13/socketd/transport/stream/SendStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/stream/Stream.py` & `socket.d-2.4.13/socketd/transport/stream/Stream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/stream/StreamMangerDefault.py` & `socket.d-2.4.13/socketd/transport/stream/StreamMangerDefault.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 from socketd.transport.stream.Stream import StreamInternal
 from socketd.transport.stream.StreamManger import StreamManger
+from socketd.utils.MapUtils import MapUtils
 
 logger = logging.getLogger(__name__)
 
 
 class StreamMangerDefault(StreamManger):
     def __init__(self, config):
         self.config = config
@@ -23,11 +24,11 @@
 
         # Add stream timeout handling as a backup insurance
         stream_timeout = stream.timeout() if stream.timeout() > 0 else self.config.get_stream_timeout()
         if stream_timeout > 0:
             stream.insurance_start(self, stream_timeout)
 
     def remove_stream(self, sid):
-        stream: StreamInternal = self.stream_map.pop(sid, None)
+        stream: StreamInternal = MapUtils.remove(self.stream_map, sid)
         if stream:
             stream.insurance_cancel()
             logger.debug(f"{self.config.get_role_name()} stream removed, sid={sid}")
```

### Comparing `socket.d-2.4.12/socketd/transport/stream/SubscribeStream.py` & `socket.d-2.4.13/socketd/transport/stream/RequestStream.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from abc import abstractmethod
 from typing import Callable
-
-from socketd.transport.core.Entity import Reply
 from socketd.transport.stream.Stream import Stream
+from socketd.transport.core.Entity import Reply
 
 
-class SubscribeStream(Stream):
+class RequestStream(Stream):
     @abstractmethod
-    def then_error(self, onError: Callable[[Exception], None]) -> 'SubscribeStream':
+    async def waiter(self) -> Reply:
+        ...
+
+    @abstractmethod
+    def then_error(self, onError: Callable[[Exception], None]) -> 'RequestStream':
         """
         异常发生
         :param onError: 当异常发生时执行的函数，接受一个异常参数
         """
         ...
 
     @abstractmethod
-    def then_progress(self, onProgress: Callable[[bool, int, int], None]) -> 'SubscribeStream':
+    def then_progress(self, onProgress: Callable[[bool, int, int], None]) -> 'RequestStream':
         """
         进度发生时
         :param onProgress (isSend, val, max)
         """
         ...
 
     @abstractmethod
-    def then_reply(self, onReply: Callable[[Reply], None]) -> 'SubscribeStream':
+    def then_reply(self, onReply: Callable[[Reply], None]) -> 'RequestStream':
         """
         答复发生时
         """
         ...
+
```

### Comparing `socket.d-2.4.12/socketd/transport/stream/impl/RequestStreamImpl.py` & `socket.d-2.4.13/socketd/transport/stream/impl/RequestStreamImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/stream/impl/SendStreamImpl.py` & `socket.d-2.4.13/socketd/transport/stream/impl/SendStreamImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/transport/stream/impl/StreamBase.py` & `socket.d-2.4.13/socketd/transport/stream/impl/StreamBase.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,28 +13,27 @@
     """流接收器基类"""
 
     def __init__(self, sid: str, demands: int, timeout: int):
         self.__sid = sid
         self.__timeout = timeout
         self.__demands = demands
 
-        self.__onError: Callable[[Exception], None] = None
         self.__doOnError: Callable[[Exception], None] = None
         self.__doOnProgress: Callable[[bool, int, int], None] = None
 
         self.__insuranceFuture: Optional[asyncio.Future] = None
 
     def sid(self) -> str:
         return self.__sid
 
     def is_done(self):
         return True
 
     def then_error_do(self, onError: Callable[[Exception], None]):
-        self.__onError = onError
+        self.__doOnError = onError
 
     def then_progress_do(self, onProgress: Callable[[bool, int, int], None]):
         self.__doOnProgress = onProgress
 
     def demands(self) -> int:
         return self.__demands
 
@@ -59,15 +58,15 @@
         if self.__insuranceFuture:
             self.__insuranceFuture.cancel()
 
     def on_reply(self, reply:MessageInternal):
         ...
 
     def on_error(self, error: Exception):
-        if error:
+        if error and self.__doOnError:
             self.__doOnError(error)
 
     def on_progress(self, is_send, val, max_val):
         if self.__doOnProgress:
             self.__doOnProgress(is_send, val, max_val)
```

### Comparing `socket.d-2.4.12/socketd/transport/stream/impl/SubscribeStreamImpl.py` & `socket.d-2.4.13/socketd/transport/stream/impl/SubscribeStreamImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/utils/AsyncUtils.py` & `socket.d-2.4.13/socketd/utils/AsyncUtils.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/utils/CompletableFuture.py` & `socket.d-2.4.13/socketd/utils/CompletableFuture.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import asyncio
 import functools
 from threading import Lock
 from typing import Generic, TypeVar, Callable
 
-from loguru import logger
+from socketd.utils.LogConfig import log
 
 T = TypeVar('T')
 
 
 class CompletableFuture(Generic[T]):
 
     def __init__(self, _future=None, loop=None):
         if loop is None:
             loop = asyncio.get_running_loop()
         if _future and not asyncio.iscoroutine(_future):
-            logger.warning("{name}对象不是协程对象", name=_future.__name__)
+            log.warning("{name} invalid coroutine object", name=_future.__name__)
             return
         self._future: asyncio.Task = loop.create_task(_future) if _future else loop.create_future()
         self._lock = Lock()
 
     def get(self, timeout:float):
         with self._lock:
             async def _get():
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `socket.d-2.4.12/socketd/utils/StrUtils.py` & `socket.d-2.4.13/socketd/utils/StrUtils.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/utils/async_api/AtomicRefer.py` & `socket.d-2.4.13/socketd/utils/async_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd/utils/sync_api/AtomicRefer.py` & `socket.d-2.4.13/socketd/utils/sync_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_aio_tcp/TCPAIOServer.py` & `socket.d-2.4.13/socketd_aio_tcp/TCPAIOServer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_aio_tcp/TCPStreamIO.py` & `socket.d-2.4.13/socketd_aio_tcp/TCPStreamIO.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_aio_tcp/TcpAIOChannelAssistant.py` & `socket.d-2.4.13/socketd_aio_tcp/TcpAIOChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_aio_tcp/TcpAioClient.py` & `socket.d-2.4.13/socketd_aio_tcp/TcpAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_aio_tcp/TcpAioClientConnector.py` & `socket.d-2.4.13/socketd_aio_tcp/TcpAioClientConnector.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_aio_tcp/TcpAioProvider.py` & `socket.d-2.4.13/socketd_aio_tcp/TcpAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_websocket/WsAioChannelAssistant.py` & `socket.d-2.4.13/socketd_websocket/WsAioChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_websocket/WsAioClient.py` & `socket.d-2.4.13/socketd_websocket/WsAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_websocket/WsAioClientConnector.py` & `socket.d-2.4.13/socketd_websocket/WsAioClientConnector.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_websocket/WsAioProvider.py` & `socket.d-2.4.13/socketd_websocket/WsAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_websocket/WsAioServer.py` & `socket.d-2.4.13/socketd_websocket/WsAioServer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_websocket/impl/AIOConnect.py` & `socket.d-2.4.13/socketd_websocket/impl/AIOConnect.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_websocket/impl/AIOServe.py` & `socket.d-2.4.13/socketd_websocket/impl/AIOServe.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.12/socketd_websocket/impl/AIOWebSocketClientImpl.py` & `socket.d-2.4.13/socketd_websocket/impl/AIOWebSocketClientImpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
+import traceback
 from asyncio import CancelledError
 from typing import Optional, Sequence, List
-from loguru import logger
 from websockets.extensions import ClientExtensionFactory
 from websockets.uri import WebSocketURI
 
 from socketd.exception.SocketDExecption import SocketDConnectionException
 from socketd.transport.client.ClientHandshakeResult import ClientHandshakeResult
 from socketd.utils.LogConfig import log
 from socketd.transport.core.impl.ChannelDefault import ChannelDefault
@@ -54,26 +54,26 @@
         while True:
             await asyncio.sleep(0)
             if self.closed or self.status_state == Flags.Close:
                 break
             try:
                 await self.on_message()
             except Exception as e:
-                log.warning(e)
+                e_msg = traceback.format_exc()
+                log.warning(e_msg)
                 break
 
     def connection_open(self) -> None:
         """
         打开握手完成回调函数。
         :return: 无返回值
         """
         super().connection_open()
         self._handler_future = self.loop.create_task(self._handler())
 
-    @logger.catch
     async def on_open(self):
         """开始建立连接"""
         try:
             log.info("Client:Websocket onOpen...")
             await self.channel.send_connect(self.client.get_config().get_url(), self.client.get_config().get_meta_map())
             while self.status_state == Flags.Connect:
                 await self.on_message()
@@ -114,18 +114,19 @@
                     log.debug("{sessionId} 服务端主动关闭",
                               sessionId=self.channel.get_session().session_id())
         except CancelledError as c:
             # 超时自动推出
             log.debug(c)
             raise c
         except SocketDConnectionException as s:
+            s_msg = traceback.format_exc()
             self.handshake_future.accept(ClientHandshakeResult(self.channel, s))
-            logger.warning(s)
+            log.warning(s_msg)
         except ConnectionClosedOK as e:
-            logger.info(e)
+            log.info(e)
         except Exception as e:
             self.on_error(e)
 
     async def on_close(self):
         await self.client.get_processor().on_close(self.channel)
         if self.handshake_future is not None:
             if self.__on_receive_tasks:
```

### Comparing `socket.d-2.4.12/socketd_websocket/impl/AIOWebSocketServerImpl.py` & `socket.d-2.4.13/socketd_websocket/impl/AIOWebSocketServerImpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import asyncio
+import traceback
 from typing import Optional, Union
 
 from websockets import ConnectionClosedOK
 from websockets.frames import Opcode
 from websockets.server import WebSocketServer, WebSocketServerProtocol
 
 from socketd.transport.core.Channel import Channel
@@ -54,15 +55,16 @@
     async def on_error(self, conn: Union[AIOWebSocketServerImpl, WebSocketServerProtocol], ex: Exception):
         try:
             channel: ChannelInternal = conn.get_attachment()
             if channel is not None:
                 # 有可能未 onOpen，就 onError 了；此时通道未成
                 self.ws_aio_server.get_processor().on_error(channel, ex)
         except Exception as e:
-            log.warning(e)
+            e_msg = traceback.format_exc()
+            log.warning(e_msg)
 
     async def on_message(self, conn: Union[AIOWebSocketServerImpl, WebSocketServerProtocol], path: str):
         """ws_handler"""
         loop = asyncio.get_running_loop()
         tasks: list[asyncio.Task] = []
         while True:
             if conn.closed:
```

