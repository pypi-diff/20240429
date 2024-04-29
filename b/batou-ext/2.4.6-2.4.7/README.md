# Comparing `tmp/batou_ext-2.4.6.tar.gz` & `tmp/batou_ext-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batou_ext-2.4.6.tar", last modified: Tue Apr 23 14:53:48 2024, max compression
+gzip compressed data, was "batou_ext-2.4.7.tar", last modified: Mon Apr 29 08:52:23 2024, max compression
```

## Comparing `batou_ext-2.4.6.tar` & `batou_ext-2.4.7.tar`

### file list

```diff
@@ -1,96 +1,98 @@
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.232453 batou_ext-2.4.6/
--rw-r--r--   0 flanitz    (501) staff       (20)     1832 2024-04-23 14:53:47.000000 batou_ext-2.4.6/CHANGES.md
--rw-r--r--   0 flanitz    (501) staff       (20)     1608 2024-04-23 14:53:47.000000 batou_ext-2.4.6/LICENSE.txt
--rw-r--r--   0 flanitz    (501) staff       (20)      144 2024-04-23 14:53:47.000000 batou_ext-2.4.6/MANIFEST.in
--rw-r--r--   0 flanitz    (501) staff       (20)     3626 2024-04-23 14:53:48.232549 batou_ext-2.4.6/PKG-INFO
--rw-r--r--   0 flanitz    (501) staff       (20)     1163 2024-04-23 14:53:47.000000 batou_ext-2.4.6/README.md
--rw-r--r--   0 flanitz    (501) staff       (20)      121 2024-04-23 14:53:47.000000 batou_ext-2.4.6/pyproject.toml
--rw-r--r--   0 flanitz    (501) staff       (20)      491 2024-04-23 14:53:48.232816 batou_ext-2.4.6/setup.cfg
--rw-r--r--   0 flanitz    (501) staff       (20)     1737 2024-04-23 14:53:47.000000 batou_ext-2.4.6/setup.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.222394 batou_ext-2.4.6/src/
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.227900 batou_ext-2.4.6/src/batou_ext/
--rw-r--r--   0 flanitz    (501) staff       (20)       23 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/__init__.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1213 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/acl.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1080 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/archive.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3560 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/config.py
--rw-r--r--   0 flanitz    (501) staff       (20)     6795 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/cron.py
--rw-r--r--   0 flanitz    (501) staff       (20)    10472 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/fcio.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4854 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/file.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1498 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/geoip.py
--rw-r--r--   0 flanitz    (501) staff       (20)     8165 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/git.py
--rw-r--r--   0 flanitz    (501) staff       (20)      616 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/htpasswd.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1892 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/http.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4162 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/jenkins.py
--rw-r--r--   0 flanitz    (501) staff       (20)      714 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/journalbeat.py
--rw-r--r--   0 flanitz    (501) staff       (20)      831 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/keypair.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5641 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/mail.py
--rw-r--r--   0 flanitz    (501) staff       (20)      245 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/mailhog.py
--rw-r--r--   0 flanitz    (501) staff       (20)      972 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/memcached.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3325 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/mirror.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1512 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/mysql.py
--rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/nfs.py
--rw-r--r--   0 flanitz    (501) staff       (20)    24116 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/nix.py
--rw-r--r--   0 flanitz    (501) staff       (20)     2214 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/nixos.py
--rw-r--r--   0 flanitz    (501) staff       (20)     6111 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/oci.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3923 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/php.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.229229 batou_ext-2.4.6/src/batou_ext/postfixadmin/
--rw-r--r--   0 flanitz    (501) staff       (20)     1997 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/__init__.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.229454 batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot/
--rw-r--r--   0 flanitz    (501) staff       (20)      751 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot/database.conf
--rw-r--r--   0 flanitz    (501) staff       (20)      447 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot/local.conf
--rw-r--r--   0 flanitz    (501) staff       (20)      584 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot.py
--rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/goceptnet.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.230018 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/
--rw-r--r--   0 flanitz    (501) staff       (20)      668 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/local.cf
--rw-r--r--   0 flanitz    (501) staff       (20)      369 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_alias
--rw-r--r--   0 flanitz    (501) staff       (20)      371 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_domains
--rw-r--r--   0 flanitz    (501) staff       (20)      376 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_mailboxes
--rw-r--r--   0 flanitz    (501) staff       (20)      457 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_sender_login
--rw-r--r--   0 flanitz    (501) staff       (20)     1541 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.230126 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfixadmin/
--rw-r--r--   0 flanitz    (501) staff       (20)      864 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfixadmin/config.local.php
--rw-r--r--   0 flanitz    (501) staff       (20)      607 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postgres.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5294 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postgres.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3296 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/python.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5691 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/rabbitmq.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1268 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/redis.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.231490 batou_ext-2.4.6/src/batou_ext/resources/
--rw-r--r--   0 flanitz    (501) staff       (20)      541 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/cert.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      388 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/check_systemd_unit.py
--rw-r--r--   0 flanitz    (501) staff       (20)      117 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/cron-wrapper.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      200 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/geoip-update.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      203 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/journalbeat.nix
--rw-r--r--   0 flanitz    (501) staff       (20)      955 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/loader.c
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.231587 batou_ext-2.4.6/src/batou_ext/resources/mailhog/
--rw-r--r--   0 flanitz    (501) staff       (20)     1371 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/mailhog/mailhog.nix
--rw-r--r--   0 flanitz    (501) staff       (20)      946 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/mirror.conf
--rw-r--r--   0 flanitz    (501) staff       (20)     1898 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/oci-template.nix
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.231890 batou_ext-2.4.6/src/batou_ext/resources/php/
--rw-r--r--   0 flanitz    (501) staff       (20)      588 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/php/php-fpm.conf
--rw-r--r--   0 flanitz    (501) staff       (20)      296 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/php/php-fpm.sh
--rw-r--r--   0 flanitz    (501) staff       (20)    71038 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/php/php.ini
--rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/python.nix
--rw-r--r--   0 flanitz    (501) staff       (20)      118 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/rediscleanup.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      560 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/setupEnv.sh
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.232045 batou_ext-2.4.6/src/batou_ext/resources/ssl/
--rw-r--r--   0 flanitz    (501) staff       (20)      597 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/ssl/local_certificate_check.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      178 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/systemd.service
--rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/userenv.nix
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.232361 batou_ext-2.4.6/src/batou_ext/roundcube/
--rw-r--r--   0 flanitz    (501) staff       (20)     3456 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/roundcube/__init__.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4181 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/roundcube/config.inc.php
--rw-r--r--   0 flanitz    (501) staff       (20)      623 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/roundcube/postgres.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1525 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/run.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4745 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/s3.py
--rw-r--r--   0 flanitz    (501) staff       (20)     9400 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/s3_bootstrap.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3572 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/ssh.py
--rw-r--r--   0 flanitz    (501) staff       (20)    11133 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/ssl.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5258 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/versions.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.228659 batou_ext-2.4.6/src/batou_ext.egg-info/
--rw-r--r--   0 flanitz    (501) staff       (20)     3626 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/PKG-INFO
--rw-r--r--   0 flanitz    (501) staff       (20)     2609 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/SOURCES.txt
--rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/dependency_links.txt
--rw-r--r--   0 flanitz    (501) staff       (20)      171 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/entry_points.txt
--rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/not-zip-safe
--rw-r--r--   0 flanitz    (501) staff       (20)      153 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/requires.txt
--rw-r--r--   0 flanitz    (501) staff       (20)       10 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/top_level.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.112029 batou_ext-2.4.7/
+-rw-r--r--   0 zagy       (501) staff       (20)     2244 2024-04-29 08:52:22.000000 batou_ext-2.4.7/CHANGES.md
+-rw-r--r--   0 zagy       (501) staff       (20)     1608 2024-04-29 08:52:22.000000 batou_ext-2.4.7/LICENSE.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      144 2024-04-29 08:52:22.000000 batou_ext-2.4.7/MANIFEST.in
+-rw-r--r--   0 zagy       (501) staff       (20)     4474 2024-04-29 08:52:23.111944 batou_ext-2.4.7/PKG-INFO
+-rw-r--r--   0 zagy       (501) staff       (20)     1163 2024-04-29 08:52:22.000000 batou_ext-2.4.7/README.md
+-rw-r--r--   0 zagy       (501) staff       (20)      121 2024-04-29 08:52:22.000000 batou_ext-2.4.7/pyproject.toml
+-rw-r--r--   0 zagy       (501) staff       (20)      491 2024-04-29 08:52:23.112329 batou_ext-2.4.7/setup.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)     1737 2024-04-29 08:52:22.000000 batou_ext-2.4.7/setup.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.097672 batou_ext-2.4.7/src/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.104041 batou_ext-2.4.7/src/batou_ext/
+-rw-r--r--   0 zagy       (501) staff       (20)       23 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1213 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/acl.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1080 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/archive.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3560 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/config.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6795 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/cron.py
+-rw-r--r--   0 zagy       (501) staff       (20)    10472 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/fcio.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5087 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/file.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1498 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/geoip.py
+-rw-r--r--   0 zagy       (501) staff       (20)     8165 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/git.py
+-rw-r--r--   0 zagy       (501) staff       (20)      616 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/htpasswd.py
+-rw-r--r--   0 zagy       (501) staff       (20)     9614 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/http.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4162 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/jenkins.py
+-rw-r--r--   0 zagy       (501) staff       (20)      714 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/journalbeat.py
+-rw-r--r--   0 zagy       (501) staff       (20)      831 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/keypair.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5641 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/mail.py
+-rw-r--r--   0 zagy       (501) staff       (20)      245 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/mailhog.py
+-rw-r--r--   0 zagy       (501) staff       (20)      972 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/memcached.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3325 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/mirror.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1512 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/mysql.py
+-rw-r--r--   0 zagy       (501) staff       (20)      617 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/nfs.py
+-rw-r--r--   0 zagy       (501) staff       (20)    24116 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/nix.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2214 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/nixos.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6111 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/oci.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3923 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/php.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.105528 batou_ext-2.4.7/src/batou_ext/postfixadmin/
+-rw-r--r--   0 zagy       (501) staff       (20)     1997 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/__init__.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.105750 batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot/
+-rw-r--r--   0 zagy       (501) staff       (20)      751 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot/database.conf
+-rw-r--r--   0 zagy       (501) staff       (20)      447 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot/local.conf
+-rw-r--r--   0 zagy       (501) staff       (20)      584 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot.py
+-rw-r--r--   0 zagy       (501) staff       (20)      576 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/goceptnet.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.106798 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/
+-rw-r--r--   0 zagy       (501) staff       (20)      668 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/local.cf
+-rw-r--r--   0 zagy       (501) staff       (20)      369 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_alias
+-rw-r--r--   0 zagy       (501) staff       (20)      371 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_domains
+-rw-r--r--   0 zagy       (501) staff       (20)      376 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_mailboxes
+-rw-r--r--   0 zagy       (501) staff       (20)      457 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_sender_login
+-rw-r--r--   0 zagy       (501) staff       (20)     1541 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.107102 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfixadmin/
+-rw-r--r--   0 zagy       (501) staff       (20)      864 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postfixadmin/config.local.php
+-rw-r--r--   0 zagy       (501) staff       (20)      607 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postfixadmin/postgres.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5294 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/postgres.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3296 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/python.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5691 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/rabbitmq.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1268 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/redis.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.109884 batou_ext-2.4.7/src/batou_ext/resources/
+-rw-r--r--   0 zagy       (501) staff       (20)      541 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/cert.sh
+-rw-r--r--   0 zagy       (501) staff       (20)      388 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/check_systemd_unit.py
+-rw-r--r--   0 zagy       (501) staff       (20)      117 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/cron-wrapper.sh
+-rw-r--r--   0 zagy       (501) staff       (20)      200 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/geoip-update.sh
+-rw-r--r--   0 zagy       (501) staff       (20)     1552 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/http-watchdog.nix
+-rw-r--r--   0 zagy       (501) staff       (20)      203 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/journalbeat.nix
+-rw-r--r--   0 zagy       (501) staff       (20)      955 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/loader.c
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.110033 batou_ext-2.4.7/src/batou_ext/resources/mailhog/
+-rw-r--r--   0 zagy       (501) staff       (20)     1371 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/mailhog/mailhog.nix
+-rw-r--r--   0 zagy       (501) staff       (20)      946 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/mirror.conf
+-rw-r--r--   0 zagy       (501) staff       (20)     1898 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/oci-template.nix
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.110395 batou_ext-2.4.7/src/batou_ext/resources/php/
+-rw-r--r--   0 zagy       (501) staff       (20)      588 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/php/php-fpm.conf
+-rw-r--r--   0 zagy       (501) staff       (20)      296 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/php/php-fpm.sh
+-rw-r--r--   0 zagy       (501) staff       (20)    71038 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/php/php.ini
+-rw-r--r--   0 zagy       (501) staff       (20)      576 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/python.nix
+-rw-r--r--   0 zagy       (501) staff       (20)      118 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/rediscleanup.sh
+-rw-r--r--   0 zagy       (501) staff       (20)      560 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/setupEnv.sh
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.110582 batou_ext-2.4.7/src/batou_ext/resources/ssl/
+-rw-r--r--   0 zagy       (501) staff       (20)      597 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/ssl/local_certificate_check.sh
+-rw-r--r--   0 zagy       (501) staff       (20)      178 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/systemd.service
+-rw-r--r--   0 zagy       (501) staff       (20)      617 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/userenv.nix
+-rw-r--r--   0 zagy       (501) staff       (20)     6869 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/resources/watchdog-wrapper.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.110991 batou_ext-2.4.7/src/batou_ext/roundcube/
+-rw-r--r--   0 zagy       (501) staff       (20)     3456 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/roundcube/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4181 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/roundcube/config.inc.php
+-rw-r--r--   0 zagy       (501) staff       (20)      623 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/roundcube/postgres.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1525 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/run.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4745 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/s3.py
+-rw-r--r--   0 zagy       (501) staff       (20)     9400 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/s3_bootstrap.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3572 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/ssh.py
+-rw-r--r--   0 zagy       (501) staff       (20)    11133 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/ssl.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5258 2024-04-29 08:52:22.000000 batou_ext-2.4.7/src/batou_ext/versions.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-29 08:52:23.111173 batou_ext-2.4.7/src/batou_ext.egg-info/
+-rw-r--r--   0 zagy       (501) staff       (20)     4474 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/PKG-INFO
+-rw-r--r--   0 zagy       (501) staff       (20)     2695 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        1 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      171 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/entry_points.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        1 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/not-zip-safe
+-rw-r--r--   0 zagy       (501) staff       (20)      153 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/requires.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       10 2024-04-29 08:52:23.000000 batou_ext-2.4.7/src/batou_ext.egg-info/top_level.txt
```

### Comparing `batou_ext-2.4.6/CHANGES.md` & `batou_ext-2.4.7/CHANGES.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,19 @@
 
+## 2.4.7 (2024-04-29)
+
+
+* Added component `batou_ext.http.HTTPServiceWatchdog` that adds a check to a systemd unit
+  whether a given URL is reachable (e.g. a `/health` endpoint). If the URL cannot be reached within
+  a certain interval, the service will be restarted. Further details are documented in the
+  docstring.
+
+- Fix `SymlinkAndCleanup` async delete and allow custom extra arguments to `systemd run`.
+
+
 ## 2.4.6 (2024-04-23)
 
 
 - OCI: Support registries where the docker login is different than the registry used in referencing containers.
 
 - OCI: Improve change detection of remote images (required for docker.io)
```

### Comparing `batou_ext-2.4.6/LICENSE.txt` & `batou_ext-2.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/PKG-INFO` & `batou_ext-2.4.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 Metadata-Version: 2.1
 Name: batou_ext
-Version: 2.4.6
+Version: 2.4.7
 Summary: A library of components for batou.
 Home-page: https://github.com/flyingcircusio/batou_ext
 Author: Flying Circus <support@flyingcircus.io>
 Author-email: support@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: batou>=2.3b4
+Requires-Dist: pyaml
+Requires-Dist: setuptools
+Requires-Dist: six
+Requires-Dist: InquirerPy
 Provides-Extra: test
+Requires-Dist: boto3; extra == "test"
+Requires-Dist: passlib>=1.7; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: version-select
+Requires-Dist: InquirerPy; extra == "version-select"
 Provides-Extra: s3-bootstrap
-License-File: LICENSE.txt
+Requires-Dist: boto3; extra == "s3-bootstrap"
+Requires-Dist: InquirerPy; extra == "s3-bootstrap"
 
 # batou_ext - a library of components for batou
 
 `batou_ext` master is now supporting Python3 and is depending on batou2. If you still want to use batou_ext with batou 1.x running Python2 you still can use the [batou1-py2](https://github.com/flyingcircusio/batou_ext/tree/batou1-py2) branch.
 
 To add `batou_ext` to your deployment, add a like to the `requirements.txt` of your batou deployment::
 
@@ -54,14 +66,25 @@
 creating an [S3 bucket](https://wiki.flyingcircus.io/S3) and - if needed -
 an access keypair and lifecycle rules.
 
 On an activated virtualenv this can be tested with `python -m batou_ext.s3_bootstrap`.
 
 
 
+## 2.4.7 (2024-04-29)
+
+
+* Added component `batou_ext.http.HTTPServiceWatchdog` that adds a check to a systemd unit
+  whether a given URL is reachable (e.g. a `/health` endpoint). If the URL cannot be reached within
+  a certain interval, the service will be restarted. Further details are documented in the
+  docstring.
+
+- Fix `SymlinkAndCleanup` async delete and allow custom extra arguments to `systemd run`.
+
+
 ## 2.4.6 (2024-04-23)
 
 
 - OCI: Support registries where the docker login is different than the registry used in referencing containers.
 
 - OCI: Improve change detection of remote images (required for docker.io)
```

### Comparing `batou_ext-2.4.6/README.md` & `batou_ext-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/setup.py` & `batou_ext-2.4.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def project_path(*names):
     return os.path.join(*names)
 
 
 setup(
     name="batou_ext",
-    version="2.4.6",
+    version="2.4.7",
     install_requires=[
         "batou >= 2.3b4",
         "pyaml",
         "setuptools",
         "six",
         "InquirerPy",
     ],
```

### Comparing `batou_ext-2.4.6/src/batou_ext/acl.py` & `batou_ext-2.4.7/src/batou_ext/acl.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/archive.py` & `batou_ext-2.4.7/src/batou_ext/archive.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/config.py` & `batou_ext-2.4.7/src/batou_ext/config.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/cron.py` & `batou_ext-2.4.7/src/batou_ext/cron.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/fcio.py` & `batou_ext-2.4.7/src/batou_ext/fcio.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/file.py` & `batou_ext-2.4.7/src/batou_ext/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,19 @@
     _current_link = None
     _last_link = None
 
     prefix = None
 
     use_systemd_run_async_cleanup = False
 
+    # Use extra args to e.g. limit IOPS:
+    #     ["--property=IOReadIOPSMax=/dev/vda 100",
+    #      "--property=IOWriteIOPSMax=/dev/vda 100"]
+    systemd_extra_args: list = None
+
     def configure(self):
         self._current_link = (
             f"{self.prefix}-current" if self.prefix else "current"
         )
         self._last_link = f"{self.prefix}-last" if self.prefix else "last"
         self.dir = os.path.dirname(self.current)
         self.current = os.path.basename(self.current)
@@ -96,37 +101,39 @@
                     pass
 
                 batou.output.annotate("current -> {}".format(self.current))
                 os.symlink(self.current, self._current_link)
                 if current:
                     batou.output.annotate("last -> {}".format(current))
                     os.symlink(current, self._last_link)
+
             candidates = self._list_removals()
-            if self.use_systemd_run_async_cleanup:
-                # spawns a IOPS limited systemd-run cleanup job
+            if not candidates:
+                batou.output.annotate("Nothing to remove.")
+            elif self.use_systemd_run_async_cleanup:
+                # Spawns an systemd-run cleanup job with custom args.
+                candidates = [os.path.join(self.dir, c) for c in candidates]
+                rm_cmd = [
+                    "rm",
+                    "-rfv",
+                    *candidates,  # consider: ARG_MAX is limited
+                ]
+                extra_args = self.systemd_extra_args or []
+                cmd = [
+                    "systemd-run",
+                    "--unit",
+                    f"batou-cleanup-{self.prefix}",
+                    "--user",
+                    *extra_args,
+                    *rm_cmd,
+                ]
+                batou.output.annotate(f"Removing: {candidates}")
+                batou.output.annotate(f"    {cmd}")
                 try:
-                    batou.output.annotate(
-                        "Removing using systemd-run: {}".format(candidates)
-                    )
-                    rm_cmd = [
-                        "rm",
-                        "-rf",
-                        *candidates,  # consider: ARG_MAX is limited
-                    ]
-                    subprocess.run(
-                        [
-                            "systemd-run",
-                            "--unit",
-                            f"batou-cleanup-{self.prefix}",
-                            "--property=IOReadIOPSMax=100",
-                            "--property=IOWriteIOPSMax=100",
-                            *rm_cmd,
-                        ],
-                        check=True,
-                    )
+                    subprocess.run(cmd, check=True)
                 except subprocess.CalledProcessError as e:
                     batou.output.error(f"Failed to remove: {e}")
             else:
                 for el in candidates:
                     batou.output.annotate("Removing: {}".format(el))
                     try:
                         if os.path.isdir(el):
```

### Comparing `batou_ext-2.4.6/src/batou_ext/geoip.py` & `batou_ext-2.4.7/src/batou_ext/geoip.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/git.py` & `batou_ext-2.4.7/src/batou_ext/git.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/htpasswd.py` & `batou_ext-2.4.7/src/batou_ext/htpasswd.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/jenkins.py` & `batou_ext-2.4.7/src/batou_ext/jenkins.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/journalbeat.py` & `batou_ext-2.4.7/src/batou_ext/journalbeat.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/keypair.py` & `batou_ext-2.4.7/src/batou_ext/keypair.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/mail.py` & `batou_ext-2.4.7/src/batou_ext/mail.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/memcached.py` & `batou_ext-2.4.7/src/batou_ext/memcached.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/mirror.py` & `batou_ext-2.4.7/src/batou_ext/mirror.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/mysql.py` & `batou_ext-2.4.7/src/batou_ext/mysql.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/nfs.py` & `batou_ext-2.4.7/src/batou_ext/nfs.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/nix.py` & `batou_ext-2.4.7/src/batou_ext/nix.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/nixos.py` & `batou_ext-2.4.7/src/batou_ext/nixos.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/oci.py` & `batou_ext-2.4.7/src/batou_ext/oci.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/php.py` & `batou_ext-2.4.7/src/batou_ext/php.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/postfixadmin/__init__.py` & `batou_ext-2.4.7/src/batou_ext/postfixadmin/__init__.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot/database.conf` & `batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot/database.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot.py` & `batou_ext-2.4.7/src/batou_ext/postfixadmin/dovecot.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/postfixadmin/goceptnet.py` & `batou_ext-2.4.7/src/batou_ext/postfixadmin/goceptnet.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/local.cf` & `batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix/local.cf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix.py` & `batou_ext-2.4.7/src/batou_ext/postfixadmin/postfix.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/postfixadmin/postfixadmin/config.local.php` & `batou_ext-2.4.7/src/batou_ext/postfixadmin/postfixadmin/config.local.php`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/postfixadmin/postgres.py` & `batou_ext-2.4.7/src/batou_ext/postfixadmin/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/postgres.py` & `batou_ext-2.4.7/src/batou_ext/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/python.py` & `batou_ext-2.4.7/src/batou_ext/python.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/rabbitmq.py` & `batou_ext-2.4.7/src/batou_ext/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/redis.py` & `batou_ext-2.4.7/src/batou_ext/redis.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/resources/cert.sh` & `batou_ext-2.4.7/src/batou_ext/resources/cert.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/resources/loader.c` & `batou_ext-2.4.7/src/batou_ext/resources/loader.c`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/resources/mailhog/mailhog.nix` & `batou_ext-2.4.7/src/batou_ext/resources/mailhog/mailhog.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/resources/mirror.conf` & `batou_ext-2.4.7/src/batou_ext/resources/mirror.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/resources/oci-template.nix` & `batou_ext-2.4.7/src/batou_ext/resources/oci-template.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/resources/php/php-fpm.conf` & `batou_ext-2.4.7/src/batou_ext/resources/php/php-fpm.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/resources/php/php.ini` & `batou_ext-2.4.7/src/batou_ext/resources/php/php.ini`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/resources/python.nix` & `batou_ext-2.4.7/src/batou_ext/resources/python.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/resources/setupEnv.sh` & `batou_ext-2.4.7/src/batou_ext/resources/setupEnv.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/resources/ssl/local_certificate_check.sh` & `batou_ext-2.4.7/src/batou_ext/resources/ssl/local_certificate_check.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/resources/userenv.nix` & `batou_ext-2.4.7/src/batou_ext/resources/userenv.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/roundcube/__init__.py` & `batou_ext-2.4.7/src/batou_ext/roundcube/__init__.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/roundcube/config.inc.php` & `batou_ext-2.4.7/src/batou_ext/roundcube/config.inc.php`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/roundcube/postgres.py` & `batou_ext-2.4.7/src/batou_ext/roundcube/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/run.py` & `batou_ext-2.4.7/src/batou_ext/run.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/s3.py` & `batou_ext-2.4.7/src/batou_ext/s3.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/s3_bootstrap.py` & `batou_ext-2.4.7/src/batou_ext/s3_bootstrap.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/ssh.py` & `batou_ext-2.4.7/src/batou_ext/ssh.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/ssl.py` & `batou_ext-2.4.7/src/batou_ext/ssl.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext/versions.py` & `batou_ext-2.4.7/src/batou_ext/versions.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.6/src/batou_ext.egg-info/PKG-INFO` & `batou_ext-2.4.7/src/batou_ext.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 Metadata-Version: 2.1
-Name: batou-ext
-Version: 2.4.6
+Name: batou_ext
+Version: 2.4.7
 Summary: A library of components for batou.
 Home-page: https://github.com/flyingcircusio/batou_ext
 Author: Flying Circus <support@flyingcircus.io>
 Author-email: support@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: batou>=2.3b4
+Requires-Dist: pyaml
+Requires-Dist: setuptools
+Requires-Dist: six
+Requires-Dist: InquirerPy
 Provides-Extra: test
+Requires-Dist: boto3; extra == "test"
+Requires-Dist: passlib>=1.7; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: version-select
+Requires-Dist: InquirerPy; extra == "version-select"
 Provides-Extra: s3-bootstrap
-License-File: LICENSE.txt
+Requires-Dist: boto3; extra == "s3-bootstrap"
+Requires-Dist: InquirerPy; extra == "s3-bootstrap"
 
 # batou_ext - a library of components for batou
 
 `batou_ext` master is now supporting Python3 and is depending on batou2. If you still want to use batou_ext with batou 1.x running Python2 you still can use the [batou1-py2](https://github.com/flyingcircusio/batou_ext/tree/batou1-py2) branch.
 
 To add `batou_ext` to your deployment, add a like to the `requirements.txt` of your batou deployment::
 
@@ -54,14 +66,25 @@
 creating an [S3 bucket](https://wiki.flyingcircus.io/S3) and - if needed -
 an access keypair and lifecycle rules.
 
 On an activated virtualenv this can be tested with `python -m batou_ext.s3_bootstrap`.
 
 
 
+## 2.4.7 (2024-04-29)
+
+
+* Added component `batou_ext.http.HTTPServiceWatchdog` that adds a check to a systemd unit
+  whether a given URL is reachable (e.g. a `/health` endpoint). If the URL cannot be reached within
+  a certain interval, the service will be restarted. Further details are documented in the
+  docstring.
+
+- Fix `SymlinkAndCleanup` async delete and allow custom extra arguments to `systemd run`.
+
+
 ## 2.4.6 (2024-04-23)
 
 
 - OCI: Support registries where the docker login is different than the registry used in referencing containers.
 
 - OCI: Improve change detection of remote images (required for docker.io)
```

### Comparing `batou_ext-2.4.6/src/batou_ext.egg-info/SOURCES.txt` & `batou_ext-2.4.7/src/batou_ext.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -59,23 +59,25 @@
 src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_mailboxes
 src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_sender_login
 src/batou_ext/postfixadmin/postfixadmin/config.local.php
 src/batou_ext/resources/cert.sh
 src/batou_ext/resources/check_systemd_unit.py
 src/batou_ext/resources/cron-wrapper.sh
 src/batou_ext/resources/geoip-update.sh
+src/batou_ext/resources/http-watchdog.nix
 src/batou_ext/resources/journalbeat.nix
 src/batou_ext/resources/loader.c
 src/batou_ext/resources/mirror.conf
 src/batou_ext/resources/oci-template.nix
 src/batou_ext/resources/python.nix
 src/batou_ext/resources/rediscleanup.sh
 src/batou_ext/resources/setupEnv.sh
 src/batou_ext/resources/systemd.service
 src/batou_ext/resources/userenv.nix
+src/batou_ext/resources/watchdog-wrapper.py
 src/batou_ext/resources/mailhog/mailhog.nix
 src/batou_ext/resources/php/php-fpm.conf
 src/batou_ext/resources/php/php-fpm.sh
 src/batou_ext/resources/php/php.ini
 src/batou_ext/resources/ssl/local_certificate_check.sh
 src/batou_ext/roundcube/__init__.py
 src/batou_ext/roundcube/config.inc.php
```

