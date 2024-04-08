# Comparing `tmp/cpop-32.0.1.tar.gz` & `tmp/cpop-32.0.2.tar.gz`

## Comparing `cpop-32.0.1.tar` & `cpop-32.0.2.tar`

### file list

```diff
@@ -1,177 +1,173 @@
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 cpop-32.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 cpop-32.0.1/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-32.0.1/src/cpop/data.pyx
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/config.yaml
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/dirs.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/exc.py
--rw-r--r--   0        0        0    24850 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/hub.py
--rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/loader.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/ref.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/scanner.py
--rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/verify.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/log/async.py
--rw-r--r--   0        0        0     7615 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/mods/config.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/mods/contract.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/mods/sub.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/mods/task.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-32.0.1/src/pop/mods/test.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/contracts/test.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/contracts/testing.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/coro/contracts/test.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/csigs/sigs.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/csigs/contracts/sigs.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/external_module/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/func/__init__.py
--rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/func/test_bench.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/func/test_cli.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/func/test_coro.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/func/test_fail.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/func/test_serial.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/func/test_sub.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/bad.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/falias_func.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/falias_wrap.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/proc.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/vtrue.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/alias_bad/init.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/alias_clash/init.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/README.rst
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/ca/config.yaml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/ca/contract_alias/init.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/config.yaml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/init.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/clash.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/dup1.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/dup2.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/float.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/init.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/invalid.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/neg.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/neg_last.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/pos.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/pos_first.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/pos_first_tie.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/unordered_1.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/unordered_2.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/verify_fail.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/verify_pass.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/verify_raise.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/contracts/zero.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/nest/init.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/recursive_contracts/clash.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/recursive_contracts/init.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_3.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_4.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/config/config.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/unit/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 cpop-32.0.1/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-32.0.1/.gitignore
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 cpop-32.0.1/README.rst
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cpop-32.0.1/pyproject.toml
--rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 cpop-32.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 cpop-32.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8448 2020-02-02 00:00:00.000000 cpop-32.0.2/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-32.0.2/src/cpop/data.pyx
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/config.yaml
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/dirs.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/exc.py
+-rw-r--r--   0        0        0    24935 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/hub.py
+-rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/loader.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/ref.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/scanner.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/verify.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/log/async.py
+-rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/config.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/task.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/test.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/test.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/testing.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/csigs/sigs.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/csigs/contracts/sigs.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/external_module/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/__init__.py
+-rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_cli.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_coro.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_cpop.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_fail.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_sub.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/bad.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/falias_func.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/proc.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/vtrue.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/README.rst
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/config.yaml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/init.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/clash.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/dup1.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/dup2.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/float.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/init.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/invalid.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/neg.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/neg_last.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/pos.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/pos_first.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/pos_first_tie.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/unordered_1.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/unordered_2.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/verify_fail.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/verify_pass.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/verify_raise.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/zero.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/nest/init.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/recursive_contracts/clash.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/recursive_contracts/init.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_3.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_4.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/config/config.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-32.0.2/.gitignore
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 cpop-32.0.2/README.rst
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cpop-32.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 cpop-32.0.2/PKG-INFO
```

### Comparing `cpop-32.0.1/.pre-commit-config.yaml` & `cpop-32.0.2/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 minimum_pre_commit_version: 2.10.1
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-merge-conflict
         description: Check for files that contain merge conflict strings.
         language_version: python3
       - id: trailing-whitespace
         description: Trims trailing whitespace.
         args: [--markdown-linebreak-ext=md]
@@ -53,19 +53,33 @@
 
   - repo: https://github.com/asottile/reorder_python_imports
     rev: v3.12.0
     hooks:
       - id: reorder-python-imports
         args: [--py310-plus]
 
-  - repo: https://github.com/psf/black
-    rev: 24.3.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.5
     hooks:
-      - id: black
-        args: []
+      - id: ruff-format
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
+        types_or: [python, pyi]
+        require_serial: true
+        exclude: |
+          (?x)^(
+            crates/ruff_linter/resources/.*|
+            crates/ruff_python_formatter/resources/.*
+          )$
+
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: v4.0.0-alpha.8
+    hooks:
+      - id: prettier
+        types: [yaml, toml]
 
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.16.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==24.3.0]
 
@@ -88,7 +102,14 @@
         files: .*\.py
         exclude: >
             (?x)^(
                 tests/.*
             )$
 
   # <---- Security ---------------------------------------------------------------------------------------------------
+  #
+  # ----- Release --------------------------------------------------------------------------------------------------->
+  - repo: https://github.com/abravalheri/validate-pyproject
+    rev: v0.16
+    hooks:
+      - id: validate-pyproject
+  # <---- Release ----------------------------------------------------------------------------------------------------
```

### Comparing `cpop-32.0.1/src/cpop/contract.pyx` & `cpop-32.0.2/src/cpop/contract.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             )
             # Apply any default values from the signature
             self.__cache["__bound_signature__"].apply_defaults()
         return self.__cache["__bound_signature__"].arguments
 
 
 def load_contract(
-    contracts: "pop.hub.Sub",
+    contracts,
     default_contracts: Iterable[str],
     mod: object,
     name: str,
 ) -> list[object]:
     """
     return a Contract object loaded up
     Dynamically create the correct Contracted type
@@ -242,15 +242,15 @@
         for fn in self.contract_functions["post"]:
             contract_context.ret = ret
             post_ret = await fn(contract_context)
             if post_ret is not None:
                 ret = post_ret
 
 def create_contracted(
-    hub: "pop.hub.Hub",
+    hub,
     contracts: list["pop.loader.LoadedMod"],
     func: functools.partial,
     ref: str,
     name: str,
     implicit_hub: bool = True,
 ) -> Contracted:
     """
```

### Comparing `cpop-32.0.1/src/cpop/data.pyx` & `cpop-32.0.2/src/cpop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/src/pop/config.yaml` & `cpop-32.0.2/src/pop/config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/src/pop/dirs.py` & `cpop-32.0.2/src/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/src/pop/exc.py` & `cpop-32.0.2/src/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/src/pop/hub.py` & `cpop-32.0.2/src/pop/hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
             self._attrs[key] = value
 
     def __setattr__(self, key: str, value):
         if key.startswith("_"):
             object.__setattr__(self, key, value)
         else:
             self[key] = value
+            self._clear()
 
 
 class Hub(PopMeta):
     """
     The redistributed pop central hub. All components of the system are
     rooted to the Hub.
     """
@@ -536,14 +537,17 @@
             return pop.ref.last(self._hub, item)
 
         try:
             return self[item]
         except KeyError:
             raise AttributeError(f"'{self._subname}' has no attribute '{item}'")
 
+    def __iter__(self):
+        return iter(self._loaded)
+
     async def _sub_init(self):
         """
         Run load init.py for the sub, running '__init__' function if present
         """
         await self._find_mod("init", match_only=True)
 
     def _process_load_error(
```

### Comparing `cpop-32.0.1/src/pop/loader.py` & `cpop-32.0.2/src/pop/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import types
 from collections.abc import Callable
 from typing import Any
 from typing import List
 
 import cpop.contract
 import cpop.data
-import pop.exc
 
 BASE_TYPES = (int, float, str, bytes, bool, type(None))
 
 
 class LoadError(Exception):
     """
     Errors from the loader are contained herein
@@ -84,15 +83,15 @@
     :param mod: A loader module or a LoadError if the module didn't load
     """
     base_name = os.path.basename(bname)
     return base_name, getattr(mod, "__virtualname__", base_name)
 
 
 async def _load_virtual(
-    hub: "pop.hub.Hub",
+    hub,
     mod: "LoadedMod" or LoadError,
     bname: str,
     vtype: str,
 ) -> dict[str, Any]:
     """
     Run the virtual function to name the module and check for all loader
     errors
@@ -131,44 +130,42 @@
         err = LoadError(f"Module {bname} returned virtual FALSE", verror=verror)
         # Return the load error with name as the base_name because another
         # module is still allowed to load under the same __virtualname__
         # but also return the vname information
         return {"name": base_name, "vname": name, "error": err}
 
 
-def load_virtual(
-    hub: "pop.hub.Hub", mod: "LoadedMod" or LoadError, bname: str
-) -> dict[str, Any]:
+def load_virtual(hub, mod: "LoadedMod" or LoadError, bname: str) -> dict[str, Any]:
     """
     Run the __virtual__ function to name the module and check for all loader errors
     :param hub: The redistributed pop central hub
     :param virtual: Toggle whether or not to process __virtual__ functions
     :param mod: A loader module or a LoadError if the module didn't load
     :param bname: The base name of the mod's path
     """
     return _load_virtual(hub, mod, bname, "__virtual__")
 
 
 async def load_sub_virtual(
-    hub: "pop.hub.Hub", mod: "LoadedMod" or LoadError, bname: str
+    hub, mod: "LoadedMod" or LoadError, bname: str
 ) -> dict[str, Any]:
     """
     Run the __sub_virtual__ function to name the module and check for all loader errors
     :param hub: The redistributed pop central hub
     :param virtual: Toggle whether or not to process __virtual__ functions
     :param mod: A loader module or a LoadError if the module didn't load
     :param bname: The base name of the mod's path
     """
     _, name = _base_name(bname, mod)
     if name != "init":
         return {"name": name}
     return await _load_virtual(hub, mod, bname, "__sub_virtual__")
 
 
-async def mod_init(sub: "pop.hub.Sub", mod: "LoadedMod", mod_name: str):
+async def mod_init(sub, mod: "LoadedMod", mod_name: str):
     """
     Process module's __init__ function if defined
     :param sub: The pop object that contains the loaded module data
     :param mod: A loader modul
     :param mod_name: The name of the module to get from the loader
     """
     if "__init__" in dir(mod):
@@ -178,29 +175,29 @@
             func=mod.__init__,
             ref=f"{sub._subname}.{mod_name}",
             name="__init__",
         )
         await init()
 
 
-def sub_alias(this_sub: "pop.hub.Sub", mod: "LoadedMod", mod_name: str):
+def sub_alias(this_sub, mod: "LoadedMod", mod_name: str):
     """
     Check the sub alias settings and apply the alias names locally so they can be gathered into the higher level object on the hub
     :param this_sub: The pop object that contains the loaded module data
     :param mod: A loader module
     :param mod_name: The name of the module to get from the loader
     """
     if mod_name == "init":
         alias = getattr(mod, "__sub_alias__", None)
         if alias:
             this_sub._alias = alias
 
 
 async def prep_loaded_mod(
-    this_sub: "pop.hub.Sub",
+    this_sub,
     mod: "LoadedMod",
     mod_name: str,
     contracts: "List[cpop.contract.Wrapper]",
     recursive_contracts: "List[cpop.contract.Wrapper]",
 ) -> "LoadedMod":
     """
     Read the attributes of a python module and create a LoadedMod, which resolves
```

### Comparing `cpop-32.0.1/src/pop/scanner.py` & `cpop-32.0.2/src/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/src/pop/verify.py` & `cpop-32.0.2/src/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/src/pop/log/async.py` & `cpop-32.0.2/src/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/src/pop/mods/contract.py` & `cpop-32.0.2/src/pop/mods/contract.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from collections.abc import Callable
 
 import pop.exc
 
 
 async def process_pre_result(
-    hub, pre_ret, pre: Callable, cn: "cpop.contract.Contracted"
+    hub,
+    pre_ret,
+    pre: Callable,
+    cn,
 ):
     if pre_ret is None:
         return
 
     if isinstance(pre_ret, bool):
         status = pre_ret
         msg = None
```

### Comparing `cpop-32.0.1/src/pop/mods/sub.py` & `cpop-32.0.2/src/pop/mods/sub.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Control and add subsystems to the running daemon hub
 """
 
 import pop.hub
 
 
 async def add(
-    hub: "pop.hub.Hub",
+    hub,
     dyne_name: str = None,
     *,
     pypath: list[str] = None,
     subname: str = None,
-    sub: "pop.hub.Sub" = None,
+    sub=None,
     static: list[str] = None,
     contracts_pypath: list[str] = None,
     contracts_static: list[str] = None,
     default_contracts: list[str] = None,
     virtual: bool = True,
     omit_start: tuple[str] = ("_",),
     omit_end: tuple[str] = (),
@@ -101,24 +101,24 @@
     # init the sub (init.py:__init__) after it can be referenced on the hub!
     await root._subs[subname]._sub_init()
     await root._subs[subname]._load_all()
     for alias in root._subs[subname]._alias:
         root._sub_alias[alias] = root._subs[subname]
 
 
-async def get_dirs(hub: "pop.hub.Hub", sub: "pop.hub.Sub") -> list[str]:
+async def get_dirs(hub, sub) -> list[str]:
     """
     Return a list of directories that contain the modules for this subname
     :param hub: The redistributed pop central hub
     :param sub: The pop object that contains the loaded module data
     """
     return sub._dirs
 
 
-async def load_subdirs(hub: "pop.hub.Hub", sub: "pop.hub.Sub", recurse: bool = False):
+async def load_subdirs(hub, sub, recurse: bool = False):
     """
     Given a sub, load all subdirectories found under the sub into a lower namespace
     :param hub: The redistributed pop central hub
     :param sub: The pop object that contains the loaded module data
     :param recurse: Recursively iterate over nested subs
     """
     if not sub._sub_virtual:
@@ -158,15 +158,15 @@
             stop_on_failures=sub._stop_on_failures,
         )
         if recurse:
             if isinstance(getattr(sub, name), pop.hub.Sub):
                 await hub.pop.sub.load_subdirs(getattr(sub, name), recurse)
 
 
-async def reload(hub: "pop.hub.Hub", subname: str):
+async def reload(hub, subname: str):
     """
     Instruct the hub to reload the modules for the given sub. This does not call
     the init.new function or remove sub level variables. But it does re-read the
     directory list and re-initialize the loader causing all modules to be re-evaluated
     when started.
     :param hub: The redistributed pop central hub
     :param subname: The name that the sub is going to take on the hub
```

### Comparing `cpop-32.0.1/src/pop/mods/task.py` & `cpop-32.0.2/src/pop/mods/task.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/src/pop/mods/test.py` & `cpop-32.0.2/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/conftest.py` & `cpop-32.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/contracts/ctx.py` & `cpop-32.0.2/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/contracts/many.py` & `cpop-32.0.2/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/contracts/test.py` & `cpop-32.0.2/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/func/test_basic.py` & `cpop-32.0.2/tests/func/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,54 +68,54 @@
     with pytest.raises(Exception):
         await hub.mods.test.module_level_non_aliased_ping_call()
     assert await hub.mods.test.module_level_non_aliased_ping_call_fw_hub() == {}
 
 
 async def test_contract(hub):
     await hub.pop.sub.add(pypath=["tests.mods"], contracts_pypath=["tests.contracts"])
-    with pytest.raises(Exception) as context:
+    with pytest.raises(Exception):
         await hub.mods.test.ping(4)
 
 
 async def test_inline_contract(hub):
     await hub.pop.sub.add(pypath=["tests.cmods"])
     assert await hub.cmods.ctest.cping()
     assert hub.CPING
 
 
 async def test_no_contract(hub):
     await hub.pop.sub.add(pypath=["tests.mods"])
-    with pytest.raises(TypeError) as context:
+    with pytest.raises(TypeError):
         await hub.mods.test.ping(4)
 
 
 async def test_contract_manipulate(hub):
     await hub.pop.sub.add(pypath=["tests.mods"], contracts_pypath=["tests.contracts"])
     assert "override" in await hub.mods.all.list()
     assert "post called" in await hub.mods.all.list()
     assert "post" in await hub.mods.all.dict()
 
 
 async def test_private_function_cross_access(hub):
     hub.opts = "OPTS!"
     await hub.pop.sub.add(pypath=["tests.mods"])
     # Let's make sure that the private function is not accessible through the sub
-    with pytest.raises(AttributeError) as exc:
+    with pytest.raises(AttributeError):
         await hub.mods.priv._private() == "OPTS!"
 
     # Let's confirm that the private function has access to the cross
     # objects
     assert await hub.mods.priv.public() == "OPTS!"
 
 
 async def test_private_function_cross_access_with_contracts(hub):
     hub.opts = "OPTS!"
     await hub.pop.sub.add(pypath=["tests.mods"], contracts_pypath=["tests.contracts"])
     # Let's make sure that the private function is not accessible through the sub
-    with pytest.raises(AttributeError) as exc:
+    with pytest.raises(AttributeError):
         await hub.mods.priv._private() == "OPTS!"
 
     # Let's confirm that the private function has access to the cross objects
     assert await hub.mods.priv.public() == "OPTS!"
 
 
 async def test_cross_in_virtual(hub):
```

### Comparing `cpop-32.0.1/tests/func/test_contract_ctx.py` & `cpop-32.0.2/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/func/test_fail.py` & `cpop-32.0.2/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/func/test_no_raise_on_pre_failure.py` & `cpop-32.0.2/tests/func/test_no_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/func/test_raise_on_pre_failure.py` & `cpop-32.0.2/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/mods/proc.py` & `cpop-32.0.2/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/mods/test.py` & `cpop-32.0.2/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/regression/contract_masking/test_contract_masking.py` & `cpop-32.0.2/tests/regression/contract_masking/test_contract_masking.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-32.0.2/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/tpath/cn/contract/test.py` & `cpop-32.0.2/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/tpath/co1/contract_ordering/init.py` & `cpop-32.0.2/tests/tpath/co1/contract_ordering/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/tpath/co1/contract_ordering/nest/init.py` & `cpop-32.0.2/tests/tpath/co1/contract_ordering/nest/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/unit/test_contract.py` & `cpop-32.0.2/tests/unit/test_contract.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/tests/unit/test_sigs.py` & `cpop-32.0.2/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/.gitignore` & `cpop-32.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/README.rst` & `cpop-32.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-32.0.1/pyproject.toml` & `cpop-32.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "32.0.1"
+version = "32.0.2"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch45@gmail.com"},
 ]
 classifiers = [
```

### Comparing `cpop-32.0.1/PKG-INFO` & `cpop-32.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 32.0.1
+Version: 32.0.2
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch45@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

