# Comparing `tmp/cpop-35.0.7.tar.gz` & `tmp/cpop-35.2.0.tar.gz`

## Comparing `cpop-35.0.7.tar` & `cpop-35.2.0.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cpop-35.0.7/.coveragerc
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 cpop-35.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/Makefile
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/make.bat
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/outline.rst
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/conf.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/index.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/releases/32.rst
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/app_merging.rst
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/conf.rst
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/conf_integrate.rst
--rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/contracts.rst
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/dyne_name.rst
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/func_alias.rst
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/glossary.rst
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/hub_overview.rst
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/ideas_that_were_not_used.rst
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/learning.rst
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/pop.rst
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/pre_contract_returns.rst
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/story.rst
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/sub_patterns.rst
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/subs_overview.rst
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/virtual.rst
--rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/tutorial/quickstart.rst
--rw-r--r--   0        0        0     9926 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/data.pyx
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/dirs.pyx
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/exc.pyx
--rw-r--r--   0        0        0    28261 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/hub.pyx
--rw-r--r--   0        0        0    10445 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/loader.pyx
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/ref.pyx
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/scanner.pyx
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/verify.pyx
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/config.yaml
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/log/basic.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/log/init.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/log/timed_rolling.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/log/contracts/init.py
--rw-r--r--   0        0        0     9610 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/config.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/contract.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/sub.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/task.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/test.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/test.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/coro/contracts/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/__init__.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_bench.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_cli.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_config.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_coro.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_cpop.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_dyne.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_fail.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_hub.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_log.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_ref.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_relative.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_serial.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_sub.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_task.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/bad.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/dunder.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/falias_func.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/proc.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/vtrue.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/README.rst
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/unit/__init__.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-35.0.7/.gitignore
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 cpop-35.0.7/README.rst
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 cpop-35.0.7/pyproject.toml
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 cpop-35.0.7/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cpop-35.2.0/.coveragerc
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 cpop-35.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/Makefile
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/make.bat
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/outline.rst
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/releases/32.rst
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/app_merging.rst
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/conf.rst
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/conf_integrate.rst
+-rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/contracts.rst
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/dyne_name.rst
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/func_alias.rst
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/glossary.rst
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/hub_overview.rst
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/ideas_that_were_not_used.rst
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/learning.rst
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/pop.rst
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/pre_contract_returns.rst
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/story.rst
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/sub_patterns.rst
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/subs_overview.rst
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/topics/virtual.rst
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-35.2.0/docs/source/tutorial/quickstart.rst
+-rw-r--r--   0        0        0     9926 2020-02-02 00:00:00.000000 cpop-35.2.0/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 cpop-35.2.0/src/cpop/data.pyx
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 cpop-35.2.0/src/cpop/dirs.pyx
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-35.2.0/src/cpop/exc.pyx
+-rw-r--r--   0        0        0    28519 2020-02-02 00:00:00.000000 cpop-35.2.0/src/cpop/hub.pyx
+-rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 cpop-35.2.0/src/cpop/loader.pyx
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 cpop-35.2.0/src/cpop/ref.pyx
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.2.0/src/cpop/scanner.pyx
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-35.2.0/src/cpop/verify.pyx
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 cpop-35.2.0/src/pop/config.yaml
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 cpop-35.2.0/src/pop/log/basic.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 cpop-35.2.0/src/pop/log/init.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 cpop-35.2.0/src/pop/log/timed_rolling.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.2.0/src/pop/log/contracts/init.py
+-rw-r--r--   0        0        0     9610 2020-02-02 00:00:00.000000 cpop-35.2.0/src/pop/mods/config.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-35.2.0/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-35.2.0/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 cpop-35.2.0/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cpop-35.2.0/src/pop/mods/task.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cpop-35.2.0/src/pop/mods/test.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/contracts/test.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/__init__.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_cli.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_config.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_coro.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_cpop.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_dyne.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_fail.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_hub.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_log.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_ref.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_relative.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_sub.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/func/test_task.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/bad.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/dunder.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/falias_func.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/proc.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/vtrue.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/README.rst
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-35.2.0/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-35.2.0/.gitignore
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 cpop-35.2.0/README.rst
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 cpop-35.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 cpop-35.2.0/PKG-INFO
```

### Comparing `cpop-35.0.7/.pre-commit-config.yaml` & `cpop-35.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/Makefile` & `cpop-35.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/make.bat` & `cpop-35.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/outline.rst` & `cpop-35.2.0/docs/outline.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/conf.py` & `cpop-35.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/index.rst` & `cpop-35.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/app_merging.rst` & `cpop-35.2.0/docs/source/topics/app_merging.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/conf.rst` & `cpop-35.2.0/docs/source/topics/conf.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/conf_integrate.rst` & `cpop-35.2.0/docs/source/topics/conf_integrate.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/contracts.rst` & `cpop-35.2.0/docs/source/topics/contracts.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/dyne_name.rst` & `cpop-35.2.0/docs/source/topics/dyne_name.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/func_alias.rst` & `cpop-35.2.0/docs/source/topics/func_alias.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/glossary.rst` & `cpop-35.2.0/docs/source/topics/glossary.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/hub_overview.rst` & `cpop-35.2.0/docs/source/topics/hub_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/ideas_that_were_not_used.rst` & `cpop-35.2.0/docs/source/topics/ideas_that_were_not_used.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/learning.rst` & `cpop-35.2.0/docs/source/topics/learning.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/pop.rst` & `cpop-35.2.0/docs/source/topics/pop.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/pre_contract_returns.rst` & `cpop-35.2.0/docs/source/topics/pre_contract_returns.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/story.rst` & `cpop-35.2.0/docs/source/topics/story.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/sub_patterns.rst` & `cpop-35.2.0/docs/source/topics/sub_patterns.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/subs_overview.rst` & `cpop-35.2.0/docs/source/topics/subs_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/topics/virtual.rst` & `cpop-35.2.0/docs/source/topics/virtual.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/docs/source/tutorial/quickstart.rst` & `cpop-35.2.0/docs/source/tutorial/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/cpop/contract.pyx` & `cpop-35.2.0/src/cpop/contract.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/cpop/data.pyx` & `cpop-35.2.0/src/cpop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/cpop/dirs.pyx` & `cpop-35.2.0/src/cpop/dirs.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/cpop/exc.pyx` & `cpop-35.2.0/src/cpop/exc.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/cpop/hub.pyx` & `cpop-35.2.0/src/cpop/hub.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -135,26 +135,33 @@
         loop.add_signal_handler(signal.SIGINT, lambda s=signal.SIGINT: loop.create_task(sigint(s)))
         sigterm = self.pop.task.sigterm
         loop.add_signal_handler(signal.SIGTERM, lambda s=signal.SIGTERM: loop.create_task(sigterm(s)))
 
         self._load_all_dynes = self.__init_kwargs["load_all_dynes"]
         self._load_all_subdirs = self.__init_kwargs["load_all_subdirs"]
         self._recurse_subdirs = self.__init_kwargs["recurse_subdirs"]
-        if self._load_all_dynes:
-            await self._scan_dynamic()
-            await self._load_all()
+        await self._scan_dynamic()
+        await self.pop.sub.add(dyne_name="log")
+        await self._subs["log"]._load_all()
 
-            if self.__init_kwargs["load_config"]:
-                # Overwrite opt with config data
-                self._opt = await self.pop.config.load(cli=self.__init_kwargs["cli"], **self._dynamic.config)
+        # Set up config first
+        if self.__init_kwargs["load_config"]:
+            # Overwrite opt with config data
+            self._opt = await self.pop.config.load(cli=self.__init_kwargs["cli"], **self._dynamic.config)
 
         # Set up a logger
-        if "log" in self._subs and self.__init_kwargs["logs"]:
+        if self.__init_kwargs["logs"]:
+            await self.pop.sub.load_subdirs(self._subs["log"])
             await self.log.init.setup(**self._opt.log.copy())
 
+        # Load all other dynes
+        if self._load_all_dynes:
+            # Load dynes after config so they can use hub.OPT in their __init__s
+            await self._load_all()
+
         return self
 
     async def __aexit__(self, exc_type, exc_value, tb):
         if exc_type is not None and exc_value is not None:
             self._traceback(exc_type, exc_value, tb)
         await self._tasks.put(SHUTDOWN_SIGNAL)
```

### Comparing `cpop-35.0.7/src/cpop/loader.pyx` & `cpop-35.2.0/src/cpop/loader.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -124,27 +124,27 @@
         err = LoadError(f"Module {bname} returned virtual FALSE", verror=verror)
         # Return the load error with name as the base_name because another
         # module is still allowed to load under the same __virtualname__
         # but also return the vname information
         return {"name": base_name, "vname": name, "error": err}
 
 
-async def load_virtual(hub, mod: "LoadedMod" or LoadError, bname: str, ref:str) -> dict[str, Any]:
+async def load_virtual(hub, mod: "LoadedMod" or LoadError, bname: str, ref: str) -> dict[str, Any]:
     """
     Run the __virtual__ function to name the module and check for all loader errors
     :param hub: The redistributed pop central hub
     :param virtual: Toggle whether or not to process __virtual__ functions
     :param mod: A loader module or a LoadError if the module didn't load
     :param bname: The base name of the mod's path
     """
     return await _load_virtual(hub, mod, bname, "__virtual__", ref)
 
 
 async def load_sub_virtual(
-    hub, mod: "LoadedMod" or LoadError, bname: str, ref:str
+    hub, mod: "LoadedMod" or LoadError, bname: str, ref: str
 ) -> dict[str, Any]:
     """
     Run the __sub_virtual__ function to name the module and check for all loader errors
     :param hub: The redistributed pop central hub
     :param virtual: Toggle whether or not to process __virtual__ functions
     :param mod: A loader module or a LoadError if the module didn't load
     :param bname: The base name of the mod's path
```

### Comparing `cpop-35.0.7/src/cpop/ref.pyx` & `cpop-35.2.0/src/cpop/ref.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/cpop/scanner.pyx` & `cpop-35.2.0/src/cpop/scanner.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/cpop/verify.pyx` & `cpop-35.2.0/src/cpop/verify.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/pop/config.yaml` & `cpop-35.2.0/src/pop/config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/pop/log/basic.py` & `cpop-35.2.0/src/pop/log/basic.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/pop/log/init.py` & `cpop-35.2.0/src/pop/log/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/pop/log/timed_rolling.py` & `cpop-35.2.0/src/pop/log/timed_rolling.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/pop/mods/config.py` & `cpop-35.2.0/src/pop/mods/config.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/pop/mods/contract.py` & `cpop-35.2.0/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/pop/mods/sub.py` & `cpop-35.2.0/src/pop/mods/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/pop/mods/task.py` & `cpop-35.2.0/src/pop/mods/task.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/src/pop/mods/test.py` & `cpop-35.2.0/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/conftest.py` & `cpop-35.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/contracts/ctx.py` & `cpop-35.2.0/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/contracts/many.py` & `cpop-35.2.0/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/contracts/test.py` & `cpop-35.2.0/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/func/test_basic.py` & `cpop-35.2.0/tests/func/test_basic.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/func/test_config.py` & `cpop-35.2.0/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/func/test_contract_ctx.py` & `cpop-35.2.0/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/func/test_fail.py` & `cpop-35.2.0/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/func/test_log.py` & `cpop-35.2.0/tests/func/test_log.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/func/test_no_raise_on_pre_failure.py` & `cpop-35.2.0/tests/func/test_no_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/func/test_raise_on_pre_failure.py` & `cpop-35.2.0/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/func/test_ref.py` & `cpop-35.2.0/tests/func/test_ref.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/func/test_relative.py` & `cpop-35.2.0/tests/func/test_relative.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/func/test_serial.py` & `cpop-35.2.0/tests/func/test_serial.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-35.2.0/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-35.2.0/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-35.2.0/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-35.2.0/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-35.2.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-35.2.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-35.2.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-35.2.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-35.2.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-35.2.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/mods/proc.py` & `cpop-35.2.0/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/mods/test.py` & `cpop-35.2.0/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/regression/contract_masking/test_contract_masking.py` & `cpop-35.2.0/tests/regression/contract_masking/test_contract_masking.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-35.2.0/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/tpath/cn/contract/test.py` & `cpop-35.2.0/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/unit/test_contract.py` & `cpop-35.2.0/tests/unit/test_contract.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/tests/unit/test_sigs.py` & `cpop-35.2.0/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/.gitignore` & `cpop-35.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/README.rst` & `cpop-35.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.7/pyproject.toml` & `cpop-35.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython", "hatch-compile-yaml>=18.0.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "35.0.7"
+version = "35.2.0"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch45@gmail.com"},
 ]
 classifiers = [
```

### Comparing `cpop-35.0.7/PKG-INFO` & `cpop-35.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 35.0.7
+Version: 35.2.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch45@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

