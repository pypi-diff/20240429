# Comparing `tmp/trytond_account-7.0.6.tar.gz` & `tmp/trytond_account-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account-7.0.6.tar", last modified: Wed Apr 17 10:46:01 2024, max compression
+gzip compressed data, was "trytond_account-7.2.0.tar", last modified: Mon Apr 29 15:31:25 2024, max compression
```

## Comparing `trytond_account-7.0.6.tar` & `trytond_account-7.2.0.tar`

### file list

```diff
@@ -1,258 +1,259 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:46:01.437108 trytond_account-7.0.6/
--rw-r--r--   0 ced       (1000) ced       (1000)    11094 2024-04-17 10:45:58.000000 trytond_account-7.0.6/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-17 10:45:58.000000 trytond_account-7.0.6/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:37.000000 trytond_account-7.0.6/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:37.000000 trytond_account-7.0.6/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-04-17 10:46:01.437108 trytond_account-7.0.6/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account-7.0.6/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3898 2023-10-30 17:06:37.000000 trytond_account-7.0.6/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)   126888 2024-04-12 20:44:51.000000 trytond_account-7.0.6/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    47195 2023-10-30 17:06:37.000000 trytond_account-7.0.6/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    51736 2023-10-30 17:06:38.000000 trytond_account-7.0.6/aged_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)     6318 2023-10-30 17:06:38.000000 trytond_account-7.0.6/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6045 2023-10-30 17:06:37.000000 trytond_account-7.0.6/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3080 2023-10-30 17:06:37.000000 trytond_account-7.0.6/company.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8831 2023-10-30 17:06:37.000000 trytond_account-7.0.6/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-10-30 17:06:37.000000 trytond_account-7.0.6/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:46:01.420442 trytond_account-7.0.6/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2786 2024-03-03 16:24:20.000000 trytond_account-7.0.6/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-10-30 17:06:37.000000 trytond_account-7.0.6/doc/configuration.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:46:01.420442 trytond_account-7.0.6/doc/design/
--rw-r--r--   0 ced       (1000) ced       (1000)     6585 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/design/account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/design/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3062 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/design/fiscal-year.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      198 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/design/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2124 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/design/journal.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6739 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/design/move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4330 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/design/tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4793 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/design/template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account-7.0.6/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1558 2023-10-30 17:06:38.000000 trytond_account-7.0.6/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:37.000000 trytond_account-7.0.6/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:37.000000 trytond_account-7.0.6/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2410 2023-10-30 17:06:38.000000 trytond_account-7.0.6/doc/setup.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:46:01.420442 trytond_account-7.0.6/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/usage/close.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1984 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/usage/create.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2858 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/usage/report.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1327 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/usage/structure.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2092 2024-02-05 16:24:27.000000 trytond_account-7.0.6/doc/usage/view.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1764 2024-02-05 16:24:27.000000 trytond_account-7.0.6/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26145 2024-02-05 16:24:27.000000 trytond_account-7.0.6/fiscalyear.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7617 2023-10-30 17:06:37.000000 trytond_account-7.0.6/fiscalyear.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    52160 2023-10-30 17:06:38.000000 trytond_account-7.0.6/general_journal.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    81559 2023-10-30 17:06:38.000000 trytond_account-7.0.6/general_ledger.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:46:01.420442 trytond_account-7.0.6/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_account-7.0.6/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:37.000000 trytond_account-7.0.6/icons/tryton-account-block.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-10-30 17:06:37.000000 trytond_account-7.0.6/icons/tryton-account-close.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-30 17:06:38.000000 trytond_account-7.0.6/icons/tryton-account-open.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-10-30 17:06:37.000000 trytond_account-7.0.6/icons/tryton-account.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    13034 2024-02-29 11:37:15.000000 trytond_account-7.0.6/journal.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11585 2023-10-30 17:06:38.000000 trytond_account-7.0.6/journal.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:46:01.423775 trytond_account-7.0.6/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)   131031 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)   130273 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)   114028 2023-10-30 17:06:37.000000 trytond_account-7.0.6/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)   133893 2023-10-30 17:06:37.000000 trytond_account-7.0.6/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)   130589 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)   118850 2023-10-30 17:06:37.000000 trytond_account-7.0.6/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)   126934 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   138509 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)   117820 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)   132568 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125409 2023-10-30 17:06:37.000000 trytond_account-7.0.6/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)   116858 2023-10-30 17:06:37.000000 trytond_account-7.0.6/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122752 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)   143136 2023-10-30 17:06:37.000000 trytond_account-7.0.6/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)   134636 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   130971 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122026 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125322 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   128774 2023-10-30 17:06:37.000000 trytond_account-7.0.6/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)   132947 2023-10-30 17:06:37.000000 trytond_account-7.0.6/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122943 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   113860 2023-10-30 17:06:37.000000 trytond_account-7.0.6/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   147904 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125886 2023-10-30 17:06:38.000000 trytond_account-7.0.6/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1494 2023-10-30 17:06:38.000000 trytond_account-7.0.6/localize.xsl
--rw-r--r--   0 ced       (1000) ced       (1000)    17440 2024-02-05 16:24:27.000000 trytond_account-7.0.6/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22110 2023-10-30 17:06:37.000000 trytond_account-7.0.6/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11303 2023-10-30 17:06:37.000000 trytond_account-7.0.6/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11052 2023-10-30 17:06:38.000000 trytond_account-7.0.6/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11058 2023-10-30 17:06:37.000000 trytond_account-7.0.6/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11004 2023-10-30 17:06:38.000000 trytond_account-7.0.6/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11069 2023-10-30 17:06:38.000000 trytond_account-7.0.6/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11050 2023-10-30 17:06:38.000000 trytond_account-7.0.6/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11083 2023-10-30 17:06:38.000000 trytond_account-7.0.6/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11090 2023-10-30 17:06:37.000000 trytond_account-7.0.6/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11405 2023-10-30 17:06:37.000000 trytond_account-7.0.6/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11056 2023-10-30 17:06:38.000000 trytond_account-7.0.6/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   116246 2024-03-25 21:44:24.000000 trytond_account-7.0.6/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27018 2023-10-30 17:06:38.000000 trytond_account-7.0.6/move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15750 2023-10-30 17:06:38.000000 trytond_account-7.0.6/move_template.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6825 2023-10-30 17:06:38.000000 trytond_account-7.0.6/move_template.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13724 2023-10-30 17:06:38.000000 trytond_account-7.0.6/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4226 2023-10-30 17:06:37.000000 trytond_account-7.0.6/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16034 2024-02-05 16:24:27.000000 trytond_account-7.0.6/period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4175 2023-10-30 17:06:38.000000 trytond_account-7.0.6/period.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:46:01.437108 trytond_account-7.0.6/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4586 2024-03-03 16:24:03.000000 trytond_account-7.0.6/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    70835 2024-01-08 10:53:54.000000 trytond_account-7.0.6/tax.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24586 2023-10-30 17:06:38.000000 trytond_account-7.0.6/tax.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:46:01.427108 trytond_account-7.0.6/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-10-30 17:06:38.000000 trytond_account-7.0.6/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4654 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_account_active.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-10-30 17:06:37.000000 trytond_account-7.0.6/tests/scenario_account_reconcile.json
--rw-r--r--   0 ced       (1000) ced       (1000)     3992 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_account_reconcile.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2456 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_account_reconcile_automatic.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6220 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_account_reconciliation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-10-30 17:06:38.000000 trytond_account-7.0.6/tests/scenario_account_reconciliation_alternate_currency.json
--rw-r--r--   0 ced       (1000) ced       (1000)     3640 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_account_reconciliation_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-10-30 17:06:38.000000 trytond_account-7.0.6/tests/scenario_account_reconciliation_alternate_currency_write_off.json
--rw-r--r--   0 ced       (1000) ced       (1000)     4369 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_account_reconciliation_alternate_currency_write_off.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4816 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_close_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4337 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_move_cancel.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_move_line_delegate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5034 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_move_line_group.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4919 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_move_line_reschedule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4696 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_move_template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2276 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    10880 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_reports.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2670 2024-02-05 16:24:27.000000 trytond_account-7.0.6/tests/scenario_tax_code.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    75953 2024-02-29 15:13:04.000000 trytond_account-7.0.6/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account-7.0.6/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4788 2023-10-30 17:06:38.000000 trytond_account-7.0.6/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account-7.0.6/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)    47972 2023-10-30 17:06:38.000000 trytond_account-7.0.6/trial_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-04 07:53:46.000000 trytond_account-7.0.6/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:46:01.437108 trytond_account-7.0.6/trytond_account.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-04-17 10:46:00.000000 trytond_account-7.0.6/trytond_account.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    12365 2024-04-17 10:46:01.000000 trytond_account-7.0.6/trytond_account.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:46:00.000000 trytond_account-7.0.6/trytond_account.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-17 10:46:00.000000 trytond_account-7.0.6/trytond_account.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:28.000000 trytond_account-7.0.6/trytond_account.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-17 10:46:00.000000 trytond_account-7.0.6/trytond_account.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:46:00.000000 trytond_account-7.0.6/trytond_account.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    54595 2023-10-30 17:06:38.000000 trytond_account-7.0.6/type_statement.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:46:01.437108 trytond_account-7.0.6/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/account_balance_sheet_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_deferral_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_deferral_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2841 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_income_statement_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_list_balance_sheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1074 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/account_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/account_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1283 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1103 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_type_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/account_type_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/account_type_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/account_type_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/aged_balance_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/aged_balance_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/balance_sheet_context_comparison_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/balance_sheet_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      710 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/company_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1353 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/create_chart_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/create_chart_properties_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/create_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/fiscalyear_balance_non_deferral_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/fiscalyear_create_periods_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      910 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/fiscalyear_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/fiscalyear_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      700 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/general_ledger_account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/general_ledger_account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/general_ledger_account_party_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/general_ledger_line_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      784 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/general_ledger_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1138 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/income_statement_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/journal_list_cash.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/journal_open_cash_context.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/journal_period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/journal_period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/journal_period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      272 2024-02-29 11:37:15.000000 trytond_account-7.0.6/view/journal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_cancel_default_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/move_line_delegate_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1753 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1241 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_line_form_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_line_group_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_line_list_payable_receivable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_line_list_reconcile.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_line_receivable_payable_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/move_line_reschedule_preview_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/move_line_reschedule_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_line_reschedule_term_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1026 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      636 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_line_tree_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_reconciliation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_reconciliation_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/move_template_create_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      857 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_template_keyword_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_template_keyword_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_template_keyword_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      614 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/open_journal_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1161 2023-10-30 17:06:37.000000 trytond_account-7.0.6/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/reconcile_lines_writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      755 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/reconcile_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/reconcile_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/renew_fiscalyear_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      555 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_code_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1122 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_code_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_code_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_code_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_code_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      843 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_code_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_code_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_code_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_code_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2193 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_group_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_rule_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_rule_line_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_rule_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_rule_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_rule_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_rule_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_rule_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2101 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/tax_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      250 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/update_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/update_chart_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-10-30 17:06:38.000000 trytond_account-7.0.6/view/writeoff_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.416906 trytond_account-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10737 2024-04-29 15:12:38.000000 trytond_account-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:12:38.000000 trytond_account-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-04-29 15:31:25.413573 trytond_account-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-25 11:39:10.000000 trytond_account-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3898 2024-01-27 09:58:52.000000 trytond_account-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   129467 2024-04-27 16:30:39.000000 trytond_account-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    46672 2024-04-27 16:30:39.000000 trytond_account-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    51736 2023-01-16 14:00:20.000000 trytond_account-7.2.0/aged_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2023-04-15 07:12:14.000000 trytond_account-7.2.0/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6045 2024-01-27 09:58:52.000000 trytond_account-7.2.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3024 2024-04-27 16:30:39.000000 trytond_account-7.2.0/company.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8831 2024-01-27 09:58:52.000000 trytond_account-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1998 2024-04-27 16:30:39.000000 trytond_account-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.396907 trytond_account-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-04-15 07:12:14.000000 trytond_account-7.2.0/doc/configuration.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.396907 trytond_account-7.2.0/doc/design/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6585 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/account.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/configuration.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3062 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/fiscal-year.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2246 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/journal.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6739 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/move.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4330 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/tax.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4793 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/design/template.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-25 11:39:10.000000 trytond_account-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1558 2023-04-15 07:12:14.000000 trytond_account-7.2.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:14.000000 trytond_account-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:50.000000 trytond_account-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2929 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/setup.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.396907 trytond_account-7.2.0/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/close.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1984 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/create.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2858 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/report.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/structure.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2092 2024-04-27 16:30:39.000000 trytond_account-7.2.0/doc/usage/view.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1808 2024-04-22 12:14:36.000000 trytond_account-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26581 2024-03-17 11:01:35.000000 trytond_account-7.2.0/fiscalyear.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7424 2024-04-27 16:30:39.000000 trytond_account-7.2.0/fiscalyear.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    52160 2023-04-15 07:12:14.000000 trytond_account-7.2.0/general_journal.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    81559 2024-02-04 18:51:26.000000 trytond_account-7.2.0/general_ledger.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.400240 trytond_account-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:14.000000 trytond_account-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-7.2.0/icons/tryton-account-block.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account-7.2.0/icons/tryton-account-close.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:14.000000 trytond_account-7.2.0/icons/tryton-account-open.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-01-16 14:00:20.000000 trytond_account-7.2.0/icons/tryton-account.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    13491 2024-04-27 16:30:39.000000 trytond_account-7.2.0/journal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12289 2024-04-27 16:30:39.000000 trytond_account-7.2.0/journal.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.400240 trytond_account-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)   130819 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   130189 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   114018 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   133816 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   130504 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   118696 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   126852 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   138321 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   117810 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   132544 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125268 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   116922 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   122609 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   142915 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   134510 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   130863 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   122016 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125178 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   129562 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   132756 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   122826 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   113850 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   147710 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125787 2024-04-29 13:17:17.000000 trytond_account-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1494 2023-04-15 07:12:14.000000 trytond_account-7.2.0/localize.xsl
+-rw-r--r--   0 ced       (1000) ced       (1000)    17448 2024-03-17 11:01:36.000000 trytond_account-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22110 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11303 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11052 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11058 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11004 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11069 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11050 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11083 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11090 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11405 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11056 2024-02-12 08:50:24.000000 trytond_account-7.2.0/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   116642 2024-04-27 16:37:33.000000 trytond_account-7.2.0/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26295 2024-04-27 16:30:39.000000 trytond_account-7.2.0/move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15750 2024-02-04 18:51:26.000000 trytond_account-7.2.0/move_template.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6717 2024-04-27 16:30:39.000000 trytond_account-7.2.0/move_template.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13726 2024-04-27 16:30:39.000000 trytond_account-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4156 2024-04-27 16:30:39.000000 trytond_account-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16319 2024-03-17 11:01:36.000000 trytond_account-7.2.0/period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4083 2024-04-27 16:30:39.000000 trytond_account-7.2.0/period.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:31:25.416906 trytond_account-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4586 2024-04-27 16:30:39.000000 trytond_account-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    70885 2024-04-27 16:30:39.000000 trytond_account-7.2.0/tax.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24263 2024-04-27 16:30:39.000000 trytond_account-7.2.0/tax.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.403574 trytond_account-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-04-15 07:12:14.000000 trytond_account-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4618 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_active.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-03-17 11:01:36.000000 trytond_account-7.2.0/tests/scenario_account_reconcile.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     3995 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_reconcile.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2442 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_reconcile_automatic.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_reconciliation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-02-04 18:51:26.000000 trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     3706 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-02-04 18:51:26.000000 trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency_write_off.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     4420 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency_write_off.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4736 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_close_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4270 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_move_cancel.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_move_line_delegate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5021 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_move_line_group.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4907 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_move_line_reschedule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4796 2024-04-27 16:37:33.000000 trytond_account-7.2.0/tests/scenario_move_template.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2223 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    10860 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_reports.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2658 2024-04-22 12:14:36.000000 trytond_account-7.2.0/tests/scenario_tax_code.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    80138 2024-04-27 16:30:39.000000 trytond_account-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-07-29 12:33:26.000000 trytond_account-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4788 2024-01-27 09:58:52.000000 trytond_account-7.2.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:50.000000 trytond_account-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)    47972 2023-04-15 07:12:14.000000 trytond_account-7.2.0/trial_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-29 15:12:34.000000 trytond_account-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.413573 trytond_account-7.2.0/trytond_account.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-04-29 15:31:24.000000 trytond_account-7.2.0/trytond_account.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    12499 2024-04-29 15:31:25.000000 trytond_account-7.2.0/trytond_account.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:31:24.000000 trytond_account-7.2.0/trytond_account.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:31:24.000000 trytond_account-7.2.0/trytond_account.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account-7.2.0/trytond_account.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-29 15:31:24.000000 trytond_account-7.2.0/trytond_account.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:31:24.000000 trytond_account-7.2.0/trytond_account.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    54595 2023-04-15 07:12:14.000000 trytond_account-7.2.0/type_statement.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:25.413573 trytond_account-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_balance_sheet_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_deferral_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_deferral_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2841 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_income_statement_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_list_balance_sheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1074 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1283 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1103 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/account_type_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/aged_balance_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/aged_balance_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/balance_sheet_context_comparison_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/balance_sheet_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      710 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/company_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1353 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/create_chart_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/create_chart_properties_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/create_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/fiscalyear_balance_non_deferral_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/fiscalyear_create_periods_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      910 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/fiscalyear_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/fiscalyear_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      750 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/general_ledger_account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/general_ledger_account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/general_ledger_account_party_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/general_ledger_line_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      784 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/general_ledger_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1138 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/income_statement_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2024-02-12 22:20:37.000000 trytond_account-7.2.0/view/journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/journal_list_cash.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/journal_list_matching_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/journal_open_cash_context.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/journal_period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/journal_period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/journal_period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      272 2024-04-27 16:30:39.000000 trytond_account-7.2.0/view/journal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/move_cancel_default_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_delegate_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1753 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1241 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/move_line_form_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_group_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_list_payable_receivable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_list_reconcile.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      443 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/move_line_receivable_payable_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_reschedule_preview_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/move_line_reschedule_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/move_line_reschedule_term_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/move_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/move_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1026 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      636 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_line_tree_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/move_reconciliation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/move_reconciliation_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_template_create_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      857 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/move_template_keyword_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/move_template_keyword_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/move_template_keyword_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/move_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      614 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/open_journal_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1161 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/reconcile_lines_writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      755 2024-01-27 09:58:52.000000 trytond_account-7.2.0/view/reconcile_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/reconcile_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/renew_fiscalyear_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      555 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1122 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_code_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_code_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_code_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      843 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_code_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_code_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2193 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_group_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_line_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_rule_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_rule_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2101 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/tax_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/tax_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      250 2023-01-16 14:00:20.000000 trytond_account-7.2.0/view/update_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/update_chart_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-02-04 18:51:26.000000 trytond_account-7.2.0/view/writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:14.000000 trytond_account-7.2.0/view/writeoff_tree.xml
```

### Comparing `trytond_account-7.0.6/CHANGELOG` & `trytond_account-7.2.0/CHANGELOG`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,14 @@
 
-Version 7.0.6 - 2024-04-17
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.5 - 2024-04-04
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.4 - 2024-03-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.3 - 2024-01-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.2 - 2024-01-01
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2023-12-16
---------------------------
-* Bug fixes (see mercurial logs for details)
-
+* Convert recursive calls of reconcile accounts wizard into loop
+* Remove active field on journal - period
+* Allow modifying period dates with moves
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Use origin description as fallback description
 * Post write-off and exchange moves when reconcile posted lines
```

### Comparing `trytond_account-7.0.6/COPYRIGHT` & `trytond_account-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/LICENSE` & `trytond_account-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/PKG-INFO` & `trytond_account-7.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account
-Version: 7.0.6
+Version: 7.2.0
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-account/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -51,20 +51,20 @@
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-dateutil
 Requires-Dist: python-sql>=0.7
 Requires-Dist: simpleeval
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##############
 Account Module
 ##############
 
 The *Account Module* defines the fundamentals needed for basic double entry
 accounting.
```

### Comparing `trytond_account-7.0.6/__init__.py` & `trytond_account-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/account.py` & `trytond_account-7.2.0/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -830,22 +830,28 @@
             update(childs)
             childs = sum((c.childs for c in childs), ())
 
 
 class AccountTemplateTaxTemplate(ModelSQL):
     'Account Template - Tax Template'
     __name__ = 'account.account.template-account.tax.template'
-    _table = 'account_account_template_tax_rel'
     account = fields.Many2One(
         'account.account.template', "Account Template",
         ondelete='CASCADE', required=True)
     tax = fields.Many2One(
         'account.tax.template', "Tax Template",
         ondelete='RESTRICT', required=True)
 
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'account_account_template_tax_rel', cls._table)
+        super().__register__(module)
+
 
 class Account(
         AccountMixin(), ContextCompanyMixin, ActivePeriodMixin, tree(),
         ModelSQL, ModelView):
     'Account'
     __name__ = 'account.account'
     _states = {
@@ -944,16 +950,16 @@
             })
     taxes = fields.Many2Many('account.account-account.tax',
         'account', 'tax', 'Default Taxes',
         domain=[
             ('company', '=', Eval('company')),
             ('parent', '=', None),
             ],
-        help="Default tax for manual encoding of move lines\n"
-        'for journal types: "expense" and "revenue".')
+        help="Default taxes for documents to be applied "
+        "when there is no other source.")
     replaced_by = fields.Many2One(
         'account.account', "Replaced By",
         domain=[('company', '=', Eval('company', -1))],
         states={
             'readonly': _states['readonly'],
             'invisible': ~Eval('end_date'),
             })
@@ -1802,20 +1808,26 @@
     def write(cls, deferrals, values, *args):
         raise AccessError(gettext('account.msg_write_deferral'))
 
 
 class AccountTax(ModelSQL):
     'Account - Tax'
     __name__ = 'account.account-account.tax'
-    _table = 'account_account_tax_rel'
     account = fields.Many2One(
         'account.account', "Account", ondelete='CASCADE', required=True)
     tax = fields.Many2One(
         'account.tax', "Tax", ondelete='RESTRICT', required=True)
 
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'account_account_tax_rel', cls._table)
+        super().__register__(module)
+
 
 class AccountContext(ModelView):
     'Account Context'
     __name__ = 'account.account.context'
 
     company = fields.Many2One('company.company', "Company", required=True)
     fiscalyear = fields.Many2One(
@@ -2227,17 +2239,26 @@
 
     @classmethod
     def default_to_date(cls):
         return Transaction().context.get('to_date')
 
     @fields.depends('company', 'fiscalyear', methods=['on_change_fiscalyear'])
     def on_change_company(self):
-        if self.fiscalyear and self.fiscalyear.company != self.company:
+        pool = Pool()
+        FiscalYear = pool.get('account.fiscalyear')
+        if not self.company:
             self.fiscalyear = None
             self.on_change_fiscalyear()
+        elif not self.fiscalyear or self.fiscalyear.company != self.company:
+            try:
+                self.fiscalyear = FiscalYear.find(
+                    self.company, test_state=False)
+                self.on_change_fiscalyear()
+            except FiscalYearNotFoundError:
+                pass
 
     @fields.depends('fiscalyear', 'start_period', 'end_period')
     def on_change_fiscalyear(self):
         if (self.start_period
                 and self.start_period.fiscalyear != self.fiscalyear):
             self.start_period = None
         if (self.end_period
@@ -2711,41 +2732,51 @@
             ])
     start_period_cmp = fields.Many2One('account.period', 'Start Period',
         domain=[
             ('fiscalyear', '=', Eval('fiscalyear_cmp')),
             ('start_date', '<=', (Eval('end_period_cmp'), 'start_date'))
             ],
         states={
-            'invisible': ~Eval('comparison', False),
+            'invisible': (
+                ~Eval('comparison', False)
+                | Eval('from_date_cmp', False) | Eval('to_date_cmp', False)),
             })
     end_period_cmp = fields.Many2One('account.period', 'End Period',
         domain=[
             ('fiscalyear', '=', Eval('fiscalyear_cmp')),
             ('start_date', '>=', (Eval('start_period_cmp'), 'start_date')),
             ],
         states={
-            'invisible': ~Eval('comparison', False),
+            'invisible': (
+                ~Eval('comparison', False)
+                | Eval('from_date_cmp', False) | Eval('to_date_cmp', False)),
             })
     from_date_cmp = fields.Date("From Date",
         domain=[
             If(Eval('to_date_cmp') & Eval('from_date_cmp'),
                 ('from_date_cmp', '<=', Eval('to_date_cmp')),
                 ()),
             ],
         states={
-            'invisible': ~Eval('comparison', False),
+            'invisible': (
+                ~Eval('comparison', False)
+                | Eval('start_period_cmp', False)
+                | Eval('end_period_cmp', False)),
             })
     to_date_cmp = fields.Date("To Date",
         domain=[
             If(Eval('from_date_cmp') & Eval('to_date_cmp'),
                 ('to_date_cmp', '>=', Eval('from_date_cmp')),
                 ()),
             ],
         states={
-            'invisible': ~Eval('comparison', False),
+            'invisible': (
+                ~Eval('comparison', False)
+                | Eval('start_period_cmp', False)
+                | Eval('end_period_cmp', False)),
             })
 
     @classmethod
     def default_fiscalyear(cls):
         pool = Pool()
         FiscalYear = pool.get('account.fiscalyear')
         try:
@@ -2765,17 +2796,28 @@
 
     @classmethod
     def default_comparison(cls):
         return False
 
     @fields.depends('company', 'fiscalyear', methods=['on_change_fiscalyear'])
     def on_change_company(self):
-        if self.fiscalyear and self.fiscalyear.company != self.company:
+        pool = Pool()
+        FiscalYear = pool.get('account.fiscalyear')
+        if not self.company:
             self.fiscalyear = None
             self.on_change_fiscalyear()
+            self.fiscalyear_cmp = None
+            self.on_change_fiscalyear_cmp()
+        elif not self.fiscalyear or self.fiscalyear.company != self.company:
+            try:
+                self.fiscalyear = FiscalYear.find(
+                    self.company, test_state=False)
+                self.on_change_fiscalyear()
+            except FiscalYearNotFoundError:
+                pass
 
     @fields.depends('fiscalyear', 'start_period', 'end_period')
     def on_change_fiscalyear(self):
         if (self.start_period
                 and self.start_period.fiscalyear != self.fiscalyear):
             self.start_period = None
         if (self.end_period
@@ -2798,14 +2840,43 @@
             self.start_period = self.end_period = None
 
     @fields.depends('to_date')
     def on_change_to_date(self):
         if self.to_date:
             self.start_period = self.end_period = None
 
+    @fields.depends('fiscalyear_cmp', 'start_period_cmp', 'end_period_cmp')
+    def on_change_fiscalyear_cmp(self):
+        if (self.start_period_cmp
+                and self.start_period_cmp.fiscalyear != self.fiscalyear):
+            self.start_period_cmp = None
+        if (self.end_period_cmp
+                and self.end_period_cmp.fiscalyear != self.fiscalyear):
+            self.end_period_cmp = None
+
+    @fields.depends('start_period_cmp')
+    def on_change_start_period_cmp(self):
+        if self.start_period_cmp:
+            self.from_date_cmp = self.to_date_cmp = None
+
+    @fields.depends('end_period_cmp')
+    def on_change_end_period_cmp(self):
+        if self.end_period_cmp:
+            self.from_date_cmp = self.to_date_cmp = None
+
+    @fields.depends('from_date_cmp')
+    def on_change_from_date_cmp(self):
+        if self.from_date_cmp:
+            self.start_period_cmp = self.end_period_cmp = None
+
+    @fields.depends('to_date_cmp')
+    def on_change_to_date_cmp(self):
+        if self.to_date_cmp:
+            self.start_period_cmp = self.end_period_cmp = None
+
     @classmethod
     def view_attributes(cls):
         return super().view_attributes() + [
             ('/form/separator[@id="comparison"]', 'states', {
                     'invisible': ~Eval('comparison', False),
                     }),
             ]
@@ -3137,17 +3208,15 @@
             pool.get('account.tax.rule.line.template')
         Config = pool.get('ir.configuration')
         Account = pool.get('account.account')
         Warning = pool.get('res.user.warning')
         transaction = Transaction()
 
         company = self.account.company
-        # Skip access rule
-        with transaction.set_user(0):
-            accounts = Account.search([('company', '=', company.id)], limit=1)
+        accounts = Account.search([('company', '=', company.id)], limit=1)
         if accounts:
             key = 'duplicated_chart.%d' % company.id
             if Warning.check(key):
                 raise ChartWarning(key,
                     gettext('account.msg_account_chart_exists',
                         company=company.rec_name))
```

### Comparing `trytond_account-7.0.6/account.xml` & `trytond_account-7.2.0/account.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account-7.0.6/account.xml` & `trytond_account-7.2.0/account.xml`

```diff
@@ -141,49 +141,53 @@
     <record model="ir.action.act_window.view" id="act_account_type_list_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="account_type_view_form"/>
       <field name="act_window" ref="act_account_type_list"/>
     </record>
     <menuitem parent="menu_account_type_tree" action="act_account_type_list" sequence="10" id="menu_account_type_list"/>
     <record model="ir.model.access" id="access_account_type">
-      <field name="model" search="[('model', '=', 'account.account.type')]"/>
+      <field name="model">account.account.type</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_account_type_account_admin">
-      <field name="model" search="[('model', '=', 'account.account.type')]"/>
+      <field name="model">account.account.type</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_account_type_amount">
-      <field name="field" search="[('model.model', '=', 'account.account.type'), ('name', '=', 'amount')]"/>
+      <field name="model">account.account.type</field>
+      <field name="field">amount</field>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_account_type_amount_account">
-      <field name="field" search="[('model.model', '=', 'account.account.type'), ('name', '=', 'amount')]"/>
+      <field name="model">account.account.type</field>
+      <field name="field">amount</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_account_type_amount_cmp">
-      <field name="field" search="[('model.model', '=', 'account.account.type'), ('name', '=', 'amount_cmp')]"/>
+      <field name="model">account.account.type</field>
+      <field name="field">amount_cmp</field>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_account_type_amount_cmp_account">
-      <field name="field" search="[('model.model', '=', 'account.account.type'), ('name', '=', 'amount_cmp')]"/>
+      <field name="model">account.account.type</field>
+      <field name="field">amount_cmp</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_account_type_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.account.type')]"/>
+      <field name="model">account.account.type</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_account_type_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_account_type_companies"/>
     </record>
     <record model="ir.action.report" id="report_account_type_statement">
@@ -233,15 +237,15 @@
     <record model="ir.action.act_window.view" id="act_account_template_tree_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="account_template_view_form"/>
       <field name="act_window" ref="act_account_template_tree"/>
     </record>
     <menuitem parent="menu_templates" action="act_account_template_tree" sequence="20" id="menu_account_template_tree"/>
     <record model="ir.model.access" id="access_account_template">
-      <field name="model" search="[('model', '=', 'account.account.template')]"/>
+      <field name="model">account.account.template</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="account_deferral_view_form">
       <field name="model">account.account.deferral</field>
@@ -384,67 +388,75 @@
     <record model="ir.action.act_window.view" id="act_account_tree_chart_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="account_view_tree_chart"/>
       <field name="act_window" ref="act_account_tree_chart"/>
     </record>
     <menuitem parent="menu_reporting" action="act_account_tree_chart" sequence="30" id="menu_account_tree_chart"/>
     <record model="ir.model.access" id="access_account">
-      <field name="model" search="[('model', '=', 'account.account')]"/>
+      <field name="model">account.account</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_account_account_admin">
-      <field name="model" search="[('model', '=', 'account.account')]"/>
+      <field name="model">account.account</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_account_balance">
-      <field name="field" search="[('model.model', '=', 'account.account'), ('name', '=', 'balance')]"/>
+      <field name="model">account.account</field>
+      <field name="field">balance</field>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_account_balance_account">
-      <field name="field" search="[('model.model', '=', 'account.account'), ('name', '=', 'balance')]"/>
+      <field name="model">account.account</field>
+      <field name="field">balance</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_account_credit">
-      <field name="field" search="[('model.model', '=', 'account.account'), ('name', '=', 'credit')]"/>
+      <field name="model">account.account</field>
+      <field name="field">credit</field>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_account_credit_account">
-      <field name="field" search="[('model.model', '=', 'account.account'), ('name', '=', 'credit')]"/>
+      <field name="model">account.account</field>
+      <field name="field">credit</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_account_debit">
-      <field name="field" search="[('model.model', '=', 'account.account'), ('name', '=', 'debit')]"/>
+      <field name="model">account.account</field>
+      <field name="field">debit</field>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_account_debit_account">
-      <field name="field" search="[('model.model', '=', 'account.account'), ('name', '=', 'debit')]"/>
+      <field name="model">account.account</field>
+      <field name="field">debit</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_account_amount_second_currency">
-      <field name="field" search="[('model.model', '=', 'account.account'), ('name', '=', 'amount_second_currency')]"/>
+      <field name="model">account.account</field>
+      <field name="field">amount_second_currency</field>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_account_amount_second_currency_account">
-      <field name="field" search="[('model.model', '=', 'account.account'), ('name', '=', 'amount_second_currency')]"/>
+      <field name="model">account.account</field>
+      <field name="field">amount_second_currency</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_account_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.account')]"/>
+      <field name="model">account.account</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_account_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_account_companies"/>
     </record>
     <record model="ir.ui.view" id="account_context_view_form">
@@ -502,31 +514,31 @@
     </record>
     <record model="ir.action.act_window.view" id="act_account_general_ledger_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="general_ledger_account_view_list"/>
       <field name="act_window" ref="act_account_general_ledger"/>
     </record>
     <record model="ir.model.access" id="access_general_ledger_account">
-      <field name="model" search="[('model', '=', 'account.general_ledger.account')]"/>
+      <field name="model">account.general_ledger.account</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_general_ledger_account_account">
-      <field name="model" search="[('model', '=', 'account.general_ledger.account')]"/>
+      <field name="model">account.general_ledger.account</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.rule.group" id="rule_group_general_ledger_account_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.general_ledger.account')]"/>
+      <field name="model">account.general_ledger.account</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_general_ledger_account_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_general_ledger_account_companies"/>
     </record>
     <record model="ir.ui.view" id="general_ledger_account_party_view_list">
@@ -577,31 +589,31 @@
     </record>
     <record model="ir.action.keyword" id="act_general_ledger_account_party_form_party_relate_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">party.party,-1</field>
       <field name="action" ref="act_general_ledger_account_party_form_party"/>
     </record>
     <record model="ir.model.access" id="access_general_ledger_account_party">
-      <field name="model" search="[('model', '=', 'account.general_ledger.account.party')]"/>
+      <field name="model">account.general_ledger.account.party</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_general_ledger_account_account_party">
-      <field name="model" search="[('model', '=', 'account.general_ledger.account.party')]"/>
+      <field name="model">account.general_ledger.account.party</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.rule.group" id="rule_group_general_ledger_account_party_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.general_ledger.account.party')]"/>
+      <field name="model">account.general_ledger.account.party</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_general_ledger_account_party_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_general_ledger_account_party_companies"/>
     </record>
     <record model="ir.ui.view" id="general_ledger_line_view_list">
@@ -628,15 +640,15 @@
     <record model="ir.action.keyword" id="act_general_ledger_line_form_keyword_account">
       <field name="keyword">form_relate</field>
       <field name="model">account.account,-1</field>
       <field name="action" ref="act_general_ledger_line_form"/>
     </record>
     <record model="ir.rule.group" id="rule_group_general_ledger_line_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.general_ledger.line')]"/>
+      <field name="model">account.general_ledger.line</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_general_ledger_line_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_general_ledger_line_companies"/>
     </record>
     <record model="ir.ui.view" id="general_ledger_account_context_view_form">
@@ -716,31 +728,31 @@
     <record model="ir.action.act_window.view" id="act_aged_balance_list_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="aged_balance_view_list"/>
       <field name="act_window" ref="act_aged_balance_list"/>
     </record>
     <menuitem parent="menu_reporting" action="act_aged_balance_list" sequence="50" id="menu_aged_balance"/>
     <record model="ir.model.access" id="access_aged_balance">
-      <field name="model" search="[('model', '=', 'account.aged_balance')]"/>
+      <field name="model">account.aged_balance</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_aged_balance_account">
-      <field name="model" search="[('model', '=', 'account.aged_balance')]"/>
+      <field name="model">account.aged_balance</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.rule.group" id="rule_group_aged_balance_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.aged_balance')]"/>
+      <field name="model">account.aged_balance</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_aged_balance_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_aged_balance_companies"/>
     </record>
     <record model="ir.ui.view" id="aged_balance_context_view_form">
```

### Comparing `trytond_account-7.0.6/aged_balance.fodt` & `trytond_account-7.2.0/aged_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/common.py` & `trytond_account-7.2.0/common.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/company.py` & `trytond_account-7.2.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/company.xml` & `trytond_account-7.2.0/company.xml`

 * *Files 22% similar despite different names*

#### Comparing `trytond_account-7.0.6/company.xml` & `trytond_account-7.2.0/company.xml`

```diff
@@ -10,44 +10,52 @@
     </record>
     <record model="ir.ui.view" id="company_view_form">
       <field name="model">company.company</field>
       <field name="inherit" ref="company.company_view_form"/>
       <field name="name">company_form</field>
     </record>
     <record model="ir.model.field.access" id="access_company_receivable">
-      <field name="field" search="[('model.model', '=', 'company.company'), ('name', '=', 'receivable')]"/>
+      <field name="model">company.company</field>
+      <field name="field">receivable</field>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_company_receivable_account">
-      <field name="field" search="[('model.model', '=', 'company.company'), ('name', '=', 'receivable')]"/>
+      <field name="model">company.company</field>
+      <field name="field">receivable</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_company_payable">
-      <field name="field" search="[('model.model', '=', 'company.company'), ('name', '=', 'payable')]"/>
+      <field name="model">company.company</field>
+      <field name="field">payable</field>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_company_payable_account">
-      <field name="field" search="[('model.model', '=', 'company.company'), ('name', '=', 'payable')]"/>
+      <field name="model">company.company</field>
+      <field name="field">payable</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_company_receivable_today">
-      <field name="field" search="[('model.model', '=', 'company.company'), ('name', '=', 'receivable_today')]"/>
+      <field name="model">company.company</field>
+      <field name="field">receivable_today</field>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_company_receivable_today_account">
-      <field name="field" search="[('model.model', '=', 'company.company'), ('name', '=', 'receivable_today')]"/>
+      <field name="model">company.company</field>
+      <field name="field">receivable_today</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_company_payable_today">
-      <field name="field" search="[('model.model', '=', 'company.company'), ('name', '=', 'payable_today')]"/>
+      <field name="model">company.company</field>
+      <field name="field">payable_today</field>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_company_payable_today_account">
-      <field name="field" search="[('model.model', '=', 'company.company'), ('name', '=', 'payable_today')]"/>
+      <field name="model">company.company</field>
+      <field name="field">payable_today</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_account-7.0.6/configuration.py` & `trytond_account-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/configuration.xml` & `trytond_account-7.2.0/configuration.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account-7.0.6/configuration.xml` & `trytond_account-7.2.0/configuration.xml`

```diff
@@ -15,22 +15,22 @@
     <record model="ir.action.act_window.view" id="act_configuration_view1">
       <field name="sequence" eval="1"/>
       <field name="view" ref="configuration_view_form"/>
       <field name="act_window" ref="act_configuration_form"/>
     </record>
     <menuitem parent="menu_account_configuration" action="act_configuration_form" sequence="0" id="menuitem_account_configuration" icon="tryton-list"/>
     <record model="ir.model.access" id="access_account_configuration">
-      <field name="model" search="[('model', '=', 'account.configuration')]"/>
+      <field name="model">account.configuration</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_account_configuration_account_admin">
-      <field name="model" search="[('model', '=', 'account.configuration')]"/>
+      <field name="model">account.configuration</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_account-7.0.6/doc/conf.py` & `trytond_account-7.2.0/doc/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,22 +67,33 @@
     }
 html_title = info['description']
 master_doc = 'index'
 project = info['name']
 release = version = info['series']
 default_role = 'ref'
 highlight_language = 'none'
+exclude_patterns = ['**/*.inc.rst']
 extensions = [
     'sphinx_copybutton',
     'sphinx.ext.intersphinx',
     ]
 intersphinx_mapping = {
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
 linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
+try:
+    with open(os.path.join(
+                os.path.dirname(__file__),
+                'linkcheck_ignore.json'), 'r') as f:
+        import json
+        linkcheck_ignore.extend(json.load(f))
+        del json
+except FileNotFoundError:
+    pass
+
 del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_account-7.0.6/doc/configuration.rst` & `trytond_account-7.2.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/design/account.rst` & `trytond_account-7.2.0/doc/design/account.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/design/configuration.rst` & `trytond_account-7.2.0/doc/design/configuration.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/design/fiscal-year.rst` & `trytond_account-7.2.0/doc/design/fiscal-year.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/design/journal.rst` & `trytond_account-7.2.0/doc/design/journal.inc.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 to be grouped together.
 Every account move gets associated with a journal, and the journal defines
 what sequence is then used to number the account move.
 
 Among the journal's properties is a type.
 This limits where the journal can be used.
 
+When the system needs a journal, it chooses the first journal from the ordered
+list that matches the requested criteria.
+
 .. seealso::
 
    The journals can be found by opening the main menu item:
 
       |Financial --> Configuration --> Journals --> Journals|__
 
       .. |Financial --> Configuration --> Journals --> Journals| replace:: :menuselection:`Financial --> Configuration --> Journals --> Journals`
```

### Comparing `trytond_account-7.0.6/doc/design/move.rst` & `trytond_account-7.2.0/doc/design/move.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/design/tax.rst` & `trytond_account-7.2.0/doc/design/tax.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/design/template.rst` & `trytond_account-7.2.0/doc/design/template.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/reference.rst` & `trytond_account-7.2.0/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/setup.rst` & `trytond_account-7.2.0/doc/setup.rst`

 * *Files 14% similar despite different names*

```diff
@@ -58,7 +58,23 @@
 `Company <company:model-company.company>`, bearing in mind some reports are
 generated based on periods, and periods allow you to build up your accounts in
 smaller chunks.
 
 .. tip::
 
    Tryton also provides easy ways of `Creating additional fiscal years`.
+
+.. _Fill opening balance:
+
+Fill opening balance
+====================
+
+If your company already had a balance before the first :ref:`Fiscal Year
+<model-account.fiscalyear>` created in Tryton, you should `create a journal
+entry <Creating journal entries>` with one line for each `Account
+<model-account.account>` with the balance as credit or debit.
+
+.. tip::
+
+   It is best to use an adjustment `Period <model-account.period>` at the
+   begining the fiscal year and a ``Situation`` `Journal
+   <model-account.journal>`.
```

### Comparing `trytond_account-7.0.6/doc/usage/close.rst` & `trytond_account-7.2.0/doc/usage/close.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/usage/create.rst` & `trytond_account-7.2.0/doc/usage/create.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/usage/process.rst` & `trytond_account-7.2.0/doc/usage/process.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/usage/report.rst` & `trytond_account-7.2.0/doc/usage/report.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/usage/structure.rst` & `trytond_account-7.2.0/doc/usage/structure.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/doc/usage/view.rst` & `trytond_account-7.2.0/doc/usage/view.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/exceptions.py` & `trytond_account-7.2.0/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,18 @@
     pass
 
 
 class FiscalYearReOpenError(UserError):
     pass
 
 
+class JournalMissing(UserError):
+    pass
+
+
 class AccountMissing(UserError):
     pass
 
 
 class AccountValidationError(ValidationError):
     pass
```

### Comparing `trytond_account-7.0.6/fiscalyear.py` & `trytond_account-7.2.0/fiscalyear.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
             }.get(self.state)
 
     @classmethod
     def validate_fields(cls, fiscalyears, field_names):
         super().validate_fields(fiscalyears, field_names)
         cls.check_dates(fiscalyears, field_names)
         cls.check_post_move_sequence(fiscalyears, field_names)
+        cls.check_period_dates(fiscalyears, field_names)
 
     @classmethod
     def check_dates(cls, fiscalyears, field_names=None):
         if field_names and not (field_names & {
                     'start_date', 'end_date', 'state', 'company'}):
             return
         transaction = Transaction()
@@ -171,14 +172,23 @@
             if years:
                 raise FiscalYearSequenceError(gettext(
                         'account.msg_fiscalyear_different_post_move_sequence',
                         first=fiscalyear.rec_name,
                         second=years[0].rec_name))
 
     @classmethod
+    def check_period_dates(cls, fiscalyears, field_names=None):
+        pool = Pool()
+        Period = pool.get('account.period')
+        if field_names and not (field_names & {'start_date', 'end_date'}):
+            return
+        periods = [p for f in fiscalyears for p in f.periods]
+        Period.check_fiscalyear_dates(periods, field_names={'fiscalyear'})
+
+    @classmethod
     def create(cls, vlist):
         fiscalyears = super().create(vlist)
         cls._find_cache.clear()
         return fiscalyears
 
     @classmethod
     def write(cls, *args):
```

### Comparing `trytond_account-7.0.6/fiscalyear.xml` & `trytond_account-7.2.0/fiscalyear.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_account-7.0.6/fiscalyear.xml` & `trytond_account-7.2.0/fiscalyear.xml`

```diff
@@ -31,52 +31,52 @@
     <record model="ir.action.act_window.view" id="act_fiscalyear_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="fiscalyear_view_form"/>
       <field name="act_window" ref="act_fiscalyear_form"/>
     </record>
     <menuitem parent="menu_fiscalyear_configuration" action="act_fiscalyear_form" sequence="10" id="menu_fiscalyear_form"/>
     <record model="ir.model.access" id="access_fiscalyear">
-      <field name="model" search="[('model', '=', 'account.fiscalyear')]"/>
+      <field name="model">account.fiscalyear</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_fiscalyear_account_admin">
-      <field name="model" search="[('model', '=', 'account.fiscalyear')]"/>
+      <field name="model">account.fiscalyear</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="fiscalyear_create_periods_button">
+      <field name="model">account.fiscalyear</field>
       <field name="name">create_periods</field>
       <field name="string">Create Periods</field>
-      <field name="model" search="[('model', '=', 'account.fiscalyear')]"/>
     </record>
     <record model="ir.model.button" id="fiscalyear_reopen_button">
+      <field name="model">account.fiscalyear</field>
       <field name="name">reopen</field>
       <field name="string">Re-Open</field>
-      <field name="model" search="[('model', '=', 'account.fiscalyear')]"/>
     </record>
     <record model="ir.model.button" id="fiscalyear_close_button">
+      <field name="model">account.fiscalyear</field>
       <field name="name">close</field>
       <field name="string">Close</field>
-      <field name="model" search="[('model', '=', 'account.fiscalyear')]"/>
     </record>
     <record model="ir.model.button" id="fiscalyear_lock_button">
+      <field name="model">account.fiscalyear</field>
       <field name="name">lock_</field>
       <field name="string">Lock</field>
       <field name="confirm">Are you sure you want to lock the fiscal year?</field>
-      <field name="model" search="[('model', '=', 'account.fiscalyear')]"/>
     </record>
     <record model="ir.rule.group" id="rule_group_fiscalyear_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.fiscalyear')]"/>
+      <field name="model">account.fiscalyear</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_fiscalyear_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_fiscalyear_companies"/>
     </record>
     <record model="ir.action.act_window" id="act_fiscalyear_form_close">
```

### Comparing `trytond_account-7.0.6/general_journal.fodt` & `trytond_account-7.2.0/general_journal.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/general_ledger.fodt` & `trytond_account-7.2.0/general_ledger.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/icons/LICENSE` & `trytond_account-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/journal.py` & `trytond_account-7.2.0/journal.py`

 * *Files 4% similar despite different names*

```diff
@@ -221,22 +221,29 @@
 
     @classmethod
     def default_start_date(cls):
         return Pool().get('ir.date').today()
     default_end_date = default_start_date
 
 
-class JournalPeriod(
-        DeactivableMixin, Workflow, ModelSQL, ModelView):
+class JournalPeriod(Workflow, ModelSQL, ModelView):
     'Journal - Period'
     __name__ = 'account.journal.period'
-    journal = fields.Many2One('account.journal', 'Journal', required=True,
-            ondelete='CASCADE', states=STATES)
+    journal = fields.Many2One(
+        'account.journal', 'Journal', required=True, ondelete='CASCADE',
+        states=STATES,
+        context={
+            'company': Eval('company', None),
+            },
+        depends=['company'])
     period = fields.Many2One('account.period', 'Period', required=True,
             ondelete='CASCADE', states=STATES)
+    company = fields.Function(fields.Many2One(
+            'company.company', "Company"),
+        'on_change_with_company', searcher='search_company')
     icon = fields.Function(fields.Char('Icon'), 'get_icon')
     state = fields.Selection([
         ('open', 'Open'),
         ('closed', 'Closed'),
         ], 'State', readonly=True, required=True, sort=False)
 
     @classmethod
@@ -257,25 +264,32 @@
                     'depends': ['state'],
                     },
                 'reopen': {
                     'invisible': Eval('state') != 'closed',
                     'depends': ['state'],
                     },
                 })
-        cls.active.states = STATES
 
     @classmethod
     def __register__(cls, module):
         cursor = Transaction().connection.cursor()
         t = cls.__table__()
         super().__register__(module)
         # Migration from 6.8: rename state close to closed
         cursor.execute(
             *t.update([t.state], ['closed'], where=t.state == 'close'))
 
+    @fields.depends('period')
+    def on_change_with_company(self, name=None):
+        return self.period.company if self.period else None
+
+    @classmethod
+    def search_company(cls, name, clause):
+        return [('period.' + clause[0], *clause[1:])]
+
     @staticmethod
     def default_state():
         return 'open'
 
     def get_rec_name(self, name):
         return '%s - %s' % (self.journal.rec_name, self.period.rec_name)
```

### Comparing `trytond_account-7.0.6/journal.xml` & `trytond_account-7.2.0/journal.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account-7.0.6/journal.xml` & `trytond_account-7.2.0/journal.xml`

```diff
@@ -7,30 +7,38 @@
     <record model="ir.ui.view" id="journal_view_form">
       <field name="model">account.journal</field>
       <field name="type">form</field>
       <field name="name">journal_form</field>
     </record>
     <record model="ir.ui.view" id="journal_view_tree">
       <field name="model">account.journal</field>
+      <field name="priority" eval="10"/>
       <field name="type">tree</field>
       <field name="name">journal_tree</field>
     </record>
+    <record model="ir.ui.view" id="journal_view_list_matching_sequence">
+      <field name="model">account.journal</field>
+      <field name="priority" eval="20"/>
+      <field name="type">tree</field>
+      <field name="name">journal_list_matching_sequence</field>
+    </record>
     <record model="ir.ui.view" id="journal_view_list_cash">
       <field name="model">account.journal</field>
       <field name="priority" eval="20"/>
       <field name="type">tree</field>
       <field name="name">journal_list_cash</field>
     </record>
     <record model="ir.action.act_window" id="act_journal_form">
       <field name="name">Journals</field>
       <field name="res_model">account.journal</field>
+      <field name="order" eval="[('matching_sequence', 'ASC'), ('id', 'ASC')]" pyson="1"/>
     </record>
     <record model="ir.action.act_window.view" id="act_journal_form_view1">
       <field name="sequence" eval="10"/>
-      <field name="view" ref="journal_view_tree"/>
+      <field name="view" ref="journal_view_list_matching_sequence"/>
       <field name="act_window" ref="act_journal_form"/>
     </record>
     <record model="ir.action.act_window.view" id="act_journal_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="journal_view_form"/>
       <field name="act_window" ref="act_journal_form"/>
     </record>
@@ -49,22 +57,22 @@
     <record model="ir.action.act_window.view" id="act_journal_open_cash_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="journal_view_list_cash"/>
       <field name="act_window" ref="act_journal_open_cash"/>
     </record>
     <menuitem parent="menu_reporting" action="act_journal_open_cash" sequence="50" id="menu_journal_open_cash"/>
     <record model="ir.model.access" id="access_journal">
-      <field name="model" search="[('model', '=', 'account.journal')]"/>
+      <field name="model">account.journal</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_journal_account_admin">
-      <field name="model" search="[('model', '=', 'account.journal')]"/>
+      <field name="model">account.journal</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.sequence.type" id="sequence_type_account_journal">
@@ -129,47 +137,54 @@
     <record model="ir.action.act_window.view" id="act_journal_period_form_close_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="journal_period_view_list_close"/>
       <field name="act_window" ref="act_journal_period_form_close"/>
     </record>
     <menuitem parent="menu_processing" action="act_journal_period_form_close" sequence="20" id="menu_close_journal_period"/>
     <record model="ir.model.access" id="access_journal_period">
-      <field name="model" search="[('model', '=', 'account.journal.period')]"/>
+      <field name="model">account.journal.period</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_journal_period_account">
-      <field name="model" search="[('model', '=', 'account.journal.period')]"/>
+      <field name="model">account.journal.period</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_journal_period_account_admin">
-      <field name="model" search="[('model', '=', 'account.journal.period')]"/>
+      <field name="model">account.journal.period</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
-    <record model="ir.model.button" id="journal_period_open_button">
-      <field name="name">open</field>
-      <field name="model" search="[('model', '=', 'account.journal.period')]"/>
+    <record model="ir.rule.group" id="rule_group_journal_period_companies">
+      <field name="name">User in companies</field>
+      <field name="model">account.journal.period</field>
+      <field name="global_p" eval="True"/>
+    </record>
+    <record model="ir.rule" id="rule_journal_period_companies">
+      <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
+      <field name="rule_group" ref="rule_group_journal_period_companies"/>
     </record>
     <record model="ir.model.button" id="journal_period_close_button">
+      <field name="model">account.journal.period</field>
       <field name="name">close</field>
-      <field name="model" search="[('model', '=', 'account.journal.period')]"/>
+      <field name="string">Close</field>
     </record>
     <record model="ir.model.button" id="journal_period_reopen_button">
+      <field name="model">account.journal.period</field>
       <field name="name">reopen</field>
-      <field name="model" search="[('model', '=', 'account.journal.period')]"/>
+      <field name="string">Reopen</field>
     </record>
   </data>
   <data noupdate="1">
     <record model="account.journal" id="journal_revenue">
       <field name="name">Revenue</field>
       <field name="code">REV</field>
       <field name="type">revenue</field>
```

### Comparing `trytond_account-7.0.6/locale/bg.po` & `trytond_account-7.2.0/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -2660,22 +2660,18 @@
 #, fuzzy
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Всички движение по тази сметка\n"
 "задължително да имат втора валута"
 
-#, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Данък по подразбиране за ръчно кодиране на редове за движение\n"
-"за видове дневници: \"разход\" и \"приход\""
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr ""
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3792,19 +3788,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3901,14 +3892,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/ca.po` & `trytond_account-7.2.0/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -2331,19 +2331,16 @@
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Força a tots els assentaments d'aquest compte a tenir aquesta moneda "
 "secundària."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Impost per defecte per a l'entrada manual\n"
-"d'apunts per diaris de tipus: \"despesa\" i \"ingressos\"."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Marca per sobreescriure la definició de la plantilla"
 
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
@@ -3400,21 +3397,14 @@
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 "No es pot modificar o eliminar el diari-període \"%(journal_period)s\" "
 "perquè conté assentaments."
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-"No es pot modificar o eliminar el període \"%(period)s\" perquè conté "
-"assentaments."
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 "No podeu afegir/modificar/eliminar apunts al diari-període tancat "
 "\"%(journal_period)s\"."
@@ -3539,14 +3529,23 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "Les dates del període \"%(period)s\" ha d'estar dins de les dates del seu "
 "exercici fiscal \"%(fiscalyear)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+"Les dates del període \"%(period)s\" ha d'estar dins de les dates del seu "
+"exercici fiscal \"%(fiscalyear)s\"."
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "El períodes \"%(first)s\" i \"%(second)s\" es sobreposen, heu d'utilitzar "
 "dates diferents."
```

### Comparing `trytond_account-7.0.6/locale/cs.po` & `trytond_account-7.2.0/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -2479,16 +2479,15 @@
 
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr ""
 
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3566,19 +3565,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3675,14 +3669,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/de.po` & `trytond_account-7.2.0/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -2329,19 +2329,16 @@
 
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr "Für alle Buchungen auf dieses Konto diese Fremdwährung verwenden."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Standardsteuer für manuell erstellte Buchungszeilen\n"
-"in Journalen vom Typ \"Aufwand\" und \"Ertrag\"."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Aktivieren um die Vorlage zu überschreiben"
 
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
@@ -3433,21 +3430,14 @@
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 "Journal - Buchungszeitraum \"%(journal_period)s\" kann nicht geändert oder "
 "gelöscht werden, da Buchungen enthalten sind."
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-"Buchungszeitraum \"%(period)s\" kann nicht geändert oder gelöscht werden, da"
-" er Buchungssätze enthält."
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 "Sie können keine Buchungszeilen hinzufügen/ändern/löschen, die zum "
 "geschlossenen Journal - Buchungszeitraum \"%(journal_period)s\" gehören."
@@ -3579,14 +3569,23 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "Die Daten für den Buchungszeitraum \"%(period)s\" müssen zwischen den Daten "
 "des zugehörigen Geschäftsjahres \"%(fiscalyear)s\" liegen."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+"Die Daten für den Buchungszeitraum \"%(period)s\" müssen zwischen den Daten "
+"des zugehörigen Geschäftsjahres \"%(fiscalyear)s\" liegen."
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "Die Buchungszeiträume \"%(first)s\" und \"%(second)s\" dürfen sich zeitlich "
 "nicht überschneiden."
```

### Comparing `trytond_account-7.0.6/locale/es.po` & `trytond_account-7.2.0/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -2328,19 +2328,16 @@
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Fuerza todos los asientos de esta cuenta a tener esta moneda secundaria."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Impuesto por defecto para la introducción manual\n"
-"de apuntes para diarios de tipo: \"gastos\" e \"ingresos\"."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Marcar para sobrescribir la definición de la plantilla"
 
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
@@ -3399,21 +3396,14 @@
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 "No puede modificar o eliminar el diario periodo \"%(journal_period)s\" "
 "porque contiene asientos."
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-"No puede modificar o eliminar el periodo \"%(period)s\" porque contiene "
-"asientos."
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 "No puede crear/modificar/eliminar apuntes en el diario periodo cerrado "
 "\"%(journal_period)s\"."
@@ -3542,14 +3532,23 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "Las fechas del periodo \"%(period)s\" deben estar dentro de las fechas de su"
 " ejercicio fiscal \"%(fiscalyear)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+"Las fechas del periodo \"%(period)s\" deben estar dentro de las fechas de su"
+" ejercicio fiscal \"%(fiscalyear)s\"."
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "Los periodos \"%(first)s\" y \"%(second)s\" se superponen, debe usar fechas "
 "diferentes."
```

### Comparing `trytond_account-7.0.6/locale/es_419.po` & `trytond_account-7.2.0/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -2505,22 +2505,18 @@
 msgstr "Permite conciliar las líneas de asiento de esta cuenta."
 
 #, fuzzy
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr "Permite conciliar las líneas de asiento de esta cuenta."
 
-#, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Impuesto por defecto para la codificación manual\n"
-"de líneas de asientos para libros diarios de tipo: \"gastos\" e \"ingresos\"."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr ""
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3609,19 +3605,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3727,14 +3718,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/et.po` & `trytond_account-7.2.0/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -2463,22 +2463,18 @@
 #, fuzzy
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Sunni kõigile selle konto kannetele \n"
 "see sekundaarne valuuta."
 
-#, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Vaikimisi maks käsikodeerimiseks kande ridadel \n"
-"registri tüüpidele: \"kulu\" ja \"müügitulu\"."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Märgi et kirjutada üle vormi definitsioon."
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3585,20 +3581,14 @@
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 "Ei saa muuta vi kustutada andmiku-perioodi \"%(andmiku-periood)e\" kuna "
 "selles on kandeid"
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-"Ei saa muuta või kustutada perioodi \"%(periood)e\" kuna sellel on kandeid."
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 "Ei saa lisada/muuta/kustutada ridu suletud andmiku-perioodis \"%(andmiku-"
 "periood)ides\""
@@ -3714,14 +3704,23 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "Perioodi \"%(perioodide) kuupäevad peavad olema majandusaasta "
 "\"%(majandusaastate)\" kuupäevade vahemikus"
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+"Perioodi \"%(perioodide) kuupäevad peavad olema majandusaasta "
+"\"%(majandusaastate)\" kuupäevade vahemikus"
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr "Majandusaasta \"%(esmane)\" ja \"%(teisene)\" kattub, kausta teisi kuupäevi."
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/fa.po` & `trytond_account-7.2.0/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -2481,22 +2481,18 @@
 #, fuzzy
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "مجموع تمام جابجایی های این حساب\n"
 " برای داشتن ارز ثانویه."
 
-#, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"مالیات پیش فرض برای رمزگذاری دستی سطرهای جابجایی \n"
-"برای انواع روزنامه : \"هزینه\" و \"درآمد\""
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "علامت گذاری برای بازنویسی تعاریف الگو"
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3607,21 +3603,14 @@
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 "شما نمیتوانید روزنامه-دوره : \"%(journal_period)s\" را اصلاح یا حذف کنید، "
 "زیرا دارای جابجایی ها میباشد."
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-"شما نمیتوانید دوره : \"%(period)s\" را اصلاح یا حذف کنید، زیرا دارای جابجایی"
-" ها میباشد."
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 "شما نمیتوانید سطرهایی را در روزنامه-دوره بسته شده :\"%(journal_period)s\"، "
 "اضافه / اصلاح/ حذف کنید."
@@ -3744,14 +3733,23 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "تاریخ های دوره : \"%(period)s\" باید مابین تاریخ های این سال مای : "
 "\"%(fiscalyear)s\" باشد."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+"تاریخ های دوره : \"%(period)s\" باید مابین تاریخ های این سال مای : "
+"\"%(fiscalyear)s\" باشد."
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "دوره های : \"%(اولیه)s\" و \"%(ثانویه)s\" دارای همپوشانی هستند، شما باید از "
 "تاریخ های متفاوت استفاده کنید."
```

### Comparing `trytond_account-7.0.6/locale/fi.po` & `trytond_account-7.2.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -2671,16 +2671,15 @@
 
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr ""
 
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3761,19 +3760,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3870,14 +3864,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/fr.po` & `trytond_account-7.2.0/locale/fr.po`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
 
 msgctxt "field:account.account.type,revenue:"
 msgid "Revenue"
 msgstr "Produit"
 
 msgctxt "field:account.account.type,statement:"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Rapport"
 
 msgctxt "field:account.account.type,stock:"
 msgid "Stock"
 msgstr "Stock"
 
 msgctxt "field:account.account.type,template:"
 msgid "Template"
@@ -436,15 +436,15 @@
 
 msgctxt "field:account.account.type.template,revenue:"
 msgid "Revenue"
 msgstr "Produit"
 
 msgctxt "field:account.account.type.template,statement:"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Rapport"
 
 msgctxt "field:account.account.type.template,stock:"
 msgid "Stock"
 msgstr "Stock"
 
 msgctxt "field:account.aged_balance,balance:"
 msgid "Balance"
@@ -2326,19 +2326,18 @@
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Force tous les mouvements pour ce compte à avoir cette devise secondaire."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Taxe par défaut pour les lignes de mouvement manuelles\n"
-"pour le type de journal : « charge » et « produit »."
+"Les taxes par défaut à appliquer pour les documents lorsqu'il n'y a pas "
+"d'autre source."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Cochez pour remplacer la définition du modèle"
 
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
@@ -3137,15 +3136,15 @@
 
 msgctxt "model:ir.action,name:act_unreconcile_lines"
 msgid "Unreconcile Lines"
 msgstr "Dé-réconcilier les lignes"
 
 msgctxt "model:ir.action,name:report_account_type_statement"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Rapport"
 
 msgctxt "model:ir.action,name:report_aged_balance"
 msgid "Aged Balance"
 msgstr "Balance âgée"
 
 msgctxt "model:ir.action,name:report_general_journal"
 msgid "General Journal"
@@ -3417,21 +3416,14 @@
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 "Vous ne pouvez pas modifier ou supprimer la relation journal - période "
 "« %(journal_period)s » parce qu'elle contient des mouvements."
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-"Vous ne pouvez pas modifier ou supprimer la période « %(period)s » car elle "
-"contient des mouvements."
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 "Vous ne pouvez pas ajouter/modifier/supprimer des lignes sur la relation "
 "journal - période clôturée « %(journal_period)s »."
@@ -3561,14 +3553,22 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "Les dates de la période « %(period)s » doivent être entre les dates de son "
 "année fiscale « %(fiscalyear)s »."
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+"Les dates de la période « %(period)s » doivent inclure la date "
+"« %(move_date)s » du mouvement « %(move)s »."
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "Les périodes « %(first)s » et « %(second)s » se chevauchent, vous devez "
 "utiliser des dates différentes."
@@ -4111,15 +4111,15 @@
 
 msgctxt "report:account.account.type.statement:"
 msgid "Print Date:"
 msgstr "Date d'impression :"
 
 msgctxt "report:account.account.type.statement:"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Rapport"
 
 msgctxt "report:account.account.type.statement:"
 msgid "To"
 msgstr "à"
 
 msgctxt "report:account.account.type.statement:"
 msgid "User:"
```

### Comparing `trytond_account-7.0.6/locale/hu.po` & `trytond_account-7.2.0/locale/hu.po`

 * *Files 0% similar despite different names*

```diff
@@ -2414,19 +2414,16 @@
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Engedélyezi, hogy a számlára könyvelt tételeket le lehessen egyeztetni."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Az alapértelmezett adót akkor használja, ha kézzel könyvel a „költségek” "
-"vagy „bevételek” típusú naplókra."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "A sablonból származó adatok felülírásához jelölje be"
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3497,19 +3494,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3615,14 +3607,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/id.po` & `trytond_account-7.2.0/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -2372,16 +2372,15 @@
 
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr ""
 
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3436,19 +3435,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3553,14 +3547,21 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr "Untuk menutup tahun fiskal, saldo akun \"%(account)s\" harus nol."
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/it.po` & `trytond_account-7.2.0/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -2533,19 +2533,16 @@
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Forza tutti i movimenti di questo conto \n"
 "ad avere questa seconda valuta."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Imposte predefinite per completamento manuale di movimenti contabili \n"
-"per il tipo di libro giornale: \"spese\" and \"ricavi\"."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr ""
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3653,19 +3650,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3766,14 +3758,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/lo.po` & `trytond_account-7.2.0/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -2543,20 +2543,18 @@
 "ໃຫ້ສາມາດທຽບຍອດໄດ້."
 
 #, fuzzy
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr "ບັງຄັບການເຄື່ອນໄຫວທັງໝົດສໍາລັບບັນຊີນີ້ ໃຫ້ມີສະກຸນເງິນທີສອງ."
 
-#, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
-msgstr "ພາສີສຳລັບປ້ອນດ້ວຍມື ສຳລັບລາຍການປະເພດບັນຊີປະຈຳວັນ: \"ລາຍຈ່າຍ\" ແລະ \"ລາຍຮັບ\""
+"Default taxes for documents to be applied when there is no other source."
+msgstr ""
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr ""
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3683,19 +3681,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3799,14 +3792,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/lt.po` & `trytond_account-7.2.0/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -2456,19 +2456,16 @@
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Visoms operacijoms šioje koresponduojančioje \n"
 "sąskaitoje priskirti šią papildomą valiutą."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Numatytieji mokesčiai, kuriant operacijų eilutes \n"
-"\"išlaidų\" ir \"pajamų\" tipo žurnalams rankiniu būdu."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Pažymėkite, kad perrašyti duomenis iš šablono"
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3563,21 +3560,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-"Negalima keisti ar pašalinti periodą \"%(period)s\", nes jo metu jau "
-"atliktos operacijos."
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 "Negalima sukurti, keisti ar ištrinti eilučių, kai žurnalo periodas "
 "\"%(journal_period)s\" yra uždarytas."
@@ -3700,14 +3690,23 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "Periodo \"%(period)s\" datos turi priklausyti finansiniams metams "
 "\"%(fiscalyear)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+"Periodo \"%(period)s\" datos turi priklausyti finansiniams metams "
+"\"%(fiscalyear)s\"."
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "Periodai \"%(first)s\" ir \"%(second)s\" persidengia, reikia nurodyti kitas "
 "datas."
```

### Comparing `trytond_account-7.0.6/locale/nl.po` & `trytond_account-7.2.0/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -2327,19 +2327,16 @@
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Forceer alle boekingen voor deze grootboekrekening om deze secundaire valuta"
 " te gebruiken."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Standaard belasting voor handmatig coderen van boekingen\n"
-"voor de dagboeksoorten: \"kosten\" en \"opbrengsten\"."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Vink aan om de template te overschrijven"
 
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
@@ -3409,21 +3406,14 @@
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 "U kunt de journaalperiode \"% (journal_period) s\" niet wijzigen of "
 "verwijderen omdat deze boekingen bevat."
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-"U kunt periode \"% (period)s\" niet wijzigen of verwijderen omdat deze "
-"boekingen bevat."
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 "U kunt geen regels toevoegen / wijzigen / verwijderen in de gesloten dagboek"
 " periode \"%(journal_period)s\"."
@@ -3552,14 +3542,22 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "De datums voor periode \"%(period)s\" moeten binnen het gerelateerde "
 "boekjaar \"%(fiscalyear)s\" vallen."
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+"De datums voor periode \"%(period)s\" moeten de datum \"%(move_date)s\" van "
+"boeking \"%(move)s\" bevatten ."
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "De periodes \"%(first)s\" en \"%(second)s\" overlappen elkaar, gebruikt "
 "verschillende datums."
```

### Comparing `trytond_account-7.0.6/locale/pl.po` & `trytond_account-7.2.0/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -2521,16 +2521,15 @@
 #, fuzzy
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr "Pozwala uzgadniać zapisy księgowe dla tego konta."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr ""
 
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3657,19 +3656,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3775,14 +3769,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/pt.po` & `trytond_account-7.2.0/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -2507,22 +2507,18 @@
 #, fuzzy
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Forçar os lançamentos dessa conta\n"
 "a ter essa moeda secundária"
 
-#, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Tributo padrão para codificação manual da linha de lançamento \n"
-"para os tipos de diário: \"despesa\" e \"receita\""
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Marcar para sobrescrever definições de modelo"
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3655,19 +3651,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3773,14 +3764,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/ro.po` & `trytond_account-7.2.0/locale/ro.po`

 * *Files 4% similar despite different names*

```diff
@@ -35,18 +35,17 @@
 msgid "Context Company"
 msgstr "Companie"
 
 msgctxt "field:account.account,credit:"
 msgid "Credit"
 msgstr "Credit"
 
-#, fuzzy
 msgctxt "field:account.account,credit_type:"
 msgid "Credit Type"
-msgstr "Tip de Debit"
+msgstr "Tip de Credit"
 
 msgctxt "field:account.account,currency:"
 msgid "Currency"
 msgstr "Valută"
 
 msgctxt "field:account.account,debit:"
 msgid "Debit"
@@ -72,17 +71,18 @@
 msgid "General Ledger Balance"
 msgstr "Sold registru general contabil"
 
 msgctxt "field:account.account,left:"
 msgid "Left"
 msgstr "Rămas"
 
+#, fuzzy
 msgctxt "field:account.account,line_count:"
 msgid "Line Count"
-msgstr ""
+msgstr "Număr Rânduri"
 
 msgctxt "field:account.account,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:account.account,note:"
 msgid "Note"
@@ -90,15 +90,15 @@
 
 msgctxt "field:account.account,parent:"
 msgid "Parent"
 msgstr "Parinte"
 
 msgctxt "field:account.account,party_required:"
 msgid "Party Required"
-msgstr "Parte obligatorie"
+msgstr "Parte Obligatorie"
 
 msgctxt "field:account.account,reconcile:"
 msgid "Reconcile"
 msgstr "Reconciliere"
 
 msgctxt "field:account.account,replaced_by:"
 msgid "Replaced By"
@@ -107,15 +107,15 @@
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Dreapta"
 
 #, fuzzy
 msgctxt "field:account.account,second_currency:"
 msgid "Second Currency"
-msgstr "Valută Secundara"
+msgstr "Valută Secundară"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Data Inițierii"
 
 msgctxt "field:account.account,taxes:"
 msgid "Default Taxes"
@@ -154,14 +154,15 @@
 msgid "Posted Moves"
 msgstr "Mișcari Postate"
 
 msgctxt "field:account.account.deferral,account:"
 msgid "Account"
 msgstr "Cont"
 
+#, fuzzy
 msgctxt "field:account.account.deferral,amount_second_currency:"
 msgid "Amount Second Currency"
 msgstr "Suma Valută Secundara"
 
 msgctxt "field:account.account.deferral,balance:"
 msgid "Balance"
 msgstr "Sold"
@@ -178,30 +179,32 @@
 msgid "Debit"
 msgstr "Debit"
 
 msgctxt "field:account.account.deferral,fiscalyear:"
 msgid "Fiscal Year"
 msgstr "An Fiscal"
 
+#, fuzzy
 msgctxt "field:account.account.deferral,line_count:"
 msgid "Line Count"
-msgstr ""
+msgstr "Număr Rânduri"
 
 msgctxt "field:account.account.deferral,second_currency:"
 msgid "Second Currency"
 msgstr "Valută Secundara"
 
 msgctxt "field:account.account.party,account:"
 msgid "Account"
 msgstr "Cont"
 
 msgctxt "field:account.account.party,active:"
 msgid "Active"
 msgstr "Activ"
 
+#, fuzzy
 msgctxt "field:account.account.party,amount_second_currency:"
 msgid "Amount Second Currency"
 msgstr "Suma Valută Secundara"
 
 msgctxt "field:account.account.party,balance:"
 msgid "Balance"
 msgstr "Sold"
@@ -218,18 +221,17 @@
 msgid "Company"
 msgstr "Companie"
 
 msgctxt "field:account.account.party,credit:"
 msgid "Credit"
 msgstr "Credit"
 
-#, fuzzy
 msgctxt "field:account.account.party,credit_type:"
 msgid "Credit Type"
-msgstr "Tip de Debit"
+msgstr "Tip de Credit"
 
 msgctxt "field:account.account.party,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.account.party,debit:"
 msgid "Debit"
@@ -239,17 +241,18 @@
 msgid "Debit Type"
 msgstr "Tip de Debit"
 
 msgctxt "field:account.account.party,end_date:"
 msgid "End Date"
 msgstr "Data de încheiere"
 
+#, fuzzy
 msgctxt "field:account.account.party,line_count:"
 msgid "Line Count"
-msgstr ""
+msgstr "Număr Rânduri"
 
 msgctxt "field:account.account.party,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:account.account.party,party:"
 msgid "Party"
@@ -275,18 +278,17 @@
 msgid "Closed"
 msgstr "Închis"
 
 msgctxt "field:account.account.template,code:"
 msgid "Code"
 msgstr "Cod"
 
-#, fuzzy
 msgctxt "field:account.account.template,credit_type:"
 msgid "Credit Type"
-msgstr "Tip de Debit"
+msgstr "Tip de Credit"
 
 msgctxt "field:account.account.template,debit_type:"
 msgid "Debit Type"
 msgstr "Tip de Debit"
 
 msgctxt "field:account.account.template,deferral:"
 msgid "Deferral"
@@ -549,23 +551,25 @@
 msgctxt "field:account.balance_sheet.context,posted:"
 msgid "Posted Moves"
 msgstr "Mișcari Postate"
 
 #, fuzzy
 msgctxt "field:account.configuration,currency_exchange_credit_account:"
 msgid "Currency Exchange Credit Account"
-msgstr "Cont Credit"
+msgstr "Cont de Credit de Schimb Valutar"
 
+#, fuzzy
 msgctxt "field:account.configuration,currency_exchange_debit_account:"
 msgid "Currency Exchange Debit Account"
-msgstr ""
+msgstr "Cont de Debit de Schimb Valutar"
 
+#, fuzzy
 msgctxt "field:account.configuration,currency_exchange_journal:"
 msgid "Currency Exchange Journal"
-msgstr ""
+msgstr "Jurnal de Schimb Valutar"
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Cont Implicit Furnizor"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -591,20 +595,21 @@
 msgid "Company"
 msgstr "Companie"
 
 #, fuzzy
 msgctxt ""
 "field:account.configuration.default_account,currency_exchange_credit_account:"
 msgid "Currency Exchange Credit Account"
-msgstr "Cont Credit"
+msgstr "Cont de Credit de Schimb Valutar"
 
+#, fuzzy
 msgctxt ""
 "field:account.configuration.default_account,currency_exchange_debit_account:"
 msgid "Currency Exchange Debit Account"
-msgstr ""
+msgstr "Cont de Debit de Schimb Valutar"
 
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Cont Implicit Furnizor"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
@@ -621,22 +626,22 @@
 msgstr "Regula Implicita de Impozitare al Clientului"
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Regula Implicita de Impozitare al Furnizorului"
 
-#, fuzzy
 msgctxt "field:account.configuration.journal,company:"
 msgid "Company"
 msgstr "Companie"
 
+#, fuzzy
 msgctxt "field:account.configuration.journal,currency_exchange_journal:"
 msgid "Currency Exchange Journal"
-msgstr ""
+msgstr "Jurnal Schimb Valutar"
 
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Companie"
 
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -781,15 +786,15 @@
 msgctxt "field:account.general_ledger.account,credit:"
 msgid "Credit"
 msgstr "Credit"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account,credit_type:"
 msgid "Credit Type"
-msgstr "Tip de Debit"
+msgstr "Tip de Credit"
 
 msgctxt "field:account.general_ledger.account,currency:"
 msgid "Currency"
 msgstr "Valută"
 
 msgctxt "field:account.general_ledger.account,debit:"
 msgid "Debit"
@@ -815,17 +820,18 @@
 msgid "End Debit"
 msgstr "Sfarsit Debit"
 
 msgctxt "field:account.general_ledger.account,general_ledger_balance:"
 msgid "General Ledger Balance"
 msgstr "Sold registru general contabil"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account,line_count:"
 msgid "Line Count"
-msgstr ""
+msgstr "Număr Rânduri"
 
 msgctxt "field:account.general_ledger.account,lines:"
 msgid "Lines"
 msgstr "Rânduri"
 
 msgctxt "field:account.general_ledger.account,start_balance:"
 msgid "Start Balance"
@@ -916,17 +922,18 @@
 msgid "End Date"
 msgstr "Data de încheiere"
 
 msgctxt "field:account.general_ledger.account.party,end_debit:"
 msgid "End Debit"
 msgstr "Sfarsit Debit"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.party,line_count:"
 msgid "Line Count"
-msgstr ""
+msgstr "Număr Rânduri"
 
 msgctxt "field:account.general_ledger.account.party,party:"
 msgid "Party"
 msgstr "Parte"
 
 msgctxt "field:account.general_ledger.account.party,start_balance:"
 msgid "Start Balance"
@@ -1202,15 +1209,14 @@
 msgid "Effective Date"
 msgstr "Data Efectiva"
 
 msgctxt "field:account.move,description:"
 msgid "Description"
 msgstr "Descriere"
 
-#, fuzzy
 msgctxt "field:account.move,description_used:"
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "field:account.move,journal:"
 msgid "Journal"
 msgstr "Jurnal"
@@ -1243,18 +1249,17 @@
 msgid "State"
 msgstr "Stare"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Descriere"
 
-#, fuzzy
 msgctxt "field:account.move.cancel.default,reversal:"
 msgid "Reversal"
-msgstr "fiecare"
+msgstr "Inversare"
 
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Cont"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
@@ -1287,21 +1292,20 @@
 msgctxt "field:account.move.line,debit:"
 msgid "Debit"
 msgstr "Debit"
 
 #, fuzzy
 msgctxt "field:account.move.line,delegated_amount:"
 msgid "Delegated Amount"
-msgstr "Delegat la"
+msgstr "Suma Delegata"
 
 msgctxt "field:account.move.line,description:"
 msgid "Description"
 msgstr "Descriere"
 
-#, fuzzy
 msgctxt "field:account.move.line,description_used:"
 msgid "Description"
 msgstr "Descriere"
 
 #, fuzzy
 msgctxt "field:account.move.line,has_maturity_date:"
 msgid "Has Maturity Date"
@@ -1340,18 +1344,17 @@
 msgid "Party"
 msgstr "Parte"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Parte obligatorie"
 
-#, fuzzy
 msgctxt "field:account.move.line,payable_receivable_balance:"
 msgid "Payable/Receivable Balance"
-msgstr "Rânduri Client/Furnizor"
+msgstr "Sold Furnizor/Client"
 
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Perioadă"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
@@ -1381,41 +1384,37 @@
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "field:account.move.line.delegate.start,journal:"
 msgid "Journal"
 msgstr "Jurnal"
 
-#, fuzzy
 msgctxt "field:account.move.line.delegate.start,party:"
 msgid "Party"
 msgstr "Parte"
 
 msgctxt "field:account.move.line.group.start,description:"
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Jurnal"
 
-#, fuzzy
 msgctxt "field:account.move.line.receivable_payable.context,payable:"
 msgid "Payable"
 msgstr "Furnizor"
 
-#, fuzzy
 msgctxt "field:account.move.line.receivable_payable.context,receivable:"
 msgid "Receivable"
 msgstr "Client"
 
-#, fuzzy
 msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
 msgid "Reconciled"
-msgstr "Reconciliere"
+msgstr "Reconciliat"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Valută"
 
 msgctxt "field:account.move.line.reschedule.preview,description:"
@@ -1427,20 +1426,18 @@
 msgstr "Jurnal"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,terms:"
 msgid "Terms"
 msgstr "Termene"
 
-#, fuzzy
 msgctxt "field:account.move.line.reschedule.start,amount:"
 msgid "Amount"
 msgstr "Suma"
 
-#, fuzzy
 msgctxt "field:account.move.line.reschedule.start,currency:"
 msgid "Currency"
 msgstr "Valută"
 
 msgctxt "field:account.move.line.reschedule.start,frequency:"
 msgid "Frequency"
 msgstr "Frecvență"
@@ -1454,25 +1451,22 @@
 msgstr "Număr"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.start,start_date:"
 msgid "Start Date"
 msgstr "Data Inițierii"
 
-#, fuzzy
 msgctxt "field:account.move.line.reschedule.start,total_amount:"
 msgid "Total Amount"
-msgstr "Suma"
+msgstr "Suma Totala"
 
-#, fuzzy
 msgctxt "field:account.move.line.reschedule.term,amount:"
 msgid "Amount"
 msgstr "Suma"
 
-#, fuzzy
 msgctxt "field:account.move.line.reschedule.term,currency:"
 msgid "Currency"
 msgstr "Valută"
 
 msgctxt "field:account.move.line.reschedule.term,date:"
 msgid "Date"
 msgstr "Data"
@@ -1573,15 +1567,14 @@
 msgid "Delegate To"
 msgstr "Delegat la"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Rânduri"
 
-#, fuzzy
 msgctxt "field:account.move.reconciliation,number:"
 msgid "Number"
 msgstr "Număr"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Companie"
@@ -1602,15 +1595,14 @@
 msgid "Lines"
 msgstr "Rânduri"
 
 msgctxt "field:account.move.template,name:"
 msgid "Name"
 msgstr "Denumire"
 
-#, fuzzy
 msgctxt "field:account.move.template.create.template,date:"
 msgid "Effective Date"
 msgstr "Data Efectiva"
 
 msgctxt "field:account.move.template.create.template,period:"
 msgid "Period"
 msgstr "Perioadă"
@@ -1687,18 +1679,17 @@
 msgid "Account"
 msgstr "Cont"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Companie"
 
-#, fuzzy
 msgctxt "field:account.reconcile.show,currencies:"
 msgid "Currencies"
-msgstr "Valută"
+msgstr "Valute"
 
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
@@ -1910,15 +1901,15 @@
 msgctxt "field:account.tax.code.context,periods:"
 msgid "Periods"
 msgstr "Perioade"
 
 #, fuzzy
 msgctxt "field:account.tax.code.context,start_period:"
 msgid "Start Period"
-msgstr "Perioada inceput"
+msgstr "Inceput Perioada"
 
 msgctxt "field:account.tax.code.line,amount:"
 msgid "Amount"
 msgstr "Suma"
 
 msgctxt "field:account.tax.code.line,code:"
 msgid "Code"
@@ -2264,28 +2255,26 @@
 msgid "Tax"
 msgstr "Impozit"
 
 msgctxt "field:account.update_chart.start,account:"
 msgid "Root Account"
 msgstr "Cont Radacină"
 
-#, fuzzy
 msgctxt "field:company.company,payable:"
 msgid "Payable"
 msgstr "Furnizor"
 
-#, fuzzy
 msgctxt "field:company.company,payable_today:"
 msgid "Payable Today"
-msgstr "Scadent Astazi"
+msgstr "Scadent Astăzi"
 
 #, fuzzy
 msgctxt "field:company.company,receivable:"
 msgid "Receivable"
-msgstr "Client"
+msgstr "De Incasat"
 
 #, fuzzy
 msgctxt "field:company.company,receivable_today:"
 msgid "Receivable Today"
 msgstr "Scadent Astazi"
 
 msgctxt "field:party.party,account_payable:"
@@ -2306,19 +2295,19 @@
 
 msgctxt "field:party.party,customer_tax_rule:"
 msgid "Customer Tax Rule"
 msgstr "Regula de Impozitare al Clientului"
 
 msgctxt "field:party.party,payable:"
 msgid "Payable"
-msgstr "Platibil"
+msgstr "Furnizor"
 
 msgctxt "field:party.party,payable_today:"
 msgid "Payable Today"
-msgstr "Scadent Astazi"
+msgstr "Scadent Astăzi"
 
 msgctxt "field:party.party,receivable:"
 msgid "Receivable"
 msgstr "Client"
 
 msgctxt "field:party.party,receivable_today:"
 msgid "Receivable Today"
@@ -2352,54 +2341,47 @@
 msgid "Supplier Tax Rule"
 msgstr "Regula de Impozitare Furnizor"
 
 msgctxt "help:account.account,closed:"
 msgid "Check to prevent posting move on the account."
 msgstr "Bifați pentru a nu permite o mișcare pe contul."
 
-#, fuzzy
 msgctxt "help:account.account,credit_type:"
 msgid "The type used if not empty and debit < credit."
-msgstr "Tipul folosit dacă nu este gol şi debit > credit."
+msgstr "Tipul folosit dacă nu este gol şi debit < credit."
 
 msgctxt "help:account.account,debit_type:"
 msgid "The type used if not empty and debit > credit."
 msgstr "Tipul folosit dacă nu este gol şi debit > credit."
 
 msgctxt "help:account.account,general_ledger_balance:"
 msgid "Display only the balance in the general ledger report."
 msgstr "Afişare numai sold în registru general."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Permite reconciliere al randurilr al contului."
 
-#, fuzzy
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
-"Obligatoriu pentru toate mişcările pe acest cont\n"
-"să aiba o valută secundară."
+"Forțați toate mișcările pentru acest cont să aibă această a doua monedă."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Impozit prestabilit pentru codificare manuala al rândurilor cu mişcari\n"
-"pentru jurnale de tip: \"cheltuiala\" şi \"venit\"."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Bifaţi pentru a modifica fără să ţine cont de şablon"
 
-#, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
-msgstr "Lăsaţi gol pentru toţi anii fiscali deschişi."
+msgstr "Lăsaţi gol pentru tot anul fiscal deschis."
 
 #, fuzzy
 msgctxt "help:account.account.context,posted:"
 msgid "Only include posted moves."
 msgstr "Include numai mişcări postate."
 
 msgctxt "help:account.account.template,closed:"
@@ -2489,69 +2471,68 @@
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Cunoscut şi că Numărul Folio."
 
 msgctxt "help:account.move.cancel.default,reversal:"
 msgid "Reverse debit and credit."
-msgstr ""
+msgstr "Inverseaza debit si credit."
 
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "Sumă exprimata în valută secundară."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
-msgstr ""
+msgstr "Setați o dată pentru ca linia să fie plătibilă sau de încasat."
 
 msgctxt "help:account.move.line,second_currency:"
 msgid "The second currency."
 msgstr "Valută secundara."
 
 msgctxt "help:account.move.line.reschedule.start,interval:"
 msgid "The length of each period, in months."
 msgstr "Lungimea fiecărei perioade, în luni."
 
 msgctxt "help:account.move.line.template,amount:"
 msgid "A python expression that will be evaluated with the keywords."
 msgstr "O expresie python care va fi evaluata cu cuvintele cheie."
 
-#, fuzzy
 msgctxt "help:account.move.line.template,description:"
 msgid "Keyword value substitutions are identified by braces ('{' and '}')."
 msgstr ""
-"Substituţii de valorii al cuvintelor cheie sunt identificaţi cu ('{' şi "
-"'}')."
+"Înlocuirile de valori ale cuvintelor cheie sunt identificate prin acolade "
+"('{' și '}')."
 
 msgctxt "help:account.move.line.template,party:"
 msgid "The name of the 'Party' keyword."
 msgstr "Denumirea al cuvântului cheie 'Parte'."
 
 msgctxt "help:account.move.reconciliation,date:"
 msgid "Highest date of the reconciled lines."
 msgstr "Data cea mai mare pe rândurile reconciliate."
 
 msgctxt "help:account.move.reconciliation,delegate_to:"
 msgid "The line to which the reconciliation status is delegated."
 msgstr "Linia către care este delegat statutul de reconciliere."
 
-#, fuzzy
 msgctxt "help:account.move.template,description:"
 msgid "Keyword value substitutions are identified by braces ('{' and '}')."
 msgstr ""
-"Substituţii de valorii al cuvintelor cheie sunt identificaţi cu ('{' şi "
-"'}')."
+"Înlocuirile de valori ale cuvintelor cheie sunt identificate prin acolade "
+"('{' și '}')."
 
 msgctxt "help:account.reconcile.start,automatic:"
 msgid "Automatically reconcile suggestions."
-msgstr ""
+msgstr "Reconciliați automat sugestiile."
 
+#, fuzzy
 msgctxt "help:account.reconcile.start,only_balanced:"
 msgid "Skip suggestion with write-off."
-msgstr ""
+msgstr "Omiteti sugestia cu prescriptie."
 
 msgctxt "help:account.tax,amount:"
 msgid "In company's currency."
 msgstr "În valuta companiei."
 
 msgctxt "help:account.tax,description:"
 msgid "The name that will be used in reports."
@@ -2626,18 +2607,17 @@
 msgid "Account"
 msgstr "Cont"
 
 msgctxt "model:account.account-account.tax,name:"
 msgid "Account - Tax"
 msgstr "Cont - Impozit"
 
-#, fuzzy
 msgctxt "model:account.account.context,name:"
 msgid "Account Context"
-msgstr "Mişcare Cont"
+msgstr "Context Cont"
 
 msgctxt "model:account.account.deferral,name:"
 msgid "Account Deferral"
 msgstr ""
 
 msgctxt "model:account.account.party,name:"
 msgid "Account Party"
@@ -2684,18 +2664,17 @@
 msgid "Account Configuration Default Account"
 msgstr "Configurare Implicita pentru Cont"
 
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Configurare Implicita pentru Reguli de Impozitare"
 
-#, fuzzy
 msgctxt "model:account.configuration.journal,name:"
 msgid "Account Configuration Journal"
-msgstr "Configurare"
+msgstr "Jurnal Configurare Cont"
 
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Secvență Configurare Cont"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
@@ -2757,18 +2736,17 @@
 msgid "Journal"
 msgstr "Jurnal"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Cash"
 
-#, fuzzy
 msgctxt "model:account.journal,name:journal_currency_exchange"
 msgid "Currency Exchange"
-msgstr "Valută"
+msgstr "Schimb Valutar"
 
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Cheltuiala"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
@@ -2802,42 +2780,37 @@
 msgid "Cancel Moves"
 msgstr "Anulare Mişcari"
 
 msgctxt "model:account.move.line,name:"
 msgid "Account Move Line"
 msgstr "Rând Mişcare Cont"
 
-#, fuzzy
 msgctxt "model:account.move.line.delegate.start,name:"
 msgid "Delegate Lines"
-msgstr "Delegat la"
+msgstr "Rânduri Delegate"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Grup de Rânduri"
 
-#, fuzzy
 msgctxt "model:account.move.line.receivable_payable.context,name:"
 msgid "Receivable/Payable Line Context"
-msgstr "Registru General Context Rând"
+msgstr "Context Rând de Client/Furnizor"
 
-#, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
-msgstr "Reconciliere Rânduri"
+msgstr "Reprogramare Rânduri"
 
-#, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
-msgstr "Reconciliere Rânduri"
+msgstr "Reprogramare Rânduri"
 
-#, fuzzy
 msgctxt "model:account.move.line.reschedule.term,name:"
 msgid "Reschedule Lines"
-msgstr "Reconciliere Rânduri"
+msgstr "Reprogramare Rânduri"
 
 msgctxt "model:account.move.line.template,name:"
 msgid "Account Move Line Template"
 msgstr "Mişcare Cont Şablon Rând"
 
 msgctxt "model:account.move.open_journal.ask,name:"
 msgid "Open Journal Ask"
@@ -2875,15 +2848,14 @@
 msgid "Period"
 msgstr "Perioadă"
 
 msgctxt "model:account.reconcile.show,name:"
 msgid "Reconcile"
 msgstr "Reconciliere"
 
-#, fuzzy
 msgctxt "model:account.reconcile.start,name:"
 msgid "Reconcile"
 msgstr "Reconciliere"
 
 msgctxt "model:account.tax,name:"
 msgid "Account Tax"
 msgstr "Cont Impozit"
@@ -2891,15 +2863,15 @@
 msgctxt "model:account.tax.code,name:"
 msgid "Tax Code"
 msgstr "Cod Fiscal"
 
 #, fuzzy
 msgctxt "model:account.tax.code.context,name:"
 msgid "Tax Code Context"
-msgstr "Rând Cod Fiscal"
+msgstr "Context Cod Fiscal"
 
 msgctxt "model:account.tax.code.line,name:"
 msgid "Tax Code Line"
 msgstr "Rând Cod Fiscal"
 
 msgctxt "model:account.tax.code.line.template,name:"
 msgid "Tax Code Line Template"
@@ -2981,27 +2953,25 @@
 msgid "Accounts"
 msgstr "Conturi"
 
 msgctxt "model:ir.action,name:act_account_tree"
 msgid "Accounts"
 msgstr "Conturi"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_account_tree_chart"
 msgid "Chart of Accounts"
-msgstr "Deschidere Plan de Conturi"
+msgstr "Plan de Conturi"
 
 msgctxt "model:ir.action,name:act_account_type_list"
 msgid "Account Types"
 msgstr "Tipuri de Conturi"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_account_type_template_tree"
 msgid "Account Types"
-msgstr "Tipuri de Conturi"
+msgstr "Tipuri de Cont"
 
 msgctxt "model:ir.action,name:act_account_type_tree"
 msgid "Account Types"
 msgstr "Tipuri de Conturi"
 
 msgctxt "model:ir.action,name:act_aged_balance_list"
 msgid "Aged Balance"
@@ -3019,18 +2989,17 @@
 msgid "Configuration"
 msgstr "Configurare"
 
 msgctxt "model:ir.action,name:act_create_periods"
 msgid "Create Periods"
 msgstr "Creare Perioade"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_delegate_lines_wizard"
 msgid "Delegate Lines"
-msgstr "Delegat la"
+msgstr "Rânduri Delegate"
 
 msgctxt "model:ir.action,name:act_fiscalyear_form"
 msgid "Fiscal Years"
 msgstr "Ani Fiscali"
 
 msgctxt "model:ir.action,name:act_fiscalyear_form_close"
 msgid "Close Fiscal Years"
@@ -3092,15 +3061,15 @@
 msgctxt "model:ir.action,name:act_move_form_grouping"
 msgid "Grouped Account Move"
 msgstr "Mişcari Cont Grupate"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_move_form_rescheduling"
 msgid "Reschedule Account Move"
-msgstr "Mişcari Cont Grupate"
+msgstr "Reprogrameaza Miscare Cont"
 
 msgctxt "model:ir.action,name:act_move_from_template"
 msgid "Account Move"
 msgstr "Mişcare Cont"
 
 msgctxt "model:ir.action,name:act_move_line_form"
 msgid "Account Move Lines"
@@ -3159,18 +3128,17 @@
 msgid "Write-off Methods"
 msgstr "Metode de Prescriere"
 
 msgctxt "model:ir.action,name:act_renew_fiscalyear"
 msgid "Renew Fiscal Year"
 msgstr "Renoire An Fiscal"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reschedule_lines_wizard"
 msgid "Reschedule Lines"
-msgstr "Reconciliere Rânduri"
+msgstr "Reprogramare Rânduri"
 
 msgctxt "model:ir.action,name:act_tax_code_list"
 msgid "Codes"
 msgstr "Coduri"
 
 msgctxt "model:ir.action,name:act_tax_code_template_tree"
 msgid "Tax Codes"
@@ -3179,15 +3147,15 @@
 msgctxt "model:ir.action,name:act_tax_code_tree"
 msgid "Codes"
 msgstr "Coduri"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_tax_code_tree_chart"
 msgid "Chart of Tax Codes"
-msgstr "Deschidere Plan Coduri Impozitare"
+msgstr "Plan Coduri Impozitare"
 
 msgctxt "model:ir.action,name:act_tax_group_form"
 msgid "Groups"
 msgstr "Grupuri"
 
 msgctxt "model:ir.action,name:act_tax_line_form"
 msgid "Tax Lines"
@@ -3200,15 +3168,15 @@
 msgctxt "model:ir.action,name:act_tax_rule_form"
 msgid "Rules"
 msgstr "Reguli"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_tax_rule_template_form"
 msgid "Tax Rules"
-msgstr "Regule de Impozitare"
+msgstr "Reguli de Impozitare"
 
 msgctxt "model:ir.action,name:act_tax_template_list"
 msgid "Taxes"
 msgstr "Impozite"
 
 msgctxt "model:ir.action,name:act_unreconcile_lines"
 msgid "Unreconcile Lines"
@@ -3246,46 +3214,43 @@
 msgid "Update Chart of Accounts from Template"
 msgstr "Actualizare Plan de Conturi de la Șablon"
 
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "Un plan de conturi exista deja pentru compania \"%(company)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
-msgstr ""
-"Contul \"%(account)s\" nu se poate şterge deoarece are rânduri de mişcări."
+msgstr "Nu puteți închide contul \"%(account)s\" deoarece are rânduri de mişcare."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_invalid_deferral_second_currency"
 msgid "To set a second currency for account \"%(account)s\", it must be deferral."
 msgstr "Pentru a seta valuta secundară pentru contul \"%(account)s\""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_account_invalid_lines_second_currency"
 msgid ""
 "To set a second currency for account \"%(account)s\", its lines must have "
 "the same second currency \"%(currency)s\"."
-msgstr "Pentru a seta valuta secundară pentru contul \"%(account)s\""
+msgstr ""
+"Pentru a seta o a doua monedă pentru contul \"%(account)s\", rândurile "
+"acestuia trebuie să aibă aceeași a doua monedă \"%(currency)s\"."
 
 msgctxt "model:ir.message,text:msg_account_invalid_type_second_currency"
 msgid ""
 "To set a second currency for account \"%(account)s\", it must not have a "
 "type \"payable\", \"revenue\", \"receivable\" nor \"expense\"."
 msgstr ""
 "Pentru a seta o valută secundara pentru cont \"%(account)s\", nu trebuie sa "
 "aiba tip \"furnizor\", \"venit\", \"client\" şi nici \"cheltuială\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_account_no_type_lines"
 msgid ""
 "You cannot remove type of account \"%(account)s\" because it has move lines."
-msgstr ""
-"Contul \"%(account)s\" nu se poate şterge deoarece are rânduri de mişcări."
+msgstr "Nu puteți şterge Contul \"%(account)s\" deoarece are rânduri de mişcare."
 
 msgctxt "model:ir.message,text:msg_cancel_line_delegated"
 msgid ""
 "The moves \"%(moves)s\" contain grouped lines, cancelling them will ungroup "
 "the lines."
 msgstr ""
 "Mişcările \"%(moves)s\" conşin rânduri grupate, anularea lor o sa le "
@@ -3319,20 +3284,21 @@
 msgid ""
 "To close fiscal year \"%(fiscalyear)s\", you must close all earlier fiscal "
 "years."
 msgstr ""
 "Pentru a închide anul fiscal \"%(fiscalyear)s\", trebuie închişi toţi ani "
 "fiscali anteriori."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_close_period_inactive_accounts"
 msgid ""
 "To close period \"%(period)s\", you must balance the inactive account "
 "\"%(account)s\"."
-msgstr "Pentru a închide perioada \"%(period)s\", contului inactiv \"%(account)s\"."
+msgstr ""
+"Pentru a închide perioada \"%(period)s\", trebuie să soldați contul inactiv "
+"\"%(account)s\"."
 
 msgctxt "model:ir.message,text:msg_close_period_non_posted_moves"
 msgid "To close period \"%(period)s\" you must post the moves \"%(moves)s\"."
 msgstr ""
 "Pentru a închide perioada \"%(period)s\" trebuie postate mişcările "
 "\"%(moves)s\"."
 
@@ -3385,14 +3351,16 @@
 "client/furnizor cu compania \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_fiscalyear_different_post_move_sequence"
 msgid ""
 "The fiscal years \"%(first)s\" and \"%(second)s\" cannot have the same post "
 "move sequence, you must use different sequences."
 msgstr ""
+"Anii fiscali \"%(first)s\" și \"%(second)s\" nu pot avea aceeași secvență de"
+" post mutare, trebuie să utilizați secvențe diferite."
 
 msgctxt "model:ir.message,text:msg_fiscalyear_overlap"
 msgid ""
 "The fiscal years \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
 "Anii fiscali \"%(first)s\" și \"%(second)s\" se suprapun, folosiți date "
@@ -3476,21 +3444,14 @@
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 "Nu puteți modifica sau șterge perioada jurnal \"%(journal_period)s\" pentru "
 "că conține mișcări."
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-"Nu puteți modifica sau șterge perioada \"%(period)s\" pentru că conține "
-"mișcări."
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 "Nu puteți adăuga/modifica/ștege rânduri în perioada jurnal închisă "
 "\"%(journal_period)s\"."
@@ -3522,66 +3483,73 @@
 "Folosiți perioada curentă pentru a anula mișcarea?"
 
 msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
+"Valoarea \"%(value)s\" a lui \"%(expression)s\" din șablonul "
+"\"%(template)s\" nu este un număr."
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
+"Nu s-a putut evalua expresia \"%(expression)s\" din șablonul \"%(template)s\" cu eroarea:\n"
+"\"%(error)s\""
 
 msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
 msgid "The keyword name \"%(name)s\" is not a valid identifier."
-msgstr ""
+msgstr "Numele cuvântului cheie \"%(name)s\" nu este un identificator valid."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
 msgid ""
 "To continue, you must create a fiscal year for the date \"%(date)s\" and "
 "company \"%(company)s\"."
-msgstr "Pentru a continua, trebuie creat anul fiscal pentru data \"%(date)s\"."
+msgstr ""
+"Pentru a continua, trebuie creat anul fiscal pentru data \"%(date)s\" și "
+"compania \"%(company)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
 msgid ""
 "To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
 "\"%(company)s\"for the date \"%(date)s\"."
-msgstr "Pentru a continua, trebuie creat anul fiscal pentru data \"%(date)s\"."
+msgstr ""
+"Pentru a continua, trebuie să redeschideți anul fiscal \"%(fiscalyear)s\" al"
+" companiei \"%(company)s\" pentru data \"%(date)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_no_open_period_date"
 msgid ""
 "To continue, you must reopen the period \"%(period)s\" of company "
 "\"%(company)s\" for the date \"%(date)s\"."
-msgstr "Pentru a continua, trebuie creată perioada pentru data \"%(date)s\"."
+msgstr ""
+"Pentru a continua, trebuie să redeschideți perioada \"%(period)s\" a "
+"companiei \"%(company)s\" pentru data \"%(date)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_no_period_date"
 msgid ""
 "To continue, you must create a period for the date \"%(date)s\" and company "
 "\"%(company)s\"."
-msgstr "Pentru a continua, trebuie creată perioada pentru data \"%(date)s\"."
+msgstr ""
+"Pentru a continua, trebuie să creați o perioadă pentru data \"%(date)s\" și "
+"compania \"%(company)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
-msgstr "Nu puteți seta debit și credit pe rând."
+msgstr "Contul poate avea setat doar un singur tip de debit sau credit."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
 msgid ""
 "The open fiscal year \"%(open)s\" can not be before the close fiscal year "
 "\"%(closed)s\"."
 msgstr ""
-"Datele pentru perioada \"%(period)s\" trebuie să fie în intervalul anului "
-"fiscal \"%(fiscalyear)s\"."
+"Anul fiscal deschis \"%(open)s\" nu poate fi anterior celui de închidere "
+"\"%(closed)s\"."
 
 msgctxt "model:ir.message,text:msg_open_journal_period_closed_period"
 msgid ""
 "You cannot reopen journal-period \"%(journal_period)s\" in closed period "
 "\"%(period)s\"."
 msgstr ""
 "Nu puteți redeschide perioda jurnal \"%(journal_period)s\" în perioada "
@@ -3611,27 +3579,39 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "Datele pentru perioada \"%(period)s\" trebuie să fie în intervalul anului "
 "fiscal \"%(fiscalyear)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+"Datele pentru perioada \"%(period)s\" trebuie să fie în intervalul anului "
+"fiscal \"%(fiscalyear)s\"."
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "Perioadele \"%(first)s\" și \"%(second)s\" se suprapun, trebuie folosite "
 "date diferite."
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
 msgid ""
 "You cannot use the same post move sequence for the periods \"%(first)s\" and"
 " \"%(second)s\" because they are from different fiscal years."
 msgstr ""
+"Nu puteți utiliza aceeași secvență de post mutare pentru perioadele "
+"\"%(first)s\" și \"%(second)s\" deoarece acestea provin din ani fiscali "
+"diferiți."
 
 msgctxt "model:ir.message,text:msg_post_empty_move"
 msgid "To post move \"%(move)s\", you must fill in its lines."
 msgstr "Pentru a posta mișcarea \"%(move)s\", trebuie completate rândurile."
 
 msgctxt "model:ir.message,text:msg_post_unbalanced_move"
 msgid ""
@@ -3645,43 +3625,40 @@
 msgid ""
 "To reconcile line \"%(line)s\", you must set its account \"%(account)s\" as "
 "reconcilable."
 msgstr ""
 "Pentru a reconcilia rândul \"%(line)s\", contul \"%(account)s\" trebuie "
 "setat ca reconciliabil."
 
-#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_reconciliation_currency_exchange_credit_account_missing"
 msgid ""
 "To reconcile lines, you must define a currency exchange credit account for "
 "\"%(company)s\"."
 msgstr ""
-"Pentru a continua, trebuie definit un cont de client pentru parte "
-"\"%(party)s\"."
+"Pentru a reconcilia rândurile trebuie să definiți un cont de credit de "
+"schimb valutar pentru \"%(company)s\"."
 
-#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_reconciliation_currency_exchange_debit_account_missing"
 msgid ""
 "To reconcile lines, you must define a currency exchange debit account for "
 "\"%(company)s\"."
 msgstr ""
-"Pentru a continua, trebuie definit un cont de client pentru parte "
-"\"%(party)s\"."
+"Pentru a reconcilia rânduri, trebuie să definiți un cont de debit de schimb "
+"valutar pentru \"%(company)s\"."
 
-#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_reconciliation_currency_exchange_journal_missing"
 msgid ""
 "To reconcile lines, you must define a currency exchange journal for "
 "\"%(company)s\"."
 msgstr ""
-"Pentru a continua, trebuie definit un cont de client pentru parte "
-"\"%(party)s\"."
+"Pentru a reconcilia rânduri trebuie să definiți un jurnal de schimb valutar "
+"pentru \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 "Reconcilierea \"%(reconciliation)s\" este corelată cu rândul \"%(line)s\".\n"
@@ -3689,15 +3666,15 @@
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
-"Reconcilierea \"%(reconciliation)s\" este corelată cu rândul \"%(line)s\".\n"
+"Reconcilierea \"%(reconciliation)s\" este corelată cu rândul de prescriptie \"%(line)s\".\n"
 "Posibil să fie nevoie de anularea mișcării \"%(move)s\"."
 
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
@@ -3720,57 +3697,58 @@
 msgid ""
 "To reconcile lines, they must have the same debit \"%(debit)s\" and credit "
 "\"%(credit)s\"."
 msgstr ""
 "Pentru a reconcilia, rândurile trebuie să aibă același debit \"%(debit)s\" "
 "și credit \"%(credit)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_reconciliation_write_off_missing"
 msgid ""
 "To reconcile lines with \"%(amount)s\" write-off, you must select a write-"
 "off method."
-msgstr "Pentru a crea un rând în contul \"%(account)s\", setați un tip sau"
+msgstr ""
+"Pentru a reconcilia rândurile cu prescriptia \"%(amount)s\", trebuie să "
+"selectați o metodă de prescriptie."
 
 msgctxt "model:ir.message,text:msg_reopen_fiscalyear_later"
 msgid ""
 "To reopen fiscal year \"%(fiscalyear)s\", you must reopen all later fiscal "
 "years."
 msgstr ""
 "Pentru a redeschide anul fiscal \"%(fiscalyear)s\", trebuie redeschiși toți "
 "anii fiscali recenți."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reschedule_line_same_account"
 msgid "You cannot reschedule lines with different accounts."
-msgstr "Nu se pot diviza rânduri cu părţi diferite."
+msgstr "Nu se pot diviza rânduri cu conturi diferite."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reschedule_line_same_currency"
 msgid "You cannot reschedule lines with different currencies."
 msgstr "Nu se pot diviza rânduri cu valute diferite."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reschedule_line_same_origins"
 msgid "You cannot reschedule lines with different origins."
 msgstr "Nu se pot diviza rânduri cu diferite surse."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reschedule_line_same_party"
 msgid "You cannot reschedule lines with different parties."
-msgstr "Nu se pot grupa rânduri cu diferite părţi."
+msgstr "Nu se pot grupa rânduri cu părţi diferite."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reschedule_line_wrong_amount"
 msgid ""
 "To reschedule the lines you must change the terms to have a total amount of "
 "%(total_amount)s instead of %(amount)s."
 msgstr ""
-"Pentru a diviza rânduri, trebuie schimbați termenii pentru suma totală de "
-"%(total_amount)s în loc de %(amount)s."
+"Pentru a reprograma rândurile, trebuie să modificați termenii astfel încât "
+"să aibă o sumă totală de %(total_amount)s în loc de %(amount)s."
 
 msgctxt "model:ir.message,text:msg_tax_update_unit_price_with_parent"
 msgid "You cannot set \"Update Unit Price\" on child tax \"%(tax)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_write_deferral"
 msgid "You cannot modify any account deferrals."
@@ -3893,18 +3871,19 @@
 msgid "Account Journal"
 msgstr "Jurnal Cont"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_account_move"
 msgid "Account Move"
 msgstr "Mişcare Cont"
 
+#, fuzzy
 msgctxt ""
 "model:ir.sequence.type,name:sequence_type_account_move_reconciliation"
 msgid "Account Move Reconciliation"
-msgstr ""
+msgstr "Reconciliere Mutare Cont"
 
 msgctxt "model:ir.ui.menu,name:menu_account"
 msgid "Financial"
 msgstr "Financiar"
 
 msgctxt "model:ir.ui.menu,name:menu_account_configuration"
 msgid "Configuration"
@@ -3921,24 +3900,23 @@
 msgctxt "model:ir.ui.menu,name:menu_account_tree"
 msgid "Accounts"
 msgstr "Conturi"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree_chart"
 msgid "Chart of Accounts"
-msgstr "Deschidere Plan de Conturi"
+msgstr "Plan de Conturi"
 
 msgctxt "model:ir.ui.menu,name:menu_account_type_list"
 msgid "Account Types"
 msgstr "Tipuri de Conturi"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_type_template_tree"
 msgid "Account Types"
-msgstr "Tipuri de Conturi"
+msgstr "Tipuri de Cont"
 
 msgctxt "model:ir.ui.menu,name:menu_account_type_tree"
 msgid "Account Types"
 msgstr "Tipuri de Conturi"
 
 msgctxt "model:ir.ui.menu,name:menu_aged_balance"
 msgid "Aged Balance"
@@ -4064,25 +4042,24 @@
 msgctxt "model:ir.ui.menu,name:menu_tax_code_tree"
 msgid "Codes"
 msgstr "Coduri"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_tax_code_tree_chart"
 msgid "Chart of Tax Codes"
-msgstr "Deschidere Plan Coduri Impozitare"
+msgstr "Plan Coduri Impozitare"
 
 msgctxt "model:ir.ui.menu,name:menu_tax_group_form"
 msgid "Groups"
 msgstr "Grupuri"
 
 msgctxt "model:ir.ui.menu,name:menu_tax_list"
 msgid "Taxes"
 msgstr "Impozite"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_tax_rule_form"
 msgid "Rules"
 msgstr "Reguli"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_tax_rule_template_form"
 msgid "Tax Rules"
@@ -4252,23 +4229,21 @@
 msgid "Date"
 msgstr "Data"
 
 msgctxt "report:account.general_ledger:"
 msgid "Debit"
 msgstr "Debit"
 
-#, fuzzy
 msgctxt "report:account.general_ledger:"
 msgid "Description"
 msgstr "Descriere"
 
-#, fuzzy
 msgctxt "report:account.general_ledger:"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciorna"
 
 msgctxt "report:account.general_ledger:"
 msgid "Fiscal Year:"
 msgstr "An Fiscal:"
 
 msgctxt "report:account.general_ledger:"
 msgid "From Date:"
@@ -4388,15 +4363,15 @@
 
 msgctxt "report:account.trial_balance:"
 msgid "Debit"
 msgstr "Debit"
 
 msgctxt "report:account.trial_balance:"
 msgid "End Balance"
-msgstr "Balanță Finală"
+msgstr "Sold Final"
 
 msgctxt "report:account.trial_balance:"
 msgid "Fiscal Year:"
 msgstr "An Fiscal:"
 
 msgctxt "report:account.trial_balance:"
 msgid "From Date:"
@@ -4404,19 +4379,19 @@
 
 msgctxt "report:account.trial_balance:"
 msgid "From Period:"
 msgstr "De la Perioada:"
 
 msgctxt "report:account.trial_balance:"
 msgid "Print Date:"
-msgstr "Tiparește Data:"
+msgstr "Data Tipărire:"
 
 msgctxt "report:account.trial_balance:"
 msgid "Start Balance"
-msgstr "Sold Initial"
+msgstr "Sold Inițial"
 
 msgctxt "report:account.trial_balance:"
 msgid "To"
 msgstr "La"
 
 msgctxt "report:account.trial_balance:"
 msgid "Total"
@@ -4498,15 +4473,14 @@
 msgid "Per Document"
 msgstr "Pe Document"
 
 msgctxt "selection:account.configuration.tax_rounding,tax_rounding:"
 msgid "Per Line"
 msgstr "Pe rând"
 
-#, fuzzy
 msgctxt "selection:account.fiscalyear,state:"
 msgid "Closed"
 msgstr "Închis"
 
 msgctxt "selection:account.fiscalyear,state:"
 msgid "Locked"
 msgstr "Blocat"
@@ -4555,15 +4529,14 @@
 msgid "Situation"
 msgstr "Situație"
 
 msgctxt "selection:account.journal,type:"
 msgid "Write-Off"
 msgstr "Prescriere"
 
-#, fuzzy
 msgctxt "selection:account.journal.period,state:"
 msgid "Closed"
 msgstr "Închis"
 
 msgctxt "selection:account.journal.period,state:"
 msgid "Open"
 msgstr "Deschis"
@@ -4580,25 +4553,22 @@
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "selection:account.move.line,state:"
 msgid "Valid"
 msgstr "Valabil"
 
-#, fuzzy
 msgctxt "selection:account.move.line.reschedule.start,frequency:"
 msgid "Monthly"
 msgstr "Lunar"
 
-#, fuzzy
 msgctxt "selection:account.move.line.reschedule.start,frequency:"
 msgid "Other"
-msgstr "Alte"
+msgstr "Altele"
 
-#, fuzzy
 msgctxt "selection:account.move.line.reschedule.start,frequency:"
 msgid "Quarterly"
 msgstr "Trimestrial"
 
 msgctxt "selection:account.move.line.template,operation:"
 msgid "Credit"
 msgstr "Credit"
@@ -4619,15 +4589,14 @@
 msgid "Numeric"
 msgstr "Numeric"
 
 msgctxt "selection:account.move.template.keyword,type_:"
 msgid "Party"
 msgstr "Parte"
 
-#, fuzzy
 msgctxt "selection:account.period,state:"
 msgid "Closed"
 msgstr "Închis"
 
 msgctxt "selection:account.period,state:"
 msgid "Locked"
 msgstr "Blocat"
@@ -4652,28 +4621,26 @@
 msgid "None"
 msgstr "Nici unul"
 
 msgctxt "selection:account.tax,type:"
 msgid "Percentage"
 msgstr "Procent"
 
-#, fuzzy
 msgctxt "selection:account.tax.code.context,method:"
 msgid "By Fiscal Year"
 msgstr "Pe An Fiscal"
 
-#, fuzzy
 msgctxt "selection:account.tax.code.context,method:"
 msgid "By Period"
-msgstr "Pe Perioade"
+msgstr "Pe Perioada"
 
 #, fuzzy
 msgctxt "selection:account.tax.code.context,method:"
 msgid "Over Periods"
-msgstr "Perioade"
+msgstr "Dupa Perioade"
 
 msgctxt "selection:account.tax.code.line,amount:"
 msgid "Base"
 msgstr "Baza"
 
 msgctxt "selection:account.tax.code.line,amount:"
 msgid "Tax"
@@ -4791,43 +4758,38 @@
 msgid "Children"
 msgstr "Copii"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Informații Generale"
 
-#, fuzzy
 msgctxt "view:account.account:"
 msgid "General Ledger"
 msgstr "Registru General"
 
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Termene"
 
-#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Credit Account"
-msgstr "Cont Credit"
+msgstr "Cont de Credit"
 
-#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Currency Exchange"
-msgstr "Valută"
+msgstr "Schimb Valutar"
 
-#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Debit Account"
-msgstr "Cont Debit"
+msgstr "Cont de Debit"
 
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Factura fiscala"
 
-#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Journal"
 msgstr "Jurnal"
 
 msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Mișcare"
@@ -4864,29 +4826,26 @@
 msgid "Close"
 msgstr "Închidere"
 
 msgctxt "view:account.journal.period:"
 msgid "Re-Open"
 msgstr "Re-Deschide"
 
-#, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "every"
 msgstr "fiecare"
 
-#, fuzzy
 msgctxt "view:account.move.line.reschedule.start:"
 msgid "months"
 msgstr "luni"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Alte Informații"
 
-#, fuzzy
 msgctxt "view:account.move.line:"
 msgid "Balance"
 msgstr "Sold"
 
 msgctxt "view:account.move.line:"
 msgid "Other Info"
 msgstr "Alte Informații"
@@ -4911,20 +4870,18 @@
 msgid "General Information"
 msgstr "Informații Generale"
 
 msgctxt "view:account.update_chart.succeed:"
 msgid "Chart of accounts updated successfully."
 msgstr "Planul de Conturi a fost actualizat cu success."
 
-#, fuzzy
 msgctxt "view:company.company:"
 msgid "Account"
 msgstr "Cont"
 
-#, fuzzy
 msgctxt "view:company.company:"
 msgid "Accounting"
 msgstr "Contabilitate"
 
 msgctxt "view:party.party:"
 msgid "Account"
 msgstr "Cont"
@@ -4990,47 +4947,42 @@
 msgid "OK"
 msgstr "OK"
 
 msgctxt "wizard_button:account.move.cancel,default,end:"
 msgid "Cancel"
 msgstr "Anulare"
 
-#, fuzzy
 msgctxt "wizard_button:account.move.line.delegate,start,delegate:"
 msgid "Delegate"
-msgstr "Delegat la"
+msgstr "Delegat"
 
-#, fuzzy
 msgctxt "wizard_button:account.move.line.delegate,start,end:"
 msgid "Cancel"
 msgstr "Anulare"
 
 msgctxt "wizard_button:account.move.line.group,start,end:"
 msgid "Cancel"
 msgstr "Anulare"
 
 msgctxt "wizard_button:account.move.line.group,start,group:"
 msgid "Group"
 msgstr "Grup"
 
-#, fuzzy
 msgctxt "wizard_button:account.move.line.reschedule,preview,end:"
 msgid "Cancel"
 msgstr "Anulare"
 
 msgctxt "wizard_button:account.move.line.reschedule,preview,reschedule:"
 msgid "Reschedule"
-msgstr ""
+msgstr "Reprogramare"
 
-#, fuzzy
 msgctxt "wizard_button:account.move.line.reschedule,start,end:"
 msgid "Cancel"
 msgstr "Anulare"
 
-#, fuzzy
 msgctxt "wizard_button:account.move.line.reschedule,start,preview:"
 msgid "Preview"
 msgstr "Previzualizare"
 
 msgctxt "wizard_button:account.move.open_journal,ask,end:"
 msgid "Cancel"
 msgstr "Anulare"
@@ -5071,20 +5023,18 @@
 msgid "Skip"
 msgstr "Sare Peste"
 
 msgctxt "wizard_button:account.reconcile,show,reconcile:"
 msgid "Reconcile"
 msgstr "Reconciliere"
 
-#, fuzzy
 msgctxt "wizard_button:account.reconcile,start,end:"
 msgid "Cancel"
 msgstr "Anulare"
 
-#, fuzzy
 msgctxt "wizard_button:account.reconcile,start,next_:"
 msgid "Reconcile"
 msgstr "Reconciliere"
 
 msgctxt "wizard_button:account.tax.test,test,end:"
 msgid "Close"
 msgstr "Închidere"
```

### Comparing `trytond_account-7.0.6/locale/ru.po` & `trytond_account-7.2.0/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -2648,22 +2648,18 @@
 msgstr "Позволяет проводить сверку по проводкам этого счета"
 
 #, fuzzy
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr "Все проводки для этого счета будут иметь вторичную валюту"
 
-#, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Налоги по умолчанию для ручного расчета проводок для типов журналов: "
-"\"расходы\" и \"доходы\"."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr ""
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3787,19 +3783,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3903,14 +3894,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/sl.po` & `trytond_account-7.2.0/locale/sl.po`

 * *Files 0% similar despite different names*

```diff
@@ -2517,22 +2517,18 @@
 msgstr "Dopušča usklajevanje knjiženih postavk tega konta."
 
 #, fuzzy
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr "Vsem vknjižbam za ta konto prisili uporabo te druge valute."
 
-#, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Privzeti davek pri ročno vnešenih postavkah \n"
-"za dnevnike tipa \"odhodek\" in \"prihodek\""
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr ""
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3655,19 +3651,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3773,14 +3764,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/tr.po` & `trytond_account-7.2.0/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -2472,16 +2472,15 @@
 
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr ""
 
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3559,19 +3558,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3668,14 +3662,20 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/locale/uk.po` & `trytond_account-7.2.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -2371,19 +2371,16 @@
 msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Примусово використати цю другу валюту \n"
 "для всіх проводок цього рахунку."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"Податок за умовчанням для ручного кодування рядків проводок\n"
-"для типів журналів: \"витрати\" і \"дохід\"."
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "Позначте, щоб перевизначити визначення шаблону"
 
 #, fuzzy
 msgctxt "help:account.account.context,fiscalyear:"
@@ -3460,21 +3457,14 @@
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr ""
 "Ви не можете змінити або видалити період журналу \"%(journal_period)s\", "
 "оскільки він містить проводки."
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr ""
-"Ви не можете змінити або видалити період \"%(period)s\", оскільки він "
-"містить проводки."
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr ""
 "Ви не можете додати/змінити/видалити рядки в закритому періоді журналу "
 "\"%(journal_period)s\"."
@@ -3598,14 +3588,23 @@
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr ""
 "Дати для періоду \"%(period)s\" мають бути між датами його фінансового року "
 "\"%(fiscalyear)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr ""
+"Дати для періоду \"%(period)s\" мають бути між датами його фінансового року "
+"\"%(fiscalyear)s\"."
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr ""
 "Періоди \"%(first)s\" і \"%(second)s\" збігаються, ви повинні використати "
 "різні дати."
```

### Comparing `trytond_account-7.0.6/locale/zh_CN.po` & `trytond_account-7.2.0/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -2325,19 +2325,16 @@
 
 msgctxt "help:account.account,second_currency:"
 msgid "Force all moves for this account to have this second currency."
 msgstr "强制此帐户的所有记账凭证都拥有这种第二货币。"
 
 msgctxt "help:account.account,taxes:"
 msgid ""
-"Default tax for manual encoding of move lines\n"
-"for journal types: \"expense\" and \"revenue\"."
+"Default taxes for documents to be applied when there is no other source."
 msgstr ""
-"记账凭证明细手动编码的默认税\n"
-"对于日记帐类型：“费用”和“收入”。"
 
 msgctxt "help:account.account,template_override:"
 msgid "Check to override template definition"
 msgstr "选中后可重写模板定义"
 
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
@@ -3343,19 +3340,14 @@
 
 msgctxt "model:ir.message,text:msg_modify_delete_journal_period_moves"
 msgid ""
 "You cannot modify or delete journal-period \"%(journal_period)s\" because it"
 " contains moves."
 msgstr "无法更改或者删除分期日记账 \"%(journal_period)s\"，因为它已经登记记账凭证."
 
-msgctxt "model:ir.message,text:msg_modify_delete_period_moves"
-msgid ""
-"You cannot modify or delete period \"%(period)s\" because it contains moves."
-msgstr "无法更改或者删除分期 \"%(period)s\"，因为它已经包含记账凭证."
-
 msgctxt "model:ir.message,text:msg_modify_line_closed_journal_period"
 msgid ""
 "You cannot add/modify/delete lines on closed journal-period "
 "\"%(journal_period)s\"."
 msgstr "已经结账的分期日记账 \"%(journal_period)s\" 无法添加/编辑/删除明细."
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
@@ -3456,14 +3448,21 @@
 
 msgctxt "model:ir.message,text:msg_period_fiscalyear_dates"
 msgid ""
 "The dates for period \"%(period)s\" must be between the dates of its fiscal "
 "year \"%(fiscalyear)s\"."
 msgstr "分期 \"%(period)s\" 的日期必须在会计年度 \"%(fiscalyear)s\" 的日期之间."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_period_move_dates"
+msgid ""
+"The dates for period \"%(period)s\" must include the date \"%(move_date)s\" "
+"of move \"%(move)s\"."
+msgstr "分期 \"%(period)s\" 的日期必须在会计年度 \"%(fiscalyear)s\" 的日期之间."
+
 msgctxt "model:ir.message,text:msg_period_overlap"
 msgid ""
 "The periods \"%(first)s\" and \"%(second)s\" overlap, you must use different"
 " dates."
 msgstr "分期 \"%(first)s\" 和 \"%(second)s\" 重叠，必须使用不同的日期."
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
```

### Comparing `trytond_account-7.0.6/localize.xsl` & `trytond_account-7.2.0/localize.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/message.xml` & `trytond_account-7.2.0/message.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account-7.0.6/message.xml` & `trytond_account-7.2.0/message.xml`

```diff
@@ -5,17 +5,14 @@
   <data grouped="1">
     <record model="ir.message" id="msg_no_period_date">
       <field name="text">To continue, you must create a period for the date &quot;%(date)s&quot; and company &quot;%(company)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_no_open_period_date">
       <field name="text">To continue, you must reopen the period &quot;%(period)s&quot; of company &quot;%(company)s&quot; for the date &quot;%(date)s&quot;.</field>
     </record>
-    <record model="ir.message" id="msg_modify_delete_period_moves">
-      <field name="text">You cannot modify or delete period &quot;%(period)s&quot; because it contains moves.</field>
-    </record>
     <record model="ir.message" id="msg_create_period_closed_fiscalyear">
       <field name="text">You cannot create a period in fiscal year &quot;%(fiscalyear)s&quot; because it is closed.</field>
     </record>
     <record model="ir.message" id="msg_open_period_closed_fiscalyear">
       <field name="text">You cannot reopen period &quot;%(period)s&quot; because its fiscal year &quot;%(fiscalyear)s&quot; is closed.</field>
     </record>
     <record model="ir.message" id="msg_change_period_post_move_sequence">
@@ -29,14 +26,17 @@
     </record>
     <record model="ir.message" id="msg_period_same_sequence">
       <field name="text">You cannot use the same post move sequence for the periods &quot;%(first)s&quot; and &quot;%(second)s&quot; because they are from different fiscal years.</field>
     </record>
     <record model="ir.message" id="msg_period_fiscalyear_dates">
       <field name="text">The dates for period &quot;%(period)s&quot; must be between the dates of its fiscal year &quot;%(fiscalyear)s&quot;.</field>
     </record>
+    <record model="ir.message" id="msg_period_move_dates">
+      <field name="text">The dates for period &quot;%(period)s&quot; must include the date &quot;%(move_date)s&quot; of move &quot;%(move)s&quot;.</field>
+    </record>
     <record model="ir.message" id="msg_journal_period_unique">
       <field name="text">You can create only one journal per period.</field>
     </record>
     <record model="ir.message" id="msg_modify_delete_journal_period_moves">
       <field name="text">You cannot modify or delete journal-period &quot;%(journal_period)s&quot; because it contains moves.</field>
     </record>
     <record model="ir.message" id="msg_create_journal_period_closed_period">
```

### Comparing `trytond_account-7.0.6/minimal_chart.xml` & `trytond_account-7.2.0/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/minimal_chart_bg.xml` & `trytond_account-7.2.0/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/minimal_chart_ca.xml` & `trytond_account-7.2.0/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/minimal_chart_de.xml` & `trytond_account-7.2.0/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/minimal_chart_en.xml` & `trytond_account-7.2.0/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/minimal_chart_es.xml` & `trytond_account-7.2.0/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/minimal_chart_fr.xml` & `trytond_account-7.2.0/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/minimal_chart_nl.xml` & `trytond_account-7.2.0/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/minimal_chart_pt.xml` & `trytond_account-7.2.0/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/minimal_chart_ru.xml` & `trytond_account-7.2.0/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/minimal_chart_sl.xml` & `trytond_account-7.2.0/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/move.py` & `trytond_account-7.2.0/move.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 from trytond.rpc import RPC
 from trytond.tools import firstline, grouped_slice, reduce_ids
 from trytond.transaction import Transaction, check_access
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 from .exceptions import (
-    CancelDelegatedWarning, CancelWarning, DelegateLineError, GroupLineError,
-    PeriodNotFoundError, PostError, ReconciliationDeleteWarning,
-    ReconciliationError, RescheduleLineError)
+    AccountMissing, CancelDelegatedWarning, CancelWarning, DelegateLineError,
+    GroupLineError, JournalMissing, PeriodNotFoundError, PostError,
+    ReconciliationDeleteWarning, ReconciliationError, RescheduleLineError)
 
 _MOVE_STATES = {
     'readonly': Eval('state') == 'posted',
     }
 _LINE_STATES = {
     'readonly': Eval('state') == 'valid',
     }
@@ -799,15 +799,15 @@
                         line.amount_second_currency),
                     else_=line.debit - line.credit)
                 if database.has_window_functions():
                     balance = Sum(balance,
                         window=Window(
                             [line.party, currency],
                             order_by=[
-                                line.maturity_date.asc,
+                                Coalesce(line.maturity_date, move.date).asc,
                                 move.date.desc,
                                 line.id.desc,
                                 ]))
 
                 party_where = Literal(False)
                 parties = {l.party for l in sub_lines}
                 if None in parties:
@@ -1205,14 +1205,28 @@
             return self.move.date
 
     @fields.depends('move', '_parent_move.state')
     def on_change_with_move_state(self, name=None):
         if self.move:
             return self.move.state
 
+    @classmethod
+    def order_maturity_date(self, tables):
+        pool = Pool()
+        Move = pool.get('account.move')
+        table, _ = tables[None]
+        if 'move' not in tables:
+            move = Move.__table__()
+            tables['move'] = {
+                None: (move, table.move == move.id),
+                }
+        else:
+            move, _ = tables['move'][None]
+        return [Coalesce(table.maturity_date, move.date)]
+
     @fields.depends('account')
     def on_change_with_has_maturity_date(self, name=None):
         if self.account:
             type_ = self.account.type
             return type_.receivable or type_.payable
 
     order_journal = MoveLineMixin._order_move_field('journal')
@@ -1697,15 +1711,15 @@
         period_id = Period.find(company.id, date=date)
 
         move = Move()
         move.company = company
         move.journal = configuration.get_multivalue(
             'currency_exchange_journal', company=company.id)
         if not move.journal:
-            raise ReconciliationError(gettext(
+            raise JournalMissing(gettext(
                     'account.'
                     'msg_reconciliation_currency_exchange_journal_missing',
                     company=company.rec_name))
         move.period = period_id
         move.date = date
 
         lines = []
@@ -1721,24 +1735,24 @@
         lines.append(line)
         line.debit = amount if amount > 0 else 0
         line.credit = -amount if amount < 0 else 0
         if line.credit:
             line.account = configuration.get_multivalue(
                 'currency_exchange_credit_account', company=company.id)
             if not line.account:
-                raise ReconciliationError(gettext(
+                raise AccountMissing(gettext(
                         'account.'
                         'msg_reconciliation_currency_exchange_'
                         'credit_account_missing',
                         company=company.rec_name))
         else:
             line.account = configuration.get_multivalue(
                 'currency_exchange_debit_account', company=company.id)
             if not line.account:
-                raise ReconciliationError(gettext(
+                raise AccountMissing(gettext(
                         'account.'
                         'msg_reconciliation_currency_exchange_'
                         'debit_account_missing',
                         company=company.rec_name))
 
         move.lines = lines
         return move
@@ -2231,31 +2245,29 @@
             self.show.parties = self.get_parties(self.show.account)
             if not next_party():
                 return 'end'
         if getattr(self.show, 'currencies', None) is None:
             self.show.currencies = self.get_currencies(
                 self.show.account, self.show.party)
 
-        while not next_currency():
-            while not next_party():
-                if not next_account():
-                    return 'end'
-        if self.start.automatic or self.start.only_balanced:
-            lines = self._default_lines()
-            if lines and self.start.automatic:
-                while lines:
-                    Line.reconcile(lines)
-                    lines = self._default_lines()
-                if not self.get_currencies(
-                        self.show.account, self.show.party,
-                        currency=self.show.currency):
-                    return 'next_'
-            elif not lines and self.start.only_balanced:
-                return 'next_'
-        return 'show'
+        while True:
+            while not next_currency():
+                while not next_party():
+                    if not next_account():
+                        return 'end'
+            if self.start.automatic or self.start.only_balanced:
+                lines = self._default_lines()
+                if lines and self.start.automatic:
+                    while lines:
+                        Line.reconcile(lines)
+                        lines = self._default_lines()
+                    continue
+                elif not lines and self.start.only_balanced:
+                    continue
+            return 'show'
 
     def default_show(self, fields):
         pool = Pool()
         Date = pool.get('ir.date')
 
         defaults = {}
         defaults['accounts'] = [a.id for a in self.show.accounts]
@@ -2469,14 +2481,15 @@
 
     def transition_cancel(self):
         pool = Pool()
         Line = pool.get('account.move.line')
         Move = pool.get('account.move')
         Warning = pool.get('res.user.warning')
         Unreconcile = pool.get('account.move.unreconcile_lines', type='wizard')
+        transaction = Transaction()
 
         moves = self.records
         moves_w_delegation = {
             m: [ml for ml in m.lines
                 if ml.reconciliation and ml.reconciliation.delegate_to]
             for m in moves}
         if any(dml for dml in moves_w_delegation.values()):
@@ -2489,16 +2502,15 @@
                 raise CancelDelegatedWarning(
                     key, gettext(
                         'account.msg_cancel_line_delegated', moves=names))
 
         to_post = []
         for move in moves:
             if moves_w_delegation.get(move):
-                # Skip further warnings
-                with Transaction().set_user(0):
+                with transaction.set_context(_skip_warnings=True):
                     Unreconcile.make_unreconciliation(moves_w_delegation[move])
             default = self.default_cancel(move)
             cancel_move = move.cancel(
                 default=default, reversal=self.default.reversal)
             if move.state == 'posted':
                 to_post.append(cancel_move)
             to_reconcile = defaultdict(list)
```

### Comparing `trytond_account-7.0.6/move.xml` & `trytond_account-7.2.0/move.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account-7.0.6/move.xml` & `trytond_account-7.2.0/move.xml`

```diff
@@ -28,48 +28,40 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="move_view_form"/>
       <field name="act_window" ref="act_move_form"/>
     </record>
     <menuitem parent="menu_entries" action="act_move_form" sequence="50" id="menu_move_form"/>
     <record model="ir.rule.group" id="rule_group_move_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.move')]"/>
+      <field name="model">account.move</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_move_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_move_companies"/>
     </record>
     <record model="ir.model.access" id="access_move">
-      <field name="model" search="[('model', '=', 'account.move')]"/>
+      <field name="model">account.move</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_move_account">
-      <field name="model" search="[('model', '=', 'account.move')]"/>
+      <field name="model">account.move</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_move_account_admin">
-      <field name="model" search="[('model', '=', 'account.move')]"/>
-      <field name="group" ref="group_account_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="move_post_button">
+      <field name="model">account.move</field>
       <field name="name">post</field>
       <field name="string">Post</field>
-      <field name="model" search="[('model', '=', 'account.move')]"/>
     </record>
     <record model="ir.sequence.type" id="sequence_type_account_move">
       <field name="name">Account Move</field>
     </record>
     <record model="ir.sequence.type-res.group" id="sequence_type_account_move_group_admin">
       <field name="sequence_type" ref="sequence_type_account_move"/>
       <field name="group" ref="res.group_admin"/>
@@ -96,38 +88,38 @@
     <record model="ir.action.keyword" id="act_move_reconciliation_lines_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">account.move.reconciliation,-1</field>
       <field name="action" ref="act_move_reconciliation_lines"/>
     </record>
     <record model="ir.rule.group" id="rule_group_move_reconciliation_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.move.reconciliation')]"/>
+      <field name="model">account.move.reconciliation</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_move_reconciliation_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_move_reconciliation_companies"/>
     </record>
     <record model="ir.model.access" id="access_move_reconciliation">
-      <field name="model" search="[('model', '=', 'account.move.reconciliation')]"/>
+      <field name="model">account.move.reconciliation</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_move_reconciliation_account">
-      <field name="model" search="[('model', '=', 'account.move.reconciliation')]"/>
+      <field name="model">account.move.reconciliation</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_move_reconciliation_account_admin">
-      <field name="model" search="[('model', '=', 'account.move.reconciliation')]"/>
+      <field name="model">account.move.reconciliation</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.sequence.type" id="sequence_type_account_move_reconciliation">
@@ -258,30 +250,30 @@
       <field name="model">account.move.reconcile_lines.writeoff</field>
       <field name="type">form</field>
       <field name="name">reconcile_lines_writeoff_form</field>
     </record>
     <record model="ir.action.wizard" id="act_reconcile_lines">
       <field name="name">Reconcile Lines</field>
       <field name="wiz_name">account.move.reconcile_lines</field>
-      <field name="model"/>
+      <field name="model" eval="None"/>
     </record>
     <record model="ir.action.keyword" id="act_reconcile_lines_keyword">
       <field name="keyword">form_action</field>
       <field name="model">account.move.line,-1</field>
       <field name="action" ref="act_reconcile_lines"/>
     </record>
     <record model="ir.action.keyword" id="act_reconcile_lines_keyword_general_ledger_line">
       <field name="keyword">form_action</field>
       <field name="model">account.general_ledger.line,-1</field>
       <field name="action" ref="act_reconcile_lines"/>
     </record>
     <record model="ir.action.wizard" id="act_unreconcile_lines">
       <field name="name">Unreconcile Lines</field>
       <field name="wiz_name">account.move.unreconcile_lines</field>
-      <field name="model"/>
+      <field name="model" eval="None"/>
     </record>
     <record model="ir.action.keyword" id="act_unreconcile_lines_keyword">
       <field name="keyword">form_action</field>
       <field name="model">account.move.line,-1</field>
       <field name="action" ref="act_unreconcile_lines"/>
     </record>
     <record model="ir.action.keyword" id="act_unreconcile_lines_keyword_general_ledger_line">
@@ -342,30 +334,30 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="reconcile_writeoff_view_form"/>
       <field name="act_window" ref="act_reconcile_writeoff_form"/>
     </record>
     <menuitem parent="menu_journal_configuration" action="act_reconcile_writeoff_form" sequence="20" id="menu_reconcile_writeoff_form"/>
     <record model="ir.rule.group" id="rule_group_reconcile_writeoff_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.move.reconcile.write_off')]"/>
+      <field name="model">account.move.reconcile.write_off</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reconcile_writeoff_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reconcile_writeoff_companies"/>
     </record>
     <record model="ir.model.access" id="access_reconcile_writeoff">
-      <field name="model" search="[('model', '=', 'account.move.reconcile.write_off')]"/>
+      <field name="model">account.move.reconcile.write_off</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reconcile_writeoff_account_admin">
-      <field name="model" search="[('model', '=', 'account.move.reconcile.write_off')]"/>
+      <field name="model">account.move.reconcile.write_off</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.action.wizard" id="act_group_lines_wizard">
```

### Comparing `trytond_account-7.0.6/move_template.py` & `trytond_account-7.2.0/move_template.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/move_template.xml` & `trytond_account-7.2.0/move_template.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account-7.0.6/move_template.xml` & `trytond_account-7.2.0/move_template.xml`

```diff
@@ -27,38 +27,38 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="move_template_view_form"/>
       <field name="act_window" ref="act_move_template_form"/>
     </record>
     <menuitem parent="menu_templates" action="act_move_template_form" sequence="10" id="menu_move_template_form"/>
     <record model="ir.rule.group" id="rule_group_move_template_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.move.template')]"/>
+      <field name="model">account.move.template</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_move_template_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_move_template_companies"/>
     </record>
     <record model="ir.model.access" id="access_move_template">
-      <field name="model" search="[('model', '=', 'account.move.template')]"/>
+      <field name="model">account.move.template</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_move_template_account">
-      <field name="model" search="[('model', '=', 'account.move.template')]"/>
+      <field name="model">account.move.template</field>
       <field name="group" ref="group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_move_template_account_admin">
-      <field name="model" search="[('model', '=', 'account.move.template')]"/>
+      <field name="model">account.move.template</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="move_template_keyword_view_form">
```

### Comparing `trytond_account-7.0.6/party.py` & `trytond_account-7.2.0/party.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,17 +107,17 @@
     def default_supplier_tax_rule(cls, **pattern):
         return cls._default_tax_rule('supplier', **pattern)
 
     def get_currency(self, name):
         pool = Pool()
         Company = pool.get('company.company')
         company_id = Transaction().context.get('company')
-        if company_id:
+        if company_id >= 0:
             company = Company(company_id)
-            return company.currency.id
+            return company.currency
 
     @classmethod
     def get_receivable_payable(cls, parties, names):
         '''
         Function to compute receivable, payable (today or not) for party ids.
         '''
         result = {}
```

### Comparing `trytond_account-7.0.6/party.xml` & `trytond_account-7.2.0/party.xml`

 * *Files 18% similar despite different names*

#### Comparing `trytond_account-7.0.6/party.xml` & `trytond_account-7.2.0/party.xml`

```diff
@@ -10,63 +10,73 @@
     </record>
     <record model="ir.ui.view" id="party_view_form">
       <field name="model">party.party</field>
       <field name="inherit" ref="party.party_view_form"/>
       <field name="name">party_form</field>
     </record>
     <record model="ir.model.field.access" id="access_party_accounts">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'accounts')]"/>
+      <field name="model">party.party</field>
+      <field name="field">accounts</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_accounts_account_party">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'accounts')]"/>
+      <field name="model">party.party</field>
+      <field name="field">accounts</field>
       <field name="group" ref="group_account_party"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_party_account_payable">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'account_payable')]"/>
+      <field name="model">party.party</field>
+      <field name="field">account_payable</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_account_payable_account_party">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'account_payable')]"/>
+      <field name="model">party.party</field>
+      <field name="field">account_payable</field>
       <field name="group" ref="group_account_party"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_party_account_receivable">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'account_receivable')]"/>
+      <field name="model">party.party</field>
+      <field name="field">account_receivable</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_account_receivable_account_party">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'account_receivable')]"/>
+      <field name="model">party.party</field>
+      <field name="field">account_receivable</field>
       <field name="group" ref="group_account_party"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_party_customer_tax_rule">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'customer_tax_rule')]"/>
+      <field name="model">party.party</field>
+      <field name="field">customer_tax_rule</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_customer_tax_rule_account_party">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'customer_tax_rule')]"/>
+      <field name="model">party.party</field>
+      <field name="field">customer_tax_rule</field>
       <field name="group" ref="group_account_party"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_party_supplier_tax_rule">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'supplier_tax_rule')]"/>
+      <field name="model">party.party</field>
+      <field name="field">supplier_tax_rule</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_supplier_tax_rule_account_party">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'supplier_tax_rule')]"/>
+      <field name="model">party.party</field>
+      <field name="field">supplier_tax_rule</field>
       <field name="group" ref="group_account_party"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_account-7.0.6/period.py` & `trytond_account-7.2.0/period.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from trytond.cache import Cache
 from trytond.const import OPERATORS
 from trytond.i18n import gettext
 from trytond.model import Index, ModelSQL, ModelView, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool
 from trytond.pyson import Eval, Id
+from trytond.tools import grouped_slice
 from trytond.transaction import Transaction
 
 from .exceptions import (
     ClosePeriodError, PeriodDatesError, PeriodNotFoundError,
     PeriodSequenceError)
 
 _STATES = {
@@ -118,14 +119,15 @@
             }.get(self.state)
 
     @classmethod
     def validate_fields(cls, periods, field_names):
         super().validate_fields(periods, field_names)
         cls.check_dates(periods, field_names)
         cls.check_fiscalyear_dates(periods, field_names)
+        cls.check_move_dates(periods, field_names)
         cls.check_post_move_sequence(periods, field_names)
 
     @classmethod
     def check_dates(cls, periods, field_names=None):
         if field_names and not (
                 field_names & {
                     'start_date', 'end_date', 'fiscalyear', 'type'}):
@@ -168,14 +170,42 @@
                     or period.end_date > fiscalyear.end_date):
                 raise PeriodDatesError(
                     gettext('account.msg_period_fiscalyear_dates',
                         period=period.rec_name,
                         fiscalyear=fiscalyear.rec_name))
 
     @classmethod
+    def check_move_dates(cls, periods, field_names=None):
+        pool = Pool()
+        Move = pool.get('account.move')
+        Lang = pool.get('ir.lang')
+        if field_names and not (field_names & {'start_date', 'end_date'}):
+            return
+        lang = Lang.get()
+
+        for sub_periods in grouped_slice(periods):
+            domain = ['OR']
+            for period in sub_periods:
+                domain.append([
+                        ('period', '=', period.id),
+                        ['OR',
+                            ('date', '<', period.start_date),
+                            ('date', '>', period.end_date),
+                            ],
+                        ])
+            moves = Move.search(domain, limit=1)
+            if moves:
+                move, = moves
+                raise PeriodDatesError(
+                    gettext('account.msg_period_move_dates',
+                        period=move.period.rec_name,
+                        move=move.rec_name,
+                        move_date=lang.strftime(move.date)))
+
+    @classmethod
     def check_post_move_sequence(cls, periods, field_names=None):
         if field_names and not (
                 field_names & {'post_move_sequence', 'fiscalyear'}):
             return
         for period in periods:
             if not period.post_move_sequence:
                 continue
@@ -239,25 +269,14 @@
                         date=lang.strftime(date),
                         period=period.rec_name,
                         company=company.rec_name if company else ''))
         else:
             return period
 
     @classmethod
-    def _check(cls, periods):
-        Move = Pool().get('account.move')
-        moves = Move.search([
-                ('period', 'in', [p.id for p in periods]),
-                ], limit=1)
-        if moves:
-            raise AccessError(
-                gettext('account.msg_modify_delete_period_moves',
-                    period=moves[0].period.rec_name))
-
-    @classmethod
     def search(cls, args, offset=0, limit=None, order=None, count=False,
             query=False):
         args = args[:]
 
         def process_args(args):
             i = 0
             while i < len(args):
@@ -301,23 +320,14 @@
 
     @classmethod
     def write(cls, *args):
         Move = Pool().get('account.move')
         actions = iter(args)
         args = []
         for periods, values in zip(actions, actions):
-            for key, value in values.items():
-                if key in ('start_date', 'end_date', 'fiscalyear'):
-                    def modified(period):
-                        if key in ['start_date', 'end_date']:
-                            return getattr(period, key) != value
-                        else:
-                            return period.fiscalyear .id != value
-                    cls._check(list(filter(modified, periods)))
-                    break
             if values.get('state') == 'open':
                 for period in periods:
                     if period.fiscalyear.state != 'open':
                         raise AccessError(
                             gettext(
                                 'account.msg_open_period_closed_fiscalyear',
                                 period=period.rec_name,
@@ -337,15 +347,14 @@
                                     period=period.rec_name))
             args.extend((periods, values))
         super(Period, cls).write(*args)
         cls._find_cache.clear()
 
     @classmethod
     def delete(cls, periods):
-        cls._check(periods)
         super(Period, cls).delete(periods)
         cls._find_cache.clear()
 
     @classmethod
     @ModelView.button
     @Workflow.transition('closed')
     def close(cls, periods):
```

### Comparing `trytond_account-7.0.6/period.xml` & `trytond_account-7.2.0/period.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_account-7.0.6/period.xml` & `trytond_account-7.2.0/period.xml`

```diff
@@ -31,28 +31,28 @@
     <record model="ir.action.act_window.view" id="act_period_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="period_view_form"/>
       <field name="act_window" ref="act_period_form"/>
     </record>
     <menuitem parent="menu_fiscalyear_configuration" action="act_period_form" sequence="20" id="menu_period_form"/>
     <record model="ir.model.button" id="period_close_button">
+      <field name="model">account.period</field>
       <field name="name">close</field>
       <field name="string">Close</field>
-      <field name="model" search="[('model', '=', 'account.period')]"/>
     </record>
     <record model="ir.model.button" id="period_reopen_button">
+      <field name="model">account.period</field>
       <field name="name">reopen</field>
       <field name="string">Re-Open</field>
-      <field name="model" search="[('model', '=', 'account.period')]"/>
     </record>
     <record model="ir.model.button" id="period_lock_button">
+      <field name="model">account.period</field>
       <field name="name">lock_</field>
       <field name="string">Lock</field>
       <field name="confirm">Are you sure you want to lock the period?</field>
-      <field name="model" search="[('model', '=', 'account.period')]"/>
     </record>
     <record model="ir.action.act_window" id="act_period_form_close">
       <field name="name">Close Periods</field>
       <field name="res_model">account.period</field>
       <field name="search_value" eval="[('state', '=', 'open')]" pyson="1"/>
       <field name="order" eval="[('start_date', 'ASC'), ('id', 'ASC')]" pyson="1"/>
     </record>
@@ -60,15 +60,15 @@
       <field name="sequence" eval="10"/>
       <field name="view" ref="period_view_list_close"/>
       <field name="act_window" ref="act_period_form_close"/>
     </record>
     <menuitem parent="menu_processing" action="act_period_form_close" sequence="30" id="menu_close_period"/>
     <record model="ir.rule.group" id="rule_group_period_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.period')]"/>
+      <field name="model">account.period</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_period_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_period_companies"/>
     </record>
   </data>
```

### Comparing `trytond_account-7.0.6/setup.py` & `trytond_account-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/tax.py` & `trytond_account-7.2.0/tax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1259,18 +1259,19 @@
 
         # We need to compensate the rounding we did
         remainder = self.currency.round(remainder, opposite=True)
         if abs(remainder) >= self.currency.rounding:
             offset_amount = self.currency.rounding.copy_sign(remainder)
 
             for tax in cycle(taxes.values()):
-                tax['amount'] -= offset_amount
-                remainder -= offset_amount
-                if abs(remainder) < self.currency.rounding:
-                    break
+                if tax['amount']:
+                    tax['amount'] -= offset_amount
+                    remainder -= offset_amount
+                    if abs(remainder) < self.currency.rounding:
+                        break
 
     @fields.depends('company', methods=['_get_tax_context', '_round_taxes'])
     def _get_taxes(self):
         pool = Pool()
         Tax = pool.get('account.tax')
         Configuration = pool.get('account.configuration')
```

### Comparing `trytond_account-7.0.6/tax.xml` & `trytond_account-7.2.0/tax.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account-7.0.6/tax.xml` & `trytond_account-7.2.0/tax.xml`

```diff
@@ -26,22 +26,22 @@
     <record model="ir.action.act_window.view" id="act_tax_group_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="tax_group_view_form"/>
       <field name="act_window" ref="act_tax_group_form"/>
     </record>
     <menuitem parent="menu_taxes" action="act_tax_group_form" sequence="20" id="menu_tax_group_form"/>
     <record model="ir.model.access" id="access_tax_group">
-      <field name="model" search="[('model', '=', 'account.tax.group')]"/>
+      <field name="model">account.tax.group</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_tax_group_account_admin">
-      <field name="model" search="[('model', '=', 'account.tax.group')]"/>
+      <field name="model">account.tax.group</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="tax_code_template_view_form">
@@ -68,15 +68,15 @@
     <record model="ir.action.act_window.view" id="act_tax_code_template_tree_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="tax_code_template_view_form"/>
       <field name="act_window" ref="act_tax_code_template_tree"/>
     </record>
     <menuitem parent="menu_templates" action="act_tax_code_template_tree" sequence="20" id="menu_tax_code_template_tree"/>
     <record model="ir.model.access" id="access_tax_code_template">
-      <field name="model" search="[('model', '=', 'account.tax.code.template')]"/>
+      <field name="model">account.tax.code.template</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="tax_code_view_form">
       <field name="model">account.tax.code</field>
@@ -145,31 +145,31 @@
     <menuitem parent="menu_reporting" action="act_tax_code_tree_chart" sequence="30" id="menu_tax_code_tree_chart"/>
     <record model="ir.ui.view" id="tax_code_context_view_form">
       <field name="model">account.tax.code.context</field>
       <field name="type">form</field>
       <field name="name">tax_code_context_form</field>
     </record>
     <record model="ir.model.access" id="access_tax_code">
-      <field name="model" search="[('model', '=', 'account.tax.code')]"/>
+      <field name="model">account.tax.code</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_tax_code_account_admin">
-      <field name="model" search="[('model', '=', 'account.tax.code')]"/>
+      <field name="model">account.tax.code</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_tax_code_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.tax.code')]"/>
+      <field name="model">account.tax.code</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_tax_code_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_tax_code_companies"/>
     </record>
     <record model="ir.ui.view" id="tax_code_line_template_view_form">
@@ -216,15 +216,15 @@
     <record model="ir.action.act_window.view" id="act_tax_template_list_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="tax_template_view_form"/>
       <field name="act_window" ref="act_tax_template_list"/>
     </record>
     <menuitem parent="menu_templates" action="act_tax_template_list" sequence="40" id="menu_tax_template_list"/>
     <record model="ir.model.access" id="access_tax_template">
-      <field name="model" search="[('model', '=', 'account.tax.template')]"/>
+      <field name="model">account.tax.template</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="tax_view_form">
       <field name="model">account.tax</field>
@@ -250,31 +250,31 @@
     <record model="ir.action.act_window.view" id="act_tax_list_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="tax_view_form"/>
       <field name="act_window" ref="act_tax_list"/>
     </record>
     <menuitem parent="menu_taxes" action="act_tax_list" sequence="10" id="menu_tax_list"/>
     <record model="ir.model.access" id="access_tax">
-      <field name="model" search="[('model', '=', 'account.tax')]"/>
+      <field name="model">account.tax</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_tax_account_admin">
-      <field name="model" search="[('model', '=', 'account.tax')]"/>
+      <field name="model">account.tax</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_tax_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.tax')]"/>
+      <field name="model">account.tax</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_tax_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_tax_companies"/>
     </record>
     <record model="ir.action.wizard" id="wizard_tax_test">
@@ -353,15 +353,15 @@
     <record model="ir.action.act_window.view" id="act_tax_rule_template_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="tax_rule_template_view_form"/>
       <field name="act_window" ref="act_tax_rule_template_form"/>
     </record>
     <menuitem parent="menu_templates" action="act_tax_rule_template_form" sequence="50" id="menu_tax_rule_template_form"/>
     <record model="ir.model.access" id="access_tax_rule_template">
-      <field name="model" search="[('model', '=', 'account.tax.rule.template')]"/>
+      <field name="model">account.tax.rule.template</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="tax_rule_view_form">
       <field name="model">account.tax.rule</field>
@@ -386,31 +386,31 @@
     <record model="ir.action.act_window.view" id="act_tax_rule_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="tax_rule_view_form"/>
       <field name="act_window" ref="act_tax_rule_form"/>
     </record>
     <menuitem parent="menu_taxes" action="act_tax_rule_form" sequence="50" id="menu_tax_rule_form"/>
     <record model="ir.model.access" id="access_tax_rule">
-      <field name="model" search="[('model', '=', 'account.tax.rule')]"/>
+      <field name="model">account.tax.rule</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_tax_rule_account_admin">
-      <field name="model" search="[('model', '=', 'account.tax.rule')]"/>
+      <field name="model">account.tax.rule</field>
       <field name="group" ref="group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_tax_rule_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.tax.rule')]"/>
+      <field name="model">account.tax.rule</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_tax_rule_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_tax_rule_companies"/>
     </record>
     <record model="ir.ui.view" id="tax_rule_line_template_view_form">
```

### Comparing `trytond_account-7.0.6/tests/scenario_account_active.rst` & `trytond_account-7.2.0/tests/scenario_account_active.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 =======================
 Account Active Scenario
 =======================
 
 Imports::
 
-    >>> import datetime
     >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
 Create company::
```

### Comparing `trytond_account-7.0.6/tests/scenario_account_reconcile.rst` & `trytond_account-7.2.0/tests/scenario_account_reconcile.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ==========================
 Account Reconcile Scenario
 ==========================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> party_required = globals().get('party_required', True)
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
@@ -112,16 +112,15 @@
     >>> reconcile.state
     'end'
 
 Run Reconcile wizard::
 
     >>> reconcile = Wizard('account.reconcile')
     >>> reconcile.execute('next_')
-    >>> reconcile.form.party == (customer if party_required else None)
-    True
+    >>> assertEqual(reconcile.form.party, (customer if party_required else None))
     >>> reconcile.form.write_off_amount
     Decimal('0.00')
     >>> len(reconcile.form.lines)
     0
     >>> reconcile.form.lines.extend(reconcile.form.lines.find())
     >>> len(reconcile.form.lines)
     2
```

### Comparing `trytond_account-7.0.6/tests/scenario_account_reconcile_automatic.rst` & `trytond_account-7.2.0/tests/scenario_account_reconcile_automatic.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ====================================
 Account Reconcile Automatic Scenario
 ====================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
     >>> Journal = Model.get('account.journal')
     >>> Line = Model.get('account.move.line')
```

### Comparing `trytond_account-7.0.6/tests/scenario_account_reconciliation.rst` & `trytond_account-7.2.0/tests/scenario_account_reconciliation.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ===============================
 Account Reconciliation Scenario
 ===============================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, assertTrue
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
     >>> GLLine = Model.get('account.general_ledger.line')
 
@@ -81,53 +81,53 @@
     >>> move.save()
     >>> reconcile2, = [l for l in move.lines if l.account == receivable]
 
 Reconcile Lines without writeoff::
 
     >>> reconcile_lines = Wizard('account.move.reconcile_lines',
     ...     [reconcile1, reconcile2])
-    >>> reconcile_lines.state == 'end'
-    True
+    >>> reconcile_lines.state
+    'end'
     >>> reconcile1.reload()
     >>> reconcile2.reload()
-    >>> reconcile1.reconciliation == reconcile2.reconciliation != None
-    True
+    >>> assertEqual(reconcile1.reconciliation, reconcile2.reconciliation)
+    >>> assertTrue(reconcile1.reconciliation)
     >>> len(reconcile1.reconciliation.lines)
     2
 
 Unreconcile lines::
 
     >>> unreconcile_lines = Wizard(
     ...     'account.move.unreconcile_lines', [reconcile1])
-    >>> unreconcile_lines.state == 'end'
-    True
+    >>> unreconcile_lines.state
+    'end'
     >>> reconcile1.reload()
     >>> reconcile1.reconciliation
     >>> reconcile2.reload()
     >>> reconcile2.reconciliation
 
 Reconcile general ledger lines::
 
     >>> gl_reconcile1 = GLLine(reconcile1.id)
     >>> gl_reconcile2 = GLLine(reconcile2.id)
     >>> reconcile_lines = Wizard('account.move.reconcile_lines',
     ...     [gl_reconcile1, gl_reconcile2])
-    >>> reconcile_lines.state == 'end'
-    True
+    >>> reconcile_lines.state
+    'end'
     >>> gl_reconcile1.reload()
     >>> gl_reconcile2.reload()
-    >>> gl_reconcile1.reconciliation == gl_reconcile2.reconciliation != None
-    True
+    >>> assertEqual(gl_reconcile1.reconciliation, gl_reconcile2.reconciliation)
+    >>> assertTrue(gl_reconcile1.reconciliation)
 
 Unreconcile general ledger, lines::
 
     >>> unreconcile_lines = Wizard(
     ...     'account.move.unreconcile_lines', [gl_reconcile1])
-    >>> unreconcile_lines.state == 'end'
-    True
+    >>> unreconcile_lines.state
+    'end'
     >>> gl_reconcile1.reload()
     >>> gl_reconcile1.reconciliation
     >>> gl_reconcile2.reload()
     >>> gl_reconcile2.reconciliation
 
 Create Moves for writeoff reconciliation::
 
@@ -174,25 +174,24 @@
     >>> writeoff_method.credit_account = expense
     >>> writeoff_method.save()
 
 Reconcile Lines with write-off::
 
     >>> reconcile_lines = Wizard('account.move.reconcile_lines',
     ...     [reconcile1, reconcile2])
-    >>> reconcile_lines.form_state == 'writeoff'
-    True
+    >>> reconcile_lines.form_state
+    'writeoff'
     >>> reconcile_lines.form.writeoff = writeoff_method
     >>> reconcile_lines.execute('reconcile')
     >>> reconcile1.reload()
     >>> reconcile2.reload()
-    >>> reconcile1.reconciliation == reconcile2.reconciliation != None
-    True
+    >>> assertEqual(reconcile1.reconciliation, reconcile2.reconciliation)
+    >>> assertTrue(reconcile1.reconciliation)
     >>> len(reconcile1.reconciliation.lines)
     3
     >>> writeoff_line1, = [l for l in reconcile1.reconciliation.lines
     ...     if l.credit == Decimal(3)]
     >>> writeoff_line2, = [l for l in writeoff_line1.move.lines
     ...     if l != writeoff_line1]
-    >>> writeoff_line2.account == expense
-    True
+    >>> assertEqual(writeoff_line2.account, expense)
     >>> writeoff_line2.debit
     Decimal('3.0')
```

### Comparing `trytond_account-7.0.6/tests/scenario_account_reconciliation_alternate_currency.rst` & `trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 =========================================
 Account Reconciliation Alternate Currency
 =========================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import create_company
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.tests.tools import activate_modules, assertEqual, assertTrue
 
     >>> post_moves = globals().get('post_moves', False)
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
@@ -103,16 +104,16 @@
 Reconcile lines::
 
     >>> reconcile_lines = Wizard(
     ...     'account.move.reconcile_lines', [reconcile1, reconcile2])
     >>> reconcile_lines.state
     'end'
 
-    >>> reconcile1.reconciliation == reconcile2.reconciliation != None
-    True
+    >>> assertEqual(reconcile1.reconciliation, reconcile2.reconciliation)
+    >>> assertTrue(reconcile1.reconciliation)
     >>> reconciliation, = Reconciliation.find([])
     >>> len(reconciliation.lines)
     3
     >>> currency_exchange_account.reload()
     >>> currency_exchange_account.balance
     Decimal('-5.00')
```

### Comparing `trytond_account-7.0.6/tests/scenario_account_reconciliation_alternate_currency_write_off.rst` & `trytond_account-7.2.0/tests/scenario_account_reconciliation_alternate_currency_write_off.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 ========================================================
 Account Reconciliation Alternate Currency with Write-Off
 ========================================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import create_company
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.tests.tools import activate_modules, assertTrue
 
     >>> post_moves = globals().get('post_moves', False)
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
@@ -118,16 +119,17 @@
     >>> reconcile_lines = Wizard(
     ...     'account.move.reconcile_lines', [reconcile1, reconcile2])
     >>> reconcile_lines.form_state
     'writeoff'
     >>> reconcile_lines.form.writeoff = write_off
     >>> reconcile_lines.execute('reconcile')
 
-    >>> reconcile1.reconciliation == reconcile2.reconciliation != None
+    >>> reconcile1.reconciliation == reconcile2.reconciliation
     True
+    >>> assertTrue(reconcile1.reconciliation)
     >>> reconciliation, = Reconciliation.find([])
     >>> len(reconciliation.lines)
     4
     >>> write_off.credit_account.reload()
     >>> write_off.credit_account.balance
     Decimal('-0.50')
     >>> currency_exchange_account.reload()
```

### Comparing `trytond_account-7.0.6/tests/scenario_close_fiscalyear.rst` & `trytond_account-7.2.0/tests/scenario_close_fiscalyear.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from dateutil.relativedelta import relativedelta
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
-    >>> from trytond.modules.currency.tests.tools import get_currency
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
     >>> last_year = today - relativedelta(years=1)
 
 Activate modules::
 
     >>> config = activate_modules('account')
@@ -48,16 +46,16 @@
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
 
 Prepare the closing settings for fiscalyear close::
 
     >>> journal_sequence, = Sequence.find([
-    ...        ('sequence_type.name', '=', "Account Journal"),
-    ...     ], limit=1)
+    ...         ('sequence_type.name', '=', "Account Journal"),
+    ...         ], limit=1)
     >>> journal_closing = Journal()
     >>> journal_closing.name = 'Closing'
     >>> journal_closing.code = 'CLO'
     >>> journal_closing.type = 'situation'
     >>> journal_closing.sequence = journal_sequence
     >>> journal_closing.save()
     >>> period_closing = Period()
```

### Comparing `trytond_account-7.0.6/tests/scenario_move_cancel.rst` & `trytond_account-7.2.0/tests/scenario_move_template.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,144 @@
-====================
-Move Cancel Scenario
-====================
+======================
+Move Template Scenario
+======================
 
 Imports::
 
+    >>> import datetime
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, create_tax_code, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import (
+    ...     activate_modules, assertEqual, assertGreaterEqual, assertLessEqual)
+
+    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
-    >>> Reconciliation = Model.get('account.move.reconciliation')
-
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = create_fiscalyear(company)
     >>> fiscalyear.click('create_period')
-    >>> period = fiscalyear.periods[0]
+    >>> period_ids = [p.id for p in fiscalyear.periods]
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
-    >>> receivable = accounts['receivable']
-    >>> revenue = accounts['revenue']
+    >>> payable = accounts['payable']
+    >>> expense = accounts['expense']
+    >>> tax = accounts['tax']
+
+Create tax code::
+
+    >>> TaxCode = Model.get('account.tax.code')
+    >>> tax = create_tax(Decimal('0.1'))
+    >>> tax.save()
+    >>> base_code = create_tax_code(tax, amount='base')
+    >>> base_code.save()
+    >>> tax_code = create_tax_code(tax)
+    >>> tax_code.save()
 
 Create parties::
 
     >>> Party = Model.get('party.party')
-    >>> customer = Party(name='Customer')
-    >>> customer.save()
-    >>> party = Party(name='Party')
-    >>> party.save()
+    >>> supplier = Party(name='Supplier')
+    >>> supplier.save()
 
-Create Move to cancel::
+Create Template::
 
+    >>> MoveTemplate = Model.get('account.move.template')
     >>> Journal = Model.get('account.journal')
-    >>> Move = Model.get('account.move')
-    >>> journal_revenue, = Journal.find([
-    ...         ('code', '=', 'REV'),
-    ...         ])
-    >>> journal_cash, = Journal.find([
+    >>> template = MoveTemplate()
+    >>> template.name = 'Test'
+    >>> template.journal, = Journal.find([
     ...         ('code', '=', 'CASH'),
     ...         ])
-    >>> move = Move()
-    >>> move.period = period
-    >>> move.journal = journal_revenue
-    >>> move.date = period.start_date
-    >>> line = move.lines.new()
-    >>> line.account = revenue
-    >>> line.credit = Decimal(42)
-    >>> line = move.lines.new()
-    >>> line.account = receivable
-    >>> line.debit = Decimal(32)
-    >>> line.party = customer
-    >>> line.second_currency = get_currency('EUR')
-    >>> line.amount_second_currency = Decimal(30)
-    >>> line = move.lines.new()
-    >>> line.account = receivable
-    >>> line.debit = Decimal(10)
-    >>> line.party = party
-    >>> move.save()
-    >>> revenue.reload()
-    >>> revenue.credit
-    Decimal('42.00')
-    >>> receivable.reload()
-    >>> receivable.debit
-    Decimal('42.00')
-
-Cancel reversal Move::
-
-    >>> cancel_move = Wizard('account.move.cancel', [move])
-    >>> cancel_move.form.description = "Reversal"
-    >>> cancel_move.form.reversal = True
-    >>> cancel_move.execute('cancel')
-    >>> cancel_move.state
-    'end'
-    >>> move.reload()
-    >>> [bool(l.reconciliation) for l in move.lines if l.account == receivable]
-    [True, True]
-    >>> line, _ = [l for l in move.lines if l.account == receivable]
-    >>> cancel_move, = [l.move for l in line.reconciliation.lines
-    ...     if l.move != move]
-    >>> cancel_move.origin == move
-    True
-    >>> cancel_move.description
-    'Reversal'
-    >>> sorted([l.origin.id for l in cancel_move.lines]) == \
-    ...     sorted(map(int, move.lines))
-    True
-    >>> revenue.reload()
-    >>> revenue.credit
-    Decimal('42.00')
-    >>> revenue.debit
-    Decimal('42.00')
-    >>> receivable.reload()
-    >>> receivable.credit
-    Decimal('42.00')
-    >>> receivable.debit
-    Decimal('42.00')
-
-    >>> reconciliations = {
-    ...     l.reconciliation for l in cancel_move.lines if l.reconciliation}
-    >>> Reconciliation.delete(list(reconciliations))
-    >>> cancel_move.reload()
-    >>> cancel_move.delete()
-
-Cancel Move::
-
-    >>> cancel_move = Wizard('account.move.cancel', [move])
-    >>> cancel_move.form.description = 'Cancel'
-    >>> cancel_move.form.reversal = False
-    >>> cancel_move.execute('cancel')
-    >>> cancel_move.state
-    'end'
-    >>> move.reload()
-    >>> [bool(l.reconciliation) for l in move.lines if l.account == receivable]
-    [True, True]
-    >>> line, _ = [l for l in move.lines if l.account == receivable]
-    >>> cancel_move, = [l.move for l in line.reconciliation.lines
-    ...     if l.move != move]
-    >>> cancel_move.origin == move
-    True
-    >>> cancel_move.description
-    'Cancel'
-    >>> sorted([l.origin.id for l in cancel_move.lines]) == \
-    ...     sorted(map(int, move.lines))
-    True
-    >>> revenue.reload()
-    >>> revenue.credit
-    Decimal('0.00')
-    >>> receivable.reload()
-    >>> receivable.debit
-    Decimal('0.00')
+    >>> _ = template.keywords.new(name='party', string='Party',
+    ...     type_='party')
+    >>> _ = template.keywords.new(name='description', string='Description',
+    ...     type_='char')
+    >>> _ = template.keywords.new(name='amount', string='Amount',
+    ...     type_='numeric', digits=2)
+    >>> template.description = '{party} - {description}'
+    >>> line = template.lines.new()
+    >>> line.operation = 'credit'
+    >>> line.account = payable
+    >>> line.party = 'party'
+    >>> line.amount = 'amount'
+    >>> line = template.lines.new()
+    >>> line.operation = 'debit'
+    >>> line.account = expense
+    >>> line.amount = 'amount / 1.1'
+    >>> ttax = line.taxes.new()
+    >>> ttax.amount = line.amount
+    >>> ttax.tax = tax
+    >>> ttax.type = 'base'
+    >>> line = template.lines.new()
+    >>> line.operation = 'debit'
+    >>> line.account = tax.invoice_account
+    >>> line.amount = 'amount * (1 - 1/1.1)'
+    >>> ttax = line.taxes.new()
+    >>> ttax.amount = line.amount
+    >>> ttax.tax = tax
+    >>> ttax.type = 'tax'
+    >>> template.save()
+
+Create Move::
+
+    >>> create_move = Wizard('account.move.template.create')
+    >>> assertEqual(create_move.form.date, today)
+    >>> period = create_move.form.period
+    >>> assertLessEqual(period.start_date, today)
+    >>> assertGreaterEqual(period.end_date, today)
+    >>> index = fiscalyear.periods.index(create_move.form.period)
+    >>> next_period = fiscalyear.periods[index + 1]
+    >>> create_move.form.date = next_period.start_date
+    >>> assertEqual(create_move.form.period, next_period)
+    >>> prev_period = fiscalyear.periods[index - 1]
+    >>> create_move.form.period = prev_period
+    >>> assertEqual(create_move.form.date, prev_period.end_date)
+    >>> create_move.form.period = next_period
+    >>> assertEqual(create_move.form.date, next_period.start_date)
+    >>> create_move.form.template = template
+    >>> create_move.execute('keywords')
+    >>> data = {}
+    >>> keywords = data['keywords'] = {}
+    >>> keywords['party'] = supplier.id
+    >>> keywords['description'] = 'Test'
+    >>> keywords['amount'] = Decimal('12.24')
+    >>> context = create_move._context.copy()
+    >>> context.update(create_move._config.context)
+    >>> _ = create_move._proxy.execute(create_move.session_id, data, 'create_',
+    ...     context)
+
+.. note:: using custom call because proteus doesn't support fake model
+
+Check the Move::
+
+    >>> Move = Model.get('account.move')
+    >>> move, = Move.find([])
+    >>> len(move.lines)
+    3
+    >>> sorted((l.debit, l.credit) for l in move.lines)
+    [(Decimal('0'), Decimal('12.24')), (Decimal('1.11'), Decimal('0')), (Decimal('11.13'), Decimal('0'))]
+    >>> move.description
+    'Supplier - Test'
+    >>> with config.set_context(periods=period_ids):
+    ...     base_code = TaxCode(base_code.id)
+    ...     base_code.amount
+    Decimal('11.13')
+    >>> with config.set_context(periods=period_ids):
+    ...     tax_code = TaxCode(tax_code.id)
+    ...     tax_code.amount
+    Decimal('1.11')
```

### Comparing `trytond_account-7.0.6/tests/scenario_move_line_delegate.rst` & `trytond_account-7.2.0/tests/scenario_move_line_delegate.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 =======================
 
 Imports::
 
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
     >>> Journal = Model.get('account.journal')
     >>> Move = Model.get('account.move')
@@ -82,16 +81,15 @@
     >>> party2.reload()
     >>> party2.receivable
     Decimal('0.0')
 
 Delegate lines::
 
     >>> delegate = Wizard('account.move.line.delegate', receivable_lines)
-    >>> delegate.form.journal == journal
-    True
+    >>> assertEqual(delegate.form.journal, journal)
     >>> delegate.form.party = party2
     >>> delegate.form.description = "Delegate lines"
     >>> delegate.execute('delegate')
 
     >>> accounts['receivable'].reload()
     >>> accounts['receivable'].balance
     Decimal('100.00')
```

### Comparing `trytond_account-7.0.6/tests/scenario_move_line_group.rst` & `trytond_account-7.2.0/tests/scenario_move_line_group.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Group Lines Scenario
 ====================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
     >>> from trytond.modules.account.exceptions import CancelDelegatedWarning
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
 Create company::
 
@@ -128,32 +128,31 @@
     >>> Reconciliation = Model.get('account.move.reconciliation')
     >>> reconciliations = Reconciliation.find([])
     >>> len(reconciliations)
     2
     >>> all(r.delegate_to for r in reconciliations)
     True
     >>> delegate_to = reconciliations[0].delegate_to
-    >>> delegate_to.account == receivable
-    True
+    >>> assertEqual(delegate_to.account, receivable)
     >>> delegate_to.debit
     Decimal('50')
-    >>> delegate_to.maturity_date == period.start_date + dt.timedelta(days=2)
-    True
+    >>> assertEqual(
+    ...     delegate_to.maturity_date, period.start_date + dt.timedelta(days=2))
     >>> delegate_to.move_description_used
     'Group lines'
 
 Cancelling the delegation move::
 
    >>> delegation_move = delegate_to.move
    >>> cancel = Wizard('account.move.cancel', [delegation_move])
    >>> try:
-   ...   cancel.execute('cancel')
+   ...     cancel.execute('cancel')
    ... except CancelDelegatedWarning as warning:
-   ...   _, (key, *_) = warning.args
-   ...   raise  # doctest: +IGNORE_EXCEPTION_DETAIL
+   ...     _, (key, *_) = warning.args
+   ...     raise
    Traceback (most recent call last):
       ...
    CancelDelegatedWarning: ...
 
    >>> Warning = Model.get('res.user.warning')
    >>> Warning(user=config.user, name=key).save()
    >>> cancel.execute('cancel')
```

### Comparing `trytond_account-7.0.6/tests/scenario_move_line_reschedule.rst` & `trytond_account-7.2.0/tests/scenario_move_line_reschedule.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 =========================
 Reschedule Lines Scenario
 =========================
 
 Imports::
 
-    >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from dateutil.relativedelta import relativedelta
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
     >>> Journal = Model.get('account.journal')
     >>> Line = Model.get('account.move.line')
@@ -85,22 +83,18 @@
     >>> reschedule.form.start_date = period.end_date
     >>> reschedule.form.frequency = 'other'
     >>> reschedule.form.interval = 2
     >>> reschedule.form.amount = Decimal('30.00')
     >>> reschedule.execute('preview')
 
     >>> term1, term2, term3, term4 = reschedule.form.terms
-    >>> term1.date == period.end_date
-    True
-    >>> term2.date == period.end_date + relativedelta(months=2)
-    True
-    >>> term3.date == period.end_date + relativedelta(months=4)
-    True
-    >>> term4.date == period.end_date + relativedelta(months=6)
-    True
+    >>> assertEqual(term1.date, period.end_date)
+    >>> assertEqual(term2.date, period.end_date + relativedelta(months=2))
+    >>> assertEqual(term3.date, period.end_date + relativedelta(months=4))
+    >>> assertEqual(term4.date, period.end_date + relativedelta(months=6))
     >>> term1.amount, term2.amount, term3.amount, term4.amount
     (Decimal('30.00'), Decimal('30.00'), Decimal('30.00'), Decimal('10.00'))
 
 Split line by number::
 
     >>> reschedule = Wizard('account.move.line.reschedule', [line])
     >>> reschedule.form.total_amount
@@ -108,20 +102,17 @@
     >>> reschedule.form.start_date = period.end_date
     >>> reschedule.form.frequency = 'monthly'
     >>> reschedule.form.number = 3
     >>> reschedule.execute('preview')
 
     >>> reschedule.form.description = "Split 3 months"
     >>> term1, term2, term3 = reschedule.form.terms
-    >>> term1.date == period.end_date
-    True
-    >>> term2.date == period.end_date + relativedelta(months=1)
-    True
-    >>> term3.date == period.end_date + relativedelta(months=2)
-    True
+    >>> assertEqual(term1.date, period.end_date)
+    >>> assertEqual(term2.date, period.end_date + relativedelta(months=1))
+    >>> assertEqual(term3.date, period.end_date + relativedelta(months=2))
     >>> term1.amount, term2.amount, term3.amount
     (Decimal('33.33'), Decimal('33.33'), Decimal('33.34'))
     >>> term1.amount = Decimal('40.00')
     >>> term2.amount = term3.amount = Decimal('30.00')
     >>> term3.date = period.end_date + relativedelta(months=3)
 
     >>> reschedule.execute('reschedule')
@@ -139,19 +130,16 @@
     ...     ('account', '=', receivable.id),
     ...     ('reconciliation', '=', None),
     ...     ], order=[('maturity_date', 'ASC')])
     >>> line1, line2, line3 = lines
 
     >>> line1.debit, line1.amount
     (Decimal('36.00'), Decimal('40.00'))
-    >>> line1.maturity_date == period.end_date
-    True
+    >>> assertEqual(line1.maturity_date, period.end_date)
 
     >>> line2.debit, line2.amount
     (Decimal('27.00'), Decimal('30.00'))
-    >>> line2.maturity_date == period.end_date + relativedelta(months=1)
-    True
+    >>> assertEqual(line2.maturity_date, period.end_date + relativedelta(months=1))
 
     >>> line3.debit, line3.amount
     (Decimal('27.00'), Decimal('30.00'))
-    >>> line3.maturity_date == period.end_date + relativedelta(months=3)
-    True
+    >>> assertEqual(line3.maturity_date, period.end_date + relativedelta(months=3))
```

### Comparing `trytond_account-7.0.6/tests/scenario_renew_fiscalyear.rst` & `trytond_account-7.2.0/tests/scenario_renew_fiscalyear.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 =================================
 Account Renew Fiscalyear Scenario
 =================================
 
 Imports::
 
-    >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from proteus import Wizard
     >>> from trytond.modules.account.tests.tools import create_fiscalyear
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
 Create company::
 
@@ -65,10 +63,9 @@
 
 Renew fiscalyear and test sequence name is updated::
 
     >>> renew_fiscalyear = Wizard('account.fiscalyear.renew')
     >>> renew_fiscalyear.form.reset_sequences = True
     >>> renew_fiscalyear.execute('create_')
     >>> new_fiscalyear, = renew_fiscalyear.actions[0]
-    >>> new_fiscalyear.post_move_sequence.name == (
+    >>> assertEqual(new_fiscalyear.post_move_sequence.name,
     ...     'Sequence %s' % new_fiscalyear.name)
-    True
```

### Comparing `trytond_account-7.0.6/tests/scenario_reports.rst` & `trytond_account-7.2.0/tests/scenario_reports.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Account Reports Scenario
 ========================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard, Report
+
+    >>> from proteus import Model, Report
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account')
```

### Comparing `trytond_account-7.0.6/tests/scenario_tax_code.rst` & `trytond_account-7.2.0/tests/scenario_tax_code.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 =========================
 Account Tax Code Scenario
 =========================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, create_tax_code, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax, create_tax_code
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
 Create company::
```

### Comparing `trytond_account-7.0.6/tests/test_module.py` & `trytond_account-7.2.0/tests/test_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import datetime
 from decimal import Decimal
 
 from dateutil.relativedelta import relativedelta
 
 from trytond.exceptions import UserError
-from trytond.modules.account.exceptions import FiscalYearDatesError
+from trytond.modules.account.exceptions import (
+    FiscalYearDatesError, PeriodDatesError)
 from trytond.modules.account.tax import TaxableMixin
 from trytond.modules.company.tests import (
     CompanyTestMixin, PartyCompanyCheckEraseMixin, create_company, set_company)
 from trytond.modules.currency.tests import create_currency
 from trytond.pool import Pool
 from trytond.tests.test_tryton import ModuleTestCase, with_transaction
 from trytond.transaction import Transaction, inactive_records
@@ -307,14 +308,73 @@
                 company,
                 start_date=datetime.date(2021, 1, 1),
                 end_date=datetime.date(2021, 12, 31))
             with self.assertRaises(FiscalYearDatesError):
                 earlier_fiscalyear.save()
 
     @with_transaction()
+    def test_change_fiscalyear_dates_with_periods(self):
+        "Test change fiscal year dates"
+        company = create_company()
+        with set_company(company):
+            fiscalyear = get_fiscalyear(
+                company,
+                start_date=datetime.date(2023, 1, 1),
+                end_date=datetime.date(2023, 12, 31))
+            fiscalyear.save()
+            fiscalyear.create_period([fiscalyear])
+
+            # Extend
+            fiscalyear.end_date = datetime.date(2024, 5, 31)
+            fiscalyear.save()
+
+            # Shorten
+            with self.assertRaises(PeriodDatesError):
+                fiscalyear.end_date = datetime.date(2023, 5, 31)
+                fiscalyear.save()
+
+    @with_transaction()
+    def test_change_period_dates_with_move(self):
+        "Test change period dates"
+        pool = Pool()
+        Period = pool.get('account.period')
+        Move = pool.get('account.move')
+        Journal = pool.get('account.journal')
+        company = create_company()
+        with set_company(company):
+            create_chart(company)
+            fiscalyear = get_fiscalyear(company)
+            fiscalyear.save()
+
+            period = Period(
+                fiscalyear=fiscalyear,
+                type='adjustment',
+                name="Period",
+                start_date=fiscalyear.start_date,
+                end_date=fiscalyear.start_date)
+            period.save()
+
+            journal, = Journal.search([], limit=1)
+
+            move, = Move.create([{
+                        'period': period.id,
+                        'journal': journal.id,
+                        'date': period.start_date,
+                        }])
+
+            # Extend
+            period.end_date = fiscalyear.end_date
+            period.save()
+
+            # Shorten
+            with self.assertRaises(PeriodDatesError):
+                period.start_date = fiscalyear.end_date
+                period.save()
+
+    @with_transaction()
     def test_account_debit_credit(self):
         'Test account debit/credit'
         pool = Pool()
         Party = pool.get('party.party')
         FiscalYear = pool.get('account.fiscalyear')
         Journal = pool.get('account.journal')
         Account = pool.get('account.account')
@@ -1215,14 +1275,72 @@
             taxline_1, taxline_2 = taxable._get_taxes()
             self.assertEqual(taxline_1['base'], Decimal('1.04'))
             self.assertEqual(taxline_1['amount'], Decimal('.11'))
             self.assertEqual(taxline_2['base'], Decimal('1.04'))
             self.assertEqual(taxline_2['amount'], Decimal('.10'))
 
     @with_transaction()
+    def test_taxable_mixin_tax_residual_rounding_with_0(self):
+        "Test TaxableMixin for rounding with residual amount and tax 0"
+        pool = Pool()
+        Account = pool.get('account.account')
+        Tax = pool.get('account.tax')
+        Configuration = pool.get('account.configuration')
+        currency = create_currency('cur')
+
+        company = create_company()
+        with set_company(company):
+            create_chart(company)
+
+            config = Configuration(1)
+            config.tax_rounding = 'line'
+            config.save()
+
+            tax_account, = Account.search([
+                    ('name', '=', 'Main Tax'),
+                    ])
+
+            tax0 = Tax()
+            tax0.name = tax0.description = "Tax 0"
+            tax0.type = 'percentage'
+            tax0.rate = Decimal('0')
+            tax0.invoice_account = tax_account
+            tax0.credit_note_account = tax_account
+            tax0.save()
+            tax1 = Tax()
+            tax1.name = tax1.description = "Tax 1"
+            tax1.type = 'percentage'
+            tax1.rate = Decimal('.1')
+            tax1.invoice_account = tax_account
+            tax1.credit_note_account = tax_account
+            tax1.save()
+            tax2 = Tax()
+            tax2.name = tax2.description = "Tax 2"
+            tax2.type = 'percentage'
+            tax2.rate = Decimal('.1')
+            tax2.invoice_account = tax_account
+            tax2.credit_note_account = tax_account
+            tax2.save()
+
+            taxable = self.Taxable(
+                currency=currency,
+                taxable_lines=[
+                    ([tax0, tax1, tax2], Decimal('1.0417'), 1, None),
+                    ],
+                company=company)
+
+            taxline_0, taxline_1, taxline_2 = taxable._get_taxes()
+            self.assertEqual(taxline_0['base'], Decimal('1.04'))
+            self.assertEqual(taxline_0['amount'], Decimal('0'))
+            self.assertEqual(taxline_1['base'], Decimal('1.04'))
+            self.assertEqual(taxline_1['amount'], Decimal('.11'))
+            self.assertEqual(taxline_2['base'], Decimal('1.04'))
+            self.assertEqual(taxline_2['amount'], Decimal('.10'))
+
+    @with_transaction()
     def test_taxable_mixin_tax_residual_rounding_negative_residual(self):
         "Test TaxableMixin for rounding with negative residual amount"
         pool = Pool()
         Account = pool.get('account.account')
         Tax = pool.get('account.tax')
         Configuration = pool.get('account.configuration')
         currency = create_currency('cur')
```

### Comparing `trytond_account-7.0.6/tests/tools.py` & `trytond_account-7.2.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/tox.ini` & `trytond_account-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/trial_balance.fodt` & `trytond_account-7.2.0/trial_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/tryton.cfg` & `trytond_account-7.2.0/tryton.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tryton]
-version=7.0.6
+version=7.2.0
 depends:
     company
     currency
     ir
     party
     res
 xml:
```

### Comparing `trytond_account-7.0.6/trytond_account.egg-info/PKG-INFO` & `trytond_account-7.2.0/trytond_account.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account
-Version: 7.0.6
+Version: 7.2.0
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-account/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -51,20 +51,20 @@
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-dateutil
 Requires-Dist: python-sql>=0.7
 Requires-Dist: simpleeval
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##############
 Account Module
 ##############
 
 The *Account Module* defines the fundamentals needed for basic double entry
 accounting.
```

### Comparing `trytond_account-7.0.6/trytond_account.egg-info/SOURCES.txt` & `trytond_account-7.2.0/trytond_account.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
 ./view/general_ledger_account_list.xml
 ./view/general_ledger_account_party_list.xml
 ./view/general_ledger_line_context_form.xml
 ./view/general_ledger_line_list.xml
 ./view/income_statement_context_form.xml
 ./view/journal_form.xml
 ./view/journal_list_cash.xml
+./view/journal_list_matching_sequence.xml
 ./view/journal_open_cash_context.xml
 ./view/journal_period_form.xml
 ./view/journal_period_list_close.xml
 ./view/journal_period_tree.xml
 ./view/journal_tree.xml
 ./view/move_cancel_default_form.xml
 ./view/move_form.xml
@@ -258,29 +259,29 @@
 doc/conf.py
 doc/configuration.rst
 doc/index.rst
 doc/reference.rst
 doc/releases.rst
 doc/requirements-doc.txt
 doc/setup.rst
-doc/design/account.rst
-doc/design/configuration.rst
-doc/design/fiscal-year.rst
+doc/design/account.inc.rst
+doc/design/configuration.inc.rst
+doc/design/fiscal-year.inc.rst
 doc/design/index.rst
-doc/design/journal.rst
-doc/design/move.rst
-doc/design/tax.rst
-doc/design/template.rst
-doc/usage/close.rst
-doc/usage/create.rst
+doc/design/journal.inc.rst
+doc/design/move.inc.rst
+doc/design/tax.inc.rst
+doc/design/template.inc.rst
+doc/usage/close.inc.rst
+doc/usage/create.inc.rst
 doc/usage/index.rst
-doc/usage/process.rst
-doc/usage/report.rst
-doc/usage/structure.rst
-doc/usage/view.rst
+doc/usage/process.inc.rst
+doc/usage/report.inc.rst
+doc/usage/structure.inc.rst
+doc/usage/view.inc.rst
 icons/LICENSE
 icons/tryton-account-block.svg
 icons/tryton-account-close.svg
 icons/tryton-account-open.svg
 icons/tryton-account.svg
 locale/bg.po
 locale/ca.po
@@ -373,14 +374,15 @@
 view/general_ledger_account_list.xml
 view/general_ledger_account_party_list.xml
 view/general_ledger_line_context_form.xml
 view/general_ledger_line_list.xml
 view/income_statement_context_form.xml
 view/journal_form.xml
 view/journal_list_cash.xml
+view/journal_list_matching_sequence.xml
 view/journal_open_cash_context.xml
 view/journal_period_form.xml
 view/journal_period_list_close.xml
 view/journal_period_tree.xml
 view/journal_tree.xml
 view/move_cancel_default_form.xml
 view/move_form.xml
```

### Comparing `trytond_account-7.0.6/type_statement.fodt` & `trytond_account-7.2.0/type_statement.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/account_deferral_form.xml` & `trytond_account-7.2.0/view/account_deferral_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/account_form.xml` & `trytond_account-7.2.0/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/account_template_form.xml` & `trytond_account-7.2.0/view/account_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/account_type_form.xml` & `trytond_account-7.2.0/view/account_type_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/account_type_template_form.xml` & `trytond_account-7.2.0/view/account_type_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/aged_balance_context_form.xml` & `trytond_account-7.2.0/view/aged_balance_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/company_form.xml` & `trytond_account-7.2.0/view/company_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/configuration_form.xml` & `trytond_account-7.2.0/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/fiscalyear_balance_non_deferral_start_form.xml` & `trytond_account-7.2.0/view/fiscalyear_balance_non_deferral_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/fiscalyear_create_periods_start_form.xml` & `trytond_account-7.2.0/view/fiscalyear_create_periods_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/fiscalyear_form.xml` & `trytond_account-7.2.0/view/fiscalyear_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/general_ledger_account_context_form.xml` & `trytond_account-7.2.0/view/income_statement_context_form.xml`

 * *Files 21% similar despite different names*

#### Comparing `trytond_account-7.0.6/view/general_ledger_account_context_form.xml` & `trytond_account-7.2.0/view/income_statement_context_form.xml`

```diff
@@ -13,10 +13,25 @@
   <label name="end_period"/>
   <field name="end_period"/>
   <newline/>
   <label name="from_date"/>
   <field name="from_date"/>
   <label name="to_date"/>
   <field name="to_date"/>
-  <label name="journal"/>
-  <field name="journal" widget="selection"/>
+  <newline/>
+  <label name="comparison"/>
+  <field name="comparison"/>
+  <newline/>
+  <separator id="comparison" colspan="6"/>
+  <label name="fiscalyear_cmp"/>
+  <field name="fiscalyear_cmp"/>
+  <newline/>
+  <label name="start_period_cmp"/>
+  <field name="start_period_cmp"/>
+  <label name="end_period_cmp"/>
+  <field name="end_period_cmp"/>
+  <newline/>
+  <label name="from_date_cmp"/>
+  <field name="from_date_cmp"/>
+  <label name="to_date_cmp"/>
+  <field name="to_date_cmp"/>
 </form>
```

### Comparing `trytond_account-7.0.6/view/general_ledger_line_list.xml` & `trytond_account-7.2.0/view/general_ledger_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/income_statement_context_form.xml` & `trytond_account-7.2.0/view/move_line_form.xml`

 * *Files 16% similar despite different names*

#### Comparing `trytond_account-7.0.6/view/income_statement_context_form.xml` & `trytond_account-7.2.0/view/move_line_form.xml`

```diff
@@ -1,37 +1,52 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<form col="6">
-  <label name="fiscalyear"/>
-  <field name="fiscalyear"/>
+<form>
   <label name="company"/>
   <field name="company"/>
-  <label name="posted"/>
-  <field name="posted"/>
-  <label name="start_period"/>
-  <field name="start_period"/>
-  <label name="end_period"/>
-  <field name="end_period"/>
+  <label name="period"/>
+  <field name="period"/>
+  <label name="journal"/>
+  <field name="journal" widget="selection"/>
+  <label name="move"/>
+  <field name="move"/>
+  <label name="account"/>
+  <field name="account"/>
   <newline/>
-  <label name="from_date"/>
-  <field name="from_date"/>
-  <label name="to_date"/>
-  <field name="to_date"/>
-  <newline/>
-  <label name="comparison"/>
-  <field name="comparison"/>
-  <newline/>
-  <separator id="comparison" colspan="6"/>
-  <label name="fiscalyear_cmp"/>
-  <field name="fiscalyear_cmp"/>
-  <newline/>
-  <label name="start_period_cmp"/>
-  <field name="start_period_cmp"/>
-  <label name="end_period_cmp"/>
-  <field name="end_period_cmp"/>
-  <newline/>
-  <label name="from_date_cmp"/>
-  <field name="from_date_cmp"/>
-  <label name="to_date_cmp"/>
-  <field name="to_date_cmp"/>
+  <label name="debit"/>
+  <field name="debit"/>
+  <label name="credit"/>
+  <field name="credit"/>
+  <label name="move_origin"/>
+  <field name="move_origin"/>
+  <label name="origin"/>
+  <field name="origin"/>
+  <label name="description_used"/>
+  <field name="description_used" colspan="3"/>
+  <notebook colspan="4">
+    <page string="Other Info" id="info">
+      <label name="date"/>
+      <field name="date"/>
+      <label name="maturity_date"/>
+      <field name="maturity_date"/>
+      <label name="party"/>
+      <field name="party"/>
+      <newline/>
+      <label name="reconciliation"/>
+      <field name="reconciliation"/>
+      <label name="delegated_amount"/>
+      <field name="delegated_amount" symbol="amount_currency"/>
+      <label name="amount_second_currency"/>
+      <field name="amount_second_currency"/>
+      <label name="second_currency"/>
+      <field name="second_currency"/>
+    </page>
+    <page name="tax_lines">
+      <field name="tax_lines" colspan="4"/>
+    </page>
+  </notebook>
+  <label name="move_state"/>
+  <field name="move_state"/>
+  <label name="state"/>
+  <field name="state"/>
 </form>
```

### Comparing `trytond_account-7.0.6/view/journal_form.xml` & `trytond_account-7.2.0/view/journal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/move_form.xml` & `trytond_account-7.2.0/view/move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/move_line_form_move.xml` & `trytond_account-7.2.0/view/move_line_form_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/move_line_list_payable_receivable.xml` & `trytond_account-7.2.0/view/move_line_list_payable_receivable.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/move_line_reschedule_start_form.xml` & `trytond_account-7.2.0/view/move_line_reschedule_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/move_line_template_form.xml` & `trytond_account-7.2.0/view/move_line_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/move_line_tree.xml` & `trytond_account-7.2.0/view/move_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/move_line_tree_move.xml` & `trytond_account-7.2.0/view/move_line_tree_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/move_template_form.xml` & `trytond_account-7.2.0/view/move_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/move_template_keyword_form.xml` & `trytond_account-7.2.0/view/move_template_keyword_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/move_tree.xml` & `trytond_account-7.2.0/view/move_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/party_form.xml` & `trytond_account-7.2.0/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/period_form.xml` & `trytond_account-7.2.0/view/period_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/reconcile_show_form.xml` & `trytond_account-7.2.0/view/reconcile_show_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/renew_fiscalyear_start_form.xml` & `trytond_account-7.2.0/view/renew_fiscalyear_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/tax_code_context_form.xml` & `trytond_account-7.2.0/view/tax_code_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/tax_code_form.xml` & `trytond_account-7.2.0/view/tax_code_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/tax_code_template_form.xml` & `trytond_account-7.2.0/view/tax_code_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/tax_form.xml` & `trytond_account-7.2.0/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/tax_rule_form.xml` & `trytond_account-7.2.0/view/tax_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/tax_rule_line_form.xml` & `trytond_account-7.2.0/view/tax_rule_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/tax_rule_line_template_form.xml` & `trytond_account-7.2.0/view/tax_rule_line_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/tax_template_form.xml` & `trytond_account-7.2.0/view/tax_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/tax_test_form.xml` & `trytond_account-7.2.0/view/tax_test_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.0.6/view/writeoff_form.xml` & `trytond_account-7.2.0/view/writeoff_form.xml`

 * *Files identical despite different names*

