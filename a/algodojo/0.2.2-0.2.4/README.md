# Comparing `tmp/algodojo-0.2.2.tar.gz` & `tmp/algodojo-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algodojo-0.2.2.tar", last modified: Sun Aug  6 11:12:35 2023, max compression
+gzip compressed data, was "algodojo-0.2.4.tar", last modified: Mon Apr 29 12:13:15 2024, max compression
```

## Comparing `algodojo-0.2.2.tar` & `algodojo-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:12:35.981704 algodojo-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-08-06 11:11:38.000000 algodojo-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-06 11:11:38.000000 algodojo-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-06 11:12:35.977704 algodojo-0.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:12:35.969704 algodojo-0.2.2/algodojo/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-06 11:12:18.000000 algodojo-0.2.2/algodojo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:12:35.977704 algodojo-0.2.2/algodojo/base/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-06 11:12:18.000000 algodojo-0.2.2/algodojo/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-08-06 11:12:20.000000 algodojo-0.2.2/algodojo/base/auth.cp310-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   107520 2023-08-06 11:12:18.000000 algodojo-0.2.2/algodojo/base/auth.cp311-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   116224 2023-08-06 11:12:26.000000 algodojo-0.2.2/algodojo/base/auth.cp36-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   107520 2023-08-06 11:12:25.000000 algodojo-0.2.2/algodojo/base/auth.cp37-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-08-06 11:12:23.000000 algodojo-0.2.2/algodojo/base/auth.cp38-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-08-06 11:12:22.000000 algodojo-0.2.2/algodojo/base/auth.cp39-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   155944 2023-08-06 11:12:32.000000 algodojo-0.2.2/algodojo/base/auth.cpython-36m-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)   190312 2023-08-06 11:12:31.000000 algodojo-0.2.2/algodojo/base/auth.cpython-37m-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)   189944 2023-08-06 11:12:29.000000 algodojo-0.2.2/algodojo/base/auth.cpython-38-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)   189552 2023-08-06 11:12:28.000000 algodojo-0.2.2/algodojo/base/auth.cpython-39-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)   135680 2023-08-06 11:12:20.000000 algodojo-0.2.2/algodojo/base/report.cp310-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-08-06 11:12:18.000000 algodojo-0.2.2/algodojo/base/report.cp311-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   151040 2023-08-06 11:12:26.000000 algodojo-0.2.2/algodojo/base/report.cp36-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   138752 2023-08-06 11:12:25.000000 algodojo-0.2.2/algodojo/base/report.cp37-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   136192 2023-08-06 11:12:23.000000 algodojo-0.2.2/algodojo/base/report.cp38-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   135680 2023-08-06 11:12:22.000000 algodojo-0.2.2/algodojo/base/report.cp39-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   203680 2023-08-06 11:12:32.000000 algodojo-0.2.2/algodojo/base/report.cpython-36m-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)   221408 2023-08-06 11:12:31.000000 algodojo-0.2.2/algodojo/base/report.cpython-37m-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)   220912 2023-08-06 11:12:29.000000 algodojo-0.2.2/algodojo/base/report.cpython-38-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)   220720 2023-08-06 11:12:28.000000 algodojo-0.2.2/algodojo/base/report.cpython-39-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)   488960 2023-08-06 11:12:20.000000 algodojo-0.2.2/algodojo/ib.cp310-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   492544 2023-08-06 11:12:18.000000 algodojo-0.2.2/algodojo/ib.cp311-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   517120 2023-08-06 11:12:26.000000 algodojo-0.2.2/algodojo/ib.cp36-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   491008 2023-08-06 11:12:25.000000 algodojo-0.2.2/algodojo/ib.cp37-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   491008 2023-08-06 11:12:24.000000 algodojo-0.2.2/algodojo/ib.cp38-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   488960 2023-08-06 11:12:22.000000 algodojo-0.2.2/algodojo/ib.cp39-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   681880 2023-08-06 11:12:32.000000 algodojo-0.2.2/algodojo/ib.cpython-36m-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)   715936 2023-08-06 11:12:31.000000 algodojo-0.2.2/algodojo/ib.cpython-37m-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)   715712 2023-08-06 11:12:29.000000 algodojo-0.2.2/algodojo/ib.cpython-38-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)   715328 2023-08-06 11:12:28.000000 algodojo-0.2.2/algodojo/ib.cpython-39-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)    54394 2023-08-06 11:12:18.000000 algodojo-0.2.2/algodojo/ib_backup_20230322.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:12:35.973704 algodojo-0.2.2/algodojo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-06 11:12:35.000000 algodojo-0.2.2/algodojo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-06 11:12:35.000000 algodojo-0.2.2/algodojo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 11:12:35.000000 algodojo-0.2.2/algodojo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-06 11:12:35.000000 algodojo-0.2.2/algodojo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 11:12:35.000000 algodojo-0.2.2/algodojo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 11:12:35.981704 algodojo-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-06 11:11:38.000000 algodojo-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:13:15.187936 algodojo-0.2.4/
+-rw-rw-rw-   0        0        0    40679 2024-04-29 12:11:38.000000 algodojo-0.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       33 2024-04-29 12:11:38.000000 algodojo-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1051 2024-04-29 12:13:15.187936 algodojo-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2024-04-29 12:11:38.000000 algodojo-0.2.4/README.md
+-rw-rw-rw-   0        0        0      669 2024-04-29 12:11:38.000000 algodojo-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 12:13:15.187936 algodojo-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 12:13:15.172316 algodojo-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:13:15.172316 algodojo-0.2.4/src/algodojo/
+-rw-rw-rw-   0        0        0      138 2024-04-29 12:11:38.000000 algodojo-0.2.4/src/algodojo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:13:15.172316 algodojo-0.2.4/src/algodojo/base/
+-rw-rw-rw-   0        0        0       64 2024-04-29 12:11:38.000000 algodojo-0.2.4/src/algodojo/base/__init__.py
+-rw-rw-rw-   0        0        0    11536 2024-04-29 12:11:38.000000 algodojo-0.2.4/src/algodojo/base/auth.py
+-rw-rw-rw-   0        0        0    17568 2024-04-29 12:11:38.000000 algodojo-0.2.4/src/algodojo/base/report.py
+-rw-rw-rw-   0        0        0    57539 2024-04-29 12:11:38.000000 algodojo-0.2.4/src/algodojo/ib.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:13:15.187936 algodojo-0.2.4/src/algodojo.egg-info/
+-rw-rw-rw-   0        0        0     1051 2024-04-29 12:13:15.000000 algodojo-0.2.4/src/algodojo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-04-29 12:13:15.000000 algodojo-0.2.4/src/algodojo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:13:15.000000 algodojo-0.2.4/src/algodojo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-04-29 12:13:15.000000 algodojo-0.2.4/src/algodojo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-29 12:13:15.000000 algodojo-0.2.4/src/algodojo.egg-info/top_level.txt
```

### Comparing `algodojo-0.2.2/LICENSE.txt` & `algodojo-0.2.4/LICENSE.txt`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-By using AlgoDojo (we, us, our) services (website, product, forums) you agree to the following terms of use.
-Introduction
-The website located at https://www.algodojo.com/ (the “Site”) is a copyrighted work belonging to Dojo Technologies Limited (“Company”, “us”, “our”, and “we”). Certain features of the Site may be subject to additional guidelines, terms, or rules, which will be posted on the Site in connection with such features, including, without limitation the Company’s Privacy Policy, the Platform Services Agreement, and the Subscription and Sublicense Agreement, all of which are incorporated by reference to these Terms. All such additional terms, guidelines, and rules are incorporated by reference into these Terms.
-THESE TERMS OF USE (THESE “TERMS”) SET FORTH THE LEGALLY BINDING TERMS AND CONDITIONS THAT GOVERN YOUR USE OF THE SITE. BY ACCESSING OR USING THE SITE, YOU ARE ACCEPTING THESE TERMS (ON BEHALF OF YOURSELF OR THE ENTITY THAT YOU REPRESENT), AND YOU REPRESENT AND WARRANT THAT YOU HAVE THE RIGHT, AUTHORITY, AND CAPACITY TO ENTER INTO THESE TERMS (ON BEHALF OF YOURSELF OR THE ENTITY THAT YOU REPRESENT). YOU MAY NOT ACCESS OR USE THE SITE OR ACCEPT THE TERMS IF YOU ARE NOT AT LEAST 18 YEARS OLD. IF YOU DO NOT AGREE WITH ALL OF THE PROVISIONS OF THESE TERMS, DO NOT ACCESS AND/OR USE THE SITE.
-THESE TERMS REQUIRE THE USE OF ARBITRATION (SECTION 10.2) ON AN INDIVIDUAL BASIS TO RESOLVE DISPUTES, RATHER THAN JURY TRIALS OR CLASS ACTIONS, AND ALSO LIMIT THE REMEDIES AVAILABLE TO YOU IN THE EVENT OF A DISPUTE.
-1.0 Accounts
-	1.1 Account Creation
-In order to use certain features of the Site, you must register for an account (“Account”) and provide certain information about yourself as prompted by the account registration form. You represent and warrant that: (a) all required registration information you submit is truthful and accurate; (b) you will maintain the accuracy of such information. You may delete your Account at any time, for any reason, by following the instructions on the Site. Company may suspend or terminate your Account in accordance with Section 8.
-	1.2 Account Responsibilities
-You are responsible for maintaining the confidentiality of your Account login information and are fully responsible for all activities that occur under your Account. You agree to immediately notify Company of any unauthorized use, or suspected unauthorized use of your Account or any other breach of security. Company cannot and will not be liable for any loss or damage arising from your failure to comply with the above requirements.
-	1.3 Non-Solicitation
-You are prohibited from soliciting or recruit any other users or members of the Site, including Alpha Stream Authors, for any reason, unless you have requested and received permission to solicit or recruit in writing from the Company. . This prohibition includes a prohibition against soliciting or recruiting users of the Site, including Alpha Stream Authors, to become members of competitive sites and services. IThis includes (but is not limited to) soliciting Alpha Stream Authors to make their methods, devices, models, algorithms or other automated processes available at services or sites outside of the Site. If you violate this policy, the Company reserves the right to terminate your Account without notice and to take legal action to recover lost revenues you have stolen from us, plus applicable damages. By using the Site, you specifically acknowledge that you agree to this prohibition.
-2.0 Access to the Site
-	2.1 License.
-Subject to these Terms, Company grants you a non-transferable, non-exclusive, revocable, limited license to use and access the Site solely for your own personal use.
-	2.2 Certain Restrictions.
-The rights granted to you in these Terms are subject to the following restrictions: (a) you shall not license, sell, rent, lease, transfer, assign, distribute, host, or otherwise commercially exploit the Site, whether in whole or in part, or any content displayed on the Site; (b) you shall not share with others, resell or redistribute any of the Site’s dataset (“Data”). The Data is only for internal use. You may not publish, disseminate, re-distribute or share the Data, or any part thereof, or any derivative data that allows reverse engineering of part or all of the Data, with anyone else. You may not offer the Data, or any part thereof, for sale, rent, license or commercial redistribution. Any sharing or distribution by you of your access privileges or of the Data may result in cancellation of your use of the Data without refund. Data can only be used within the AlgoDojo software. You are prohibited from downloading or exporting the data outside the AlgoDojo software; (cb) you shall not modify, make derivative works of, disassemble, reverse compile or reverse engineer any part of the Site; (dc) you shall not access the Site in order to build a similar or competitive website, product, or service; and (ed) except as expressly stated herein, no part of the Site may be copied, reproduced, distributed, republished, downloaded, displayed, posted or transmitted in any form or by any means. Unless otherwise indicated, any future release, update, or other addition to functionality of the Site shall be subject to these Terms. All copyright and other proprietary notices on the Site (or on any content displayed on the Site) must be retained on all copies thereof.
-
-
-	2.3 Modification.
-Company reserves the right, at any time, to modify, suspend, or discontinue the Site (in whole or in part) with or without notice to you. You agree that Company will not be liable to you or to any third party for any modification, suspension, or discontinuation of the Site or any part thereof.
-	2.4 No Support or Maintenance.
-You acknowledge and agree that Company will have no obligation to provide you with any support or maintenance in connection with the Site, but the Company reserves the right, on a case by case basis, to provide support or maintenance as the need arises.
-	2.5 Ownership.
-Subject to the terms hereof, and excluding any Non-Public User Content that you may provide (defined below in Section 3.0), you acknowledge that all the intellectual property rights, including copyrights, patents, trademarks, and trade secrets, in the Site and its content, whether provided by you, the Company, or Company’s suppliers, are owned by Company or Company’s suppliers. Neither these Terms (nor your access to the Site) transfers to you or any third party any rights, title or interest in or to such intellectual property rights, except for the limited access rights expressly set forth in Section 2.1. Company and its suppliers reserve all rights not granted in these Terms. There are no implied licenses granted under these Terms.
-3.0 User Content
-	3.1 User Content and Alpha Stream Content.
-“User Content” means any and all information submitted to or communicated through the Site. You are solely responsible for your User Content. You assume all risks associated with use of your User Content, including any reliance on its accuracy, completeness or usefulness by others, or any disclosure of your User Content that personally identifies you or any third party. You hereby represent and warrant that your User Content do not violate our Acceptable Use Policy (defined in Section 3.3). You may not represent or imply to others that your User Content is in any way provided, sponsored or endorsed by Company. Because you alone are responsible for your User Content, you may expose yourself to liability if, for example, your User Content violates the Acceptable Use Policy. Company is not obligated to backup any User Content, and your User Content a may be deleted at any time without prior notice. You are solely responsible for creating and maintaining your own backup copies of your User Content if you desire.
-	3.2 Non-Public User Content 
-User Content includes Non-Public User Content and Public User Content. Non-Public User Content is User Content that you communicate directly to one or more other users of the Site or that is not accessible without being logged into your account. Public User Content is all other User Content. When you submit Public User Content, you agree that all rights in such Public User Content are owned by the Company per Section 2.5 above and agree to take reasonable steps, if any, necessary to effectuate such ownership.
-	3.3 Acceptable Use Policy. 
-The following terms constitute our “Acceptable Use Policy”:
-(a) You agree not to use the Site to collect, upload, transmit, display, or distribute any User Content (i) that violates any third-party right, including any copyright, trademark, patent, trade secret, moral right, privacy right, right of publicity, or any other intellectual property or proprietary right; (ii) that is unlawful, harassing, abusive, tortious, threatening, harmful, invasive of another’s privacy, vulgar, defamatory, false, intentionally misleading, trade libelous, pornographic, obscene, patently offensive, promotes racism, bigotry, hatred, or physical harm of any kind against any group or individual or is otherwise objectionable; (iii) that is harmful to minors in any way; or (iv) that is in violation of any law, regulation, or obligations or restrictions imposed by any third party.
-(b) In addition, you agree not to: (i) upload, transmit, or distribute to or through the Site any computer viruses, worms, or any software intended to damage or alter a computer system or data; (ii ) share with others, resell or redistribute any of the Site’s historical market trading data; (iii) send through the Site unsolicited or unauthorized advertising, promotional materials, junk mail, spam, chain letters, pyramid schemes, or any other form of duplicative or unsolicited messages, whether commercial or otherwise; (ivii) use the Site to harvest, collect, gather or assemble information or data regarding other users, including e-mail addresses, without their consent; (iv) interfere with, disrupt, or create an undue burden on servers or networks connected to the Site, or violate the regulations, policies or procedures of such networks; (vi) attempt to gain unauthorized access to the Site (or to other computer systems or networks connected to or used together with the Site), whether through password mining or any other means; (vii) harass or interfere with any other user’s use and enjoyment of the Site; or (viii) use software or automated agents or scripts to produce multiple accounts on the Site, or to generate automated searches, requests, or queries to (or to strip, scrape, or mine data from) the Site (provided, however, that we conditionally grant to the operators of public search engines revocable permission to use spiders to copy materials from the Site for the sole purpose of and solely to the extent necessary for creating publicly available searchable indices of the materials, but not caches or archives of such materials, subject to the parameters set forth in our robots.txt file).
-(c) In addition, you agree not to disparage any other user of the Site to any third party based on interactions through the Site.
-	3.4 Enforcement.
-We reserve the right (but have no obligation except in rare circumstances) to review any User Content, and to investigate and/or take appropriate action against you in our sole discretion if you violate the Acceptable Use Policy or any other provision of these Terms or otherwise create liability for us or any other person. Such action may include removing or modifying your User Content, terminating your Account in accordance with Section 8, and/or reporting you to law enforcement authorities.
-	3.5 Feedback.
-If you provide Company with any feedback or suggestions regarding the Site (“Feedback”), you hereby assign to Company all rights in such Feedback and agree that Company shall have the right to use and fully exploit such Feedback and related information in any manner it deems appropriate. Company will treat any Feedback you provide to Company as non-confidential and non-proprietary. You agree that you will not submit to Company any information or ideas that you consider to be confidential or proprietary.
-	3.6 No Investment Advice; Not an Investment Advisor; Not a Broker-Dealer.
-The Company is not an investment advisory service, nor is it a registered investment advisor or broker-dealer and does not purport to tell or suggest the value of any securities or which securities customers should buy or sell for themselves. The users of the Site may hold positions in the stocks or industries discussed here. You understand and acknowledge that there is a very high degree of risk involved in trading securities. The Company, the users, the authors, the publisher, and all affiliates of the Site assume no responsibility or liability for your trading and investment results. Factual statements or publications on the Site are made as of the date stated and are subject to change without notice. It should not be assumed that the methods, techniques, or indicators presented in these products will be profitable or that they will not result in losses. Past results of any individual trader or trading system published by on the Site are not indicative of future returns by that trader or system, and are not indicative of future returns which be realized by you. In addition, the indicators, strategies, columns, articles and all other features of the Site are provided for informational and educational purposes only and should not be construed as investment advice. Examples presented on the site are for educational purposes only. Such set-ups are not solicitations of any order to buy or sell. Accordingly, you should not rely solely on the Information in making any investment. You should always check with your licensed financial advisor and tax advisor to determine the suitability of any investment.
-	3.7 Live Trading Risks.
-By using the Site, you acknowledge and agree that live algorithmic trading has various risks and the Company shall not have any liability for any losses incurred through using the Site, such risks included, without limitation:
-(a) Design risks; errors in data, incorrect assumptions, logical program errors. Even if you designed a perfect strategy, past performance is no guarantee of future results.
-(b) Data risk; Your use of, or inability to use, the Data is at your sole risk. AlgoDojo make no warranty about the accuracy or quality of the Data and do not guarantee, represent, or warrant that your use of the data will be uninterrupted, timely, secure, reliable, complete, accurate, or error-free. Data may be delayed, inaccurate, or contain errors or omissions, and AlgoDojo will have no liability with respect thereto. AlgoDojo is not responsible for the Data. All data is provided “as is” and neither party makes any other warranties, express or implied, including any implied warranty of non-infringement, accuracy, merchantability, durability, or fitness for a particular purpose. 
-
-(cb) Loss of internet connectivity; resulting in disconnections from brokerage, trades not placed, not seeing the results of algorithm, orders failing to be placed.
-(dc) Poor design of algorithm; resulting in runaway strategies, machine gun orders, run-time errors halting program operation, failure to trade when expected, termination of the algorithm.
-(ed) Unexpected market conditions; resulting in poor fill prices, rapid losses (flash crashes), late exchange openings.
-(fe) Live Ddata feed issues; broken, dirty, delayed or intermittent data connections causing algorithm errors. This includes data inaccuracies (exchanges sometimes publish bad/fictional trades). 
-(gf) Execution issues; orders submissions, updates and cancellations could be rejected or delayed. Trades could be disallowed by authorities without warning.
-(hg) Malicious activities; criminal activity could cause your algorithm to fail or your brokerage account to become compromised, leaking personal information, intellectual property or theft of your funds.
-(ih) These events can cause the loss of all funds and holdings in your brokerage account. Algorithmic trading losses can occur faster than in manual trading and you should consult an investment professional to discuss these risks. You should continually monitor the operation of a live trading algorithm to ensure it is running properly.
-EVERY TIME YOU USE THE SITE YOU AGREE THAT IN ALL CASES THE COMPANY BEARS NO RESPONSIBILITY FOR LOSSES INCURRED, AND OFFERS NO GUARANTEES OR EXPECTATIONS ON YOUR ALGORITHM PERFORMANCE OR STABILITY.
-4.0 Indemification
-	You agree to indemnify and hold Company (and its officers, employees, and agents) harmless, including costs and attorneys’ fees, from any claim or demand made by any third party due to or arising out of (a) your use of the Site, (b) your violation of these Terms, (c) your violation of applicable laws or regulations or (d) your User Content. Company reserves the right, at your expense, to assume the exclusive defense and control of any matter for which you are required to indemnify us, and you agree to cooperate with our defense of these claims. You agree not to settle any matter without the prior written consent of Company. Company will use reasonable efforts to notify you of any such claim, action or proceeding upon becoming aware of it.
-5.0 Third Party Links & Ads; Other Users
-	5.1 Third-Party Links & Ads.
-The Site may contain links to third-party websites and services, and/or display advertisements for third parties (collectively, “Third-Party Links & Ads”). Such Third-Party Links & Ads are not under the control of Company, and Company is not responsible for any Third-Party Links & Ads. Company provides access to these Third-Party Links & Ads only as a convenience to you, and does not review, approve, monitor, endorse, warrant, or make any representations with respect to Third-Party Links & Ads. You use all Third-Party Links & Ads at your own risk, and should apply a suitable level of caution and discretion in doing so. When you click on any of the Third-Party Links & Ads, the applicable third party’s terms and policies apply, including the third party’s privacy and data gathering practices. You should make whatever investigation you feel necessary or appropriate before proceeding with any transaction in connection with such Third-Party Links & Ads.
-	5.2 Other Users.
-Each Site user is solely responsible for any and all of its own User Content. Because we do not control User Content, you acknowledge and agree that we are not responsible for any User Content, whether provided by you or by others. We make no guarantees regarding the accuracy, currency, suitability, or quality of any User Content. Your interactions with other Site users are solely between you and such users. You agree that Company will not be responsible for any loss or damage incurred as the result of any such interactions. If there is a dispute between you and any Site user, we are under no obligation to become involved.
-	5.3 Release.
-You hereby release and forever discharge the Company (and our officers, employees, agents, successors, and assigns) from, and hereby waive and relinquish, each and every past, present and future dispute, claim, controversy, demand, right, obligation, liability, action and cause of action of every kind and nature (including personal injuries, death, and property damage), that has arisen or arises directly or indirectly out of, or that relates directly or indirectly to, the Site (including any interactions with, or act or omission of, other Site users or any Third-Party Links & Ads). IF YOU ARE A CALIFORNIA RESIDENT, YOU HEREBY WAIVE CALIFORNIA CIVIL CODE SECTION 1542 IN CONNECTION WITH THE FOREGOING, WHICH STATES: “A GENERAL RELEASE DOES NOT EXTEND TO CLAIMS WHICH THE CREDITOR DOES NOT KNOW OR SUSPECT TO EXIST IN HIS OR HER FAVOR AT THE TIME OF EXECUTING THE RELEASE, WHICH IF KNOWN BY HIM OR HER MUST HAVE MATERIALLY AFFECTED HIS OR HER SETTLEMENT WITH THE DEBTOR.”.
-6.0 Disclaimers.
-	THE SITE IS PROVIDED ON AN “AS-IS” AND “AS AVAILABLE” BASIS, AND COMPANY (AND OUR SUPPLIERS) EXPRESSLY DISCLAIM ANY AND ALL WARRANTIES AND CONDITIONS OF ANY KIND, WHETHER EXPRESS, IMPLIED, OR STATUTORY, INCLUDING ALL WARRANTIES OR CONDITIONS OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, TITLE, QUIET ENJOYMENT, ACCURACY, OR NON-INFRINGEMENT. WE (AND OUR SUPPLIERS) MAKE NO WARRANTY THAT THE SITE WILL MEET YOUR REQUIREMENTS, WILL BE AVAILABLE ON AN UNINTERRUPTED, TIMELY, SECURE, OR ERROR-FREE BASIS, OR WILL BE ACCURATE, RELIABLE, FREE OF VIRUSES OR OTHER HARMFUL CODE, COMPLETE, LEGAL, OR SAFE. IF APPLICABLE LAW REQUIRES ANY WARRANTIES WITH RESPECT TO THE SITE, ALL SUCH WARRANTIES ARE LIMITED IN DURATION TO NINETY (90) DAYS FROM THE DATE OF FIRST USE.
-SOME JURISDICTIONS DO NOT ALLOW THE EXCLUSION OF IMPLIED WARRANTIES, SO THE ABOVE EXCLUSION MAY NOT APPLY TO YOU. SOME JURISDICTIONS DO NOT ALLOW LIMITATIONS ON HOW LONG AN IMPLIED WARRANTY LASTS, SO THE ABOVE LIMITATION MAY NOT APPLY TO YOU.
-THE COMPANY PROVIDES THE CONTENT OF THE SITE FOR INFORMATIONAL, EDUCATIONAL AND NONCOMMERCIAL PURPOSES ONLY. SINCE EACH INDIVIDUAL'S SITUATION IS UNIQUE, A QUALIFIED PROFESSIONAL SHOULD BE CONSULTED BEFORE MAKING FINANCIAL DECISIONS. ALTHOUGH WE MAY PROVIDE DATA, INFORMATION AND CONTENT RELATING TO INVESTMENT APPROACHES AND OPPORTUNITIES TO BUY OR SELL SECURITIES, INCLUDING MUTUAL FUNDS AND EXCHANGE-TRADED FUNDS, YOU SHOULD NOT CONSTRUE ANY SUCH INFORMATION AS INVESTMENT, FINANCIAL, TAX, LEGAL OR OTHER ADVICE. YOU ALONE WILL BEAR THE SOLE RESPONSIBILITY OF EVALUATING THE MERITS AND RISKS ASSOCIATED WITH THE USE OF ANY DATA, INFORMATION OR CONTENT ON THE SITE BEFORE MAKING ANY DECISIONS BASED ON SUCH DATA, INFORMATION OR CONTENT. IN EXCHANGE FOR USING SUCH DATA, INFORMATION OR CONTENT, YOU AGREE NOT TO HOLD THE COMPANY OR ITS THIRD-PARTY CONTENT PROVIDERS LIABLE FOR ANY POSSIBLE CLAIM FOR DAMAGES ARISING FROM ANY DECISION YOU MAKE BASED ON INFORMATION MADE AVAILABLE TO YOU THROUGH THE SITE.
-WE DO NOT PROVIDE TAX, ACCOUNTING, LEGAL, INVESTMENT, OR FINANCIAL SERVICES. THE INFORMATION AVAILABLE THROUGH THE SITE IS PROVIDED BY THIRD PARTIES AND SOLELY FOR INFORMATIONAL PURPOSES ON AN “AS IS” BASIS AT YOUR SOLE RISK. THE INFORMATION IS NOT MEANT TO BE, AND SHOULD NOT BE CONSTRUED AS ADVICE OR USED FOR INVESTMENT, LEGAL, ACCOUNTING, OR TAX PURPOSES. THE COMPANY MAKES NO GUARANTEES AS TO THE ACCURATENESS, QUALITY, OR COMPLETENESS OF THE INFORMATION AND QUANTCONNECT SHALL NOT BE RESPONSIBLE OR LIABLE FOR ANY ERRORS, OMISSIONS, INACCURACIES IN THE INFORMATION OR FOR ANY USER’S RELIANCE ON THE INFORMATION. YOU ARE SOLELY AND COMPLETELY RESPONSIBLE FOR VERIFYING THE INFORMATION AS BEING APPROPRIATE FOR YOUR PERSONAL USE, INCLUDING WITHOUT LIMITATION, SEEKING THE ADVICE OF A QUALIFIED PROFESSIONAL REGARDING ANY SPECIFIC FINANCIAL, LEGAL, ACCOUNTING, OR TAX QUESTIONS A USER MAY HAVE. THE COMPANY DOES NOT ENDORSE ANY PARTICULAR FINANCIAL, LEGAL, ACCOUNTING, OR TAX PROFESSIONALS PROVIDING CONTENT ON THE SITE, AND IS NOT RESPONSIBLE FOR ANY CLAIMS MADE BY ANY FINANCIAL, LEGAL, ACCOUNTING OR TAX PROFESSIONALS. THE COMPANY IS NOT ENDORSED BY OR AFFILIATED WITH ANY STATE BAR ASSOCIATION OR OTHER LEGAL OR ACCOUNTING MEMBERSHIP ORGANIZATION OR ASSOCIATION, TAX AUTHORITIES, OR AGENCIES OR ASSOCIATIONS, OR FINRA OR ANY OTHER FINANCIAL REGULATORY AUTHORITY, AGENCY, OR ASSOCIATION.
-7.0 Limitation On Liability
-	TO THE MAXIMUM EXTENT PERMITTED BY LAW, IN NO EVENT SHALL COMPANY (OR OUR SUPPLIERS) BE LIABLE TO YOU OR ANY THIRD PARTY FOR ANY LOST PROFITS, LOST DATA, COSTS OF PROCUREMENT OF SUBSTITUTE PRODUCTS, OR ANY INDIRECT, CONSEQUENTIAL, EXEMPLARY, INCIDENTAL, SPECIAL OR PUNITIVE DAMAGES ARISING FROM OR RELATING TO THESE TERMS OR YOUR USE OF, OR INABILITY TO USE, THE SITE, EVEN IF COMPANY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES. ACCESS TO, AND USE OF, THE SITE IS AT YOUR OWN DISCRETION AND RISK, AND YOU WILL BE SOLELY RESPONSIBLE FOR ANY DAMAGE TO YOUR DEVICE OR COMPUTER SYSTEM, OR LOSS OF DATA RESULTING THEREFROM.
-TO THE MAXIMUM EXTENT PERMITTED BY LAW, NOTWITHSTANDING ANYTHING TO THE CONTRARY CONTAINED HEREIN, OUR LIABILITY TO YOU FOR ANY DAMAGES ARISING FROM OR RELATED TO THIS AGREEMENT (FOR ANY CAUSE WHATSOEVER AND REGARDLESS OF THE FORM OF THE ACTION), WILL AT ALL TIMES BE LIMITED TO A MAXIMUM OF FIFTY US DOLLARS (U.S. $50). THE EXISTENCE OF MORE THAN ONE CLAIM WILL NOT ENLARGE THIS LIMIT. YOU AGREE THAT OUR SUPPLIERS WILL HAVE NO LIABILITY OF ANY KIND ARISING FROM OR RELATING TO THIS AGREEMENT.
-SOME JURISDICTIONS DO NOT ALLOW THE LIMITATION OR EXCLUSION OF LIABILITY FOR INCIDENTAL OR CONSEQUENTIAL DAMAGES, SO THE ABOVE LIMITATION OR EXCLUSION MAY NOT APPLY TO YOU.
-8.0 Term and Termination
-	Subject to this Section, these Terms will remain in full force and effect while you use the Site. We may suspend or terminate your rights to use the Site (including your Account) at any time for any reason at our sole discretion, including for any use of the Site in violation of these Terms. Upon termination of your rights under these Terms, your Account and right to access and use the Site will terminate immediately. Even after your rights under these Terms are terminated, the following provisions of these Terms will remain in effect: Sections 2.2 through 2.5, Section 3 and Sections 4 through 10.
-9.0 Copyright Policy.
-	Company respects the intellectual property of others and asks that users of our Site do the same. In connection with our Site, we have adopted and implemented a policy respecting copyright law that provides for the removal of any infringing materials and for the termination, in appropriate circumstances, of users of our online Site who are repeat infringers of intellectual property rights, including copyrights. If you believe that one of our users is, through the use of our Site, unlawfully infringing the copyright(s) in a work, and wish to have the allegedly infringing material removed, the following information in the form of a written notification (pursuant to 17 U.S.C. § 512(c)) must be provided to our designated Copyright Agenus tvia email to support@algodojo.com:
-1.	Your physical or electronic signature;
-2.	Identification of the copyrighted work(s) that you claim to have been infringed;
-3.	Identification of the material on our services that you claim is infringing and that you request us to remove;
-4.	Sufficient information to permit us to locate such material;
-5.	Your address, telephone number, and e-mail address;
-6.	A statement that you have a good faith belief that use of the objectionable material is not authorized by the copyright owner, its agent, or under the law; and
-7.	A statement that the information in the notification is accurate, and under penalty of perjury, that you are either the owner of the copyright that has allegedly been infringed or that you are authorized to act on behalf of the copyright owner.
-Please note that, pursuant to 17 U.S.C. § 512(f), any misrepresentation of material fact (falsities) in a written notification automatically subjects the complaining party to liability for any damages, costs and attorney’s fees incurred by us in connection with the written notification and allegation of copyright infringement.
-The designated Copyright Agent for Company is: 
-Katten Muchin Rosenman LLP
-Designated Agent: Sean S. Wooden, Esq.
-Address of Agent: 2900 K Street, NW, North Tower - Suite 200, Washington, DC 20007-5118
-Telephone: 202-625-3664, Email: sean.wooden@kattenlaw.com
-10.0 General
-	10.1 Changes.
-These Terms are subject to occasional revision, and if we make any substantial changes, we may notify you by sending you an e-mail to the last e-mail address you provided to us (if any), and/or by prominently posting notice of the changes on our Site. You are responsible for providing us with your most current e-mail address. In the event that the last e-mail address that you have provided us is not valid, or for any reason is not capable of delivering to you the notice described above, our dispatch of the e-mail containing such notice will nonetheless constitute effective notice of the changes described in the notice. Any changes to these Terms will be effective upon the earlier of thirty (30) calendar days following our dispatch of an e-mail notice to you (if applicable) or thirty (30) calendar days following our posting of notice of the changes on our Site. These changes will be effective immediately for new users of our Site. Continued use of our Site following notice of such changes shall indicate your acknowledgement of such changes and agreement to be bound by the terms and conditions of such changes.
-	10.2 Dispute Resolution.
-Please read this Arbitration Agreement carefully. It is part of your contract with Company and affects your rights. It contains procedures for MANDATORY BINDING ARBITRATION AND A CLASS ACTION WAIVER.
-(a) Applicability of Arbitration Agreement. All claims and disputes (excluding claims for injunctive or other equitable relief as set forth below) in connection with the Terms or the use of any product or service provided by the Company that cannot be resolved informally or in small claims court shall be resolved by binding arbitration on an individual basis under the terms of this Arbitration Agreement. Unless otherwise agreed to, all arbitration proceedings shall be held in English. This Arbitration Agreement applies to you and the Company, and to any subsidiaries, affiliates, agents, employees, predecessors in interest, successors, and assigns, as well as all authorized or unauthorized users or beneficiaries of services or goods provided under the Terms.
-(b) Notice Requirement and Informal Dispute Resolution. Before either party may seek arbitration, the party must first send to the other party a written Notice of Dispute (“Notice”) describing the nature and basis of the claim or dispute, and the requested relief. A Notice to the Company should be sent to: 1917 1st Ave, Suite 200, Seattle, 98101, Washington(insert address of our company). After the Notice is received, you and the Company may attempt to resolve the claim or dispute informally. If you and the Company do not resolve the claim or dispute within thirty (30) days after the Notice is received, either party may begin an arbitration proceeding. The amount of any settlement offer made by any party may not be disclosed to the arbitrator until after the arbitrator has determined the amount of the award, if any, to which either party is entitled.
-(c) Arbitration Rules. Arbitration shall be initiated through the American Arbitration Association (“AAA”), an established alternative dispute resolution provider (“ADR Provider”) that offers arbitration as set forth in this section. If AAA is not available to arbitrate, the parties shall agree to select an alternative ADR Provider. The rules of the ADR Provider shall govern all aspects of the arbitration, including but not limited to the method of initiating and/or demanding arbitration, except to the extent such rules are in conflict with the Terms. The AAA Consumer Arbitration Rules (“Arbitration Rules”) governing the arbitration are available online at www.adr.org or by calling the AAA at 1-800-778-7879. The arbitration shall be conducted by a single, neutral arbitrator. Any claims or disputes where the total amount of the award sought is less than Ten Thousand U.S. Dollars (US $10,000.00) may be resolved through binding non-appearance-based arbitration, at the option of the party seeking relief. For claims or disputes where the total amount of the award sought is Ten Thousand U.S. Dollars (US $10,000.00) or more, the right to a hearing will be determined by the Arbitration Rules. Any hearing will be held in a location within 21050 miles of the Company’s principal place of businessCosta Mesa, CA, U.S.A., unless the parties agree otherwise. If you reside outside of the U.S., the arbitrator shall give the parties reasonable notice of the date, time and place of any oral hearings. Any judgment on the award rendered by the arbitrator may be entered in any court of competent jurisdiction. If the arbitrator grants you an award that is greater than the last settlement offer that the Company made to you prior to the initiation of arbitration, the Company will pay you the greater of the award or $2,500.00. Each party shall bear its own costs (including attorney’s fees) and disbursements arising out of the arbitration and shall pay an equal share of the fees and costs of the ADR Provider.
-(d) Additional Rules for Non-Appearance Based Arbitration. If non-appearance based arbitration is elected, the arbitration shall be conducted by telephone, online and/or based solely on written submissions; the specific manner shall be chosen by the party initiating the arbitration. The arbitration shall not involve any personal appearance by the parties or witnesses unless otherwise agreed by the parties.
-(e) Time Limits. If you or the Company pursue arbitration, the arbitration action must be initiated and/or demanded within the statute of limitations (i.e., the legal deadline for filing a claim) and within any deadline imposed under the AAA Rules for the pertinent claim.
-(f) Authority of Arbitrator. If arbitration is initiated, the arbitrator will decide the rights and liabilities, if any, of you and the Company, and the dispute will not be consolidated with any other matters or joined with any other cases or parties. The arbitrator shall have the authority to grant motions dispositive of all or part of any claim. The arbitrator shall have the authority to award monetary damages, and to grant any non-monetary remedy or relief available to an individual under applicable law, the AAA Rules, and the Terms. The arbitrator shall issue a written award and statement of decision describing the essential findings and conclusions on which the award is based, including the calculation of any damages awarded. The arbitrator has the same authority to award relief on an individual basis that a judge in a court of law would have. The award of the arbitrator is final and binding upon you and the Company.
-(g) Waiver of Jury Trial. THE PARTIES HEREBY WAIVE THEIR CONSTITUTIONAL AND STATUTORY RIGHTS TO GO TO COURT AND HAVE A TRIAL IN FRONT OF A JUDGE OR A JURY, instead electing that all claims and disputes shall be resolved by arbitration under this Arbitration Agreement. Arbitration procedures are typically more limited, more efficient and less costly than rules applicable in a court and are subject to very limited review by a court. In the event any litigation should arise between you and the Company in any state or federal court in a suit to vacate or enforce an arbitration award or otherwise, YOU AND THE COMPANY WAIVE ALL RIGHTS TO A JURY TRIAL, instead electing that the dispute be resolved by a judge.
-(h) Waiver of Class or Consolidated Actions. ALL CLAIMS AND DISPUTES WITHIN THE SCOPE OF THIS ARBITRATION AGREEMENT MUST BE ARBITRATED OR LITIGATED ON AN INDIVIDUAL BASIS AND NOT ON A CLASS BASIS, AND CLAIMS OF MORE THAN ONE CUSTOMER OR USER CANNOT BE ARBITRATED OR LITIGATED JOINTLY OR CONSOLIDATED WITH THOSE OF ANY OTHER CUSTOMER OR USER. 
-(i) Confidentiality. All aspects of the arbitration proceeding, including but not limited to the award of the arbitrator and compliance therewith, shall be strictly confidential. The parties agree to maintain confidentiality unless otherwise required by law. This paragraph shall not prevent a party from submitting to a court of law any information necessary to enforce this Agreement, to enforce an arbitration award, or to seek injunctive or equitable relief.
-(j) Severability. If any part or parts of this Arbitration Agreement are found under the law to be invalid or unenforceable by a court of competent jurisdiction, then such specific part or parts shall be of no force and effect and shall be severed and the remainder of the Agreement shall continue in full force and effect.
-(k) Right to Waive. Any or all of the rights and limitations set forth in this Arbitration Agreement may be waived by the party against whom the claim is asserted. Such waiver shall not waive or affect any other portion of this Arbitration Agreement.
-(l) Survival of Agreement. This Arbitration Agreement will survive the termination of your relationship with Company. 
-(m) Small Claims Court. Notwithstanding the foregoing, either you or the Company may bring an individual action in small claims court.
-(n) Emergency Equitable Relief. Notwithstanding the foregoing, either party may seek emergency equitable relief before a state or federal court in order to maintain the status quo pending arbitration. A request for interim measures shall not be deemed a waiver of any other rights or obligations under this Arbitration Agreement.
-(o) Claims Not Subject to Arbitration. Notwithstanding the foregoing, claims of defamation, violation of the Computer Fraud and Abuse Act, and infringement or misappropriation of the other party’s patent, copyright, trademark or trade secrets shall not be subject to this Arbitration Agreement.
-(p) Courts. In any circumstances where the foregoing Arbitration Agreement permits the parties to litigate in court, the parties hereby agree to submit to the personal jurisdiction of the courts located within Kings County, New York, for such purpose.
-	10.3 Export.
-The Site may be subject to U.S. export control laws and may be subject to export or import regulations in other countries. You agree not to export, reexport, or transfer, directly or indirectly, any U.S. technical data acquired from Company, or any products utilizing such data, in violation of the United States export laws or regulations. 
-	10.4 Disclosures.
-Company is located at the address in Section 10.9. If you are a California resident, you may report complaints to the Complaint Assistance Unit of the Division of Consumer Product of the California Department of Consumer Affairs by contacting them in writing at 400 R Street, Sacramento, CA 95814, or by telephone at (800) 952-5210.
-	10.45 Electronic Communications.
-The communications between you and Company use electronic means, whether you use the Site or send us emails, or whether Company posts notices on the Site or communicates with you via email. For contractual purposes, you (a) consent to receive communications from Company in an electronic form; and (b) agree that all terms and conditions, agreements, notices, disclosures, and other communications that Company provides to you electronically satisfy any legal requirement that such communications would satisfy if it were be in a hardcopy writing. The foregoing does not affect your non-waivable rights.
-	10.56 Entire Terms.
-These Terms constitute the entire agreement between you and us regarding the use of the Site. Our failure to exercise or enforce any right or provision of these Terms shall not operate as a waiver of such right or provision. The section titles in these Terms are for convenience only and have no legal or contractual effect. The word “including” means “including without limitation”. If any provision of these Terms is, for any reason, held to be invalid or unenforceable, the other provisions of these Terms will be unimpaired and the invalid or unenforceable provision will be deemed modified so that it is valid and enforceable to the maximum extent permitted by law. Your relationship to Company is that of an independent contractor, and neither party is an agent or partner of the other. These Terms, and your rights and obligations herein, may not be assigned, subcontracted, delegated, or otherwise transferred by you without Company’s prior written consent, and any attempted assignment, subcontract, delegation, or transfer in violation of the foregoing will be null and void. Company may freely assign these Terms. The terms and conditions set forth in these Terms shall be binding upon assignees.
-	10.67 Copyright/Trademark Information.
-Copyright © 202217 QuantConnect Dojo Technologies Limited Corporation. All rights reserved. All trademarks, logos and service marks ("Marks") displayed on the Site are our property or the property of other third parties. You are not permitted to use these Marks without our prior written consent or the consent of such third party which may own the Marks.
-	10.8 Contact Information
-
-
+By using AlgoDojo (we, us, our) services (website, product, forums) you agree to the following terms of use.
+Introduction
+The website located at https://www.algodojo.com/ (the “Site”) is a copyrighted work belonging to Dojo Technologies Limited (“Company”, “us”, “our”, and “we”). Certain features of the Site may be subject to additional guidelines, terms, or rules, which will be posted on the Site in connection with such features, including, without limitation the Company’s Privacy Policy, the Platform Services Agreement, and the Subscription and Sublicense Agreement, all of which are incorporated by reference to these Terms. All such additional terms, guidelines, and rules are incorporated by reference into these Terms.
+THESE TERMS OF USE (THESE “TERMS”) SET FORTH THE LEGALLY BINDING TERMS AND CONDITIONS THAT GOVERN YOUR USE OF THE SITE. BY ACCESSING OR USING THE SITE, YOU ARE ACCEPTING THESE TERMS (ON BEHALF OF YOURSELF OR THE ENTITY THAT YOU REPRESENT), AND YOU REPRESENT AND WARRANT THAT YOU HAVE THE RIGHT, AUTHORITY, AND CAPACITY TO ENTER INTO THESE TERMS (ON BEHALF OF YOURSELF OR THE ENTITY THAT YOU REPRESENT). YOU MAY NOT ACCESS OR USE THE SITE OR ACCEPT THE TERMS IF YOU ARE NOT AT LEAST 18 YEARS OLD. IF YOU DO NOT AGREE WITH ALL OF THE PROVISIONS OF THESE TERMS, DO NOT ACCESS AND/OR USE THE SITE.
+THESE TERMS REQUIRE THE USE OF ARBITRATION (SECTION 10.2) ON AN INDIVIDUAL BASIS TO RESOLVE DISPUTES, RATHER THAN JURY TRIALS OR CLASS ACTIONS, AND ALSO LIMIT THE REMEDIES AVAILABLE TO YOU IN THE EVENT OF A DISPUTE.
+1.0 Accounts
+	1.1 Account Creation
+In order to use certain features of the Site, you must register for an account (“Account”) and provide certain information about yourself as prompted by the account registration form. You represent and warrant that: (a) all required registration information you submit is truthful and accurate; (b) you will maintain the accuracy of such information. You may delete your Account at any time, for any reason, by following the instructions on the Site. Company may suspend or terminate your Account in accordance with Section 8.
+	1.2 Account Responsibilities
+You are responsible for maintaining the confidentiality of your Account login information and are fully responsible for all activities that occur under your Account. You agree to immediately notify Company of any unauthorized use, or suspected unauthorized use of your Account or any other breach of security. Company cannot and will not be liable for any loss or damage arising from your failure to comply with the above requirements.
+	1.3 Non-Solicitation
+You are prohibited from soliciting or recruit any other users or members of the Site, including Alpha Stream Authors, for any reason, unless you have requested and received permission to solicit or recruit in writing from the Company. . This prohibition includes a prohibition against soliciting or recruiting users of the Site, including Alpha Stream Authors, to become members of competitive sites and services. IThis includes (but is not limited to) soliciting Alpha Stream Authors to make their methods, devices, models, algorithms or other automated processes available at services or sites outside of the Site. If you violate this policy, the Company reserves the right to terminate your Account without notice and to take legal action to recover lost revenues you have stolen from us, plus applicable damages. By using the Site, you specifically acknowledge that you agree to this prohibition.
+2.0 Access to the Site
+	2.1 License.
+Subject to these Terms, Company grants you a non-transferable, non-exclusive, revocable, limited license to use and access the Site solely for your own personal use.
+	2.2 Certain Restrictions.
+The rights granted to you in these Terms are subject to the following restrictions: (a) you shall not license, sell, rent, lease, transfer, assign, distribute, host, or otherwise commercially exploit the Site, whether in whole or in part, or any content displayed on the Site; (b) you shall not share with others, resell or redistribute any of the Site’s dataset (“Data”). The Data is only for internal use. You may not publish, disseminate, re-distribute or share the Data, or any part thereof, or any derivative data that allows reverse engineering of part or all of the Data, with anyone else. You may not offer the Data, or any part thereof, for sale, rent, license or commercial redistribution. Any sharing or distribution by you of your access privileges or of the Data may result in cancellation of your use of the Data without refund. Data can only be used within the AlgoDojo software. You are prohibited from downloading or exporting the data outside the AlgoDojo software; (cb) you shall not modify, make derivative works of, disassemble, reverse compile or reverse engineer any part of the Site; (dc) you shall not access the Site in order to build a similar or competitive website, product, or service; and (ed) except as expressly stated herein, no part of the Site may be copied, reproduced, distributed, republished, downloaded, displayed, posted or transmitted in any form or by any means. Unless otherwise indicated, any future release, update, or other addition to functionality of the Site shall be subject to these Terms. All copyright and other proprietary notices on the Site (or on any content displayed on the Site) must be retained on all copies thereof.
+
+
+	2.3 Modification.
+Company reserves the right, at any time, to modify, suspend, or discontinue the Site (in whole or in part) with or without notice to you. You agree that Company will not be liable to you or to any third party for any modification, suspension, or discontinuation of the Site or any part thereof.
+	2.4 No Support or Maintenance.
+You acknowledge and agree that Company will have no obligation to provide you with any support or maintenance in connection with the Site, but the Company reserves the right, on a case by case basis, to provide support or maintenance as the need arises.
+	2.5 Ownership.
+Subject to the terms hereof, and excluding any Non-Public User Content that you may provide (defined below in Section 3.0), you acknowledge that all the intellectual property rights, including copyrights, patents, trademarks, and trade secrets, in the Site and its content, whether provided by you, the Company, or Company’s suppliers, are owned by Company or Company’s suppliers. Neither these Terms (nor your access to the Site) transfers to you or any third party any rights, title or interest in or to such intellectual property rights, except for the limited access rights expressly set forth in Section 2.1. Company and its suppliers reserve all rights not granted in these Terms. There are no implied licenses granted under these Terms.
+3.0 User Content
+	3.1 User Content and Alpha Stream Content.
+“User Content” means any and all information submitted to or communicated through the Site. You are solely responsible for your User Content. You assume all risks associated with use of your User Content, including any reliance on its accuracy, completeness or usefulness by others, or any disclosure of your User Content that personally identifies you or any third party. You hereby represent and warrant that your User Content do not violate our Acceptable Use Policy (defined in Section 3.3). You may not represent or imply to others that your User Content is in any way provided, sponsored or endorsed by Company. Because you alone are responsible for your User Content, you may expose yourself to liability if, for example, your User Content violates the Acceptable Use Policy. Company is not obligated to backup any User Content, and your User Content a may be deleted at any time without prior notice. You are solely responsible for creating and maintaining your own backup copies of your User Content if you desire.
+	3.2 Non-Public User Content 
+User Content includes Non-Public User Content and Public User Content. Non-Public User Content is User Content that you communicate directly to one or more other users of the Site or that is not accessible without being logged into your account. Public User Content is all other User Content. When you submit Public User Content, you agree that all rights in such Public User Content are owned by the Company per Section 2.5 above and agree to take reasonable steps, if any, necessary to effectuate such ownership.
+	3.3 Acceptable Use Policy. 
+The following terms constitute our “Acceptable Use Policy”:
+(a) You agree not to use the Site to collect, upload, transmit, display, or distribute any User Content (i) that violates any third-party right, including any copyright, trademark, patent, trade secret, moral right, privacy right, right of publicity, or any other intellectual property or proprietary right; (ii) that is unlawful, harassing, abusive, tortious, threatening, harmful, invasive of another’s privacy, vulgar, defamatory, false, intentionally misleading, trade libelous, pornographic, obscene, patently offensive, promotes racism, bigotry, hatred, or physical harm of any kind against any group or individual or is otherwise objectionable; (iii) that is harmful to minors in any way; or (iv) that is in violation of any law, regulation, or obligations or restrictions imposed by any third party.
+(b) In addition, you agree not to: (i) upload, transmit, or distribute to or through the Site any computer viruses, worms, or any software intended to damage or alter a computer system or data; (ii ) share with others, resell or redistribute any of the Site’s historical market trading data; (iii) send through the Site unsolicited or unauthorized advertising, promotional materials, junk mail, spam, chain letters, pyramid schemes, or any other form of duplicative or unsolicited messages, whether commercial or otherwise; (ivii) use the Site to harvest, collect, gather or assemble information or data regarding other users, including e-mail addresses, without their consent; (iv) interfere with, disrupt, or create an undue burden on servers or networks connected to the Site, or violate the regulations, policies or procedures of such networks; (vi) attempt to gain unauthorized access to the Site (or to other computer systems or networks connected to or used together with the Site), whether through password mining or any other means; (vii) harass or interfere with any other user’s use and enjoyment of the Site; or (viii) use software or automated agents or scripts to produce multiple accounts on the Site, or to generate automated searches, requests, or queries to (or to strip, scrape, or mine data from) the Site (provided, however, that we conditionally grant to the operators of public search engines revocable permission to use spiders to copy materials from the Site for the sole purpose of and solely to the extent necessary for creating publicly available searchable indices of the materials, but not caches or archives of such materials, subject to the parameters set forth in our robots.txt file).
+(c) In addition, you agree not to disparage any other user of the Site to any third party based on interactions through the Site.
+	3.4 Enforcement.
+We reserve the right (but have no obligation except in rare circumstances) to review any User Content, and to investigate and/or take appropriate action against you in our sole discretion if you violate the Acceptable Use Policy or any other provision of these Terms or otherwise create liability for us or any other person. Such action may include removing or modifying your User Content, terminating your Account in accordance with Section 8, and/or reporting you to law enforcement authorities.
+	3.5 Feedback.
+If you provide Company with any feedback or suggestions regarding the Site (“Feedback”), you hereby assign to Company all rights in such Feedback and agree that Company shall have the right to use and fully exploit such Feedback and related information in any manner it deems appropriate. Company will treat any Feedback you provide to Company as non-confidential and non-proprietary. You agree that you will not submit to Company any information or ideas that you consider to be confidential or proprietary.
+	3.6 No Investment Advice; Not an Investment Advisor; Not a Broker-Dealer.
+The Company is not an investment advisory service, nor is it a registered investment advisor or broker-dealer and does not purport to tell or suggest the value of any securities or which securities customers should buy or sell for themselves. The users of the Site may hold positions in the stocks or industries discussed here. You understand and acknowledge that there is a very high degree of risk involved in trading securities. The Company, the users, the authors, the publisher, and all affiliates of the Site assume no responsibility or liability for your trading and investment results. Factual statements or publications on the Site are made as of the date stated and are subject to change without notice. It should not be assumed that the methods, techniques, or indicators presented in these products will be profitable or that they will not result in losses. Past results of any individual trader or trading system published by on the Site are not indicative of future returns by that trader or system, and are not indicative of future returns which be realized by you. In addition, the indicators, strategies, columns, articles and all other features of the Site are provided for informational and educational purposes only and should not be construed as investment advice. Examples presented on the site are for educational purposes only. Such set-ups are not solicitations of any order to buy or sell. Accordingly, you should not rely solely on the Information in making any investment. You should always check with your licensed financial advisor and tax advisor to determine the suitability of any investment.
+	3.7 Live Trading Risks.
+By using the Site, you acknowledge and agree that live algorithmic trading has various risks and the Company shall not have any liability for any losses incurred through using the Site, such risks included, without limitation:
+(a) Design risks; errors in data, incorrect assumptions, logical program errors. Even if you designed a perfect strategy, past performance is no guarantee of future results.
+(b) Data risk; Your use of, or inability to use, the Data is at your sole risk. AlgoDojo make no warranty about the accuracy or quality of the Data and do not guarantee, represent, or warrant that your use of the data will be uninterrupted, timely, secure, reliable, complete, accurate, or error-free. Data may be delayed, inaccurate, or contain errors or omissions, and AlgoDojo will have no liability with respect thereto. AlgoDojo is not responsible for the Data. All data is provided “as is” and neither party makes any other warranties, express or implied, including any implied warranty of non-infringement, accuracy, merchantability, durability, or fitness for a particular purpose. 
+
+(cb) Loss of internet connectivity; resulting in disconnections from brokerage, trades not placed, not seeing the results of algorithm, orders failing to be placed.
+(dc) Poor design of algorithm; resulting in runaway strategies, machine gun orders, run-time errors halting program operation, failure to trade when expected, termination of the algorithm.
+(ed) Unexpected market conditions; resulting in poor fill prices, rapid losses (flash crashes), late exchange openings.
+(fe) Live Ddata feed issues; broken, dirty, delayed or intermittent data connections causing algorithm errors. This includes data inaccuracies (exchanges sometimes publish bad/fictional trades). 
+(gf) Execution issues; orders submissions, updates and cancellations could be rejected or delayed. Trades could be disallowed by authorities without warning.
+(hg) Malicious activities; criminal activity could cause your algorithm to fail or your brokerage account to become compromised, leaking personal information, intellectual property or theft of your funds.
+(ih) These events can cause the loss of all funds and holdings in your brokerage account. Algorithmic trading losses can occur faster than in manual trading and you should consult an investment professional to discuss these risks. You should continually monitor the operation of a live trading algorithm to ensure it is running properly.
+EVERY TIME YOU USE THE SITE YOU AGREE THAT IN ALL CASES THE COMPANY BEARS NO RESPONSIBILITY FOR LOSSES INCURRED, AND OFFERS NO GUARANTEES OR EXPECTATIONS ON YOUR ALGORITHM PERFORMANCE OR STABILITY.
+4.0 Indemification
+	You agree to indemnify and hold Company (and its officers, employees, and agents) harmless, including costs and attorneys’ fees, from any claim or demand made by any third party due to or arising out of (a) your use of the Site, (b) your violation of these Terms, (c) your violation of applicable laws or regulations or (d) your User Content. Company reserves the right, at your expense, to assume the exclusive defense and control of any matter for which you are required to indemnify us, and you agree to cooperate with our defense of these claims. You agree not to settle any matter without the prior written consent of Company. Company will use reasonable efforts to notify you of any such claim, action or proceeding upon becoming aware of it.
+5.0 Third Party Links & Ads; Other Users
+	5.1 Third-Party Links & Ads.
+The Site may contain links to third-party websites and services, and/or display advertisements for third parties (collectively, “Third-Party Links & Ads”). Such Third-Party Links & Ads are not under the control of Company, and Company is not responsible for any Third-Party Links & Ads. Company provides access to these Third-Party Links & Ads only as a convenience to you, and does not review, approve, monitor, endorse, warrant, or make any representations with respect to Third-Party Links & Ads. You use all Third-Party Links & Ads at your own risk, and should apply a suitable level of caution and discretion in doing so. When you click on any of the Third-Party Links & Ads, the applicable third party’s terms and policies apply, including the third party’s privacy and data gathering practices. You should make whatever investigation you feel necessary or appropriate before proceeding with any transaction in connection with such Third-Party Links & Ads.
+	5.2 Other Users.
+Each Site user is solely responsible for any and all of its own User Content. Because we do not control User Content, you acknowledge and agree that we are not responsible for any User Content, whether provided by you or by others. We make no guarantees regarding the accuracy, currency, suitability, or quality of any User Content. Your interactions with other Site users are solely between you and such users. You agree that Company will not be responsible for any loss or damage incurred as the result of any such interactions. If there is a dispute between you and any Site user, we are under no obligation to become involved.
+	5.3 Release.
+You hereby release and forever discharge the Company (and our officers, employees, agents, successors, and assigns) from, and hereby waive and relinquish, each and every past, present and future dispute, claim, controversy, demand, right, obligation, liability, action and cause of action of every kind and nature (including personal injuries, death, and property damage), that has arisen or arises directly or indirectly out of, or that relates directly or indirectly to, the Site (including any interactions with, or act or omission of, other Site users or any Third-Party Links & Ads). IF YOU ARE A CALIFORNIA RESIDENT, YOU HEREBY WAIVE CALIFORNIA CIVIL CODE SECTION 1542 IN CONNECTION WITH THE FOREGOING, WHICH STATES: “A GENERAL RELEASE DOES NOT EXTEND TO CLAIMS WHICH THE CREDITOR DOES NOT KNOW OR SUSPECT TO EXIST IN HIS OR HER FAVOR AT THE TIME OF EXECUTING THE RELEASE, WHICH IF KNOWN BY HIM OR HER MUST HAVE MATERIALLY AFFECTED HIS OR HER SETTLEMENT WITH THE DEBTOR.”.
+6.0 Disclaimers.
+	THE SITE IS PROVIDED ON AN “AS-IS” AND “AS AVAILABLE” BASIS, AND COMPANY (AND OUR SUPPLIERS) EXPRESSLY DISCLAIM ANY AND ALL WARRANTIES AND CONDITIONS OF ANY KIND, WHETHER EXPRESS, IMPLIED, OR STATUTORY, INCLUDING ALL WARRANTIES OR CONDITIONS OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, TITLE, QUIET ENJOYMENT, ACCURACY, OR NON-INFRINGEMENT. WE (AND OUR SUPPLIERS) MAKE NO WARRANTY THAT THE SITE WILL MEET YOUR REQUIREMENTS, WILL BE AVAILABLE ON AN UNINTERRUPTED, TIMELY, SECURE, OR ERROR-FREE BASIS, OR WILL BE ACCURATE, RELIABLE, FREE OF VIRUSES OR OTHER HARMFUL CODE, COMPLETE, LEGAL, OR SAFE. IF APPLICABLE LAW REQUIRES ANY WARRANTIES WITH RESPECT TO THE SITE, ALL SUCH WARRANTIES ARE LIMITED IN DURATION TO NINETY (90) DAYS FROM THE DATE OF FIRST USE.
+SOME JURISDICTIONS DO NOT ALLOW THE EXCLUSION OF IMPLIED WARRANTIES, SO THE ABOVE EXCLUSION MAY NOT APPLY TO YOU. SOME JURISDICTIONS DO NOT ALLOW LIMITATIONS ON HOW LONG AN IMPLIED WARRANTY LASTS, SO THE ABOVE LIMITATION MAY NOT APPLY TO YOU.
+THE COMPANY PROVIDES THE CONTENT OF THE SITE FOR INFORMATIONAL, EDUCATIONAL AND NONCOMMERCIAL PURPOSES ONLY. SINCE EACH INDIVIDUAL'S SITUATION IS UNIQUE, A QUALIFIED PROFESSIONAL SHOULD BE CONSULTED BEFORE MAKING FINANCIAL DECISIONS. ALTHOUGH WE MAY PROVIDE DATA, INFORMATION AND CONTENT RELATING TO INVESTMENT APPROACHES AND OPPORTUNITIES TO BUY OR SELL SECURITIES, INCLUDING MUTUAL FUNDS AND EXCHANGE-TRADED FUNDS, YOU SHOULD NOT CONSTRUE ANY SUCH INFORMATION AS INVESTMENT, FINANCIAL, TAX, LEGAL OR OTHER ADVICE. YOU ALONE WILL BEAR THE SOLE RESPONSIBILITY OF EVALUATING THE MERITS AND RISKS ASSOCIATED WITH THE USE OF ANY DATA, INFORMATION OR CONTENT ON THE SITE BEFORE MAKING ANY DECISIONS BASED ON SUCH DATA, INFORMATION OR CONTENT. IN EXCHANGE FOR USING SUCH DATA, INFORMATION OR CONTENT, YOU AGREE NOT TO HOLD THE COMPANY OR ITS THIRD-PARTY CONTENT PROVIDERS LIABLE FOR ANY POSSIBLE CLAIM FOR DAMAGES ARISING FROM ANY DECISION YOU MAKE BASED ON INFORMATION MADE AVAILABLE TO YOU THROUGH THE SITE.
+WE DO NOT PROVIDE TAX, ACCOUNTING, LEGAL, INVESTMENT, OR FINANCIAL SERVICES. THE INFORMATION AVAILABLE THROUGH THE SITE IS PROVIDED BY THIRD PARTIES AND SOLELY FOR INFORMATIONAL PURPOSES ON AN “AS IS” BASIS AT YOUR SOLE RISK. THE INFORMATION IS NOT MEANT TO BE, AND SHOULD NOT BE CONSTRUED AS ADVICE OR USED FOR INVESTMENT, LEGAL, ACCOUNTING, OR TAX PURPOSES. THE COMPANY MAKES NO GUARANTEES AS TO THE ACCURATENESS, QUALITY, OR COMPLETENESS OF THE INFORMATION AND QUANTCONNECT SHALL NOT BE RESPONSIBLE OR LIABLE FOR ANY ERRORS, OMISSIONS, INACCURACIES IN THE INFORMATION OR FOR ANY USER’S RELIANCE ON THE INFORMATION. YOU ARE SOLELY AND COMPLETELY RESPONSIBLE FOR VERIFYING THE INFORMATION AS BEING APPROPRIATE FOR YOUR PERSONAL USE, INCLUDING WITHOUT LIMITATION, SEEKING THE ADVICE OF A QUALIFIED PROFESSIONAL REGARDING ANY SPECIFIC FINANCIAL, LEGAL, ACCOUNTING, OR TAX QUESTIONS A USER MAY HAVE. THE COMPANY DOES NOT ENDORSE ANY PARTICULAR FINANCIAL, LEGAL, ACCOUNTING, OR TAX PROFESSIONALS PROVIDING CONTENT ON THE SITE, AND IS NOT RESPONSIBLE FOR ANY CLAIMS MADE BY ANY FINANCIAL, LEGAL, ACCOUNTING OR TAX PROFESSIONALS. THE COMPANY IS NOT ENDORSED BY OR AFFILIATED WITH ANY STATE BAR ASSOCIATION OR OTHER LEGAL OR ACCOUNTING MEMBERSHIP ORGANIZATION OR ASSOCIATION, TAX AUTHORITIES, OR AGENCIES OR ASSOCIATIONS, OR FINRA OR ANY OTHER FINANCIAL REGULATORY AUTHORITY, AGENCY, OR ASSOCIATION.
+7.0 Limitation On Liability
+	TO THE MAXIMUM EXTENT PERMITTED BY LAW, IN NO EVENT SHALL COMPANY (OR OUR SUPPLIERS) BE LIABLE TO YOU OR ANY THIRD PARTY FOR ANY LOST PROFITS, LOST DATA, COSTS OF PROCUREMENT OF SUBSTITUTE PRODUCTS, OR ANY INDIRECT, CONSEQUENTIAL, EXEMPLARY, INCIDENTAL, SPECIAL OR PUNITIVE DAMAGES ARISING FROM OR RELATING TO THESE TERMS OR YOUR USE OF, OR INABILITY TO USE, THE SITE, EVEN IF COMPANY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES. ACCESS TO, AND USE OF, THE SITE IS AT YOUR OWN DISCRETION AND RISK, AND YOU WILL BE SOLELY RESPONSIBLE FOR ANY DAMAGE TO YOUR DEVICE OR COMPUTER SYSTEM, OR LOSS OF DATA RESULTING THEREFROM.
+TO THE MAXIMUM EXTENT PERMITTED BY LAW, NOTWITHSTANDING ANYTHING TO THE CONTRARY CONTAINED HEREIN, OUR LIABILITY TO YOU FOR ANY DAMAGES ARISING FROM OR RELATED TO THIS AGREEMENT (FOR ANY CAUSE WHATSOEVER AND REGARDLESS OF THE FORM OF THE ACTION), WILL AT ALL TIMES BE LIMITED TO A MAXIMUM OF FIFTY US DOLLARS (U.S. $50). THE EXISTENCE OF MORE THAN ONE CLAIM WILL NOT ENLARGE THIS LIMIT. YOU AGREE THAT OUR SUPPLIERS WILL HAVE NO LIABILITY OF ANY KIND ARISING FROM OR RELATING TO THIS AGREEMENT.
+SOME JURISDICTIONS DO NOT ALLOW THE LIMITATION OR EXCLUSION OF LIABILITY FOR INCIDENTAL OR CONSEQUENTIAL DAMAGES, SO THE ABOVE LIMITATION OR EXCLUSION MAY NOT APPLY TO YOU.
+8.0 Term and Termination
+	Subject to this Section, these Terms will remain in full force and effect while you use the Site. We may suspend or terminate your rights to use the Site (including your Account) at any time for any reason at our sole discretion, including for any use of the Site in violation of these Terms. Upon termination of your rights under these Terms, your Account and right to access and use the Site will terminate immediately. Even after your rights under these Terms are terminated, the following provisions of these Terms will remain in effect: Sections 2.2 through 2.5, Section 3 and Sections 4 through 10.
+9.0 Copyright Policy.
+	Company respects the intellectual property of others and asks that users of our Site do the same. In connection with our Site, we have adopted and implemented a policy respecting copyright law that provides for the removal of any infringing materials and for the termination, in appropriate circumstances, of users of our online Site who are repeat infringers of intellectual property rights, including copyrights. If you believe that one of our users is, through the use of our Site, unlawfully infringing the copyright(s) in a work, and wish to have the allegedly infringing material removed, the following information in the form of a written notification (pursuant to 17 U.S.C. § 512(c)) must be provided to our designated Copyright Agenus tvia email to support@algodojo.com:
+1.	Your physical or electronic signature;
+2.	Identification of the copyrighted work(s) that you claim to have been infringed;
+3.	Identification of the material on our services that you claim is infringing and that you request us to remove;
+4.	Sufficient information to permit us to locate such material;
+5.	Your address, telephone number, and e-mail address;
+6.	A statement that you have a good faith belief that use of the objectionable material is not authorized by the copyright owner, its agent, or under the law; and
+7.	A statement that the information in the notification is accurate, and under penalty of perjury, that you are either the owner of the copyright that has allegedly been infringed or that you are authorized to act on behalf of the copyright owner.
+Please note that, pursuant to 17 U.S.C. § 512(f), any misrepresentation of material fact (falsities) in a written notification automatically subjects the complaining party to liability for any damages, costs and attorney’s fees incurred by us in connection with the written notification and allegation of copyright infringement.
+The designated Copyright Agent for Company is: 
+Katten Muchin Rosenman LLP
+Designated Agent: Sean S. Wooden, Esq.
+Address of Agent: 2900 K Street, NW, North Tower - Suite 200, Washington, DC 20007-5118
+Telephone: 202-625-3664, Email: sean.wooden@kattenlaw.com
+10.0 General
+	10.1 Changes.
+These Terms are subject to occasional revision, and if we make any substantial changes, we may notify you by sending you an e-mail to the last e-mail address you provided to us (if any), and/or by prominently posting notice of the changes on our Site. You are responsible for providing us with your most current e-mail address. In the event that the last e-mail address that you have provided us is not valid, or for any reason is not capable of delivering to you the notice described above, our dispatch of the e-mail containing such notice will nonetheless constitute effective notice of the changes described in the notice. Any changes to these Terms will be effective upon the earlier of thirty (30) calendar days following our dispatch of an e-mail notice to you (if applicable) or thirty (30) calendar days following our posting of notice of the changes on our Site. These changes will be effective immediately for new users of our Site. Continued use of our Site following notice of such changes shall indicate your acknowledgement of such changes and agreement to be bound by the terms and conditions of such changes.
+	10.2 Dispute Resolution.
+Please read this Arbitration Agreement carefully. It is part of your contract with Company and affects your rights. It contains procedures for MANDATORY BINDING ARBITRATION AND A CLASS ACTION WAIVER.
+(a) Applicability of Arbitration Agreement. All claims and disputes (excluding claims for injunctive or other equitable relief as set forth below) in connection with the Terms or the use of any product or service provided by the Company that cannot be resolved informally or in small claims court shall be resolved by binding arbitration on an individual basis under the terms of this Arbitration Agreement. Unless otherwise agreed to, all arbitration proceedings shall be held in English. This Arbitration Agreement applies to you and the Company, and to any subsidiaries, affiliates, agents, employees, predecessors in interest, successors, and assigns, as well as all authorized or unauthorized users or beneficiaries of services or goods provided under the Terms.
+(b) Notice Requirement and Informal Dispute Resolution. Before either party may seek arbitration, the party must first send to the other party a written Notice of Dispute (“Notice”) describing the nature and basis of the claim or dispute, and the requested relief. A Notice to the Company should be sent to: 1917 1st Ave, Suite 200, Seattle, 98101, Washington(insert address of our company). After the Notice is received, you and the Company may attempt to resolve the claim or dispute informally. If you and the Company do not resolve the claim or dispute within thirty (30) days after the Notice is received, either party may begin an arbitration proceeding. The amount of any settlement offer made by any party may not be disclosed to the arbitrator until after the arbitrator has determined the amount of the award, if any, to which either party is entitled.
+(c) Arbitration Rules. Arbitration shall be initiated through the American Arbitration Association (“AAA”), an established alternative dispute resolution provider (“ADR Provider”) that offers arbitration as set forth in this section. If AAA is not available to arbitrate, the parties shall agree to select an alternative ADR Provider. The rules of the ADR Provider shall govern all aspects of the arbitration, including but not limited to the method of initiating and/or demanding arbitration, except to the extent such rules are in conflict with the Terms. The AAA Consumer Arbitration Rules (“Arbitration Rules”) governing the arbitration are available online at www.adr.org or by calling the AAA at 1-800-778-7879. The arbitration shall be conducted by a single, neutral arbitrator. Any claims or disputes where the total amount of the award sought is less than Ten Thousand U.S. Dollars (US $10,000.00) may be resolved through binding non-appearance-based arbitration, at the option of the party seeking relief. For claims or disputes where the total amount of the award sought is Ten Thousand U.S. Dollars (US $10,000.00) or more, the right to a hearing will be determined by the Arbitration Rules. Any hearing will be held in a location within 21050 miles of the Company’s principal place of businessCosta Mesa, CA, U.S.A., unless the parties agree otherwise. If you reside outside of the U.S., the arbitrator shall give the parties reasonable notice of the date, time and place of any oral hearings. Any judgment on the award rendered by the arbitrator may be entered in any court of competent jurisdiction. If the arbitrator grants you an award that is greater than the last settlement offer that the Company made to you prior to the initiation of arbitration, the Company will pay you the greater of the award or $2,500.00. Each party shall bear its own costs (including attorney’s fees) and disbursements arising out of the arbitration and shall pay an equal share of the fees and costs of the ADR Provider.
+(d) Additional Rules for Non-Appearance Based Arbitration. If non-appearance based arbitration is elected, the arbitration shall be conducted by telephone, online and/or based solely on written submissions; the specific manner shall be chosen by the party initiating the arbitration. The arbitration shall not involve any personal appearance by the parties or witnesses unless otherwise agreed by the parties.
+(e) Time Limits. If you or the Company pursue arbitration, the arbitration action must be initiated and/or demanded within the statute of limitations (i.e., the legal deadline for filing a claim) and within any deadline imposed under the AAA Rules for the pertinent claim.
+(f) Authority of Arbitrator. If arbitration is initiated, the arbitrator will decide the rights and liabilities, if any, of you and the Company, and the dispute will not be consolidated with any other matters or joined with any other cases or parties. The arbitrator shall have the authority to grant motions dispositive of all or part of any claim. The arbitrator shall have the authority to award monetary damages, and to grant any non-monetary remedy or relief available to an individual under applicable law, the AAA Rules, and the Terms. The arbitrator shall issue a written award and statement of decision describing the essential findings and conclusions on which the award is based, including the calculation of any damages awarded. The arbitrator has the same authority to award relief on an individual basis that a judge in a court of law would have. The award of the arbitrator is final and binding upon you and the Company.
+(g) Waiver of Jury Trial. THE PARTIES HEREBY WAIVE THEIR CONSTITUTIONAL AND STATUTORY RIGHTS TO GO TO COURT AND HAVE A TRIAL IN FRONT OF A JUDGE OR A JURY, instead electing that all claims and disputes shall be resolved by arbitration under this Arbitration Agreement. Arbitration procedures are typically more limited, more efficient and less costly than rules applicable in a court and are subject to very limited review by a court. In the event any litigation should arise between you and the Company in any state or federal court in a suit to vacate or enforce an arbitration award or otherwise, YOU AND THE COMPANY WAIVE ALL RIGHTS TO A JURY TRIAL, instead electing that the dispute be resolved by a judge.
+(h) Waiver of Class or Consolidated Actions. ALL CLAIMS AND DISPUTES WITHIN THE SCOPE OF THIS ARBITRATION AGREEMENT MUST BE ARBITRATED OR LITIGATED ON AN INDIVIDUAL BASIS AND NOT ON A CLASS BASIS, AND CLAIMS OF MORE THAN ONE CUSTOMER OR USER CANNOT BE ARBITRATED OR LITIGATED JOINTLY OR CONSOLIDATED WITH THOSE OF ANY OTHER CUSTOMER OR USER. 
+(i) Confidentiality. All aspects of the arbitration proceeding, including but not limited to the award of the arbitrator and compliance therewith, shall be strictly confidential. The parties agree to maintain confidentiality unless otherwise required by law. This paragraph shall not prevent a party from submitting to a court of law any information necessary to enforce this Agreement, to enforce an arbitration award, or to seek injunctive or equitable relief.
+(j) Severability. If any part or parts of this Arbitration Agreement are found under the law to be invalid or unenforceable by a court of competent jurisdiction, then such specific part or parts shall be of no force and effect and shall be severed and the remainder of the Agreement shall continue in full force and effect.
+(k) Right to Waive. Any or all of the rights and limitations set forth in this Arbitration Agreement may be waived by the party against whom the claim is asserted. Such waiver shall not waive or affect any other portion of this Arbitration Agreement.
+(l) Survival of Agreement. This Arbitration Agreement will survive the termination of your relationship with Company. 
+(m) Small Claims Court. Notwithstanding the foregoing, either you or the Company may bring an individual action in small claims court.
+(n) Emergency Equitable Relief. Notwithstanding the foregoing, either party may seek emergency equitable relief before a state or federal court in order to maintain the status quo pending arbitration. A request for interim measures shall not be deemed a waiver of any other rights or obligations under this Arbitration Agreement.
+(o) Claims Not Subject to Arbitration. Notwithstanding the foregoing, claims of defamation, violation of the Computer Fraud and Abuse Act, and infringement or misappropriation of the other party’s patent, copyright, trademark or trade secrets shall not be subject to this Arbitration Agreement.
+(p) Courts. In any circumstances where the foregoing Arbitration Agreement permits the parties to litigate in court, the parties hereby agree to submit to the personal jurisdiction of the courts located within Kings County, New York, for such purpose.
+	10.3 Export.
+The Site may be subject to U.S. export control laws and may be subject to export or import regulations in other countries. You agree not to export, reexport, or transfer, directly or indirectly, any U.S. technical data acquired from Company, or any products utilizing such data, in violation of the United States export laws or regulations. 
+	10.4 Disclosures.
+Company is located at the address in Section 10.9. If you are a California resident, you may report complaints to the Complaint Assistance Unit of the Division of Consumer Product of the California Department of Consumer Affairs by contacting them in writing at 400 R Street, Sacramento, CA 95814, or by telephone at (800) 952-5210.
+	10.45 Electronic Communications.
+The communications between you and Company use electronic means, whether you use the Site or send us emails, or whether Company posts notices on the Site or communicates with you via email. For contractual purposes, you (a) consent to receive communications from Company in an electronic form; and (b) agree that all terms and conditions, agreements, notices, disclosures, and other communications that Company provides to you electronically satisfy any legal requirement that such communications would satisfy if it were be in a hardcopy writing. The foregoing does not affect your non-waivable rights.
+	10.56 Entire Terms.
+These Terms constitute the entire agreement between you and us regarding the use of the Site. Our failure to exercise or enforce any right or provision of these Terms shall not operate as a waiver of such right or provision. The section titles in these Terms are for convenience only and have no legal or contractual effect. The word “including” means “including without limitation”. If any provision of these Terms is, for any reason, held to be invalid or unenforceable, the other provisions of these Terms will be unimpaired and the invalid or unenforceable provision will be deemed modified so that it is valid and enforceable to the maximum extent permitted by law. Your relationship to Company is that of an independent contractor, and neither party is an agent or partner of the other. These Terms, and your rights and obligations herein, may not be assigned, subcontracted, delegated, or otherwise transferred by you without Company’s prior written consent, and any attempted assignment, subcontract, delegation, or transfer in violation of the foregoing will be null and void. Company may freely assign these Terms. The terms and conditions set forth in these Terms shall be binding upon assignees.
+	10.67 Copyright/Trademark Information.
+Copyright © 202217 QuantConnect Dojo Technologies Limited Corporation. All rights reserved. All trademarks, logos and service marks ("Marks") displayed on the Site are our property or the property of other third parties. You are not permitted to use these Marks without our prior written consent or the consent of such third party which may own the Marks.
+	10.8 Contact Information
+
+
```

### Comparing `algodojo-0.2.2/algodojo/ib_backup_20230322.py` & `algodojo-0.2.4/src/algodojo/ib.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 from ibapi.contract import Contract
 from ibapi.tag_value import TagValue
 from threading import Thread
 import queue
 from ibapi.order import *
 from ibapi.order_state import *
 from algodojo.base.auth import Auth
+from algodojo.base.report import Report
 import socketio
 import pandas as pd
 from datetime import timedelta
 from enum import Enum
 import re
 import quantstats as qs
 import time
 
+
 class RequestParams(Object):
     def __init__(self) -> None:
         self.startDateTime = ""
         self.endDateTime = ""
         self.barSize = ""
 
 
@@ -175,109 +177,78 @@
 
         while self.wrapper.is_error():
             print(self.get_error())
 
         return current_time
 
 
-class ibAuth(Auth):
+class Hsocket(socketio.Client):
     def __init__(self) -> None:
-        super().__init__()
-
-class MyCustomNamespace(socketio.AsyncClientNamespace):
-    async def on_connect(self):
-        print("I'm connected!")
-
-    async def on_disconnect(self):
-        print("I'm disconnected!")
-
-    async def on_my_event(self, data):
-        await self.emit('my_response', data)
-
-    async def on_message(self, data):
-        print("[echo]:", data)
-
-class mysio:
-    
-    def __init__(self) -> None:
-        global sio
-        self.sio = socketio.AsyncClient(logger=False, engineio_logger=False)
-        self.sio.register_namespace(MyCustomNamespace('/')) # bind
-
-class Hsocket():
-    async def __init__(self) -> None:
-        self.ST = mysio().sio
-        # self.ST.register_namespace()
+        # socketio.Client.__init__(self)
+        # socketio.Client.__init__(self)
+        # super(Hsocket, self).__init__()
+        # self.ST = socketio.Client()
         # self.__localhost = 'http://localhost:3000'
         # self.__localhost = 'http://request.algodojo.com:8004'
         # self.__localhost = 'http://35.84.179.106:8004'
+        self.SocketioDict = {}
         self.__localhost = 'http://request.algodojo.com:8004'
-        self.ST.on('responseData', self.__on_message)
+        # self.ST.on('responseData', self.__on_message)
         self.IsConnect = False
         self.__BarSize = 0
         self.__BarSizeType = 0
-        self.StartDate = None
-        self.EndDate = None
         self.TempData = []
+        self.CancelCount = 0
         self.BackTestData = pd.DataFrame({
             "open": [],
             "high": [],
             "low": [],
             "close": [],
             "volume": [],
             "time": []
         })
-        self.LastDataRow = None
-        self.IsLastStatus = False
-        self.__TempHistoricalDataCollect = {}
-        self.__IsHistoricalDataProcess = False
-
-    async def SendData(self, data: dict):
-        self.IsLastStatus = False
-        # self.__IsHistoricalDataProcess = False
-        # self.__TempHistoricalDataCollect = {}
-        await self.__Connect()
-        # print('self.__Connect()', 'after')
+        self.LastDataRow = {}
+        self.MappingLastDataRow = {}
+        self.IsLastStatus = {}
+        self.TempHistoricalDataCollect = {}
+        self.CloseData = {}
+
+    def SendData(self, data: dict):
+        reqId = data['reqId']
+        symbol = data['symbol']
+        if not reqId in self.IsLastStatus:
+            self.IsLastStatus[reqId] = False
+            self.MappingLastDataRow[symbol] = reqId
+
+        self.TempHistoricalDataCollect[reqId] = {
+            "data": {}, "isProcess": False, "isEnd": False}
+        self.SocketioDict[reqId] = socketio.Client()
+        self.SocketioDict[reqId].on('responseData', self.__on_message)
+        self.__Connect(reqId)
         self.__BarSizeType = data['granulariy'][0:10]
-        self.StartDate = data['startDate'][0:10]
-        self.EndDate = data['endDate'][0:10]
-
-        # 額外做加工
-        # if data.get('granulariy') == BarSizeType.MM.name:
-        #     self.__BarSize = 20
-        #     data['granulariy'] = BarSizeType.D.name
-        # elif data.get('granulariy') == BarSizeType.W.name:
-        #     self.__BarSize = 5
-        #     data['granulariy'] = BarSizeType.D.name
-        # else:
         self.__BarSize = int(data.get('barSize'))
 
-        self.__Emit(data)
+        self.__Emit(data, reqId)
 
-    async def __Connect(self):
+    def __Connect(self, reqId):
         # print('__Connect(self):', 'defore')
-        if not self.IsConnect:
-            await self.ST.connect(self.__localhost)
-            self.IsConnect = True
-        # print('__Connect(self):', 'after')
-        # pass
+        self.SocketioDict[reqId].connect(self.__localhost)
 
-    async def __Emit(self, data):
-        await self.ST.emit('getData', {'parameters': data})
-        await self.ST.wait()
+    def __Emit(self, data, reqId):
+        self.SocketioDict[reqId].emit('getData', {'parameters': data})
         # pass
 
-    async def Cancel(self):
-        await self.__Disconnect()
+    def Cancel(self):
+        self.__Disconnect()
 
-    async def __Disconnect(self):
+    def __Disconnect(self, reqId):
         # print('__Disconnect')
-        await self.ST.disconnect()
+        self.SocketioDict[reqId].disconnect()
 
-    def receive_historical(self, data):
+    def receive_historical(self, reqId, data):
         pass
 
     def __AddDateTime(self, barSize, barType, timestamp):
         if BarSizeType.H.name == barType:
             return (timestamp + timedelta(hours=barSize))
         elif BarSizeType.M.name == barType:
             return timestamp + timedelta(minutes=barSize)
@@ -294,16 +265,16 @@
                     return float(temp[:x+n+1])
                 except:
                     return float(temp)
         return float(temp)
 
     def __transationData(self, allData, barSize, barSizeType):
         # print(allData)
-        StartDateTime = self.StartDate
-        EndDateTime = self.EndDate
+        StartDateTime = allData[0]['timestamp'][0:10]
+        EndDateTime = allData[-1]['timestamp'][0:10]
         TempOpenTime = '04:00:00'
         TempCloseTime = '20:00:00'
         DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
         DATE_FORMAT = "%Y-%m-%d"
         NUM = 3
         TempDateTime = datetime.strptime(StartDateTime, DATE_FORMAT)
         # print(TempDateTime, type(TempDateTime))
@@ -315,14 +286,16 @@
                 1, BarSizeType.D.name, TempDateTime)
 
         ReceiveData_index = 0
         transationData = []
 
         for i, _Date in enumerate(DateList):
             # filter holiday data
+            if ReceiveData_index == len(allData):
+                continue
             if (datetime.strptime(allData[ReceiveData_index]['timestamp'][0:10], DATE_FORMAT) > datetime.strptime(_Date, DATE_FORMAT)):
                 continue
             _StartDateTime = _Date+' '+TempOpenTime
             _EndDateTime = datetime.strptime(
                 (_Date+' '+TempCloseTime), DATETIME_FORMAT)
             # print(_StartDateTime, _EndDateTime)
             _TempDateTime = datetime.strptime(_StartDateTime, DATETIME_FORMAT)
@@ -350,18 +323,18 @@
 
                 while True:
                     _ReceiveData_Timestamp = datetime.strptime(
                         allData[ReceiveData_index]['timestamp'], DATETIME_FORMAT)
 
                     if _RangeStartDateTime <= _ReceiveData_Timestamp and _ReceiveData_Timestamp <= _RangeEndDateTime:
                         _TempReciveData.append(allData[ReceiveData_index])
-                        if ReceiveData_index < len(allData):
+                        if ReceiveData_index < len(allData)-1:
                             ReceiveData_index = ReceiveData_index+1
 
-                    if _ReceiveData_Timestamp >= _RangeEndDateTime or ReceiveData_index == len(allData):
+                    if _ReceiveData_Timestamp >= _RangeEndDateTime or ReceiveData_index == len(allData)-1:
                         _VolumeSum = 0
                         _TempHigh = -100000
                         _TempLow = 1000000
                         for rowData in _TempReciveData:
                             if float(rowData['low']) < _TempLow:
                                 _TempLow = float(rowData['low'])
                             if float(rowData['high']) > _TempHigh:
@@ -462,124 +435,166 @@
                 'low': float(data.get('low')),
                 'close': float(data.get('close')),
                 'volume': int(data.get('volume')),
                 'time': data.get('timestamp')
             })
         return newData
 
-    def __check_historical_data(self, data,isLast):
-        key = data["time"][0]
-        # print("LV1 __check_historical_data = ",key,self.__IsHistoricalDataProcess)
-        self.__TempHistoricalDataCollect[key]={
-            'data':data,
-            'isLast':isLast
+    def __check_historical_data(self, data):
+        Data = data['data']
+        isLast = data['last']
+        reqId = data['reqId']
+        key = Data["time"][0]
+        # print("LV1 __check_historical_data = ", key,self.TempHistoricalDataCollect[reqId]['isProcess'])
+        self.TempHistoricalDataCollect[reqId]['data'][key] = {
+            'data': Data,
+            'isLast': isLast
         }
-        
+
         while True:
-            # print("LV2 while")
-            time.sleep(0.5)
-            if len(self.__TempHistoricalDataCollect) == 0:
-                # print("LV3 break")
+            # print("LV2 while wait", reqId)
+            time.sleep(0.1)
+            if reqId in self.TempHistoricalDataCollect:
+                if self.TempHistoricalDataCollect[reqId]['isEnd']:
+                    # print("LV3 last data break")
+                    self.TempHistoricalDataCollect.pop(reqId)
+                    break
+
+                if len(self.TempHistoricalDataCollect[reqId]['data']) == 0:
+                    # print("LV3 range data break")
+                    break
+
+                # if not self.__IsHistoricalDataProcess:
+                if not self.TempHistoricalDataCollect[reqId]['isProcess']:
+                    # print("LV3 not self.__IsSendHistoricalData")
+                    self.__send_historical_data(Data, isLast, reqId)
+            else:
                 break
 
-            if not self.__IsHistoricalDataProcess:
-                # print("LV3 not self.__IsSendHistoricalData")
-                self.__send_historical_data(data,isLast)
-
-    def __send_historical_data(self, data,isLast):
-        self.__IsHistoricalDataProcess = True
-        self.IsLastStatus = False
+    def __send_historical_data(self, data, isLast, reqId):
+        self.TempHistoricalDataCollect[reqId]['isProcess'] = True
+        self.IsLastStatus[reqId] = False
         key = data["time"][0]
         # print("LV4 __send_historical_data start",key,"isLast=",isLast)
         for i in data.index:
-            df = pd.DataFrame({"open": [data["open"][i]],
-                               "high": [data["high"][i]],
-                               "low": [data["low"][i]],
-                               "close": [data["close"][i]],
-                               "volume": [data["volume"][i]],
-                               "time": [data["time"][i]]
-                               })
-            self.LastDataRow = df
-
-            if isLast and i == len(data.index)-1:
-                self.IsLastStatus = True
-                # print("LV5 self.IsLastStatus = True")
+            df_value = {"open": [data["open"][i]],
+                        "high": [data["high"][i]],
+                        "low": [data["low"][i]],
+                        "close": [data["close"][i]],
+                        "volume": [data["volume"][i]],
+                        "time": [data["time"][i]],
+                        "last": False
+                        }
+
+            df = pd.DataFrame(df_value)
+            self.LastDataRow[reqId] = df
 
             if i == len(data.index)-1:
-                self.__TempHistoricalDataCollect.pop(key)
-                self.__IsHistoricalDataProcess = False
-                # print(f"LV5 __IsHistoricalDataProcess={self.__IsHistoricalDataProcess}")
+                # print(f"LV5 TempHistoricalDataCollect={self.TempHistoricalDataCollect}")
+                if key in self.TempHistoricalDataCollect[reqId]['data']:
+                    self.TempHistoricalDataCollect[reqId]['data'].pop(key)
+                    self.TempHistoricalDataCollect[reqId]['isProcess'] = False
+
+                if isLast:
+                    # print("LV5 self.IsLastStatus = True")
+                    self.IsLastStatus[reqId] = True
+                    df_value['last'] = True
+                    self.TempHistoricalDataCollect[reqId]['isEnd'] = True
 
             # print("LV5 __send_historical_data process index=",i,len(data["time"]))
-            self.receive_historical(df)
+            self.addCloseData(reqId, data["close"][i], data["time"][i])
+            self.receive_historical(reqId, df)
 
-    async def __on_message(self, data):
+    def __on_message(self, data):
         # print('socketio', data)
-        # print(self.__BarSize,self.__BarSizeType)
         trasationData = []
-        # print(data['data'])
+
         if data['data'] != None:
             if self.__BarSizeType == BarSizeType.S.name or self.__BarSize == 1:
                 trasationData = self.__transationDataSort(data['data'])
             else:
                 if (self.__BarSizeType == BarSizeType.D.name or self.__BarSizeType == BarSizeType.W.name or self.__BarSizeType == BarSizeType.MM.name):
                     trasationData = self.__transationData_D_UP(
                         data['data'], self.__BarSize, self.__BarSizeType, data['last'])
                 else:
                     trasationData = self.__transationData(
                         data['data'], self.__BarSize, self.__BarSizeType)
 
         newData = {
             'last': data['last'],
-            'data': pd.DataFrame(trasationData)
+            'data': pd.DataFrame(trasationData),
+            'reqId': data['reqId']
         }
-        
+
         if data['last']:
-            # self.IsLastStatus = True
+            self.IsLastStatus[data['reqId']] = True
             print("End of data transfer")
         else:
             # self.IsLastStatus = False
             print("Data transfering...")
         if len(trasationData) != 0:
-            self.__check_historical_data(newData['data'],data['last'])
+            self.__check_historical_data(newData)
 
         if(data['status'] == False):
-            self.__Disconnect()
+            self.__Disconnect(data['reqId'])
+
+    def addCloseData(self, symbol, price, time):
+        if not symbol in self.CloseData:
+            self.CloseData[symbol] = {}
+
+        self.CloseData[symbol][self.getDate(time)] = price
+
+    def getDate(self, datatime):
+        # 解析日期時間字串
+        datetime_obj = datetime.strptime(datatime, "%Y-%m-%d %H:%M:%S")
+
+        # 提取日期部分並轉換為字串
+        return datetime_obj.strftime("%Y-%m-%d")
 
 
 class ib(ibWrapper, ibClinet, Auth, Hsocket):
 
     def __init__(self) -> None:
         super(ib, self).__init__()
         Hsocket.__init__(self)
         Auth.__init__(self)
+        self.Report = Report()
         ibWrapper.__init__(self)
         ibClinet.__init__(self, wrapper=self)
         self.MarketDatas = {}
         self.permId2ord = {}
-        self.NextValidId = 0
         self.openOrderDatas = {}
         self.orderStatusDatas = {}
         self.__broker = 'ib'
         self.__statusData = {}
         self.__beta_toggle = False
         self.__market_barsize = 0
         self.__marketBarDatas = []
         self.__marketData_reqId = {}
         self.__marketData_FirstTime = {}
         self.__FORMART_DATETIME = "%Y/%m/%d-%H:%M:%S"
         self.__connect_error_count = 0
         self.BackTestToggle = False
         self.BackTestBalance = 100000
-        self.BT_Portfolio = []
-        self.BT_ReqId = 1
+        self.BT_Portfolio = {}
+        self.BT_ReqId = 0
         self.ClientId = None
         self.Port = None
         self.IP = None
         self.__IsConnectBroker = False
+        self.NextValidId = -99
+
+    def receiveFA(self, faData, cxml: str):
+        self.addNextValidId()
+        self.replaceFA(self.NextValidId,faData,cxml)
+        time.sleep(3)
+        print("Set up FA account")
+
+    def setFA(self, faType):
+        self.requestFA(faType)
 
     def accountSummary(self, reqId: int, account: str, tag: str, value: str, currency: str):
         super().accountSummary(reqId, account, tag, value, currency)
         # print('call accountSummary:', 'reqId', reqId, 'account',
         #       account, 'tag', tag, 'value', value, 'currency', currency)
 
         data = {
@@ -630,33 +645,28 @@
         }
         self.receive_accounts(data)
 
     def receive_accounts(self, data):
         pass
 
     def nextValidId(self, orderId: int):
-        if self.BackTestToggle:
-            return self.BT_ReqId
-        else:
-            self.__check_all()
-            super().nextValidId(orderId)
-            self.nextValidOrderId = orderId
-            self.NextValidId = orderId
-            print("NextValidId:", orderId)
-            return orderId
+        super().nextValidId(orderId)
+        self.nextValidOrderId = orderId
+        self.NextValidId = orderId
+        print("NextValidId:", orderId)
+        return orderId
 
     def addNextValidId(self):
-        if self.BackTestToggle:
-            self.BT_ReqId = self.BT_ReqId+1
-            return self.BT_ReqId
-        else:
+        self.NextValidId += 1
+
+        if not self.BackTestToggle:
             self.__check_all()
-            self.NextValidId += 1
             self.nextValidId(self.NextValidId)
-            return self.NextValidId
+
+        return self.NextValidId
 
     def openOrder(self, orderId: int, contract: Contract, order: Order, orderState: OrderState):
         # print(orderId, contract, order, orderState)
         super().openOrder(orderId, contract, order, orderState)
         data = {
             'permId': order.permId,
             'clientId': order.clientId,
@@ -805,19 +815,19 @@
                 'close': self.__marketBarDatas[0]['close'],
                 'volume': _tmpVolume,
                 'wap': _tmpWap,
                 'count': _tmpCount,
             }
             # self.MarketDatas[reqId] = data
             self.__marketBarDatas = []
-            self.receive_markets(pd.DataFrame([data]))
+            self.receive_markets(reqId, pd.DataFrame([data]))
         else:
-            self.receive_markets(pd.DataFrame([data]))
+            self.receive_markets(reqId, pd.DataFrame([data]))
 
-    def receive_markets(self, data):
+    def receive_markets(self, reqId, data):
         pass
 
     def ReqRealTimeBars(self, reqId, contract, requestParams):
         whatToShow = "MIDPOINT"
         barSize = 5
 
         if requestParams.get('whatToShow') != None:
@@ -852,47 +862,91 @@
             self.disconnect()
             self.__IsConnectBroker = False
         except Exception as ex:
             print(f"{strspan} error: {ex}")
             result.false(f"{strspan} error: {ex}")
 
         return result
-    
+
+    def __Connenct(self):
+        # print("Fun", "__Connenct")
+        try:
+            if not self.__IsConnectBroker:
+                # print(self.IP, self.Port, self.ClientId)
+                self.connect(self.IP, self.Port, self.ClientId)
+                thread = Thread(target=self.run, daemon=True)
+                thread.start()
+
+                setattr(self, "_thread", thread)
+
+                self.init_error()
+
+                temp_sec = 0
+                stop_sec = 10
+                while True:
+                    # if isinstance(self.NextValidId, int):
+                    if self.NextValidId != -99:
+                        print('Successful connection to Interactive Brokers.')
+                        self.__IsConnectBroker = True
+                        break
+                    else:
+                        temp_sec = temp_sec+1
+                        time.sleep(1)
+                        print(
+                            "Please wait to connection to the Interactive Brokers software...")
+
+                    if temp_sec > stop_sec:
+                        print("timeout")
+                        break
+        except Exception as ex:
+            print("Unsuccessful connection to Interactive Broker.")
+
     def __IsConnect(self):
+        # print("Fun","__IsConnect")
         result = Result()
         strspan = 'Connect to Interactive Brokers'
 
         try:
             try:
                 if not self.__IsConnectBroker:
+                    # print(self.IP, self.Port, self.ClientId)
                     self.connect(self.IP, self.Port, self.ClientId)
-
-                    thread = Thread(target=self.run)
+                    thread = Thread(target=self.run, daemon=True)
                     thread.start()
 
                     setattr(self, "_thread", thread)
 
                     self.init_error()
 
-                    result.true(strspan)
                     self.__connect_error_count = 0
 
-                    print("Please wait to connect to the Interactive Brokers software...")
-                    time.sleep(3)
-                    self.__IsConnectBroker = True
+                    while True:
+                        # if isinstance(self.NextValidId, int):
+                        if self.NextValidId != -99:
+                            print('Successful connection to Interactive Brokers')
+                            self.__IsConnectBroker = True
+                            result.true(strspan)
+                            break
+                        else:
+                            time.sleep(1)
+                            print(
+                                "Please wait to connection to the Interactive Brokers software...")
+
             except Exception as ex:
                 self.__connect_error_count = self.__connect_error_count+1
                 raise ValueError("ib connent fail")
         except Exception as ex:
             if str(ex) == ("ib connent fail"):
                 if self.__connect_error_count >= 3:
-                    print(f"Error connecting to Interactive Brokers at IP address {str(self.IP)}, port {str(self.Port)} with client ID {str(self.ClientId)}. Please verify that your settings are correct. ")
+                    print(
+                        f"Error connecting to Interactive Brokers at IP address {str(self.IP)}, port {str(self.Port)} with client ID {str(self.ClientId)}. Please verify that your settings are correct. ")
                     sys.exit(0)
                 else:
-                    Key = input(f"Error connecting to Interactive Brokers at IP address {str(self.IP)}, port {str(self.Port)} with client ID {str(self.ClientId)}. Please check that the settings are correct, and that either IB Trader Workstation or IB Gateway is running. Press Enter to try again, or type *Q* to quit : ")
+                    Key = input(
+                        f"Error connecting to Interactive Brokers at IP address {str(self.IP)}, port {str(self.Port)} with client ID {str(self.ClientId)}. Please check that the settings are correct, and that either IB Trader Workstation or IB Gateway is running. Press Enter to try again, or type *Q* to quit : ")
                     if str(Key) == ('Q') or str(Key) == ('q'):
                         sys.exit(0)
                     else:
                         self.__is_connect()
             else:
                 print(f"{strspan} error: {ex}")
                 result.false(f"{strspan} error: {ex}")
@@ -904,23 +958,28 @@
         # print(strspan)
 
         try:
             try:
                 self.sign_in(settingParams['token'], self.__broker)
                 self.check_status()
                 if not "ip" in settingParams:
-                    raise ValueError("The ip key doesn't exist in the dictionary")
+                    raise ValueError(
+                        "The ip key doesn't exist in the dictionary")
                 if not "port" in settingParams:
-                    raise ValueError("The port key doesn't exist in the dictionary")
+                    raise ValueError(
+                        "The port key doesn't exist in the dictionary")
                 if not "clientId" in settingParams:
-                    raise ValueError("The clientId key doesn't exist in the dictionary")
+                    raise ValueError(
+                        "The clientId key doesn't exist in the dictionary")
                 self.IP = settingParams['ip']
-                self.Port =  int(settingParams['port'])
+                self.Port = int(settingParams['port'])
                 self.ClientId = int(settingParams['clientId'])
+                self.__Connenct()
             except Exception as ex:
+                # print("ex", ex)
                 raise ValueError(ex)
         except Exception as ex:
             print(f"{strspan} error: {ex}")
             result.false(f"{strspan} error: {ex}")
         return result
 
     def fetch_account_all(self, reqId):
@@ -977,95 +1036,111 @@
         time_list = pd.to_datetime(pd.Series(time_list))
         profit_list = data.get('profit')
         stock_return = pd.Series(profit_list, index=time_list).sort_index()
         current_datetime = datetime.now()
 
         current_date_time = current_datetime.strftime("%Y%m%d%H%M%S")
         filename = current_date_time+'.html'
-        if "title" in data:   
-            qs.reports.html(stock_return,download_filename=filename,title=data.get('title'),output=True)
+        if "title" in data:
+            qs.reports.html(stock_return, download_filename=filename,
+                            title=data.get('title'), output=True)
         else:
-            qs.reports.html(stock_return,download_filename=filename,output=True)
-        
+            qs.reports.html(
+                stock_return, download_filename=filename, output=True)
+
         time.sleep(2)
 
         remove_text = 'http://quantstats.io'
         replace_text = 'https://www.algodojo.com/'
 
         with open(filename, 'r') as file:
             file_content = file.read()
 
         new_content = file_content.replace(remove_text, replace_text)
-        new_content = new_content.replace('QuantStats', 'Algodojo')
+        new_content = new_content.replace('QuantStats', 'AlgoDojo')
+        new_content = new_content.replace('(v. 0.0.59)', '')
 
         with open(filename, 'w') as file:
             file.write(new_content)
 
         print("Ended, the report was successfully generated")
 
+    def generate_report(self, title):
+        isGenerate = True
+        for isLastStatus in self.IsLastStatus:
+            if not isLastStatus:
+                isGenerate = False
 
-        
-
-
-    def generate_report(self,title):
-        if self.IsLastStatus:
+        if isGenerate:
             data = self.__BT_calculate_portfolio()
             if len(data.get('profit')) > 1:
-            # if len(data.get('profit')) > 1 and data.get('balance') <= 0:
-                self.__generate_report({
-                    'time': data.get('time'),
-                    'profit': data.get('profit'),
-                    'title':title
-                })
+                self.Report.TitleName = title
+                self.Report.BackTestBalance = self.BackTestBalance
+                self.Report.generate_report()
 
     def update_market_price(self):
         if self.BackTestToggle:
             self.__BT_limit_order_process()
-            return self.IsLastStatus
+            allDone = True
+            # print(f"self.IsLastStatus:{self.IsLastStatus}")
+            for value in self.IsLastStatus.values():
+                # print(f"value:{value}")
+                if not value:
+                    allDone = False
+            return allDone
         else:
             pass
 
     def __BT_limit_order_process(self):
-        market_price = self.LastDataRow.close.iloc[-1]
-        for index, order in enumerate(self.BT_Portfolio):
-            orderType = order.get('orderType')
-            status = order.get('status')
-            if (not orderType == 'MKT') and (not status):
-                lmtPrice = order['lmtPrice']
-                action = order['action']
-                if action == 'BUY' and lmtPrice <= market_price:
-                    self.BT_Portfolio[index]['dealPrice'] = market_price
-                    # print("action == 'BUY' and lmtPrice <= market_price")
-                if action == 'SELL' and lmtPrice >= market_price:
-                    self.BT_Portfolio[index]['dealPrice'] = market_price
-                    # print("action == 'SELL' and lmtPrice >= market_price")
+        for reqId in self.BT_Portfolio.keys():
+            market_price = self.LastDataRow[reqId].close.iloc[-1]
+
+            for index, order in enumerate(self.BT_Portfolio[reqId]):
+                orderType = order.get('orderType')
+                status = order.get('status')
+                if (not orderType == 'MKT') and (not status):
+                    lmtPrice = order['lmtPrice']
+                    action = order['action']
+                    if action == 'BUY' and lmtPrice <= market_price:
+                        self.BT_Portfolio[reqId][index]['dealPrice'] = market_price
+                        # print("action == 'BUY' and lmtPrice <= market_price")
+                    if action == 'SELL' and lmtPrice >= market_price:
+                        self.BT_Portfolio[reqId][index]['dealPrice'] = market_price
+                        # print("action == 'SELL' and lmtPrice >= market_price")
 
     def __BT_create_order(self, reqId, contract, order):
         action = order.get('action')
         totalQuantity = order.get('totalQuantity')
         orderType = order.get('orderType')
-        market_price = self.LastDataRow.close.iloc[-1]
-        time = self.LastDataRow.time.iloc[-1]
+        symbol = contract.get('symbol')
+
+        symbol_reqId = self.MappingLastDataRow[symbol]
+        market_price = self.LastDataRow[symbol_reqId].close.iloc[-1]
+        time = self.LastDataRow[symbol_reqId].time.iloc[-1]
 
         portfolio_value = {
+            'symbol': symbol,
             'action': action,
             'totalQuantity': totalQuantity,
             'orderType': orderType,
             'time': time
         }
 
         if orderType == 'MKT':
             portfolio_value['dealPrice'] = market_price
             portfolio_value['status'] = True
         else:
             lmtPrice = order.get('lmtPrice')
             portfolio_value['lmtPrice'] = lmtPrice
             portfolio_value['status'] = False
-        self.BT_Portfolio.append(portfolio_value)
 
+        if not symbol_reqId in self.BT_Portfolio:
+            self.BT_Portfolio[symbol_reqId] = []
+        # print(f"portfolio_value:{portfolio_value}")
+        self.BT_Portfolio[symbol_reqId].append(portfolio_value)
         data = {
             'orderId': reqId,
             'status': "Filled",
             'filled': totalQuantity,
             'remaining': 0,
             'avgFillPrice': market_price,
             'permId': 0,
@@ -1076,143 +1151,124 @@
             'mktCapPrice': market_price
         }
         self.receive_orderStatus(data)
 
         self.__BT_limit_order_process()
 
     def __BT_calculate_portfolio(self):
-        temp_balance = self.BackTestBalance
-        report_time_list = []
-        report_profit_list = []
-        hold = False
-        hold_action = None
-        hold_totalQuantity = 0
-        hold_price = 0
-        for portfolio_index, portfolio_value in enumerate(self.BT_Portfolio):
-
-            action = portfolio_value.get('action')
-            totalQuantity = portfolio_value.get('totalQuantity')
-            price = portfolio_value.get('dealPrice')
-            time = portfolio_value.get('time')
-
-            if not hold:
-                hold_action = action
-                hold_totalQuantity = totalQuantity
-                hold_price = price
-                hold = True
-            else:
-                if hold_action == 'SELL':
-                    if action == 'BUY':
-                        trade_profit = (hold_price - price) * totalQuantity
-                        temp_balance = temp_balance + trade_profit
-                        report_profit_list.append(trade_profit/temp_balance*100)
-                        hold_totalQuantity = hold_totalQuantity - totalQuantity
-                        report_time_list.append(time)
-                        if hold_totalQuantity <= 0:
-                            hold_totalQuantity = 0
-                            hold = False
-
-                else:
-                    if action == 'SELL':
-                        trade_profit = (price - hold_price) * totalQuantity
-                        temp_balance = temp_balance + trade_profit
-                        report_profit_list.append(trade_profit/temp_balance*100)
-                        hold_totalQuantity = hold_totalQuantity - totalQuantity
-                        report_time_list.append(time)
-                        if hold_totalQuantity <= 0:
-                            hold_totalQuantity = 0
-                            hold = False
+        self.Report.initPortfolioData()
+        # print(f"self.BT_Portfolio:{self.BT_Portfolio}")
+        for reqId in self.BT_Portfolio.keys():
+            for portfolio_index, portfolio_value in enumerate(self.BT_Portfolio[reqId]):
+                action = portfolio_value.get('action')
+                totalQuantity = portfolio_value.get('totalQuantity')
+                price = portfolio_value.get('dealPrice')
+                time = portfolio_value.get('time')
+                symbol = portfolio_value.get('symbol')
+                portfolio_value = {
+                    'symbol': reqId,
+                    'action': action,
+                    'totalQuantity': totalQuantity,
+                    'time': time,
+                    'dealPrice': price
+                }
+                self.Report.addPortfolioData(portfolio_value)
+
+        self.Report.CloseData = self.CloseData
+        # print(f"self.CloseData:{self.Report.CloseData}")
+        # print(f"self.Report:{self.Report.Portfolio}")
+        data = self.Report.calculate_portfolio()
 
         receive_portfolo_data = {
             # 'symbol': 'AAPL',
             # 'secType': 'STK',
             # 'exchange': 'NASDAQ',
             # 'currency': 'USD',
             # 'position': -10000.0,
             # 'marketPrice': 174.8500061,
             # 'marketValue': -1748500.06,
             # 'averageCost': 177.67396385,
             # 'unrealizedPNL': temp_balance,
-            'realizedPNL': temp_balance,
+            'realizedPNL': data.get('temp_balance')
             # 'accountName': 'DU2878211'
         }
 
         receive_portfolo = {
-            "balance": temp_balance,
-            "time": report_time_list,
-            "profit": report_profit_list,
+            "balance": data.get('temp_balance'),
+            "time": data.get('time'),
+            "profit": data.get('profit'),
             "receive_portfolo_data": receive_portfolo_data
         }
         return receive_portfolo
 
     def create_order(self, reqId, contractParams, orderParams):
         result = Result()
         strspan = 'send the create_order'
 
-        try:
-            self.__check_all()
-            if self.BackTestToggle:
-                self.__BT_create_order(reqId, contractParams, orderParams)
-            else:
-                # Contract
-                contract = Contract()
-
-                for key in contractParams:
-                    if hasattr(contract, key):
-                        setattr(contract, key, contractParams[key])
-                    else:
-                        raise ValueError(
-                            'The contract attribute not exist!! key:{key}'.format(key=key))
-                # Order
-                if "algorithms" in orderParams:
-                    algorithmsParams = orderParams['algorithms']
-                    del orderParams['algorithms']
-
-                order = Order()
-
-                for key in orderParams:
-                    if hasattr(order, key):
-                        setattr(order, key, orderParams[key])
-                    else:
-                        raise ValueError(
-                            'The order attribute not exist!! key:{key}'.format(key=key))
-                if 'algorithmsParams' in locals():
-                    if algorithmsParams.get('type') == 'ALGO':
-                        self.FillAdaptiveParams(
-                            order, algorithmsParams.get('priority'))
-                    elif algorithmsParams.get('type') == 'MIDPRICE':
-                        order.orderType = 'MIDPRICE'
-                    elif algorithmsParams.get('type') == 'TWAP':
-                        self.FillTwapParams(order,
-                                            algorithmsParams.get(
-                                                'strategyType'),
-                                            algorithmsParams.get('startTime'),
-                                            algorithmsParams.get('endTime'),
-                                            algorithmsParams.get(
-                                                'allowPastEndTime'),
-                                            algorithmsParams.get(
-                                                'monetaryValue')
-                                            )
-                    elif algorithmsParams.get('type') == 'VWAP':
-                        self.FillVwapParams(order,
-                                            algorithmsParams.get('maxPctVol'),
-                                            algorithmsParams.get('startTime'),
-                                            algorithmsParams.get('endTime'),
-                                            algorithmsParams.get(
-                                                'allowPastEndTime'),
-                                            algorithmsParams.get('noTakeLiq')
-                                            )
-
-                ib_return = self.placeOrder(reqId, contract, order)
+        # try:
+        self.__check_all()
+        if self.BackTestToggle:
+            self.__BT_create_order(reqId, contractParams, orderParams)
+        else:
+            # Contract
+            contract = Contract()
 
-                self.__post_order_data(reqId, contractParams, orderParams)
-            result.true(strspan)
-        except Exception as ex:
-            print('create_order error', ex)
-            result.false(f"{strspan} error: {ex}")
+            for key in contractParams:
+                if hasattr(contract, key):
+                    setattr(contract, key, contractParams[key])
+                else:
+                    raise ValueError(
+                        'The contract attribute not exist!! key:{key}'.format(key=key))
+            # Order
+            if "algorithms" in orderParams:
+                algorithmsParams = orderParams['algorithms']
+                del orderParams['algorithms']
+
+            order = Order()
+
+            for key in orderParams:
+                if hasattr(order, key):
+                    setattr(order, key, orderParams[key])
+                else:
+                    raise ValueError(
+                        'The order attribute not exist!! key:{key}'.format(key=key))
+            if 'algorithmsParams' in locals():
+                if algorithmsParams.get('type') == 'ALGO':
+                    self.FillAdaptiveParams(
+                        order, algorithmsParams.get('priority'))
+                elif algorithmsParams.get('type') == 'MIDPRICE':
+                    order.orderType = 'MIDPRICE'
+                elif algorithmsParams.get('type') == 'TWAP':
+                    self.FillTwapParams(order,
+                                        algorithmsParams.get(
+                                            'strategyType'),
+                                        algorithmsParams.get('startTime'),
+                                        algorithmsParams.get('endTime'),
+                                        algorithmsParams.get(
+                                            'allowPastEndTime'),
+                                        algorithmsParams.get(
+                                            'monetaryValue')
+                                        )
+                elif algorithmsParams.get('type') == 'VWAP':
+                    self.FillVwapParams(order,
+                                        algorithmsParams.get('maxPctVol'),
+                                        algorithmsParams.get('startTime'),
+                                        algorithmsParams.get('endTime'),
+                                        algorithmsParams.get(
+                                            'allowPastEndTime'),
+                                        algorithmsParams.get('noTakeLiq')
+                                        )
+
+            ib_return = self.placeOrder(reqId, contract, order)
+
+            self.__post_order_data(reqId, contractParams, orderParams)
+        result.true(strspan)
+        # except Exception as ex:
+        #     print('create_order error', ex)
+        #     result.false(f"{strspan} error: {ex}")
 
         return result
 
     def cancel_order(self, orderId):
         try:
             self.__check_all()
             self.cancelOrder(orderId)
@@ -1288,36 +1344,50 @@
         if not self.__IsMatch(DateFormat, startDateTime):
             raise ValueError('startDateTime value format is wrong!!')
 
         if datetime.strptime(startDateTime, "%Y-%m-%d") > datetime.strptime(endDateTime, "%Y-%m-%d"):
             raise ValueError(
                 'StartDateTime cannot be greater than endDateTime!!')
 
-    async def fetch_history(self, reqId, contractParams, requestParams):
+    def __check_request_limit(self):
+        result = False
+        limit_thread = self.requestCount
+        thread_count = len(self.TempHistoricalDataCollect)
+        if thread_count >= limit_thread:
+            result = True
+        return result
+
+    def fetch_history(self, reqId, contractParams, requestParams):
         print('Start of data transfer, Please wait...')
         result = Result()
         strspan = 'send the fetch_history'
         # print(strspan)
         try:
+            if self.__check_request_limit():
+                print("The number of data retrievals has exceeded the limit. Please log in to your AlgoDojo account and upgrade your data subscription to continue accessing data. https://www.algodojo.com/login")
+                pass
+
             self.__check_requestParams(requestParams)
             customerData = self.check_status()
             self.check_symbol(contractParams.get('symbol'))
             self.__check_barSize(requestParams)
 
             process_data = self.process_history(contractParams, requestParams)
             parameters = {
                 'startDate': process_data.get('startDateTime'),
                 'endDate': process_data.get('endDateTime'),
                 'symbol': process_data.get('symbol'),
                 'barSize': process_data.get('barSize'),
-                'granulariy': process_data.get('barSizeType')
+                'granulariy': process_data.get('barSizeType'),
+                'reqId': reqId
             }
+            process_data['reqId'] = reqId
             parameters['customerData'] = customerData
             # print('self.SendData(parameters)', 'before')
-            await self.SendData(parameters)
+            self.SendData(parameters)
             self.post_historydata(process_data)
             result.true(strspan)
         except Exception as err:
             print(f"{strspan} error: {err}")
             result.false(f"{strspan} error: {err}")
 
         return result
@@ -1403,12 +1473,14 @@
             self.reqAccountUpdates(False, acctCode)
             result.true(strspan)
         except Exception as ex:
             print(f"{strspan} error: {ex}")
             result.false(f"{strspan} error: {ex}")
 
         return result
+
     def __check_all(self):
+        # print("Fun","__check_all")
         self.check_status()
         # self.check_bata()
         if not self.BackTestToggle:
             self.__IsConnect()
```

