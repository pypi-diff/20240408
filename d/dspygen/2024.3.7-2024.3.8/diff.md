# Comparing `tmp/dspygen-2024.3.7.tar.gz` & `tmp/dspygen-2024.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspygen-2024.3.7.tar", max compression
+gzip compressed data, was "dspygen-2024.3.8.tar", max compression
```

## Comparing `dspygen-2024.3.7.tar` & `dspygen-2024.3.8.tar`

### file list

```diff
@@ -1,268 +1,506 @@
--rw-r--r--   0        0        0     1069 2024-02-26 01:14:54.588858 dspygen-2024.3.7/LICENSE
--rw-r--r--   0        0        0     7783 2024-02-26 22:30:04.933363 dspygen-2024.3.7/README.md
--rw-r--r--   0        0        0     6226 2024-03-08 06:24:44.375139 dspygen-2024.3.7/pyproject.toml
--rw-r--r--   0        0        0       69 2024-03-04 21:23:01.363615 dspygen-2024.3.7/src/dspygen/__init__.py
--rw-r--r--   0        0        0     1603 2024-03-07 04:57:22.032093 dspygen-2024.3.7/src/dspygen/api.py
--rw-r--r--   0        0        0     1337 2024-03-08 05:40:46.024228 dspygen-2024.3.7/src/dspygen/app.py
--rw-r--r--   0        0        0      731 2024-01-23 20:40:53.415200 dspygen-2024.3.7/src/dspygen/async_typer.py
--rw-r--r--   0        0        0     2864 2024-03-03 01:53:34.056414 dspygen-2024.3.7/src/dspygen/cli.py
--rw-r--r--   0        0        0       15 2024-03-02 21:25:45.285222 dspygen-2024.3.7/src/dspygen/experiments/.git/COMMIT_EDITMSG
--rw-r--r--   0        0        0       21 2024-03-02 21:00:22.720738 dspygen-2024.3.7/src/dspygen/experiments/.git/HEAD
--rw-r--r--   0        0        0      137 2024-03-02 21:25:45.250428 dspygen-2024.3.7/src/dspygen/experiments/.git/config
--rw-r--r--   0        0        0       73 2024-03-02 21:00:22.717125 dspygen-2024.3.7/src/dspygen/experiments/.git/description
--rwxr-xr-x   0        0        0      478 2024-03-02 21:00:22.718166 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      896 2024-03-02 21:00:22.717490 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     4726 2024-03-02 21:00:22.718352 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      189 2024-03-02 21:00:22.718737 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      424 2024-03-02 21:00:22.719040 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1643 2024-03-02 21:00:22.717992 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      416 2024-03-02 21:00:22.718849 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1374 2024-03-02 21:00:22.719230 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4898 2024-03-02 21:00:22.717841 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      544 2024-03-02 21:00:22.718519 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1492 2024-03-02 21:00:22.718625 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     2783 2024-03-02 21:00:22.719590 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0        0        0     3650 2024-03-02 21:00:22.719479 dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/update.sample
--rw-r--r--   0        0        0     3266 2024-03-07 22:45:58.426674 dspygen-2024.3.7/src/dspygen/experiments/.git/index
--rw-r--r--   0        0        0      240 2024-03-02 21:00:22.716869 dspygen-2024.3.7/src/dspygen/experiments/.git/info/exclude
--rw-r--r--   0        0        0      384 2024-03-02 21:25:45.286091 dspygen-2024.3.7/src/dspygen/experiments/.git/logs/HEAD
--rw-r--r--   0        0        0      384 2024-03-02 21:25:45.286375 dspygen-2024.3.7/src/dspygen/experiments/.git/logs/refs/heads/main
--rw-r--r--   0        0        0      906 2024-03-02 21:00:22.755656 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/07/2c395e5a1a2fda1ebd81855a0857a4c349aba9
--rw-r--r--   0        0        0      226 2024-03-02 21:00:22.757663 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/17/97b95f720b5217b695bcff22867a50394f3abf
--rw-r--r--   0        0        0      146 2024-03-02 21:00:22.753226 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/19/06d15bba64a214e6d9aaec6efdefe2c13c7707
--rw-r--r--   0        0        0     1224 2024-03-06 19:01:54.514198 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/1e/d7c76971abff4a041741b96643e4bbe493bd3f
--rw-r--r--   0        0        0      667 2024-03-02 21:00:22.762303 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/29/790e08d481fbcf9876f5e09e8618e0c6ff2cf4
--rw-r--r--   0        0        0      403 2024-03-02 21:00:22.758262 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/2d/dc2e65f3a5975fdf305094330840323c7eb654
--rw-r--r--   0        0        0     5058 2024-03-02 21:00:22.759386 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/34/484ad0f39e38772282a9bb02ba1df4f056b1f7
--rw-r--r--   0        0        0   356425 2024-03-02 21:00:22.751592 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/38/a98b391b7a6e8e740cae9681b5f0b295848fcc
--rw-r--r--   0        0        0      769 2024-03-02 21:00:22.758754 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/46/ed8e6d6b3d12b5bf9028d0777450412497d2aa
--rw-r--r--   0        0        0      186 2024-03-02 21:25:45.285483 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/51/e517c46227aca5ee9bb188a8f11bf1717a750e
--rw-r--r--   0        0        0      762 2024-03-02 21:25:45.283882 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/63/e5b4dd95ed8214e4f3167d66b2b139f49b0b04
--rw-r--r--   0        0        0      370 2024-03-02 21:00:22.765847 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/7b/782ba56f06f203507ed84702ce312d9e919910
--rw-r--r--   0        0        0      339 2024-03-02 21:00:22.761060 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/7c/100c125c4d4a859f02f595e05d04a437c5346d
--rw-r--r--   0        0        0      774 2024-03-02 21:25:45.266809 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/85/97acd78f726e8277a086b8a78d6d77c82f4d2c
--rw-r--r--   0        0        0      287 2024-03-02 21:00:22.764712 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/89/3f12d07852de09f2b88bcfc52a72c93110f555
--rw-r--r--   0        0        0      665 2024-03-02 21:00:22.763518 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/89/80972d4e4fe721d9a4b66d38500a387cd5d677
--rw-r--r--   0        0        0      386 2024-03-02 21:00:22.765280 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/8d/f078cc0e6ae05bd48848561f58b756b9b361d7
--rw-r--r--   0        0        0      821 2024-03-02 21:00:22.764181 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/90/838848601a0b18aafe0f31edb678a2f801f0f2
--rw-r--r--   0        0        0     1383 2024-03-07 21:20:22.717611 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/97/8bd6af4ad3a34e4016af33f921e416a723518a
--rw-r--r--   0        0        0     2669 2024-03-02 21:00:22.754966 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/9f/3b783e2f90a73bacc366d57205db068a1f130a
--rw-r--r--   0        0        0      763 2024-03-02 21:00:22.783125 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/a4/f3e1b596347a141fde89a09e19348524331fb1
--rw-r--r--   0        0        0     3489 2024-03-06 18:47:12.342771 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/a5/1355a31ec94b448a81fe23cd03407e6db9fb98
--rw-r--r--   0        0        0     1637 2024-03-02 21:00:22.754428 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/a7/f8004ca3e4019a0813e6d37454a9a1d4633732
--rw-r--r--   0        0        0     2844 2024-03-02 21:00:22.760013 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/ae/864cd37388df8a496b2e62caa5bdb338e22de8
--rw-r--r--   0        0        0     2170 2024-03-06 18:48:21.155474 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/af/54a3d8766d0686126ba2e2b3206b8270f1d5ef
--rw-r--r--   0        0        0      732 2024-03-02 21:00:22.762698 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/b9/0e196ece0bb3c298e1565c9e5ba065ae468d74
--rw-r--r--   0        0        0      907 2024-03-02 21:00:22.760483 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/bd/3ea467b227c44e9d5a1d687beef7d6d5f02f4d
--rw-r--r--   0        0        0      153 2024-03-02 21:00:22.784474 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/be/806c8525a46028aaa93e635fad9345cfb9340b
--rw-r--r--   0        0        0      215 2024-03-02 21:00:22.757066 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/c8/9b3c36bb5eabe165112fa224ec94f3b6c12600
--rw-r--r--   0        0        0      826 2024-03-02 21:25:45.266351 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/d2/5ac35cbee6a13431d6769e22c0eac72f5ed551
--rw-r--r--   0        0        0      599 2024-03-02 21:00:22.761581 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/d2/a1225cf1aa018c446ce1274a87eecb37294e03
--rw-r--r--   0        0        0      808 2024-03-02 21:00:22.753950 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/da/938270af8aa8e1b6655c68dc10042c01526cf7
--rw-r--r--   0        0        0       15 2024-03-07 22:45:58.426354 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
--rw-r--r--   0        0        0      180 2024-03-02 21:00:22.782558 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/f8/818c037929cf14c8091a9f065221faffbc15ff
--rw-r--r--   0        0        0      818 2024-03-02 21:00:22.756366 dspygen-2024.3.7/src/dspygen/experiments/.git/objects/fc/d9f4d1c396f872cc2f80e1599b961223430558
--rw-r--r--   0        0        0       41 2024-03-02 21:25:45.286042 dspygen-2024.3.7/src/dspygen/experiments/.git/refs/heads/main
--rw-r--r--   0        0        0   884736 2015-11-29 18:53:02.000000 dspygen-2024.3.7/src/dspygen/experiments/Chinook.db
--rw-r--r--   0        0        0        0 2024-02-27 17:34:57.501846 dspygen-2024.3.7/src/dspygen/experiments/__init__.py
--rw-r--r--   0        0        0      688 2024-03-06 19:17:00.425738 dspygen-2024.3.7/src/dspygen/experiments/abstract_aggregate/book_aggregate.py
--rw-r--r--   0        0        0      707 2024-03-06 19:17:00.418608 dspygen-2024.3.7/src/dspygen/experiments/abstract_aggregate/customer_aggregate.py
--rw-r--r--   0        0        0      682 2024-03-06 19:24:21.457585 dspygen-2024.3.7/src/dspygen/experiments/abstract_aggregate/main_aggregate.py
--rw-r--r--   0        0        0      697 2024-03-06 21:32:39.344335 dspygen-2024.3.7/src/dspygen/experiments/abstract_aggregate/order_aggregate.py
--rw-r--r--   0        0        0      175 2024-03-06 19:09:39.831299 dspygen-2024.3.7/src/dspygen/experiments/abstract_command/place_order.py
--rw-r--r--   0        0        0      183 2024-03-06 19:09:39.833600 dspygen-2024.3.7/src/dspygen/experiments/abstract_command/process_payment.py
--rw-r--r--   0        0        0      185 2024-03-06 19:09:39.837291 dspygen-2024.3.7/src/dspygen/experiments/abstract_command/update_inventory.py
--rw-r--r--   0        0        0      187 2024-03-06 19:09:39.881361 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/add_to_cart_button_click.py
--rw-r--r--   0        0        0      189 2024-03-06 19:09:39.884401 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/checkout_form_submitted.py
--rw-r--r--   0        0        0      201 2024-03-06 19:09:39.823046 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/external_payment_confirmation.py
--rw-r--r--   0        0        0      179 2024-03-06 19:09:39.820392 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/inventory_updated.py
--rw-r--r--   0        0        0      211 2024-03-06 19:09:39.903958 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/inventory_updated_integration_event.py
--rw-r--r--   0        0        0      191 2024-03-06 19:09:39.887942 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/order_history_page_loaded.py
--rw-r--r--   0        0        0      169 2024-03-06 19:09:39.815378 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/order_placed.py
--rw-r--r--   0        0        0      201 2024-03-06 19:09:39.898836 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/order_placed_integration_event.py
--rw-r--r--   0        0        0      179 2024-03-06 19:09:39.818037 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/payment_processed.py
--rw-r--r--   0        0        0      211 2024-03-06 19:09:39.901443 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/payment_processed_integration_event.py
--rw-r--r--   0        0        0      205 2024-03-06 19:09:39.828834 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/supplier_inventory_confirmation.py
--rw-r--r--   0        0        0      193 2024-03-06 19:09:39.825550 dspygen-2024.3.7/src/dspygen/experiments/abstract_event/supplier_inventory_update.py
--rw-r--r--   0        0        0      197 2024-03-06 19:09:39.855090 dspygen-2024.3.7/src/dspygen/experiments/abstract_policy/order_cancellation_policy.py
--rw-r--r--   0        0        0      175 2024-03-06 19:09:39.857988 dspygen-2024.3.7/src/dspygen/experiments/abstract_policy/refund_policy.py
--rw-r--r--   0        0        0      179 2024-03-06 19:09:39.861037 dspygen-2024.3.7/src/dspygen/experiments/abstract_policy/shipping_policy.py
--rw-r--r--   0        0        0      179 2024-03-06 19:09:39.844447 dspygen-2024.3.7/src/dspygen/experiments/abstract_query/check_order_status.py
--rw-r--r--   0        0        0      177 2024-03-06 19:09:39.839750 dspygen-2024.3.7/src/dspygen/experiments/abstract_query/get_order_details.py
--rw-r--r--   0        0        0      165 2024-03-06 19:09:39.842037 dspygen-2024.3.7/src/dspygen/experiments/abstract_query/list_books.py
--rw-r--r--   0        0        0      204 2024-03-06 19:09:39.866481 dspygen-2024.3.7/src/dspygen/experiments/abstract_read_model/book_catalog_read_model.py
--rw-r--r--   0        0        0      222 2024-03-06 19:09:39.870395 dspygen-2024.3.7/src/dspygen/experiments/abstract_read_model/customer_order_history_read_model.py
--rw-r--r--   0        0        0      206 2024-03-06 19:09:39.863536 dspygen-2024.3.7/src/dspygen/experiments/abstract_read_model/order_summary_read_model.py
--rw-r--r--   0        0        0     3698 2024-03-06 19:09:38.592650 dspygen-2024.3.7/src/dspygen/experiments/abstract_renderer.py
--rw-r--r--   0        0        0      173 2024-03-06 19:09:39.895864 dspygen-2024.3.7/src/dspygen/experiments/abstract_saga/book_restock_saga.py
--rw-r--r--   0        0        0      183 2024-03-06 19:09:39.890463 dspygen-2024.3.7/src/dspygen/experiments/abstract_saga/order_fulfillment_saga.py
--rw-r--r--   0        0        0      185 2024-03-06 19:09:39.893365 dspygen-2024.3.7/src/dspygen/experiments/abstract_saga/payment_processing_saga.py
--rw-r--r--   0        0        0      187 2024-03-06 19:09:39.927327 dspygen-2024.3.7/src/dspygen/experiments/abstract_task/calculate_shipping_costs.py
--rw-r--r--   0        0        0      195 2024-03-06 19:09:39.929712 dspygen-2024.3.7/src/dspygen/experiments/abstract_task/send_order_confirmation_email.py
--rw-r--r--   0        0        0      169 2024-03-06 19:09:39.922320 dspygen-2024.3.7/src/dspygen/experiments/abstract_task/validate_order.py
--rw-r--r--   0        0        0      186 2024-03-06 19:09:39.914224 dspygen-2024.3.7/src/dspygen/experiments/abstract_value_object/address.py
--rw-r--r--   0        0        0      182 2024-03-06 19:09:39.917133 dspygen-2024.3.7/src/dspygen/experiments/abstract_value_object/price.py
--rw-r--r--   0        0        0      188 2024-03-06 19:09:39.919947 dspygen-2024.3.7/src/dspygen/experiments/abstract_value_object/quantity.py
--rw-r--r--   0        0        0      167 2024-03-06 19:09:39.876298 dspygen-2024.3.7/src/dspygen/experiments/abstract_view/book_list_view.py
--rw-r--r--   0        0        0      181 2024-03-06 19:09:39.879021 dspygen-2024.3.7/src/dspygen/experiments/abstract_view/customer_profile_view.py
--rw-r--r--   0        0        0      175 2024-03-06 19:09:39.872904 dspygen-2024.3.7/src/dspygen/experiments/abstract_view/order_details_view.py
--rw-r--r--   0        0        0      283 2024-03-06 18:26:07.637250 dspygen-2024.3.7/src/dspygen/experiments/advanced_jinja.py
--rw-r--r--   0        0        0      331 2024-03-02 00:57:36.655430 dspygen-2024.3.7/src/dspygen/experiments/chatbots.py
--rw-r--r--   0        0        0      361 2024-02-29 23:34:11.662934 dspygen-2024.3.7/src/dspygen/experiments/code_generator_agent.py
--rw-r--r--   0        0        0      201 2024-03-06 19:09:39.911894 dspygen-2024.3.7/src/dspygen/experiments/domain_exception/book_out_of_stock_exception.py
--rw-r--r--   0        0        0      199 2024-03-06 19:09:39.906870 dspygen-2024.3.7/src/dspygen/experiments/domain_exception/order_not_found_exception.py
--rw-r--r--   0        0        0      203 2024-03-06 19:09:39.909144 dspygen-2024.3.7/src/dspygen/experiments/domain_exception/payment_declined_exception.py
--rw-r--r--   0        0        0      260 2024-03-06 21:06:23.944492 dspygen-2024.3.7/src/dspygen/experiments/file_path.py
--rw-r--r--   0        0        0     1145 2024-02-27 21:48:22.789420 dspygen-2024.3.7/src/dspygen/experiments/function_call.py
--rw-r--r--   0        0        0     1901 2024-03-02 20:42:29.716558 dspygen-2024.3.7/src/dspygen/experiments/gen_module.py
--rw-r--r--   0        0        0    14780 2024-03-08 05:42:36.717781 dspygen-2024.3.7/src/dspygen/experiments/gen_pydantic_class.py
--rw-r--r--   0        0        0     9304 2024-03-07 21:39:00.552977 dspygen-2024.3.7/src/dspygen/experiments/gen_pydantic_instance.py
--rw-r--r--   0        0        0     2845 2024-03-02 20:51:53.328377 dspygen-2024.3.7/src/dspygen/experiments/gen_python_primitive.py
--rw-r--r--   0        0        0     6076 2024-03-06 18:55:42.509529 dspygen-2024.3.7/src/dspygen/experiments/gherkin_parser.py
--rw-r--r--   0        0        0     3560 2024-03-07 21:15:06.538371 dspygen-2024.3.7/src/dspygen/experiments/lm_call.py
--rw-r--r--   0        0        0    11258 2024-03-06 18:55:42.474464 dspygen-2024.3.7/src/dspygen/experiments/models/dsl_project.py
--rw-r--r--   0        0        0     1061 2024-02-28 21:51:36.079683 dspygen-2024.3.7/src/dspygen/experiments/openai_ror_cli.py
--rw-r--r--   0        0        0     1753 2024-03-01 22:03:13.771206 dspygen-2024.3.7/src/dspygen/experiments/python_to_elixir.py
--rw-r--r--   0        0        0     1978 2024-03-03 02:15:32.888098 dspygen-2024.3.7/src/dspygen/experiments/ror_bot.py
--rw-r--r--   0        0        0     7582 2024-03-07 23:15:34.216913 dspygen-2024.3.7/src/dspygen/experiments/self_evolving_business_logic.py
--rw-r--r--   0        0        0     1625 2024-03-08 05:43:24.578568 dspygen-2024.3.7/src/dspygen/experiments/socket_actor_system.py
--rw-r--r--   0        0        0        0 2024-02-27 17:34:57.501846 dspygen-2024.3.7/src/dspygen/experiments/spider/__init__.py
--rw-r--r--   0        0        0     2447 2024-03-05 23:28:08.427730 dspygen-2024.3.7/src/dspygen/experiments/spider/wiki_spider.py
--rw-r--r--   0        0        0     1241 2024-03-07 05:20:40.254419 dspygen-2024.3.7/src/dspygen/experiments/sql_calling_asserts.py
--rw-r--r--   0        0        0     1793 2024-03-07 21:22:34.035184 dspygen-2024.3.7/src/dspygen/experiments/sql_optimization_function.py
--rw-r--r--   0        0        0     1278 2024-02-28 21:57:26.969572 dspygen-2024.3.7/src/dspygen/experiments/test_openai_ror_cli.py
--rw-r--r--   0        0        0      898 2024-02-27 22:00:22.608255 dspygen-2024.3.7/src/dspygen/experiments/weather_function_calling_asserts.py
--rw-r--r--   0        0        0     1029 2024-03-01 22:03:15.367794 dspygen-2024.3.7/src/dspygen/experiments/weather_functions.exs
--rw-r--r--   0        0        0     2339 2024-03-07 23:05:19.914256 dspygen-2024.3.7/src/dspygen/experiments/workflow_engine.py
--rw-r--r--   0        0        0       23 2024-02-26 00:06:54.236649 dspygen-2024.3.7/src/dspygen/lm/__init__.py
--rw-r--r--   0        0        0     1313 2024-03-01 17:38:38.956893 dspygen-2024.3.7/src/dspygen/lm/groq_lm.py
--rw-r--r--   0        0        0     1367 2024-03-07 23:35:14.800514 dspygen-2024.3.7/src/dspygen/models/BPMN.yaml
--rw-r--r--   0        0        0     1316 2024-03-07 23:39:50.809151 dspygen-2024.3.7/src/dspygen/models/CMMN.yaml
--rw-r--r--   0        0        0        0 2024-03-07 23:26:46.354560 dspygen-2024.3.7/src/dspygen/models/__init__.py
--rw-r--r--   0        0        0     2936 2024-03-07 23:43:49.167525 dspygen-2024.3.7/src/dspygen/models/bpm_plus_domain_models.py
--rw-r--r--   0        0        0     1569 2024-03-07 23:28:31.491007 dspygen-2024.3.7/src/dspygen/models/cmmn_shipping.yaml
--rw-r--r--   0        0        0      940 2024-03-07 23:29:59.479279 dspygen-2024.3.7/src/dspygen/models/dmn_shipping.yaml
--rw-r--r--   0        0        0       70 2024-02-28 21:24:01.342202 dspygen-2024.3.7/src/dspygen/module_docstring_writer.py
--rw-r--r--   0        0        0        0 2024-02-26 00:35:40.975772 dspygen-2024.3.7/src/dspygen/modules/__init__.py
--rw-r--r--   0        0        0     1359 2024-03-06 21:47:41.881978 dspygen-2024.3.7/src/dspygen/modules/binary_output.py
--rw-r--r--   0        0        0     1678 2024-03-07 05:28:21.941387 dspygen-2024.3.7/src/dspygen/modules/blog_module.py
--rw-r--r--   0        0        0     2078 2024-02-28 02:14:40.119886 dspygen-2024.3.7/src/dspygen/modules/book_appointment_module.py
--rw-r--r--   0        0        0     1109 2024-03-05 21:40:49.308631 dspygen-2024.3.7/src/dspygen/modules/business_dev_consultant.py
--rw-r--r--   0        0        0     2429 2024-03-06 21:51:35.362215 dspygen-2024.3.7/src/dspygen/modules/business_requirements.py
--rw-r--r--   0        0        0     1151 2024-02-29 22:57:56.314686 dspygen-2024.3.7/src/dspygen/modules/chat_bot_cli.py
--rw-r--r--   0        0        0     1920 2024-03-06 20:27:27.830710 dspygen-2024.3.7/src/dspygen/modules/chat_bot_module.py
--rw-r--r--   0        0        0     1058 2024-03-02 20:39:42.067411 dspygen-2024.3.7/src/dspygen/modules/checker_module.py
--rw-r--r--   0        0        0     4365 2024-03-02 20:12:27.806120 dspygen-2024.3.7/src/dspygen/modules/choose_function_module.py
--rw-r--r--   0        0        0      931 2024-03-02 20:37:43.109995 dspygen-2024.3.7/src/dspygen/modules/cli_bot.py
--rw-r--r--   0        0        0     1233 2024-03-06 21:36:42.927682 dspygen-2024.3.7/src/dspygen/modules/cobol_to_python.py
--rw-r--r--   0        0        0     1185 2024-02-28 23:11:15.274057 dspygen-2024.3.7/src/dspygen/modules/dflss_module.py
--rw-r--r--   0        0        0     1319 2024-03-08 05:46:07.183850 dspygen-2024.3.7/src/dspygen/modules/file_name_module.py
--rw-r--r--   0        0        0     4301 2024-02-29 22:58:59.155830 dspygen-2024.3.7/src/dspygen/modules/gen_cli_module.py
--rw-r--r--   0        0        0     1630 2024-03-06 20:35:36.549470 dspygen-2024.3.7/src/dspygen/modules/gen_dspy_module.py
--rw-r--r--   0        0        0     5520 2024-03-02 21:20:39.515152 dspygen-2024.3.7/src/dspygen/modules/gen_keyword_arguments_module.py
--rw-r--r--   0        0        0     1093 2024-03-06 18:39:40.232469 dspygen-2024.3.7/src/dspygen/modules/gen_message.py
--rw-r--r--   0        0        0     5555 2024-03-02 04:18:48.894579 dspygen-2024.3.7/src/dspygen/modules/gen_pydantic_instance_module.py
--rw-r--r--   0        0        0     1266 2024-02-27 18:36:46.735620 dspygen-2024.3.7/src/dspygen/modules/gen_signature_module.py
--rw-r--r--   0        0        0     4318 2024-03-05 23:02:52.641941 dspygen-2024.3.7/src/dspygen/modules/get_selector.py
--rw-r--r--   0        0        0     1421 2024-03-01 00:09:40.059558 dspygen-2024.3.7/src/dspygen/modules/html_module.py
--rw-r--r--   0        0        0     1935 2024-03-06 19:19:35.493962 dspygen-2024.3.7/src/dspygen/modules/insight_tweet_module.py
--rw-r--r--   0        0        0     2869 2024-02-29 22:41:17.052232 dspygen-2024.3.7/src/dspygen/modules/js_to_fast_api_module.py
--rw-r--r--   0        0        0     1788 2024-03-05 00:08:28.493923 dspygen-2024.3.7/src/dspygen/modules/jsx_module.py
--rw-r--r--   0        0        0     1325 2024-03-05 23:19:58.448963 dspygen-2024.3.7/src/dspygen/modules/message_module.py
--rw-r--r--   0        0        0     1239 2024-02-28 23:01:46.923037 dspygen-2024.3.7/src/dspygen/modules/module_docstring_module.py
--rw-r--r--   0        0        0     1787 2024-02-28 22:54:13.437149 dspygen-2024.3.7/src/dspygen/modules/product_bot_module.py
--rw-r--r--   0        0        0      819 2024-02-27 18:36:46.739395 dspygen-2024.3.7/src/dspygen/modules/prompt_function_call_module.py
--rw-r--r--   0        0        0     1781 2024-02-29 23:34:11.666243 dspygen-2024.3.7/src/dspygen/modules/python_expert_module.py
--rw-r--r--   0        0        0     1413 2024-02-29 22:51:24.271880 dspygen-2024.3.7/src/dspygen/modules/python_source_code_module.py
--rw-r--r--   0        0        0      848 2024-02-26 03:31:03.760752 dspygen-2024.3.7/src/dspygen/modules/react_jsx_module.py
--rw-r--r--   0        0        0     1001 2024-02-26 01:12:15.433642 dspygen-2024.3.7/src/dspygen/modules/request_contract_module.py
--rw-r--r--   0        0        0     5828 2024-02-26 22:44:59.095786 dspygen-2024.3.7/src/dspygen/modules/signature_factory.py
--rw-r--r--   0        0        0     5949 2024-02-27 18:36:46.776118 dspygen-2024.3.7/src/dspygen/modules/signature_renderer.py
--rw-r--r--   0        0        0     1744 2024-03-08 05:46:07.178290 dspygen-2024.3.7/src/dspygen/modules/source_code_pep8_docs_module.py
--rw-r--r--   0        0        0      969 2024-03-02 04:49:31.676695 dspygen-2024.3.7/src/dspygen/modules/sql_query.py
--rw-r--r--   0        0        0     2073 2024-03-06 20:50:04.369037 dspygen-2024.3.7/src/dspygen/modules/streamlit_bot.py
--rw-r--r--   0        0        0     2165 2024-02-27 18:36:46.748854 dspygen-2024.3.7/src/dspygen/modules/subject_destination_audience_newsletter_article_module.py
--rw-r--r--   0        0        0     1052 2024-03-05 21:45:44.059369 dspygen-2024.3.7/src/dspygen/modules/tax_return_agent.py
--rw-r--r--   0        0        0      914 2024-03-02 04:36:30.821840 dspygen-2024.3.7/src/dspygen/modules/test.py
--rw-r--r--   0        0        0     1486 2024-02-29 22:58:59.160532 dspygen-2024.3.7/src/dspygen/modules/test_chat_bot_cli.py
--rw-r--r--   0        0        0      799 2024-02-27 18:36:46.746185 dspygen-2024.3.7/src/dspygen/modules/text_summary_module_module.py
--rw-r--r--   0        0        0     1767 2024-03-01 20:56:18.178441 dspygen-2024.3.7/src/dspygen/modules/to_elixir_module.py
--rw-r--r--   0        0        0     2330 2024-03-06 22:01:58.222761 dspygen-2024.3.7/src/dspygen/modules/usp_connect_ship_webhook.py
--rw-r--r--   0        0        0        0 2024-03-06 20:57:56.031280 dspygen-2024.3.7/src/dspygen/pages/__init__.py
--rw-r--r--   0        0        0      474 2024-03-06 21:10:26.461757 dspygen-2024.3.7/src/dspygen/pages/hello.py
--rw-r--r--   0        0        0     1407 2024-03-08 05:44:22.663177 dspygen-2024.3.7/src/dspygen/pages/mqtt_page.py
--rw-r--r--   0        0        0      474 2024-03-06 21:10:26.461757 dspygen-2024.3.7/src/dspygen/pages/remodeling.py
--rw-r--r--   0        0        0       23 2024-02-26 00:06:54.236649 dspygen-2024.3.7/src/dspygen/rdddy/__init__.py
--rw-r--r--   0        0        0    11110 2024-03-06 19:24:49.522291 dspygen-2024.3.7/src/dspygen/rdddy/abstract_actor.py
--rw-r--r--   0        0        0     1185 2024-03-06 19:13:09.363700 dspygen-2024.3.7/src/dspygen/rdddy/abstract_aggregate.py
--rw-r--r--   0        0        0      142 2024-03-06 19:08:39.704580 dspygen-2024.3.7/src/dspygen/rdddy/abstract_command.py
--rw-r--r--   0        0        0      128 2024-03-06 19:08:39.694932 dspygen-2024.3.7/src/dspygen/rdddy/abstract_event.py
--rw-r--r--   0        0        0     2981 2024-03-06 19:08:39.682151 dspygen-2024.3.7/src/dspygen/rdddy/abstract_message.py
--rw-r--r--   0        0        0      674 2024-03-06 19:08:39.664583 dspygen-2024.3.7/src/dspygen/rdddy/abstract_policy.py
--rw-r--r--   0        0        0      128 2024-03-06 19:08:39.729843 dspygen-2024.3.7/src/dspygen/rdddy/abstract_query.py
--rw-r--r--   0        0        0      170 2024-03-08 05:41:58.821203 dspygen-2024.3.7/src/dspygen/rdddy/abstract_read_model.py
--rw-r--r--   0        0        0      685 2024-03-06 19:08:39.713205 dspygen-2024.3.7/src/dspygen/rdddy/abstract_repository.py
--rw-r--r--   0        0        0      548 2024-03-06 19:08:39.674028 dspygen-2024.3.7/src/dspygen/rdddy/abstract_saga.py
--rw-r--r--   0        0        0      460 2024-02-23 01:33:09.223883 dspygen-2024.3.7/src/dspygen/rdddy/abstract_task.py
--rw-r--r--   0        0        0      420 2024-02-19 01:34:08.066902 dspygen-2024.3.7/src/dspygen/rdddy/abstract_value_object.py
--rw-r--r--   0        0        0      419 2024-02-23 01:33:09.225043 dspygen-2024.3.7/src/dspygen/rdddy/abstract_view.py
--rw-r--r--   0        0        0    16273 2024-03-06 19:08:39.735451 dspygen-2024.3.7/src/dspygen/rdddy/actor_system.py
--rw-r--r--   0        0        0       23 2024-02-26 00:06:54.236649 dspygen-2024.3.7/src/dspygen/rdddy/browser/__init__.py
--rw-r--r--   0        0        0     2553 2024-03-06 19:19:17.280006 dspygen-2024.3.7/src/dspygen/rdddy/browser/browser_domain.py
--rw-r--r--   0        0        0     4027 2024-03-05 20:56:02.324186 dspygen-2024.3.7/src/dspygen/rdddy/browser/browser_process_supervisor.py
--rw-r--r--   0        0        0     5557 2024-03-06 19:08:39.691667 dspygen-2024.3.7/src/dspygen/rdddy/browser/browser_worker.py
--rw-r--r--   0        0        0      118 2024-02-09 18:11:20.221150 dspygen-2024.3.7/src/dspygen/rdddy/browser/run_chatgpt.py
--rw-r--r--   0        0        0      435 2024-02-23 01:33:09.263893 dspygen-2024.3.7/src/dspygen/rdddy/domain_exception.py
--rw-r--r--   0        0        0     5148 2024-03-07 21:42:05.141192 dspygen-2024.3.7/src/dspygen/rdddy/event_storm_domain_specification_model.py
--rw-r--r--   0        0        0     1091 2024-03-07 21:40:24.544605 dspygen-2024.3.7/src/dspygen/rdddy/event_storm_model.py
--rw-r--r--   0        0        0        0 2024-02-26 22:53:26.111403 dspygen-2024.3.7/src/dspygen/signatures/__init__.py
--rw-r--r--   0        0        0      400 2024-02-27 18:36:46.743576 dspygen-2024.3.7/src/dspygen/signatures/blog_article.py
--rw-r--r--   0        0        0      425 2024-02-29 22:40:58.261052 dspygen-2024.3.7/src/dspygen/signatures/generate_answer.py
--rw-r--r--   0        0        0       23 2024-02-26 00:06:54.236649 dspygen-2024.3.7/src/dspygen/subcommands/__init__.py
--rw-r--r--   0        0        0     2753 2024-03-06 19:19:49.348166 dspygen-2024.3.7/src/dspygen/subcommands/actor_cmd.py
--rw-r--r--   0        0        0     1890 2024-03-02 20:28:07.641376 dspygen-2024.3.7/src/dspygen/subcommands/assert_cmd.py
--rw-r--r--   0        0        0      993 2024-03-05 22:12:12.036819 dspygen-2024.3.7/src/dspygen/subcommands/browser_cmd.py
--rw-r--r--   0        0        0     2795 2024-03-05 00:30:03.391323 dspygen-2024.3.7/src/dspygen/subcommands/command_cmd.py
--rw-r--r--   0        0        0     2192 2024-03-03 01:56:27.502672 dspygen-2024.3.7/src/dspygen/subcommands/help.txt
--rw-r--r--   0        0        0     3654 2024-03-03 01:56:42.132578 dspygen-2024.3.7/src/dspygen/subcommands/help_cmd.py
--rw-r--r--   0        0        0      899 2024-03-05 18:28:35.881579 dspygen-2024.3.7/src/dspygen/subcommands/lm_cmd.py
--rw-r--r--   0        0        0     2255 2024-03-02 19:32:12.800452 dspygen-2024.3.7/src/dspygen/subcommands/module_cmd.py
--rw-r--r--   0        0        0      763 2024-02-29 05:00:18.699308 dspygen-2024.3.7/src/dspygen/subcommands/sig_cmd.py
--rw-r--r--   0        0        0     2660 2024-03-02 20:25:11.427224 dspygen-2024.3.7/src/dspygen/subcommands/temp_assert.py
--rw-r--r--   0        0        0      802 2024-01-05 18:58:37.983478 dspygen-2024.3.7/src/dspygen/templates/actor_template.j2
--rw-r--r--   0        0        0      187 2024-03-06 18:39:36.968464 dspygen-2024.3.7/src/dspygen/templates/dspy_module_cli_call.j2
--rw-r--r--   0        0        0      146 2024-03-06 18:38:12.997867 dspygen-2024.3.7/src/dspygen/templates/dspy_module_def_call.j2
--rw-r--r--   0        0        0      152 2024-03-06 18:38:13.008342 dspygen-2024.3.7/src/dspygen/templates/dspy_module_main.j2
--rw-r--r--   0        0        0      240 2024-03-06 18:38:13.006205 dspygen-2024.3.7/src/dspygen/templates/dspy_module_route.j2
--rw-r--r--   0        0        0      335 2024-03-06 20:44:11.743840 dspygen-2024.3.7/src/dspygen/templates/dspy_module_streamlit_input.j2
--rw-r--r--   0        0        0      577 2024-01-05 00:57:34.041149 dspygen-2024.3.7/src/dspygen/typetemp/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 00:57:34.037457 dspygen-2024.3.7/src/dspygen/typetemp/environment/__init__.py
--rw-r--r--   0        0        0     1043 2024-03-06 18:21:31.484739 dspygen-2024.3.7/src/dspygen/typetemp/environment/typed_environment.py
--rw-r--r--   0        0        0      979 2024-03-06 18:21:31.472405 dspygen-2024.3.7/src/dspygen/typetemp/environment/typed_native_environment.py
--rw-r--r--   0        0        0        0 2024-01-05 00:57:34.050547 dspygen-2024.3.7/src/dspygen/typetemp/extension/__init__.py
--rw-r--r--   0        0        0    24023 2024-02-23 01:33:09.475294 dspygen-2024.3.7/src/dspygen/typetemp/extension/faker_extension.py
--rw-r--r--   0        0        0     1098 2024-02-24 21:23:34.405664 dspygen-2024.3.7/src/dspygen/typetemp/extension/inflection_extension.py
--rw-r--r--   0        0        0     1493 2024-02-26 22:15:14.368689 dspygen-2024.3.7/src/dspygen/typetemp/functional.py
--rw-r--r--   0        0        0        0 2024-01-05 00:57:34.038203 dspygen-2024.3.7/src/dspygen/typetemp/template/__init__.py
--rw-r--r--   0        0        0     2454 2024-02-27 18:36:46.776621 dspygen-2024.3.7/src/dspygen/typetemp/template/async_render_mixin.py
--rw-r--r--   0        0        0    11207 2024-02-26 22:15:14.353910 dspygen-2024.3.7/src/dspygen/typetemp/template/dsl_project.py
--rw-r--r--   0        0        0      241 2024-01-16 06:45:52.700831 dspygen-2024.3.7/src/dspygen/typetemp/template/python
--rw-r--r--   0        0        0     1001 2024-02-19 00:24:51.709162 dspygen-2024.3.7/src/dspygen/typetemp/template/render_funcs.py
--rw-r--r--   0        0        0     2160 2024-02-19 00:24:51.709222 dspygen-2024.3.7/src/dspygen/typetemp/template/render_mixin.py
--rw-r--r--   0        0        0     3393 2024-02-26 22:16:42.440788 dspygen-2024.3.7/src/dspygen/typetemp/template/smart_template.py
--rw-r--r--   0        0        0     5497 2024-02-26 22:15:14.342848 dspygen-2024.3.7/src/dspygen/typetemp/template/typed_injector.py
--rw-r--r--   0        0        0     2348 2024-02-26 22:16:42.436845 dspygen-2024.3.7/src/dspygen/typetemp/template/typed_prompt.py
--rw-r--r--   0        0        0     2590 2024-02-26 22:15:14.346792 dspygen-2024.3.7/src/dspygen/typetemp/template/typed_python_source.py
--rw-r--r--   0        0        0     1042 2024-02-26 22:15:14.360081 dspygen-2024.3.7/src/dspygen/typetemp/template/typed_template.py
--rw-r--r--   0        0        0       23 2024-02-26 00:41:24.402416 dspygen-2024.3.7/src/dspygen/utils/__init__.py
--rw-r--r--   0        0        0      930 2024-02-29 04:59:42.454750 dspygen-2024.3.7/src/dspygen/utils/cli_tools.py
--rw-r--r--   0        0        0    12574 2024-02-23 01:33:09.514913 dspygen-2024.3.7/src/dspygen/utils/complete.py
--rw-r--r--   0        0        0     2961 2024-02-19 00:24:51.709737 dspygen-2024.3.7/src/dspygen/utils/compression_tools.py
--rw-r--r--   0        0        0    25532 2024-02-26 22:19:25.120888 dspygen-2024.3.7/src/dspygen/utils/create_prompts.py
--rw-r--r--   0        0        0      202 2024-02-28 06:40:27.680268 dspygen-2024.3.7/src/dspygen/utils/dspy_tools.py
--rw-r--r--   0        0        0      118 2024-02-09 18:11:20.285188 dspygen-2024.3.7/src/dspygen/utils/example.py
--rw-r--r--   0        0        0     6921 2024-03-06 21:08:12.189034 dspygen-2024.3.7/src/dspygen/utils/file_tools.py
--rw-r--r--   0        0        0     4684 2024-02-19 00:24:51.710023 dspygen-2024.3.7/src/dspygen/utils/models.py
--rw-r--r--   0        0        0     1639 2024-02-28 21:20:34.883565 dspygen-2024.3.7/src/dspygen/utils/module_tools.py
--rw-r--r--   0        0        0     4457 2024-02-28 21:45:32.608074 dspygen-2024.3.7/src/dspygen/utils/yaml_tools.py
--rw-r--r--   0        0        0     9504 1970-01-01 00:00:00.000000 dspygen-2024.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-02-26 01:14:54.588858 dspygen-2024.3.8/LICENSE
+-rw-r--r--   0        0        0     7783 2024-02-26 22:30:04.933363 dspygen-2024.3.8/README.md
+-rw-r--r--   0        0        0     6597 2024-04-08 20:56:04.092572 dspygen-2024.3.8/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-03-04 21:23:01.363615 dspygen-2024.3.8/src/dspygen/__init__.py
+-rw-r--r--   0        0        0     2249 2024-03-27 20:42:28.847509 dspygen-2024.3.8/src/dspygen/api.py
+-rw-r--r--   0        0        0     1019 2024-04-01 16:08:39.820504 dspygen-2024.3.8/src/dspygen/app.py
+-rw-r--r--   0        0        0      731 2024-01-23 20:40:53.415200 dspygen-2024.3.8/src/dspygen/async_typer.py
+-rw-r--r--   0        0        0        0 2024-03-10 00:26:05.385636 dspygen-2024.3.8/src/dspygen/bpel_diagrams/__init__.py
+-rw-r--r--   0        0        0     5857 2024-03-10 00:39:03.175624 dspygen-2024.3.8/src/dspygen/bpel_diagrams/mermaid_multi_module_demo.py
+-rw-r--r--   0        0        0       49 2024-03-08 21:50:07.926048 dspygen-2024.3.8/src/dspygen/bpel_models/__init__.py
+-rw-r--r--   0        0        0    12392 2024-03-09 05:17:45.343065 dspygen-2024.3.8/src/dspygen/bpel_models/activities.py
+-rw-r--r--   0        0        0     4328 2024-03-09 06:52:06.204109 dspygen-2024.3.8/src/dspygen/bpel_models/correlations.py
+-rw-r--r--   0        0        0     2976 2024-03-08 22:06:13.283896 dspygen-2024.3.8/src/dspygen/bpel_models/event_handlers.py
+-rw-r--r--   0        0        0     5007 2024-03-09 06:52:06.229273 dspygen-2024.3.8/src/dspygen/bpel_models/fault_handlers.py
+-rw-r--r--   0        0        0     3787 2024-03-09 06:52:06.211153 dspygen-2024.3.8/src/dspygen/bpel_models/links.py
+-rw-r--r--   0        0        0     1934 2024-03-09 06:52:06.224214 dspygen-2024.3.8/src/dspygen/bpel_models/partner_links.py
+-rw-r--r--   0        0        0     2125 2024-03-09 05:10:45.482280 dspygen-2024.3.8/src/dspygen/bpel_models/process.py
+-rw-r--r--   0        0        0     5256 2024-03-09 06:52:06.219929 dspygen-2024.3.8/src/dspygen/bpel_models/variables.py
+-rw-r--r--   0        0        0       49 2024-03-08 21:27:12.743325 dspygen-2024.3.8/src/dspygen/bpmn_models/__init__.py
+-rw-r--r--   0        0        0     1682 2024-03-08 21:33:53.588157 dspygen-2024.3.8/src/dspygen/bpmn_models/artifacts.py
+-rw-r--r--   0        0        0     2236 2024-03-08 21:36:53.240097 dspygen-2024.3.8/src/dspygen/bpmn_models/connecting_objects.py
+-rw-r--r--   0        0        0     2360 2024-03-08 21:36:53.234935 dspygen-2024.3.8/src/dspygen/bpmn_models/events.py
+-rw-r--r--   0        0        0     1194 2024-03-08 21:40:35.735330 dspygen-2024.3.8/src/dspygen/bpmn_models/flow_objects.py
+-rw-r--r--   0        0        0      807 2024-03-08 21:41:07.254320 dspygen-2024.3.8/src/dspygen/bpmn_models/gateways.py
+-rw-r--r--   0        0        0     2604 2024-03-08 21:43:20.467956 dspygen-2024.3.8/src/dspygen/bpmn_models/other_entities.py
+-rw-r--r--   0        0        0     1508 2024-03-08 21:44:01.436253 dspygen-2024.3.8/src/dspygen/bpmn_models/pools_and_lanes.py
+-rw-r--r--   0        0        0      816 2024-03-08 22:42:25.973034 dspygen-2024.3.8/src/dspygen/bpmn_models/sub_processes.py
+-rw-r--r--   0        0        0     7430 2024-04-08 20:54:20.890060 dspygen-2024.3.8/src/dspygen/cli.py
+-rw-r--r--   0        0        0      469 2024-04-08 20:54:20.886010 dspygen-2024.3.8/src/dspygen/config.yaml
+-rw-r--r--   0        0        0        0 2024-03-15 16:22:44.811119 dspygen-2024.3.8/src/dspygen/dsl/__init__.py
+-rw-r--r--   0        0        0     1257 2024-03-15 22:44:13.184746 dspygen-2024.3.8/src/dspygen/dsl/dsl_dspy_assertion.py
+-rw-r--r--   0        0        0     2743 2024-03-22 17:46:49.505577 dspygen-2024.3.8/src/dspygen/dsl/dsl_pipeline_executor.py
+-rw-r--r--   0        0        0     5055 2024-03-21 23:37:34.305316 dspygen-2024.3.8/src/dspygen/dsl/dsl_predict_module.py
+-rw-r--r--   0        0        0     6253 2024-03-22 17:35:27.524355 dspygen-2024.3.8/src/dspygen/dsl/dsl_pydantic_models.py
+-rw-r--r--   0        0        0     3519 2024-03-24 04:53:24.871960 dspygen-2024.3.8/src/dspygen/dsl/dsl_step_module.py
+-rw-r--r--   0        0        0      101 2024-03-16 19:59:42.261642 dspygen-2024.3.8/src/dspygen/dsl/examples/blog_pipeline.yaml
+-rw-r--r--   0        0        0      745 2024-03-22 22:46:06.263481 dspygen-2024.3.8/src/dspygen/dsl/examples/example_pipeline.yaml
+-rw-r--r--   0        0        0     1294 2024-03-28 03:34:30.952311 dspygen-2024.3.8/src/dspygen/dsl/examples/poem_pipeline.yaml
+-rw-r--r--   0        0        0     1395 2024-03-19 22:28:27.193700 dspygen-2024.3.8/src/dspygen/dsl/examples/saltcorn_plugin_generator.yaml
+-rw-r--r--   0        0        0      148 2024-03-19 21:00:49.951126 dspygen-2024.3.8/src/dspygen/dsl/examples/sql_to_nl.yaml
+-rw-r--r--   0        0        0       55 2024-03-19 19:53:57.989916 dspygen-2024.3.8/src/dspygen/dsl/examples/text_signature_pipeline.yaml
+-rw-r--r--   0        0        0       85 2024-03-18 22:38:39.718189 dspygen-2024.3.8/src/dspygen/dsl/modules/raw_to_structure_module.yaml
+-rw-r--r--   0        0        0      361 2024-03-19 20:59:43.993508 dspygen-2024.3.8/src/dspygen/dsl/signature/sql_to_natural_signature.yaml
+-rw-r--r--   0        0        0        0 2024-03-15 22:02:35.383415 dspygen-2024.3.8/src/dspygen/dsl/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 21:33:51.808107 dspygen-2024.3.8/src/dspygen/dsl/utils/dsl_assertions_utils.py
+-rw-r--r--   0        0        0      566 2024-03-18 03:32:00.006402 dspygen-2024.3.8/src/dspygen/dsl/utils/dsl_language_model_utils.py
+-rw-r--r--   0        0        0     2699 2024-03-21 23:53:52.595121 dspygen-2024.3.8/src/dspygen/dsl/utils/dsl_lm_module_utils.py
+-rw-r--r--   0        0        0      852 2024-03-22 00:46:49.172865 dspygen-2024.3.8/src/dspygen/dsl/utils/dsl_retrieval_model_utils.py
+-rw-r--r--   0        0        0     1108 2024-03-24 04:58:34.653369 dspygen-2024.3.8/src/dspygen/dsl/utils/dsl_rm_module_utils.py
+-rw-r--r--   0        0        0     2517 2024-03-19 20:53:39.318866 dspygen-2024.3.8/src/dspygen/dsl/utils/dsl_signature_utils.py
+-rw-r--r--   0        0        0     1344 2024-03-09 06:48:49.366197 dspygen-2024.3.8/src/dspygen/dspygen_app.py
+-rw-r--r--   0        0        0       15 2024-03-02 21:25:45.285222 dspygen-2024.3.8/src/dspygen/experiments/.git/COMMIT_EDITMSG
+-rw-r--r--   0        0        0       21 2024-03-02 21:00:22.720738 dspygen-2024.3.8/src/dspygen/experiments/.git/HEAD
+-rw-r--r--   0        0        0      137 2024-03-02 21:25:45.250428 dspygen-2024.3.8/src/dspygen/experiments/.git/config
+-rw-r--r--   0        0        0       73 2024-03-02 21:00:22.717125 dspygen-2024.3.8/src/dspygen/experiments/.git/description
+-rwxr-xr-x   0        0        0      478 2024-03-02 21:00:22.718166 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2024-03-02 21:00:22.717490 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4726 2024-03-02 21:00:22.718352 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2024-03-02 21:00:22.718737 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2024-03-02 21:00:22.719040 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1643 2024-03-02 21:00:22.717992 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2024-03-02 21:00:22.718849 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1374 2024-03-02 21:00:22.719230 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2024-03-02 21:00:22.717841 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2024-03-02 21:00:22.718519 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2024-03-02 21:00:22.718625 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2783 2024-03-02 21:00:22.719590 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     3650 2024-03-02 21:00:22.719479 dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/update.sample
+-rw-r--r--   0        0        0     3418 2024-03-15 00:46:19.079079 dspygen-2024.3.8/src/dspygen/experiments/.git/index
+-rw-r--r--   0        0        0      240 2024-03-02 21:00:22.716869 dspygen-2024.3.8/src/dspygen/experiments/.git/info/exclude
+-rw-r--r--   0        0        0      384 2024-03-02 21:25:45.286091 dspygen-2024.3.8/src/dspygen/experiments/.git/logs/HEAD
+-rw-r--r--   0        0        0      384 2024-03-02 21:25:45.286375 dspygen-2024.3.8/src/dspygen/experiments/.git/logs/refs/heads/main
+-rw-r--r--   0        0        0      906 2024-03-02 21:00:22.755656 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/07/2c395e5a1a2fda1ebd81855a0857a4c349aba9
+-rw-r--r--   0        0        0      226 2024-03-02 21:00:22.757663 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/17/97b95f720b5217b695bcff22867a50394f3abf
+-rw-r--r--   0        0        0      146 2024-03-02 21:00:22.753226 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/19/06d15bba64a214e6d9aaec6efdefe2c13c7707
+-rw-r--r--   0        0        0     1224 2024-03-06 19:01:54.514198 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/1e/d7c76971abff4a041741b96643e4bbe493bd3f
+-rw-r--r--   0        0        0      667 2024-03-02 21:00:22.762303 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/29/790e08d481fbcf9876f5e09e8618e0c6ff2cf4
+-rw-r--r--   0        0        0      403 2024-03-02 21:00:22.758262 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/2d/dc2e65f3a5975fdf305094330840323c7eb654
+-rw-r--r--   0        0        0     5058 2024-03-02 21:00:22.759386 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/34/484ad0f39e38772282a9bb02ba1df4f056b1f7
+-rw-r--r--   0        0        0   356425 2024-03-02 21:00:22.751592 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/38/a98b391b7a6e8e740cae9681b5f0b295848fcc
+-rw-r--r--   0        0        0      769 2024-03-02 21:00:22.758754 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/46/ed8e6d6b3d12b5bf9028d0777450412497d2aa
+-rw-r--r--   0        0        0      186 2024-03-02 21:25:45.285483 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/51/e517c46227aca5ee9bb188a8f11bf1717a750e
+-rw-r--r--   0        0        0      762 2024-03-02 21:25:45.283882 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/63/e5b4dd95ed8214e4f3167d66b2b139f49b0b04
+-rw-r--r--   0        0        0      370 2024-03-02 21:00:22.765847 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/7b/782ba56f06f203507ed84702ce312d9e919910
+-rw-r--r--   0        0        0      339 2024-03-02 21:00:22.761060 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/7c/100c125c4d4a859f02f595e05d04a437c5346d
+-rw-r--r--   0        0        0      774 2024-03-02 21:25:45.266809 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/85/97acd78f726e8277a086b8a78d6d77c82f4d2c
+-rw-r--r--   0        0        0      287 2024-03-02 21:00:22.764712 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/89/3f12d07852de09f2b88bcfc52a72c93110f555
+-rw-r--r--   0        0        0      665 2024-03-02 21:00:22.763518 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/89/80972d4e4fe721d9a4b66d38500a387cd5d677
+-rw-r--r--   0        0        0      386 2024-03-02 21:00:22.765280 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/8d/f078cc0e6ae05bd48848561f58b756b9b361d7
+-rw-r--r--   0        0        0      821 2024-03-02 21:00:22.764181 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/90/838848601a0b18aafe0f31edb678a2f801f0f2
+-rw-r--r--   0        0        0     1383 2024-03-07 21:20:22.717611 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/97/8bd6af4ad3a34e4016af33f921e416a723518a
+-rw-r--r--   0        0        0     2669 2024-03-02 21:00:22.754966 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/9f/3b783e2f90a73bacc366d57205db068a1f130a
+-rw-r--r--   0        0        0      763 2024-03-02 21:00:22.783125 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/a4/f3e1b596347a141fde89a09e19348524331fb1
+-rw-r--r--   0        0        0     3489 2024-03-06 18:47:12.342771 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/a5/1355a31ec94b448a81fe23cd03407e6db9fb98
+-rw-r--r--   0        0        0     1637 2024-03-02 21:00:22.754428 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/a7/f8004ca3e4019a0813e6d37454a9a1d4633732
+-rw-r--r--   0        0        0     2844 2024-03-02 21:00:22.760013 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/ae/864cd37388df8a496b2e62caa5bdb338e22de8
+-rw-r--r--   0        0        0     2170 2024-03-06 18:48:21.155474 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/af/54a3d8766d0686126ba2e2b3206b8270f1d5ef
+-rw-r--r--   0        0        0      732 2024-03-02 21:00:22.762698 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/b9/0e196ece0bb3c298e1565c9e5ba065ae468d74
+-rw-r--r--   0        0        0      907 2024-03-02 21:00:22.760483 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/bd/3ea467b227c44e9d5a1d687beef7d6d5f02f4d
+-rw-r--r--   0        0        0      153 2024-03-02 21:00:22.784474 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/be/806c8525a46028aaa93e635fad9345cfb9340b
+-rw-r--r--   0        0        0      215 2024-03-02 21:00:22.757066 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/c8/9b3c36bb5eabe165112fa224ec94f3b6c12600
+-rw-r--r--   0        0        0      826 2024-03-02 21:25:45.266351 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/d2/5ac35cbee6a13431d6769e22c0eac72f5ed551
+-rw-r--r--   0        0        0      599 2024-03-02 21:00:22.761581 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/d2/a1225cf1aa018c446ce1274a87eecb37294e03
+-rw-r--r--   0        0        0      808 2024-03-02 21:00:22.753950 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/da/938270af8aa8e1b6655c68dc10042c01526cf7
+-rw-r--r--   0        0        0       15 2024-03-15 00:46:19.078963 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
+-rw-r--r--   0        0        0      180 2024-03-02 21:00:22.782558 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/f8/818c037929cf14c8091a9f065221faffbc15ff
+-rw-r--r--   0        0        0      818 2024-03-02 21:00:22.756366 dspygen-2024.3.8/src/dspygen/experiments/.git/objects/fc/d9f4d1c396f872cc2f80e1599b961223430558
+-rw-r--r--   0        0        0       41 2024-03-02 21:25:45.286042 dspygen-2024.3.8/src/dspygen/experiments/.git/refs/heads/main
+-rw-r--r--   0        0        0        0 2024-02-27 17:34:57.501846 dspygen-2024.3.8/src/dspygen/experiments/__init__.py
+-rw-r--r--   0        0        0      596 2024-03-29 20:30:43.104135 dspygen-2024.3.8/src/dspygen/experiments/business_patterns_for_devs.py
+-rw-r--r--   0        0        0     1258 2024-03-27 20:37:34.688869 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/__init__.py
+-rw-r--r--   0        0        0     4623 2024-04-01 17:46:47.559247 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_aggregate/conversation_aggregate.py
+-rw-r--r--   0        0        0      197 2024-03-27 04:21:00.341581 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_command/generate_response_command.py
+-rw-r--r--   0        0        0      199 2024-03-27 04:05:01.551931 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_command/handle_user_query_command.py
+-rw-r--r--   0        0        0      199 2024-03-27 04:05:01.542100 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_command/recognize_entity_command.py
+-rw-r--r--   0        0        0      199 2024-03-27 04:05:01.539595 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_command/recognize_intent_command.py
+-rw-r--r--   0        0        0      199 2024-03-27 04:05:01.547180 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_command/transition_state_command.py
+-rw-r--r--   0        0        0      195 2024-03-27 04:05:01.544772 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_command/update_context_command.py
+-rw-r--r--   0        0        0      185 2024-03-27 04:05:01.520738 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/context_updated_event.py
+-rw-r--r--   0        0        0      187 2024-03-27 04:05:01.620171 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/database_queried_event.py
+-rw-r--r--   0        0        0      189 2024-03-27 04:05:01.517593 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/entity_recognized_event.py
+-rw-r--r--   0        0        0      195 2024-03-27 04:05:01.534301 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/external_api_response_event.py
+-rw-r--r--   0        0        0      199 2024-03-27 04:05:01.617145 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/external_service_called_event.py
+-rw-r--r--   0        0        0      189 2024-03-27 04:05:01.514939 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/intent_recognized_event.py
+-rw-r--r--   0        0        0      191 2024-03-27 04:05:01.529029 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/response_generated_event.py
+-rw-r--r--   0        0        0      187 2024-03-27 04:05:01.523184 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/state_transition_event.py
+-rw-r--r--   0        0        0      187 2024-03-27 04:05:01.537109 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/system_interrupt_event.py
+-rw-r--r--   0        0        0      201 2024-03-27 04:05:01.612166 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/system_message_displayed_event.py
+-rw-r--r--   0        0        0      191 2024-03-27 04:05:01.531585 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/user_input_received_event.py
+-rw-r--r--   0        0        0      197 2024-03-27 04:05:01.609591 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/user_message_submitted_event.py
+-rw-r--r--   0        0        0      189 2024-03-27 04:05:01.526267 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_event/user_query_handled_event.py
+-rw-r--r--   0        0        0      197 2024-03-27 04:05:01.573931 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_policy/context_management_policy.py
+-rw-r--r--   0        0        0      197 2024-03-27 04:05:01.571411 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_policy/entity_recognition_policy.py
+-rw-r--r--   0        0        0      191 2024-03-27 04:05:01.568717 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_policy/intent_handling_policy.py
+-rw-r--r--   0        0        0      199 2024-03-27 04:05:01.579263 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_policy/response_generation_policy.py
+-rw-r--r--   0        0        0      193 2024-03-27 04:05:01.576363 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_policy/state_transition_policy.py
+-rw-r--r--   0        0        0      191 2024-03-27 04:05:01.554715 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_query/get_current_context_query.py
+-rw-r--r--   0        0        0      187 2024-03-27 04:05:01.562633 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_query/get_current_state_query.py
+-rw-r--r--   0        0        0      189 2024-03-27 04:05:01.560057 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_query/get_entity_details_query.py
+-rw-r--r--   0        0        0      189 2024-03-27 04:05:01.557528 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_query/get_intent_details_query.py
+-rw-r--r--   0        0        0      212 2024-03-27 04:05:01.586903 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_read_model/context_snapshot_read_model.py
+-rw-r--r--   0        0        0      194 2024-03-27 04:05:01.584311 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_read_model/entity_read_model.py
+-rw-r--r--   0        0        0      194 2024-03-27 04:05:01.581904 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_read_model/intent_read_model.py
+-rw-r--r--   0        0        0      198 2024-03-27 04:05:01.592278 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_read_model/response_read_model.py
+-rw-r--r--   0        0        0      192 2024-03-27 04:05:01.589399 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_read_model/state_read_model.py
+-rw-r--r--   0        0        0     4109 2024-03-27 04:04:22.238668 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_renderer.py
+-rw-r--r--   0        0        0      191 2024-03-27 04:05:01.614626 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_saga/conversation_handling_saga.py
+-rw-r--r--   0        0        0      199 2024-03-27 04:05:01.652627 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_task/generate_dialogue_response_task.py
+-rw-r--r--   0        0        0      195 2024-03-27 04:05:01.658467 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_task/manage_state_transitions_task.py
+-rw-r--r--   0        0        0      183 2024-03-27 04:05:01.649598 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_task/process_user_input_task.py
+-rw-r--r--   0        0        0      201 2024-03-27 04:05:01.655434 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_task/update_conversation_context_task.py
+-rw-r--r--   0        0        0      208 2024-03-27 04:05:01.641483 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_value_object/context_value_object.py
+-rw-r--r--   0        0        0      206 2024-03-27 04:05:01.638648 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_value_object/entity_value_object.py
+-rw-r--r--   0        0        0      206 2024-03-27 04:05:01.636232 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_value_object/intent_value_object.py
+-rw-r--r--   0        0        0      210 2024-03-27 04:05:01.647050 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_value_object/response_value_object.py
+-rw-r--r--   0        0        0      204 2024-03-27 04:05:01.644282 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_value_object/state_value_object.py
+-rw-r--r--   0        0        0      165 2024-03-27 04:05:01.600898 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_view/context_view.py
+-rw-r--r--   0        0        0      163 2024-03-27 04:05:01.598195 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_view/entity_view.py
+-rw-r--r--   0        0        0      163 2024-03-27 04:05:01.595094 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_view/intent_view.py
+-rw-r--r--   0        0        0      167 2024-03-27 04:05:01.606563 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_view/response_view.py
+-rw-r--r--   0        0        0      161 2024-03-27 04:05:01.603375 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_view/state_view.py
+-rw-r--r--   0        0        0      199 2024-03-27 04:05:01.627893 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/domain_exception/context_update_exception.py
+-rw-r--r--   0        0        0      207 2024-03-27 04:05:01.625425 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/domain_exception/entity_recognition_exception.py
+-rw-r--r--   0        0        0      201 2024-03-27 04:05:01.622954 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/domain_exception/intent_not_found_exception.py
+-rw-r--r--   0        0        0      197 2024-03-27 04:05:01.630439 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/domain_exception/invalid_state_exception.py
+-rw-r--r--   0        0        0      209 2024-03-27 04:05:01.633686 dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/domain_exception/response_generation_exception.py
+-rw-r--r--   0        0        0     1900 2024-03-10 00:54:55.410333 dspygen-2024.3.8/src/dspygen/experiments/ddd/Bounded_Contexts.mmd
+-rw-r--r--   0        0        0     2273 2024-03-10 00:40:42.980599 dspygen-2024.3.8/src/dspygen/experiments/ddd/Domain_Events.mmd
+-rw-r--r--   0        0        0     4374 2024-03-10 00:42:09.188459 dspygen-2024.3.8/src/dspygen/experiments/ddd/Event_Sourcing_and_CQRS.mmd
+-rw-r--r--   0        0        0     4149 2024-03-10 00:42:41.009137 dspygen-2024.3.8/src/dspygen/experiments/ddd/Integration_and_Messaging_Channels.mmd
+-rw-r--r--   0        0        0    26057 2024-03-10 01:01:15.325675 dspygen-2024.3.8/src/dspygen/experiments/ddd/Sagas_and_Process_Managers.mmd
+-rw-r--r--   0        0        0     3296 2024-03-10 01:01:26.714202 dspygen-2024.3.8/src/dspygen/experiments/ddd/Testing_and_Simulation_of_Reactive_Systems.mmd
+-rw-r--r--   0        0        0     3592 2024-03-10 01:02:41.227873 dspygen-2024.3.8/src/dspygen/experiments/ddd/UI_and_External_Interfaces.mmd
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:04.111304 dspygen-2024.3.8/src/dspygen/experiments/ddd/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:12.509303 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_aggregate/__init__.py
+-rw-r--r--   0        0        0      215 2024-03-09 07:17:28.941940 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_aggregate/activity_execution_aggregate.py
+-rw-r--r--   0        0        0      217 2024-03-09 07:17:28.944313 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_aggregate/partner_interaction_aggregate.py
+-rw-r--r--   0        0        0      213 2024-03-09 07:17:28.939518 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_aggregate/process_execution_aggregate.py
+-rw-r--r--   0        0        0      211 2024-03-09 07:17:28.946672 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_aggregate/process_instance_aggregate.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:12.549236 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_command/__init__.py
+-rw-r--r--   0        0        0      199 2024-03-09 07:17:28.913210 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_command/execute_activity_command.py
+-rw-r--r--   0        0        0      191 2024-03-09 07:17:28.921334 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_command/handle_fault_command.py
+-rw-r--r--   0        0        0      195 2024-03-09 07:17:28.915737 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_command/invoke_partner_command.py
+-rw-r--r--   0        0        0      207 2024-03-09 07:17:28.926359 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_command/load_process_instance_command.py
+-rw-r--r--   0        0        0      205 2024-03-09 07:17:28.918455 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_command/receive_from_partner_command.py
+-rw-r--r--   0        0        0      207 2024-03-09 07:17:28.923946 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_command/save_process_instance_command.py
+-rw-r--r--   0        0        0      193 2024-03-09 07:17:28.907842 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_command/start_process_command.py
+-rw-r--r--   0        0        0      191 2024-03-09 07:17:28.910250 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_command/stop_process_command.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:12.907656 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-09 07:17:28.978700 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/button_click_event.py
+-rw-r--r--   0        0        0      181 2024-03-09 07:17:28.897776 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/data_received_event.py
+-rw-r--r--   0        0        0      181 2024-03-09 07:17:29.035268 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/data_transfer_event.py
+-rw-r--r--   0        0        0      199 2024-03-09 07:17:28.885999 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/external_event_occurred_event.py
+-rw-r--r--   0        0        0      199 2024-03-09 07:17:28.888646 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/external_system_updated_event.py
+-rw-r--r--   0        0        0      185 2024-03-09 07:17:28.981070 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/form_submission_event.py
+-rw-r--r--   0        0        0      179 2024-03-09 07:17:29.040553 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/integration_event.py
+-rw-r--r--   0        0        0      193 2024-03-09 07:17:29.037855 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/partner_interaction_event.py
+-rw-r--r--   0        0        0      195 2024-03-09 07:17:28.900296 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/partner_notification_event.py
+-rw-r--r--   0        0        0      191 2024-03-09 07:17:28.892312 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/regulation_amended_event.py
+-rw-r--r--   0        0        0      183 2024-03-09 07:17:28.905381 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/security_alert_event.py
+-rw-r--r--   0        0        0      179 2024-03-09 07:17:28.902924 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/service_down_event.py
+-rw-r--r--   0        0        0      191 2024-03-09 07:17:29.032550 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/service_invocation_event.py
+-rw-r--r--   0        0        0      183 2024-03-09 07:17:28.880472 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/task_completed_event.py
+-rw-r--r--   0        0        0      185 2024-03-09 07:17:28.983437 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/task_completion_event.py
+-rw-r--r--   0        0        0      177 2024-03-09 07:17:28.882936 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/task_failed_event.py
+-rw-r--r--   0        0        0      179 2024-03-09 07:17:28.877883 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/task_started_event.py
+-rw-r--r--   0        0        0      201 2024-03-09 07:17:28.895276 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/third_party_notification_event.py
+-rw-r--r--   0        0        0      187 2024-03-09 07:17:28.985797 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_event/user_interaction_event.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:12.963809 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_policy/__init__.py
+-rw-r--r--   0        0        0      187 2024-03-09 07:17:28.954064 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_policy/compensation_policy.py
+-rw-r--r--   0        0        0      181 2024-03-09 07:17:28.949177 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_policy/execution_policy.py
+-rw-r--r--   0        0        0      189 2024-03-09 07:17:28.956436 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_policy/fault_handling_policy.py
+-rw-r--r--   0        0        0      173 2024-03-09 07:17:28.951636 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_policy/retry_policy.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:13.002221 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_query/__init__.py
+-rw-r--r--   0        0        0      193 2024-03-09 07:17:28.931214 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_query/get_activity_details_query.py
+-rw-r--r--   0        0        0      191 2024-03-09 07:17:28.937007 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_query/get_process_metrics_query.py
+-rw-r--r--   0        0        0      189 2024-03-09 07:17:28.928819 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_query/get_process_status_query.py
+-rw-r--r--   0        0        0      189 2024-03-09 07:17:28.934248 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_query/get_variable_value_query.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:13.021736 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_read_model/__init__.py
+-rw-r--r--   0        0        0      204 2024-03-09 07:17:28.961232 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_read_model/activity_log_read_model.py
+-rw-r--r--   0        0        0      226 2024-03-09 07:17:28.965966 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_read_model/process_instance_details_read_model.py
+-rw-r--r--   0        0        0      210 2024-03-09 07:17:28.958851 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_read_model/process_summary_read_model.py
+-rw-r--r--   0        0        0      214 2024-03-09 07:17:28.963592 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_read_model/variable_snapshot_read_model.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:13.117901 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_saga/__init__.py
+-rw-r--r--   0        0        0      175 2024-03-09 07:17:28.991105 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_saga/compensation_saga.py
+-rw-r--r--   0        0        0      177 2024-03-09 07:17:28.993579 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_saga/fault_handling_saga.py
+-rw-r--r--   0        0        0      183 2024-03-09 07:17:28.988389 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_saga/process_execution_saga.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:13.148777 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_task/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-09 07:17:29.062655 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_task/data_validation_task.py
+-rw-r--r--   0        0        0      177 2024-03-09 07:17:29.067519 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_task/error_handling_task.py
+-rw-r--r--   0        0        0      173 2024-03-09 07:17:29.069898 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_task/integration_task.py
+-rw-r--r--   0        0        0      185 2024-03-09 07:17:29.065131 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_task/service_invocation_task.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:13.171456 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_value_object/__init__.py
+-rw-r--r--   0        0        0      224 2024-03-09 07:17:29.055445 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_value_object/activity_details_value_object.py
+-rw-r--r--   0        0        0      222 2024-03-09 07:17:29.057871 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_value_object/partner_details_value_object.py
+-rw-r--r--   0        0        0      212 2024-03-09 07:17:29.052849 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_value_object/process_id_value_object.py
+-rw-r--r--   0        0        0      210 2024-03-09 07:17:29.060240 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_value_object/variable_value_object.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:13.203608 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_view/__init__.py
+-rw-r--r--   0        0        0      167 2024-03-09 07:17:28.976331 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_view/error_log_view.py
+-rw-r--r--   0        0        0      181 2024-03-09 07:17:28.968436 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_view/process_overview_view.py
+-rw-r--r--   0        0        0      173 2024-03-09 07:17:28.971504 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_view/task_details_view.py
+-rw-r--r--   0        0        0      177 2024-03-09 07:17:28.973965 dspygen-2024.3.8/src/dspygen/experiments/ddd/abstract_view/user_dashboard_view.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:35:13.261455 dspygen-2024.3.8/src/dspygen/experiments/ddd/domain_exception/__init__.py
+-rw-r--r--   0        0        0      201 2024-03-09 07:17:29.045447 dspygen-2024.3.8/src/dspygen/experiments/ddd/domain_exception/data_processing_exception.py
+-rw-r--r--   0        0        0      205 2024-03-09 07:17:29.042987 dspygen-2024.3.8/src/dspygen/experiments/ddd/domain_exception/execution_failure_exception.py
+-rw-r--r--   0        0        0      195 2024-03-09 07:17:29.048016 dspygen-2024.3.8/src/dspygen/experiments/ddd/domain_exception/integration_exception.py
+-rw-r--r--   0        0        0      185 2024-03-09 07:17:29.050419 dspygen-2024.3.8/src/dspygen/experiments/ddd/domain_exception/system_exception.py
+-rw-r--r--   0        0        0     1405 2024-03-20 22:59:48.172023 dspygen-2024.3.8/src/dspygen/experiments/done/CriticFeedbackGeneratorSignature_pipeline.yaml
+-rw-r--r--   0        0        0      668 2024-03-20 22:23:03.639581 dspygen-2024.3.8/src/dspygen/experiments/done/WebsitePRD_pipeline.yaml
+-rw-r--r--   0        0        0        0 2024-03-21 18:35:05.851101 dspygen-2024.3.8/src/dspygen/experiments/done/__init__.py
+-rw-r--r--   0        0        0      331 2024-03-02 00:57:36.655430 dspygen-2024.3.8/src/dspygen/experiments/done/chatbots.py
+-rw-r--r--   0        0        0      361 2024-02-29 23:34:11.662934 dspygen-2024.3.8/src/dspygen/experiments/done/code_generator_agent.py
+-rw-r--r--   0        0        0     1790 2024-03-15 00:57:28.973632 dspygen-2024.3.8/src/dspygen/experiments/done/data_pipeline.yaml
+-rw-r--r--   0        0        0      260 2024-03-21 18:38:00.750259 dspygen-2024.3.8/src/dspygen/experiments/done/file_path.py
+-rw-r--r--   0        0        0      940 2024-03-21 23:47:50.237287 dspygen-2024.3.8/src/dspygen/experiments/done/first_step_with_user_input.py
+-rw-r--r--   0        0        0     1720 2024-03-21 23:47:50.241372 dspygen-2024.3.8/src/dspygen/experiments/done/gen_dsl_instances.py
+-rw-r--r--   0        0        0    14783 2024-03-22 18:41:18.780236 dspygen-2024.3.8/src/dspygen/experiments/done/gen_pydantic_class.py
+-rw-r--r--   0        0        0     6076 2024-03-06 18:55:42.509529 dspygen-2024.3.8/src/dspygen/experiments/done/gherkin_parser.py
+-rw-r--r--   0        0        0     3560 2024-03-07 21:15:06.538371 dspygen-2024.3.8/src/dspygen/experiments/done/lm_call.py
+-rw-r--r--   0        0        0     1061 2024-02-28 21:51:36.079683 dspygen-2024.3.8/src/dspygen/experiments/done/openai_ror_cli.py
+-rw-r--r--   0        0        0     1753 2024-03-01 22:03:13.771206 dspygen-2024.3.8/src/dspygen/experiments/done/python_to_elixir.py
+-rw-r--r--   0        0        0       87 2024-03-18 22:10:10.209738 dspygen-2024.3.8/src/dspygen/experiments/done/raw_to_structure_module.yaml
+-rw-r--r--   0        0        0      408 2024-03-19 22:12:22.596664 dspygen-2024.3.8/src/dspygen/experiments/done/saltcorn_plugin_generator.py
+-rw-r--r--   0        0        0    15627 2024-03-19 22:28:43.225124 dspygen-2024.3.8/src/dspygen/experiments/done/saltcorn_plugin_generator_output.yaml
+-rw-r--r--   0        0        0     1625 2024-03-08 05:43:24.578568 dspygen-2024.3.8/src/dspygen/experiments/done/socket_actor_system.py
+-rw-r--r--   0        0        0      286 2024-03-19 20:49:01.232725 dspygen-2024.3.8/src/dspygen/experiments/done/sql_to_natural_signature.yaml
+-rw-r--r--   0        0        0     1283 2024-03-21 18:41:05.641387 dspygen-2024.3.8/src/dspygen/experiments/done/test_openai_ror_cli.py
+-rw-r--r--   0        0        0     1864 2024-03-21 23:47:50.247855 dspygen-2024.3.8/src/dspygen/experiments/done/two_steps_with_user_input.py
+-rw-r--r--   0        0        0     1457 2024-03-20 23:05:27.609489 dspygen-2024.3.8/src/dspygen/experiments/done/understand_input_pipeline.yaml
+-rw-r--r--   0        0        0     2554 2024-03-17 18:42:33.539945 dspygen-2024.3.8/src/dspygen/experiments/done/wizard.py
+-rw-r--r--   0        0        0   884736 2015-11-29 18:53:02.000000 dspygen-2024.3.8/src/dspygen/experiments/function_calling/Chinook.db
+-rw-r--r--   0        0        0        0 2024-03-21 18:36:11.545968 dspygen-2024.3.8/src/dspygen/experiments/function_calling/__init__.py
+-rw-r--r--   0        0        0     1145 2024-02-27 21:48:22.789420 dspygen-2024.3.8/src/dspygen/experiments/function_calling/function_call.py
+-rw-r--r--   0        0        0     1241 2024-03-07 05:20:40.254419 dspygen-2024.3.8/src/dspygen/experiments/function_calling/sql_calling_asserts.py
+-rw-r--r--   0        0        0     1802 2024-03-21 18:41:05.645688 dspygen-2024.3.8/src/dspygen/experiments/function_calling/sql_optimization_function.py
+-rw-r--r--   0        0        0      915 2024-03-21 18:41:05.651765 dspygen-2024.3.8/src/dspygen/experiments/function_calling/weather_function_calling_asserts.py
+-rw-r--r--   0        0        0     1029 2024-03-01 22:03:15.367794 dspygen-2024.3.8/src/dspygen/experiments/function_calling/weather_functions.exs
+-rw-r--r--   0        0        0        0 2024-03-24 01:04:30.700418 dspygen-2024.3.8/src/dspygen/experiments/module_docstrings/__init__.py
+-rw-r--r--   0        0        0      776 2024-03-24 01:05:46.447006 dspygen-2024.3.8/src/dspygen/experiments/module_docstrings/generate_docstring_exec.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:54:28.298514 dspygen-2024.3.8/src/dspygen/experiments/pomo_bud/__init__.py
+-rw-r--r--   0        0        0      923 2024-03-26 17:58:57.653118 dspygen-2024.3.8/src/dspygen/experiments/pomo_bud/pomo_bud_dsl.yaml
+-rw-r--r--   0        0        0     4975 2024-03-26 17:57:51.273369 dspygen-2024.3.8/src/dspygen/experiments/pomo_bud/pomo_bud_models.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:58:15.990502 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/__init__.py
+-rw-r--r--   0        0        0     2380 2024-03-22 20:31:18.221865 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/api-for-document-management.tsx
+-rw-r--r--   0        0        0      729 2024-03-22 20:05:31.606695 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/confirm-signature-placement.tsx
+-rw-r--r--   0        0        0      634 2024-03-22 20:06:03.934748 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/custom-signing-instructions.tsx
+-rw-r--r--   0        0        0     1555 2024-03-22 22:50:44.801072 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/data_gherkin_pipeline.yaml
+-rw-r--r--   0        0        0      349 2024-03-22 20:05:39.992618 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/document-download.tsx
+-rw-r--r--   0        0        0     3006 2024-03-22 20:05:28.123693 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/document-preview.tsx
+-rw-r--r--   0        0        0     1100 2024-03-22 20:05:07.297217 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/document-upload.tsx
+-rw-r--r--   0        0        0      518 2024-03-22 20:06:01.209818 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/drag-and-drop-document-upload.tsx
+-rw-r--r--   0        0        0      601 2024-03-22 20:05:34.435880 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/email-confirmation-to-sender.tsx
+-rw-r--r--   0        0        0     1222 2024-03-22 20:05:15.968420 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/email-link-to-signer.tsx
+-rw-r--r--   0        0        0      165 2024-03-22 21:48:43.860621 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/feature_data_pipeline.yaml
+-rw-r--r--   0        0        0     1034 2024-03-22 20:05:10.629710 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/generate-unique-signing-link.tsx
+-rw-r--r--   0        0        0      938 2024-03-22 22:50:44.796129 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/generate_react_code_from_csv.py
+-rw-r--r--   0        0        0     1425 2024-03-22 21:56:34.158485 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/gherkin_pipeline.yaml
+-rw-r--r--   0        0        0     5785 2024-03-22 22:51:12.878045 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/hello-world.tsx
+-rw-r--r--   0        0        0      591 2024-03-22 20:06:07.775283 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/link-expiration.tsx
+-rw-r--r--   0        0        0     1965 2024-03-22 20:05:50.876254 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/mobile-responsive-design.tsx
+-rw-r--r--   0        0        0      776 2024-03-22 22:50:44.792289 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/retrieve_and_generate_pipeline.py
+-rw-r--r--   0        0        0      391 2024-03-22 20:05:29.257422 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/save-signature.tsx
+-rw-r--r--   0        0        0      816 2024-03-22 20:05:18.834156 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/signature-capture.tsx
+-rw-r--r--   0        0        0      786 2024-03-22 20:05:37.849509 dspygen-2024.3.8/src/dspygen/experiments/react_code_gen/signature-validation.tsx
+-rw-r--r--   0        0        0        0 2024-03-25 22:03:28.289166 dspygen-2024.3.8/src/dspygen/experiments/rfc5545/__init__.py
+-rw-r--r--   0        0        0    11768 2024-03-25 22:29:50.383113 dspygen-2024.3.8/src/dspygen/experiments/rfc5545/calendar_cmd.py
+-rw-r--r--   0        0        0     2819 2024-03-25 22:23:21.235474 dspygen-2024.3.8/src/dspygen/experiments/rfc5545/ical_crud.py
+-rw-r--r--   0        0        0      270 2024-03-25 23:26:22.009565 dspygen-2024.3.8/src/dspygen/experiments/rfc5545/ical_data_ret.py
+-rw-r--r--   0        0        0      442 2024-03-25 22:29:50.387492 dspygen-2024.3.8/src/dspygen/experiments/rfc5545/ical_db_session.py
+-rw-r--r--   0        0        0    14826 2024-03-25 22:40:54.333112 dspygen-2024.3.8/src/dspygen/experiments/rfc5545/ical_models.py
+-rw-r--r--   0        0        0      657 2024-03-25 23:13:36.660637 dspygen-2024.3.8/src/dspygen/experiments/rfc5545/ical_workbench.py
+-rw-r--r--   0        0        0     3246 2024-03-25 22:23:21.281848 dspygen-2024.3.8/src/dspygen/experiments/rfc5545/journal_cmd.py
+-rw-r--r--   0        0        0        0 2024-04-05 18:44:49.901569 dspygen-2024.3.8/src/dspygen/experiments/self_coding/__init__.py
+-rw-r--r--   0        0        0     2974 2024-04-05 18:55:05.235637 dspygen-2024.3.8/src/dspygen/experiments/self_coding/interview_processing.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:47:44.395017 dspygen-2024.3.8/src/dspygen/experiments/soonify_groq/__init__.py
+-rw-r--r--   0        0        0     2655 2024-03-31 02:44:23.421290 dspygen-2024.3.8/src/dspygen/experiments/soonify_groq/groq_pydantic.py
+-rw-r--r--   0        0        0     4831 2024-03-30 06:05:29.772724 dspygen-2024.3.8/src/dspygen/experiments/soonify_groq/run_groq_soon.py
+-rw-r--r--   0        0        0        0 2024-02-27 17:34:57.501846 dspygen-2024.3.8/src/dspygen/experiments/spider/__init__.py
+-rw-r--r--   0        0        0     2433 2024-03-10 19:31:23.056050 dspygen-2024.3.8/src/dspygen/experiments/spider/wiki_spider.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:52.784804 dspygen-2024.3.8/src/dspygen/experiments/wip/__init__.py
+-rw-r--r--   0        0        0     2463 2024-03-25 03:15:32.310428 dspygen-2024.3.8/src/dspygen/experiments/wip/chatgpt_conversation_parser.py
+-rw-r--r--   0        0        0      696 2024-03-22 20:32:29.232339 dspygen-2024.3.8/src/dspygen/experiments/wip/default_pipeline.yaml
+-rw-r--r--   0        0        0        0 2024-03-21 18:34:59.977792 dspygen-2024.3.8/src/dspygen/experiments/wip/models/__init__.py
+-rw-r--r--   0        0        0    11258 2024-03-06 18:55:42.474464 dspygen-2024.3.8/src/dspygen/experiments/wip/models/dsl_project.py
+-rw-r--r--   0        0        0     3117 2024-03-22 20:31:18.230063 dspygen-2024.3.8/src/dspygen/experiments/wip/one_shot_pipeline.py
+-rw-r--r--   0        0        0     7582 2024-03-07 23:15:34.216913 dspygen-2024.3.8/src/dspygen/experiments/wip/self_evolving_business_logic.py
+-rw-r--r--   0        0        0       23 2024-02-26 00:06:54.236649 dspygen-2024.3.8/src/dspygen/lm/__init__.py
+-rw-r--r--   0        0        0     1313 2024-03-19 22:46:23.571354 dspygen-2024.3.8/src/dspygen/lm/groq_lm.py
+-rw-r--r--   0        0        0     1367 2024-03-07 23:35:14.800514 dspygen-2024.3.8/src/dspygen/models/BPMN.yaml
+-rw-r--r--   0        0        0     1316 2024-03-07 23:39:50.809151 dspygen-2024.3.8/src/dspygen/models/CMMN.yaml
+-rw-r--r--   0        0        0        0 2024-03-07 23:26:46.354560 dspygen-2024.3.8/src/dspygen/models/__init__.py
+-rw-r--r--   0        0        0     2936 2024-03-07 23:43:49.167525 dspygen-2024.3.8/src/dspygen/models/bpm_plus_domain_models.py
+-rw-r--r--   0        0        0     1569 2024-03-07 23:28:31.491007 dspygen-2024.3.8/src/dspygen/models/cmmn_shipping.yaml
+-rw-r--r--   0        0        0      940 2024-03-07 23:29:59.479279 dspygen-2024.3.8/src/dspygen/models/dmn_shipping.yaml
+-rw-r--r--   0        0        0       70 2024-02-28 21:24:01.342202 dspygen-2024.3.8/src/dspygen/module_docstring_writer.py
+-rw-r--r--   0        0        0        0 2024-02-26 00:35:40.975772 dspygen-2024.3.8/src/dspygen/modules/__init__.py
+-rw-r--r--   0        0        0     1359 2024-03-06 21:47:41.881978 dspygen-2024.3.8/src/dspygen/modules/binary_output_module.py
+-rw-r--r--   0        0        0     1746 2024-03-15 17:14:35.127251 dspygen-2024.3.8/src/dspygen/modules/blog_module.py
+-rw-r--r--   0        0        0     2103 2024-03-11 17:17:35.452860 dspygen-2024.3.8/src/dspygen/modules/book_appointment_module.py
+-rw-r--r--   0        0        0     2186 2024-03-09 06:47:00.483042 dspygen-2024.3.8/src/dspygen/modules/bpmn2_bpel_module.py
+-rw-r--r--   0        0        0     1116 2024-03-10 00:19:11.772723 dspygen-2024.3.8/src/dspygen/modules/business_dev_consultant.py
+-rw-r--r--   0        0        0     2429 2024-03-06 21:51:35.362215 dspygen-2024.3.8/src/dspygen/modules/business_requirements.py
+-rw-r--r--   0        0        0     1151 2024-02-29 22:57:56.314686 dspygen-2024.3.8/src/dspygen/modules/chat_bot_cli.py
+-rw-r--r--   0        0        0     1920 2024-03-06 20:27:27.830710 dspygen-2024.3.8/src/dspygen/modules/chat_bot_module.py
+-rw-r--r--   0        0        0     1058 2024-03-02 20:39:42.067411 dspygen-2024.3.8/src/dspygen/modules/checker_module.py
+-rw-r--r--   0        0        0     4382 2024-03-21 18:41:05.605841 dspygen-2024.3.8/src/dspygen/modules/choose_function_module.py
+-rw-r--r--   0        0        0      931 2024-03-02 20:37:43.109995 dspygen-2024.3.8/src/dspygen/modules/cli_bot_module.py
+-rw-r--r--   0        0        0     1233 2024-03-06 21:36:42.927682 dspygen-2024.3.8/src/dspygen/modules/cobol_to_python_module.py
+-rw-r--r--   0        0        0     1185 2024-02-28 23:11:15.274057 dspygen-2024.3.8/src/dspygen/modules/dflss_module.py
+-rw-r--r--   0        0        0      859 2024-03-19 19:58:51.820852 dspygen-2024.3.8/src/dspygen/modules/dspygen_dsl_pipeline.py
+-rw-r--r--   0        0        0     3530 2024-03-19 19:57:31.629921 dspygen-2024.3.8/src/dspygen/modules/dspygen_module.py
+-rw-r--r--   0        0        0     1274 2024-03-09 04:45:40.331220 dspygen-2024.3.8/src/dspygen/modules/file_name_module.py
+-rw-r--r--   0        0        0     4301 2024-02-29 22:58:59.155830 dspygen-2024.3.8/src/dspygen/modules/gen_cli_module.py
+-rw-r--r--   0        0        0     2213 2024-03-13 21:36:40.801192 dspygen-2024.3.8/src/dspygen/modules/gen_dspy_module.py
+-rw-r--r--   0        0        0     5537 2024-03-21 18:41:05.655765 dspygen-2024.3.8/src/dspygen/modules/gen_keyword_arguments_module.py
+-rw-r--r--   0        0        0     1093 2024-03-06 18:39:40.232469 dspygen-2024.3.8/src/dspygen/modules/gen_message_module.py
+-rw-r--r--   0        0        0     1901 2024-03-24 01:14:21.643323 dspygen-2024.3.8/src/dspygen/modules/gen_module.py
+-rw-r--r--   0        0        0    14776 2024-03-24 01:15:05.616532 dspygen-2024.3.8/src/dspygen/modules/gen_pydantic_class.py
+-rw-r--r--   0        0        0    12450 2024-03-22 18:42:32.940850 dspygen-2024.3.8/src/dspygen/modules/gen_pydantic_instance.py
+-rw-r--r--   0        0        0     5555 2024-03-14 17:12:55.235395 dspygen-2024.3.8/src/dspygen/modules/gen_pydantic_instance_module.py
+-rw-r--r--   0        0        0     3354 2024-03-24 01:15:05.622689 dspygen-2024.3.8/src/dspygen/modules/gen_python_primitive.py
+-rw-r--r--   0        0        0     1266 2024-02-27 18:36:46.735620 dspygen-2024.3.8/src/dspygen/modules/gen_signature_module.py
+-rw-r--r--   0        0        0     4595 2024-03-10 19:34:51.822523 dspygen-2024.3.8/src/dspygen/modules/get_selector_module.py
+-rw-r--r--   0        0        0     1099 2024-03-13 17:33:07.082282 dspygen-2024.3.8/src/dspygen/modules/gusty_module.py
+-rw-r--r--   0        0        0      137 2024-03-14 20:25:40.720285 dspygen-2024.3.8/src/dspygen/modules/hello_world_module.yaml
+-rw-r--r--   0        0        0     1421 2024-03-01 00:09:40.059558 dspygen-2024.3.8/src/dspygen/modules/html_module.py
+-rw-r--r--   0        0        0     1935 2024-03-06 19:19:35.493962 dspygen-2024.3.8/src/dspygen/modules/insight_tweet_module.py
+-rw-r--r--   0        0        0     2869 2024-02-29 22:41:17.052232 dspygen-2024.3.8/src/dspygen/modules/js_to_fast_api_module.py
+-rw-r--r--   0        0        0    11103 2024-04-05 19:16:56.975488 dspygen-2024.3.8/src/dspygen/modules/json_module.py
+-rw-r--r--   0        0        0     1788 2024-03-08 19:32:52.410935 dspygen-2024.3.8/src/dspygen/modules/jsx_module.py
+-rw-r--r--   0        0        0     2732 2024-03-10 00:35:31.153393 dspygen-2024.3.8/src/dspygen/modules/mermaid_js_module.py
+-rw-r--r--   0        0        0     1325 2024-03-05 23:19:58.448963 dspygen-2024.3.8/src/dspygen/modules/message_module.py
+-rw-r--r--   0        0        0     1239 2024-02-28 23:01:46.923037 dspygen-2024.3.8/src/dspygen/modules/module_docstring_module.py
+-rw-r--r--   0        0        0      335 2024-03-13 21:29:49.228613 dspygen-2024.3.8/src/dspygen/modules/pipeline.yaml
+-rw-r--r--   0        0        0     1787 2024-02-28 22:54:13.437149 dspygen-2024.3.8/src/dspygen/modules/product_bot_module.py
+-rw-r--r--   0        0        0      819 2024-02-27 18:36:46.739395 dspygen-2024.3.8/src/dspygen/modules/prompt_function_call_module.py
+-rw-r--r--   0        0        0     1781 2024-02-29 23:34:11.666243 dspygen-2024.3.8/src/dspygen/modules/python_expert_module.py
+-rw-r--r--   0        0        0     1331 2024-03-29 18:26:49.386074 dspygen-2024.3.8/src/dspygen/modules/python_source_code_module.py
+-rw-r--r--   0        0        0     1781 2024-04-02 17:05:02.124767 dspygen-2024.3.8/src/dspygen/modules/pyts_module.py
+-rw-r--r--   0        0        0     1261 2024-03-12 22:56:41.301038 dspygen-2024.3.8/src/dspygen/modules/rails_code_module.py
+-rw-r--r--   0        0        0      849 2024-03-13 21:18:31.051517 dspygen-2024.3.8/src/dspygen/modules/react_jsx_module.py
+-rw-r--r--   0        0        0     1001 2024-02-26 01:12:15.433642 dspygen-2024.3.8/src/dspygen/modules/request_contract_module.py
+-rw-r--r--   0        0        0     5828 2024-02-26 22:44:59.095786 dspygen-2024.3.8/src/dspygen/modules/signature_factory.py
+-rw-r--r--   0        0        0     5949 2024-02-27 18:36:46.776118 dspygen-2024.3.8/src/dspygen/modules/signature_renderer.py
+-rw-r--r--   0        0        0     1744 2024-03-08 05:46:07.178290 dspygen-2024.3.8/src/dspygen/modules/source_code_pep8_docs_module.py
+-rw-r--r--   0        0        0      969 2024-03-02 04:49:31.676695 dspygen-2024.3.8/src/dspygen/modules/sql_query_module.py
+-rw-r--r--   0        0        0     2073 2024-03-06 20:50:04.369037 dspygen-2024.3.8/src/dspygen/modules/streamlit_bot_module.py
+-rw-r--r--   0        0        0     2165 2024-02-27 18:36:46.748854 dspygen-2024.3.8/src/dspygen/modules/subject_destination_audience_newsletter_article_module.py
+-rw-r--r--   0        0        0     1052 2024-03-05 21:45:44.059369 dspygen-2024.3.8/src/dspygen/modules/tax_return_agent.py
+-rw-r--r--   0        0        0      914 2024-03-02 04:36:30.821840 dspygen-2024.3.8/src/dspygen/modules/test.py
+-rw-r--r--   0        0        0     1486 2024-02-29 22:58:59.160532 dspygen-2024.3.8/src/dspygen/modules/test_chat_bot_cli.py
+-rw-r--r--   0        0        0      799 2024-02-27 18:36:46.746185 dspygen-2024.3.8/src/dspygen/modules/text_summary_module_module.py
+-rw-r--r--   0        0        0     1767 2024-03-01 20:56:18.178441 dspygen-2024.3.8/src/dspygen/modules/to_elixir_module.py
+-rw-r--r--   0        0        0     2330 2024-03-06 22:01:58.222761 dspygen-2024.3.8/src/dspygen/modules/usp_connect_ship_webhook.py
+-rw-r--r--   0        0        0        0 2024-03-06 20:57:56.031280 dspygen-2024.3.8/src/dspygen/pages/__init__.py
+-rw-r--r--   0        0        0      481 2024-03-09 06:48:49.354497 dspygen-2024.3.8/src/dspygen/pages/hello.py
+-rw-r--r--   0        0        0     1407 2024-03-08 05:44:22.663177 dspygen-2024.3.8/src/dspygen/pages/mqtt_page.py
+-rw-r--r--   0        0        0      481 2024-03-09 06:48:49.350671 dspygen-2024.3.8/src/dspygen/pages/remodeling.py
+-rw-r--r--   0        0        0       23 2024-02-26 00:06:54.236649 dspygen-2024.3.8/src/dspygen/rdddy/__init__.py
+-rw-r--r--   0        0        0    11110 2024-04-02 04:22:54.023768 dspygen-2024.3.8/src/dspygen/rdddy/abstract_actor.py
+-rw-r--r--   0        0        0     1185 2024-03-06 19:13:09.363700 dspygen-2024.3.8/src/dspygen/rdddy/abstract_aggregate.py
+-rw-r--r--   0        0        0      142 2024-03-06 19:08:39.704580 dspygen-2024.3.8/src/dspygen/rdddy/abstract_command.py
+-rw-r--r--   0        0        0      128 2024-03-06 19:08:39.694932 dspygen-2024.3.8/src/dspygen/rdddy/abstract_event.py
+-rw-r--r--   0        0        0     3278 2024-03-27 07:25:46.641437 dspygen-2024.3.8/src/dspygen/rdddy/abstract_message.py
+-rw-r--r--   0        0        0      674 2024-03-06 19:08:39.664583 dspygen-2024.3.8/src/dspygen/rdddy/abstract_policy.py
+-rw-r--r--   0        0        0      128 2024-03-06 19:08:39.729843 dspygen-2024.3.8/src/dspygen/rdddy/abstract_query.py
+-rw-r--r--   0        0        0      170 2024-03-08 05:41:58.821203 dspygen-2024.3.8/src/dspygen/rdddy/abstract_read_model.py
+-rw-r--r--   0        0        0      685 2024-03-06 19:08:39.713205 dspygen-2024.3.8/src/dspygen/rdddy/abstract_repository.py
+-rw-r--r--   0        0        0      548 2024-03-06 19:08:39.674028 dspygen-2024.3.8/src/dspygen/rdddy/abstract_saga.py
+-rw-r--r--   0        0        0      460 2024-02-23 01:33:09.223883 dspygen-2024.3.8/src/dspygen/rdddy/abstract_task.py
+-rw-r--r--   0        0        0      420 2024-02-19 01:34:08.066902 dspygen-2024.3.8/src/dspygen/rdddy/abstract_value_object.py
+-rw-r--r--   0        0        0      419 2024-02-23 01:33:09.225043 dspygen-2024.3.8/src/dspygen/rdddy/abstract_view.py
+-rw-r--r--   0        0        0    17021 2024-04-01 08:21:05.575368 dspygen-2024.3.8/src/dspygen/rdddy/actor_system.py
+-rw-r--r--   0        0        0       23 2024-02-26 00:06:54.236649 dspygen-2024.3.8/src/dspygen/rdddy/browser/__init__.py
+-rw-r--r--   0        0        0     2551 2024-03-31 03:53:07.646724 dspygen-2024.3.8/src/dspygen/rdddy/browser/browser_domain.py
+-rw-r--r--   0        0        0     4141 2024-03-31 17:09:51.319461 dspygen-2024.3.8/src/dspygen/rdddy/browser/browser_process_supervisor.py
+-rw-r--r--   0        0        0     5557 2024-03-06 19:08:39.691667 dspygen-2024.3.8/src/dspygen/rdddy/browser/browser_worker.py
+-rw-r--r--   0        0        0      118 2024-02-09 18:11:20.221150 dspygen-2024.3.8/src/dspygen/rdddy/browser/run_chatgpt.py
+-rw-r--r--   0        0        0      435 2024-02-23 01:33:09.263893 dspygen-2024.3.8/src/dspygen/rdddy/domain_exception.py
+-rw-r--r--   0        0        0     5148 2024-03-31 21:19:35.742799 dspygen-2024.3.8/src/dspygen/rdddy/event_storm_domain_specification_model.py
+-rw-r--r--   0        0        0     1028 2024-03-22 18:42:12.624042 dspygen-2024.3.8/src/dspygen/rdddy/event_storm_model.py
+-rw-r--r--   0        0        0        0 2024-03-21 23:06:59.266564 dspygen-2024.3.8/src/dspygen/rm/__init__.py
+-rw-r--r--   0        0        0     8165 2024-04-02 19:59:04.793927 dspygen-2024.3.8/src/dspygen/rm/chatgpt_chromadb_retriever.py
+-rw-r--r--   0        0        0     3240 2024-03-24 00:55:10.111810 dspygen-2024.3.8/src/dspygen/rm/code_retriever.py
+-rw-r--r--   0        0        0     4577 2024-04-02 17:34:22.274121 dspygen-2024.3.8/src/dspygen/rm/data_retriever.py
+-rw-r--r--   0        0        0     2433 2024-03-25 01:51:43.876427 dspygen-2024.3.8/src/dspygen/rm/doc_retriever.py
+-rw-r--r--   0        0        0      424 2024-03-24 00:18:31.794734 dspygen-2024.3.8/src/dspygen/rm/web_retriever.py
+-rw-r--r--   0        0        0       38 2024-03-15 16:42:08.325257 dspygen-2024.3.8/src/dspygen/signatures/__init__.py
+-rw-r--r--   0        0        0      400 2024-02-27 18:36:46.743576 dspygen-2024.3.8/src/dspygen/signatures/blog_article.py
+-rw-r--r--   0        0        0      425 2024-02-29 22:40:58.261052 dspygen-2024.3.8/src/dspygen/signatures/generate_answer.py
+-rw-r--r--   0        0        0      635 2024-03-14 18:08:24.827971 dspygen-2024.3.8/src/dspygen/signatures/signature.yaml
+-rw-r--r--   0        0        0     1972 2024-03-14 18:10:06.393883 dspygen-2024.3.8/src/dspygen/signatures/signature_dsl.py
+-rw-r--r--   0        0        0       23 2024-02-26 00:06:54.236649 dspygen-2024.3.8/src/dspygen/subcommands/__init__.py
+-rw-r--r--   0        0        0     2861 2024-03-09 07:09:53.961015 dspygen-2024.3.8/src/dspygen/subcommands/actor_cmd.py
+-rw-r--r--   0        0        0     1890 2024-03-02 20:28:07.641376 dspygen-2024.3.8/src/dspygen/subcommands/assert_cmd.py
+-rw-r--r--   0        0        0      993 2024-03-05 22:12:12.036819 dspygen-2024.3.8/src/dspygen/subcommands/browser_cmd.py
+-rw-r--r--   0        0        0     2795 2024-03-05 00:30:03.391323 dspygen-2024.3.8/src/dspygen/subcommands/cmd_cmd.py
+-rw-r--r--   0        0        0      385 2024-03-29 00:52:23.927863 dspygen-2024.3.8/src/dspygen/subcommands/code_cmd.py
+-rw-r--r--   0        0        0     2192 2024-03-03 01:56:27.502672 dspygen-2024.3.8/src/dspygen/subcommands/help.txt
+-rw-r--r--   0        0        0     3654 2024-03-03 01:56:42.132578 dspygen-2024.3.8/src/dspygen/subcommands/help_cmd.py
+-rw-r--r--   0        0        0      984 2024-03-23 23:46:34.455502 dspygen-2024.3.8/src/dspygen/subcommands/lm_cmd.py
+-rw-r--r--   0        0        0     2167 2024-03-15 20:19:12.163416 dspygen-2024.3.8/src/dspygen/subcommands/module_cmd.py
+-rw-r--r--   0        0        0     6944 2024-03-24 02:11:01.750166 dspygen-2024.3.8/src/dspygen/subcommands/pln_cmd.py
+-rw-r--r--   0        0        0      258 2024-03-29 07:26:42.117504 dspygen-2024.3.8/src/dspygen/subcommands/poet_cmd.py
+-rw-r--r--   0        0        0      810 2024-03-23 23:53:59.243352 dspygen-2024.3.8/src/dspygen/subcommands/rm_cmd.py
+-rw-r--r--   0        0        0      763 2024-02-29 05:00:18.699308 dspygen-2024.3.8/src/dspygen/subcommands/sig_cmd.py
+-rw-r--r--   0        0        0     2660 2024-03-02 20:25:11.427224 dspygen-2024.3.8/src/dspygen/subcommands/temp_assert.py
+-rw-r--r--   0        0        0     7129 2024-03-24 04:54:26.828382 dspygen-2024.3.8/src/dspygen/subcommands/wkf_cmd.py
+-rw-r--r--   0        0        0      786 2024-04-02 17:34:25.747665 dspygen-2024.3.8/src/dspygen/subcommands/wrt_cmd.py
+-rw-r--r--   0        0        0      612 2024-03-09 07:09:53.948906 dspygen-2024.3.8/src/dspygen/templates/actor_template.j2
+-rw-r--r--   0        0        0      187 2024-03-06 18:39:36.968464 dspygen-2024.3.8/src/dspygen/templates/dspy_module_cli_call.j2
+-rw-r--r--   0        0        0      146 2024-03-06 18:38:12.997867 dspygen-2024.3.8/src/dspygen/templates/dspy_module_def_call.j2
+-rw-r--r--   0        0        0      152 2024-03-06 18:38:13.008342 dspygen-2024.3.8/src/dspygen/templates/dspy_module_main.j2
+-rw-r--r--   0        0        0      240 2024-03-06 18:38:13.006205 dspygen-2024.3.8/src/dspygen/templates/dspy_module_route.j2
+-rw-r--r--   0        0        0      335 2024-03-06 20:44:11.743840 dspygen-2024.3.8/src/dspygen/templates/dspy_module_streamlit_input.j2
+-rw-r--r--   0        0        0      378 2024-03-14 18:12:55.465969 dspygen-2024.3.8/src/dspygen/templates/signature_class_def.j2
+-rw-r--r--   0        0        0     1622 2024-03-08 21:50:07.843205 dspygen-2024.3.8/src/dspygen/touch_models.sh
+-rw-r--r--   0        0        0      577 2024-01-05 00:57:34.041149 dspygen-2024.3.8/src/dspygen/typetemp/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 00:57:34.037457 dspygen-2024.3.8/src/dspygen/typetemp/environment/__init__.py
+-rw-r--r--   0        0        0     1043 2024-03-06 18:21:31.484739 dspygen-2024.3.8/src/dspygen/typetemp/environment/typed_environment.py
+-rw-r--r--   0        0        0      979 2024-03-06 18:21:31.472405 dspygen-2024.3.8/src/dspygen/typetemp/environment/typed_native_environment.py
+-rw-r--r--   0        0        0        0 2024-01-05 00:57:34.050547 dspygen-2024.3.8/src/dspygen/typetemp/extension/__init__.py
+-rw-r--r--   0        0        0    24023 2024-02-23 01:33:09.475294 dspygen-2024.3.8/src/dspygen/typetemp/extension/faker_extension.py
+-rw-r--r--   0        0        0     1098 2024-02-24 21:23:34.405664 dspygen-2024.3.8/src/dspygen/typetemp/extension/inflection_extension.py
+-rw-r--r--   0        0        0     1667 2024-03-30 00:47:00.867895 dspygen-2024.3.8/src/dspygen/typetemp/functional.py
+-rw-r--r--   0        0        0        0 2024-01-05 00:57:34.038203 dspygen-2024.3.8/src/dspygen/typetemp/template/__init__.py
+-rw-r--r--   0        0        0     2454 2024-02-27 18:36:46.776621 dspygen-2024.3.8/src/dspygen/typetemp/template/async_render_mixin.py
+-rw-r--r--   0        0        0    11207 2024-02-26 22:15:14.353910 dspygen-2024.3.8/src/dspygen/typetemp/template/dsl_project.py
+-rw-r--r--   0        0        0      241 2024-01-16 06:45:52.700831 dspygen-2024.3.8/src/dspygen/typetemp/template/python
+-rw-r--r--   0        0        0     1001 2024-02-19 00:24:51.709162 dspygen-2024.3.8/src/dspygen/typetemp/template/render_funcs.py
+-rw-r--r--   0        0        0     2160 2024-02-19 00:24:51.709222 dspygen-2024.3.8/src/dspygen/typetemp/template/render_mixin.py
+-rw-r--r--   0        0        0     3393 2024-02-26 22:16:42.440788 dspygen-2024.3.8/src/dspygen/typetemp/template/smart_template.py
+-rw-r--r--   0        0        0     5497 2024-02-26 22:15:14.342848 dspygen-2024.3.8/src/dspygen/typetemp/template/typed_injector.py
+-rw-r--r--   0        0        0     2348 2024-02-26 22:16:42.436845 dspygen-2024.3.8/src/dspygen/typetemp/template/typed_prompt.py
+-rw-r--r--   0        0        0     2590 2024-02-26 22:15:14.346792 dspygen-2024.3.8/src/dspygen/typetemp/template/typed_python_source.py
+-rw-r--r--   0        0        0     1042 2024-02-26 22:15:14.360081 dspygen-2024.3.8/src/dspygen/typetemp/template/typed_template.py
+-rw-r--r--   0        0        0       23 2024-03-27 07:08:24.965892 dspygen-2024.3.8/src/dspygen/utils/MyData.yaml
+-rw-r--r--   0        0        0       23 2024-02-26 00:41:24.402416 dspygen-2024.3.8/src/dspygen/utils/__init__.py
+-rw-r--r--   0        0        0     1698 2024-03-19 21:54:29.170775 dspygen-2024.3.8/src/dspygen/utils/cli_tools.py
+-rw-r--r--   0        0        0    12574 2024-02-23 01:33:09.514913 dspygen-2024.3.8/src/dspygen/utils/complete.py
+-rw-r--r--   0        0        0     2961 2024-02-19 00:24:51.709737 dspygen-2024.3.8/src/dspygen/utils/compression_tools.py
+-rw-r--r--   0        0        0       65 2024-03-18 22:04:12.863656 dspygen-2024.3.8/src/dspygen/utils/contact.yaml
+-rw-r--r--   0        0        0    25532 2024-02-26 22:19:25.120888 dspygen-2024.3.8/src/dspygen/utils/create_prompts.py
+-rw-r--r--   0        0        0     2197 2024-03-25 22:32:37.269236 dspygen-2024.3.8/src/dspygen/utils/crud_tools.py
+-rw-r--r--   0        0        0     1620 2024-03-25 22:26:03.804299 dspygen-2024.3.8/src/dspygen/utils/date_tools.py
+-rw-r--r--   0        0        0      202 2024-02-28 06:40:27.680268 dspygen-2024.3.8/src/dspygen/utils/dspy_tools.py
+-rw-r--r--   0        0        0      118 2024-02-09 18:11:20.285188 dspygen-2024.3.8/src/dspygen/utils/example.py
+-rw-r--r--   0        0        0     5062 2024-03-30 19:14:24.087606 dspygen-2024.3.8/src/dspygen/utils/file_tools.py
+-rw-r--r--   0        0        0     1061 2024-04-05 19:04:24.762447 dspygen-2024.3.8/src/dspygen/utils/json_tools.py
+-rw-r--r--   0        0        0     4684 2024-02-19 00:24:51.710023 dspygen-2024.3.8/src/dspygen/utils/models.py
+-rw-r--r--   0        0        0     1641 2024-03-18 20:47:13.418062 dspygen-2024.3.8/src/dspygen/utils/module_tools.py
+-rw-r--r--   0        0        0     1772 2024-03-31 02:27:32.229831 dspygen-2024.3.8/src/dspygen/utils/pydantic_tools.py
+-rw-r--r--   0        0        0     6605 2024-03-28 21:49:42.918677 dspygen-2024.3.8/src/dspygen/utils/yaml_tools.py
+-rw-r--r--   0        0        0        0 2024-03-24 01:47:26.098367 dspygen-2024.3.8/src/dspygen/workflow/__init__.py
+-rw-r--r--   0        0        0     1776 2024-03-24 01:59:32.026442 dspygen-2024.3.8/src/dspygen/workflow/control_flow_workflow.yaml
+-rw-r--r--   0        0        0     1885 2024-03-24 02:02:27.175746 dspygen-2024.3.8/src/dspygen/workflow/control_flow_workflow_output_new.yaml
+-rw-r--r--   0        0        0      956 2024-03-24 16:53:44.146892 dspygen-2024.3.8/src/dspygen/workflow/data_analysis_workflow.yaml
+-rw-r--r--   0        0        0      912 2024-03-24 16:07:38.248411 dspygen-2024.3.8/src/dspygen/workflow/data_preparation_workflow.yaml
+-rw-r--r--   0        0        0     2840 2024-03-24 16:51:23.170870 dspygen-2024.3.8/src/dspygen/workflow/workflow_engine.py
+-rw-r--r--   0        0        0     3765 2024-03-24 16:23:25.161746 dspygen-2024.3.8/src/dspygen/workflow/workflow_executor.py
+-rw-r--r--   0        0        0    10229 2024-03-26 17:26:21.603447 dspygen-2024.3.8/src/dspygen/workflow/workflow_models.py
+-rw-r--r--   0        0        0     1697 2024-03-24 04:08:37.211908 dspygen-2024.3.8/src/dspygen/workflow/workflow_router.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:24:56.447452 dspygen-2024.3.8/src/dspygen/writer/__init__.py
+-rw-r--r--   0        0        0      418 2024-04-02 17:36:44.639981 dspygen-2024.3.8/src/dspygen/writer/code_writer.py
+-rw-r--r--   0        0        0     3766 2024-03-28 23:05:23.285316 dspygen-2024.3.8/src/dspygen/writer/data_writer.py
+-rw-r--r--   0        0        0    10114 1970-01-01 00:00:00.000000 dspygen-2024.3.8/PKG-INFO
```

### Comparing `dspygen-2024.3.7/LICENSE` & `dspygen-2024.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/README.md` & `dspygen-2024.3.8/README.md`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/pyproject.toml` & `dspygen-2024.3.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "dspygen"
-version = "2024.3.7"
+version = "2024.3.8"
 description = "A Ruby on Rails style framework for the DSPy (Demonstrate, Search, Predict) project for Language Models like GPT, BERT, and LLama."
 authors = ["Sean Chatman <info@chatmangpt.com>"]
 readme = "README.md"
 repository = "https://github.com/seanchatmangpt/dspygen"
 
 [tool.poetry.scripts]  # https://python-poetry.org/docs/pyproject/#scripts
 dspygen = "dspygen.cli:app"
@@ -38,14 +38,29 @@
 reactivex = "^4.0.4"
 pytest-asyncio = "^0.23.5"
 playwright = "^1.41.2"
 python-dotenv = "^1.0.1"
 paho-mqtt = "^2.0.0"
 psutil = "^5.9.8"
 st-pages = "^0.4.5"
+pykka = "^4.0.2"
+ijson = "^3.2.3"
+munch = "^4.0.0"
+pandasql = "^0.7.3"
+sentify = "^0.7.4"
+ebooklib = "^0.18"
+python-docx = "^1.1.0"
+pypdf = "^4.1.0"
+sqlmodel = "^0.0.16"
+icontract = "^2.6.6"
+tzlocal = "^5.2"
+aiofiles = "^23.2.1"
+pydantic-settings = "^2.2.1"
+chromadb = "^0.4.24"
+anyio = "^4.3.0"
 
 [tool.poetry.group.test.dependencies]  # https://python-poetry.org/docs/master/managing-dependencies/
 coverage = { extras = ["toml"], version = ">=7.2.5" }
 mypy = ">=1.2.0"
 pre-commit = ">=3.3.1"
 pytest = ">=7.3.1"
 pytest-clarity = ">=1.0.1"
@@ -111,26 +126,29 @@
   help = "Serve a REST API"
   shell = """
     if [ $dev ]
     then {
       uvicorn \
         --host $host \
         --port $port \
+        --graceful-timeout 30 \
+        --keep-alive 30
+        --timeout 30 \
         --reload \
         dspygen.api:app
     } else {
       gunicorn \
         --access-logfile - \
         --bind $host:$port \
-        --graceful-timeout 10 \
-        --keep-alive 10 \
+        --graceful-timeout 30 \
+        --keep-alive 30 \
         --log-file - \
         --timeout 30 \
         --worker-class uvicorn.workers.UvicornWorker \
-        --workers 2 \
+        --workers 1 \
         dspygen.api:app
     } fi
     """
 
     [[tool.poe.tasks.api.args]]
     help = "Bind socket to this host (default: 0.0.0.0)"
     name = "host"
@@ -164,18 +182,18 @@
     [[tool.poe.tasks.app.args]]
     help = "Bind socket to this host (default: 0.0.0.0)"
     name = "host"
     options = ["--host"]
     default = "0.0.0.0"
 
     [[tool.poe.tasks.app.args]]
-    help = "Bind socket to this port (default: 8080)"
+    help = "Bind socket to this port (default: 80)"
     name = "port"
     options = ["--port"]
-    default = "8080"
+    default = "80"
 
   [tool.poe.tasks.docs]
   help = "Generate this package's docs"
   cmd = """
     pdoc
       --docformat $docformat
       --output-directory $outputdirectory
```

### Comparing `dspygen-2024.3.7/src/dspygen/api.py` & `dspygen-2024.3.8/src/dspygen/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,74 @@
 """dspygen REST API."""
-import importlib
-import logging
-import os
-from fastapi.middleware.cors import CORSMiddleware  # Import CORS middleware
+import datetime as dt
 
-
-import coloredlogs
-from fastapi import FastAPI
+from fastapi import FastAPI, Depends
 from fastapi.middleware.cors import CORSMiddleware  # Import CORS middleware
 
-
+from dspygen.experiments.convo_ddd.abstract_aggregate.conversation_aggregate import ConversationAggregate
+from dspygen.experiments.convo_ddd.abstract_event.user_input_received_event import UserInputReceivedEvent
+from dspygen.rdddy.abstract_command import AbstractCommand
+from dspygen.rdddy.actor_system import ActorSystem
 from dspygen.utils.file_tools import dspy_modules_dir
+from dspygen.workflow.workflow_router import router as workflow_router
+
 
 app = FastAPI()
 
 
 from importlib import import_module
 import os
 
+from dspygen.dsl.dsl_pipeline_executor import router as pipeline_router
+
+
+@app.on_event("startup")
+async def startup_event():
+    await get_actor_system()
+
+
+app.include_router(pipeline_router)
+app.include_router(workflow_router)
+
 
 def load_module_routers(app: FastAPI):
     for filename in os.listdir(dspy_modules_dir()):
         if filename.endswith(".py"):
             module_name = filename[:-3]
             module = import_module(f"dspygen.modules.{module_name}")
             if hasattr(module, "router"):
                 app.include_router(module.router)
 
 
-@app.on_event("startup")
-def startup_event() -> None:
-    """Run API startup events."""
-    # Remove all handlers associated with the root logger object.
-    for handler in logging.root.handlers:
-        logging.root.removeHandler(handler)
-    # Add coloredlogs' coloured StreamHandler to the root logger.
-    coloredlogs.install()
-    load_module_routers(app)
+async def get_actor_system():
+    global actor_system
 
+    try:
+        actor_system
+    except NameError:
+        actor_system = ActorSystem(mqtt_broker="9.tcp.ngrok.io", mqtt_port=24651)
+
+    return actor_system  # Assume actor_system is globally available
 
 
 @app.get("/")
-def read_root() -> str:
+async def read_root(user_input: str, asys: ActorSystem = Depends(get_actor_system)):
     """Read root."""
-    return "Hello world"
+    convo_agg: ConversationAggregate = await asys.actor_of(ConversationAggregate)
+    msg = await convo_agg.handle_user_input(UserInputReceivedEvent(content=user_input))
+    return msg.model_dump()
 
 
 # Define endpoint
 @app.get("/pingpong")
 def ping_pong():
     return {"message": "pong"}
 
+
 # Add CORS middleware
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],  # Adjust this to your specific origins if needed
     allow_credentials=True,
     allow_methods=["GET", "POST", "PUT", "DELETE", "OPTIONS"],  # Adjust as per your requirements
     allow_headers=["*"],  # Adjust this to your specific headers if needed
 )
-
```

### Comparing `dspygen-2024.3.7/src/dspygen/app.py` & `dspygen-2024.3.8/src/dspygen/dspygen_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from importlib.metadata import version
 
 import streamlit as st
 
 from dspygen.modules.chat_bot_module import chat_bot_call
 from dspygen.modules.insight_tweet_module import insight_tweet_call
-from dspygen.modules.streamlit_bot import streamlit_bot_call
+from dspygen.modules.streamlit_bot_module import streamlit_bot_call
 from dspygen.utils.dspy_tools import init_dspy
 from dspygen.utils.file_tools import source_dir, pages_dir
 
 st.title(f"dspygen v{version('dspygen')}")  # type: ignore[no-untyped-call]
 
 
 # # Streamlit form and display
```

### Comparing `dspygen-2024.3.7/src/dspygen/async_typer.py` & `dspygen-2024.3.8/src/dspygen/async_typer.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/commit-msg.sample` & `dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/fsmonitor-watchman.sample` & `dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/pre-commit.sample` & `dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/pre-push.sample` & `dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/pre-rebase.sample` & `dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/pre-receive.sample` & `dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/prepare-commit-msg.sample` & `dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/push-to-checkout.sample` & `dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/hooks/update.sample` & `dspygen-2024.3.8/src/dspygen/experiments/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/index` & `dspygen-2024.3.8/src/dspygen/experiments/.git/index`

 * *Files 26% similar despite different names*

#### Comparing `/tmp/diffoscope_vqno520u_/tmplzahyj_u_TarContainer/0/25` & `/tmp/diffoscope_vqno520u_/tmpm5qhf6t6_TarContainer/0/68`

```diff
@@ -65,25 +65,14 @@
 User ID:   501
 Group ID:  20
 Created:   1709412713.374035561
 Modified:  1709412713.373919853
 Inode:     55399674
 Device ID: (0, 4113)
 
-Path:      b'abstract_aggregate/main_aggregate.py'
-SHA:       e69de29bb2d1d6434b8b29ae775ad8c2e48c5391
-Size:      0
-Flags:     0b100100
-User ID:   501
-Group ID:  20
-Created:   1709752643.553592078
-Modified:  1709752643.553592078
-Inode:     57302199
-Device ID: (0, 4113)
-
 Path:      b'abstract_renderer.py'
 SHA:       1ed7c76971abff4a041741b96643e4bbe493bd3f
 Size:      3815
 Flags:     0b10100
 User ID:   501
 Group ID:  20
 Created:   1709751714.245469016
@@ -142,14 +131,47 @@
 User ID:   501
 Group ID:  20
 Created:   1709249651.662934855
 Modified:  1709249651.662934855
 Inode:     55157101
 Device ID: (0, 4113)
 
+Path:      b'data_pipeline.yaml'
+SHA:       e69de29bb2d1d6434b8b29ae775ad8c2e48c5391
+Size:      0
+Flags:     0b10010
+User ID:   501
+Group ID:  20
+Created:   1710463578.918249746
+Modified:  1710463578.918249746
+Inode:     60095961
+Device ID: (0, 4114)
+
+Path:      b'dsl_pipeline.py'
+SHA:       e69de29bb2d1d6434b8b29ae775ad8c2e48c5391
+Size:      0
+Flags:     0b1111
+User ID:   501
+Group ID:  20
+Created:   1710454378.670108396
+Modified:  1710454378.670108396
+Inode:     60062969
+Device ID: (0, 4114)
+
+Path:      b'example_pipeline.yaml'
+SHA:       e69de29bb2d1d6434b8b29ae775ad8c2e48c5391
+Size:      0
+Flags:     0b10101
+User ID:   501
+Group ID:  20
+Created:   1710454394.611021765
+Modified:  1710454394.611021765
+Inode:     60063000
+Device ID: (0, 4114)
+
 Path:      b'file_path.py'
 SHA:       e69de29bb2d1d6434b8b29ae775ad8c2e48c5391
 Size:      0
 Flags:     0b1100
 User ID:   501
 Group ID:  20
 Created:   1709758950.117644267
```

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/07/2c395e5a1a2fda1ebd81855a0857a4c349aba9` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/07/2c395e5a1a2fda1ebd81855a0857a4c349aba9`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/1e/d7c76971abff4a041741b96643e4bbe493bd3f` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/1e/d7c76971abff4a041741b96643e4bbe493bd3f`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/29/790e08d481fbcf9876f5e09e8618e0c6ff2cf4` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/29/790e08d481fbcf9876f5e09e8618e0c6ff2cf4`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/34/484ad0f39e38772282a9bb02ba1df4f056b1f7` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/34/484ad0f39e38772282a9bb02ba1df4f056b1f7`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/38/a98b391b7a6e8e740cae9681b5f0b295848fcc` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/38/a98b391b7a6e8e740cae9681b5f0b295848fcc`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/46/ed8e6d6b3d12b5bf9028d0777450412497d2aa` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/46/ed8e6d6b3d12b5bf9028d0777450412497d2aa`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/63/e5b4dd95ed8214e4f3167d66b2b139f49b0b04` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/63/e5b4dd95ed8214e4f3167d66b2b139f49b0b04`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/85/97acd78f726e8277a086b8a78d6d77c82f4d2c` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/85/97acd78f726e8277a086b8a78d6d77c82f4d2c`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/89/80972d4e4fe721d9a4b66d38500a387cd5d677` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/89/80972d4e4fe721d9a4b66d38500a387cd5d677`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/90/838848601a0b18aafe0f31edb678a2f801f0f2` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/90/838848601a0b18aafe0f31edb678a2f801f0f2`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/97/8bd6af4ad3a34e4016af33f921e416a723518a` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/97/8bd6af4ad3a34e4016af33f921e416a723518a`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/9f/3b783e2f90a73bacc366d57205db068a1f130a` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/9f/3b783e2f90a73bacc366d57205db068a1f130a`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/a4/f3e1b596347a141fde89a09e19348524331fb1` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/a4/f3e1b596347a141fde89a09e19348524331fb1`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/a5/1355a31ec94b448a81fe23cd03407e6db9fb98` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/a5/1355a31ec94b448a81fe23cd03407e6db9fb98`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/a7/f8004ca3e4019a0813e6d37454a9a1d4633732` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/a7/f8004ca3e4019a0813e6d37454a9a1d4633732`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/ae/864cd37388df8a496b2e62caa5bdb338e22de8` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/ae/864cd37388df8a496b2e62caa5bdb338e22de8`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/af/54a3d8766d0686126ba2e2b3206b8270f1d5ef` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/af/54a3d8766d0686126ba2e2b3206b8270f1d5ef`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/b9/0e196ece0bb3c298e1565c9e5ba065ae468d74` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/b9/0e196ece0bb3c298e1565c9e5ba065ae468d74`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/bd/3ea467b227c44e9d5a1d687beef7d6d5f02f4d` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/bd/3ea467b227c44e9d5a1d687beef7d6d5f02f4d`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/d2/5ac35cbee6a13431d6769e22c0eac72f5ed551` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/d2/5ac35cbee6a13431d6769e22c0eac72f5ed551`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/d2/a1225cf1aa018c446ce1274a87eecb37294e03` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/d2/a1225cf1aa018c446ce1274a87eecb37294e03`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/da/938270af8aa8e1b6655c68dc10042c01526cf7` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/da/938270af8aa8e1b6655c68dc10042c01526cf7`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/.git/objects/fc/d9f4d1c396f872cc2f80e1599b961223430558` & `dspygen-2024.3.8/src/dspygen/experiments/.git/objects/fc/d9f4d1c396f872cc2f80e1599b961223430558`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/Chinook.db` & `dspygen-2024.3.8/src/dspygen/experiments/function_calling/Chinook.db`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/abstract_renderer.py` & `dspygen-2024.3.8/src/dspygen/experiments/convo_ddd/abstract_renderer.py`

 * *Files 25% similar despite different names*

```diff
@@ -38,67 +38,71 @@
                 base_class_name=base_class_name, classname=classname
             )()
 
 
 def main():
     event_storm_model_data = {
         "domain_event_classnames": [
-            "OrderPlaced",
-            "PaymentProcessed",
-            "InventoryUpdated",
+            "IntentRecognizedEvent", "EntityRecognizedEvent",
+            "ContextUpdatedEvent", "StateTransitionEvent",
+            "UserQueryHandledEvent", "ResponseGeneratedEvent"
         ],
         "external_event_classnames": [
-            "ExternalPaymentConfirmation",
-            "SupplierInventoryUpdate",
-            "SupplierInventoryConfirmation",
+            "UserInputReceivedEvent", "ExternalAPIResponseEvent",
+            "SystemInterruptEvent"
+        ],
+        "command_classnames": [
+            "RecognizeIntentCommand", "RecognizeEntityCommand",
+            "UpdateContextCommand", "TransitionStateCommand",
+            "GenerateResponseCommand", "HandleUserQueryCommand"
+        ],
+        "query_classnames": [
+            "GetCurrentContextQuery", "GetIntentDetailsQuery",
+            "GetEntityDetailsQuery", "GetCurrentStateQuery"
         ],
-        "command_classnames": ["PlaceOrder", "ProcessPayment", "UpdateInventory"],
-        "query_classnames": ["GetOrderDetails", "ListBooks", "CheckOrderStatus"],
         "aggregate_classnames": [
-            "OrderAggregate",
-            "BookAggregate",
-            "CustomerAggregate",
+            "ConversationAggregate"
         ],
         "policy_classnames": [
-            "OrderCancellationPolicy",
-            "RefundPolicy",
-            "ShippingPolicy",
+            "IntentHandlingPolicy", "EntityRecognitionPolicy",
+            "ContextManagementPolicy", "StateTransitionPolicy",
+            "ResponseGenerationPolicy"
         ],
         "read_model_classnames": [
-            "OrderSummaryReadModel",
-            "BookCatalogReadModel",
-            "CustomerOrderHistoryReadModel",
+            "IntentReadModel", "EntityReadModel",
+            "ContextSnapshotReadModel", "StateReadModel",
+            "ResponseReadModel"
+        ],
+        "view_classnames": [
+            "IntentView", "EntityView", "ContextView",
+            "StateView", "ResponseView"
         ],
-        "view_classnames": ["OrderDetailsView", "BookListView", "CustomerProfileView"],
         "ui_event_classnames": [
-            "AddToCartButtonClick",
-            "CheckoutFormSubmitted",
-            "OrderHistoryPageLoaded",
+            "UserMessageSubmittedEvent", "SystemMessageDisplayedEvent"
         ],
         "saga_classnames": [
-            "OrderFulfillmentSaga",
-            "PaymentProcessingSaga",
-            "BookRestockSaga",
+            "ConversationHandlingSaga"
         ],
         "integration_event_classnames": [
-            "OrderPlacedIntegrationEvent",
-            "PaymentProcessedIntegrationEvent",
-            "InventoryUpdatedIntegrationEvent",
+            "ExternalServiceCalledEvent", "DatabaseQueriedEvent"
         ],
         "exception_classnames": [
-            "OrderNotFoundException",
-            "PaymentDeclinedException",
-            "BookOutOfStockException",
+            "IntentNotFoundException", "EntityRecognitionException",
+            "ContextUpdateException", "InvalidStateException",
+            "ResponseGenerationException"
+        ],
+        "value_object_classnames": [
+            "IntentValueObject", "EntityValueObject",
+            "ContextValueObject", "StateValueObject",
+            "ResponseValueObject"
         ],
-        "value_object_classnames": ["Address", "Price", "Quantity"],
         "task_classnames": [
-            "ValidateOrder",
-            "CalculateShippingCosts",
-            "SendOrderConfirmationEmail",
-        ],
+            "ProcessUserInputTask", "GenerateDialogueResponseTask",
+            "UpdateConversationContextTask", "ManageStateTransitionsTask"
+        ]
     }
 
     event_storm_model = EventStormingDomainSpecificationModel.model_validate(
         event_storm_model_data
     )
 
     generate_class_definitions(event_storm_model)
```

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/function_call.py` & `dspygen-2024.3.8/src/dspygen/experiments/function_calling/function_call.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/gen_module.py` & `dspygen-2024.3.8/src/dspygen/modules/gen_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/gen_pydantic_class.py` & `dspygen-2024.3.8/src/dspygen/modules/gen_pydantic_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inflection
 from pydantic import BaseModel, Field
 
 import dspy
 from dspy import InputField, OutputField, Signature
 
-from dspygen.experiments.gen_pydantic_instance import GenPydanticInstance
+from dspygen.modules.gen_pydantic_instance import GenPydanticInstance
 from dspygen.typetemp.functional import render
 
 
 class FieldTemplateSpecificationModel(BaseModel):
     field_name: str = Field(
         ...,
         description="The name of the field in the model. No prefixes, suffixes, or abbreviations.",
```

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/gen_python_primitive.py` & `dspygen-2024.3.8/src/dspygen/modules/gen_python_primitive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 
 from dspy import Assert
 
-from dspygen.experiments.gen_module import GenModule
+from dspygen.modules.gen_module import GenModule
 from dspygen.utils.dspy_tools import init_dspy
 
 
 def is_primitive_type(data_type):
     primitive_types = {int, float, str, bool, list, tuple, dict, set}
 
     return data_type in primitive_types
@@ -46,72 +46,103 @@
 
 
 class GenDict(GenPythonPrimitive):
     def __init__(self):
         super().__init__(primitive_type=dict)
 
 
+def gen_dict(prompt):
+    return GenDict()(prompt)
+
+
 class GenList(GenPythonPrimitive):
     def __init__(self):
         super().__init__(primitive_type=list)
 
 
 def gen_list(prompt):
     return GenList()(prompt)
 
+
 class GenBool(GenPythonPrimitive):
     def __init__(self):
         super().__init__(primitive_type=bool)
 
 
 def gen_bool(prompt):
     return GenBool()(prompt)
 
 
 class GenInt(GenPythonPrimitive):
     def __init__(self):
         super().__init__(primitive_type=int)
 
 
+def gen_int(prompt):
+    return GenInt()(prompt)
+
+
 class GenFloat(GenPythonPrimitive):
     def __init__(self):
         super().__init__(primitive_type=float)
 
 
+def gen_float(prompt):
+    return GenFloat()(prompt)
+
+
 class GenTuple(GenPythonPrimitive):
     def __init__(self):
         super().__init__(primitive_type=tuple)
 
 
+def gen_tuple(prompt):
+    return GenTuple()(prompt)
+
+
 class GenSet(GenPythonPrimitive):
     def __init__(self):
         super().__init__(primitive_type=set)
 
 
+def gen_set(prompt):
+    return GenSet()(prompt)
+
+
 class GenStr(GenPythonPrimitive):
     def __init__(self):
         super().__init__(primitive_type=str)
 
 
+def gen_str(prompt):
+    return GenStr()(prompt)
+
+
 def main():
     init_dspy()
 
-    result = GenTuple()(
+    result = gen_list(
         "Create a list of planets in our solar system sorted by largest to smallest"
     )
 
-    assert result == (
+    assert result == [
         "Jupiter",
         "Saturn",
         "Uranus",
         "Neptune",
         "Earth",
         "Venus",
         "Mars",
         "Mercury",
-    )
+    ]
 
     print(f"The planets of the solar system are {result}")
 
+    for planet in result:
+        print(planet)
+
+    if gen_bool(f"Is {result[0]} the largest planet in the solar system?"):
+        print(f"{result[0]} is the largest planet in the solar system")
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/gherkin_parser.py` & `dspygen-2024.3.8/src/dspygen/experiments/done/gherkin_parser.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/lm_call.py` & `dspygen-2024.3.8/src/dspygen/experiments/done/lm_call.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/models/dsl_project.py` & `dspygen-2024.3.8/src/dspygen/experiments/wip/models/dsl_project.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/openai_ror_cli.py` & `dspygen-2024.3.8/src/dspygen/experiments/done/openai_ror_cli.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/python_to_elixir.py` & `dspygen-2024.3.8/src/dspygen/experiments/done/python_to_elixir.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/self_evolving_business_logic.py` & `dspygen-2024.3.8/src/dspygen/experiments/wip/self_evolving_business_logic.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/socket_actor_system.py` & `dspygen-2024.3.8/src/dspygen/experiments/done/socket_actor_system.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/spider/wiki_spider.py` & `dspygen-2024.3.8/src/dspygen/experiments/spider/wiki_spider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from playwright.sync_api import sync_playwright
 
-from dspygen.modules.get_selector import get_selector_call
+from dspygen.modules.get_selector_module import get_selector_call
 from dspygen.utils.dspy_tools import init_dspy
 
 
 def find_all_inputs(page):
     """
     Finds all input elements on a given Playwright page.
 
@@ -50,15 +50,15 @@
 
 def main(goal):
     init_dspy()
 
     with sync_playwright() as p:
         browser = p.chromium.launch(headless=False)
         page = browser.new_page()
-        page.goto("https://en.wikipedia.org/wiki/Main_Page")
+        page.goto("https://google.com")
 
         inputs = find_all_inputs(page)
 
         selector = get_selector_call(str(inputs), prompt="search box")
 
         search_box = page.query_selector(selector)
```

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/sql_calling_asserts.py` & `dspygen-2024.3.8/src/dspygen/experiments/function_calling/sql_calling_asserts.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/sql_optimization_function.py` & `dspygen-2024.3.8/src/dspygen/experiments/function_calling/sql_optimization_function.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sqlite3
 
-from dspygen.experiments.lm_call import call
 from dspygen.utils.dspy_tools import init_dspy
+from dspygen.utils.pydantic_tools import InstanceMixin
+from dspygen.utils.yaml_tools import YAMLMixin
 
 # Assuming Chinook.db is located in the same directory for simplicity
 conn = sqlite3.connect("Chinook.db")
 
 poor_query = """WITH recursive cte_dates AS (
   SELECT 
     DATEADD(day, 1, MIN(order_date)) AS dt
@@ -68,28 +69,24 @@
 from pydantic import BaseModel
 
 
 class SQLQueryModel(BaseModel):
     query: str
 
 
-class OptimizedSQLQueryModel(BaseModel):
+class OptimizedSQLQueryModel(BaseModel, InstanceMixin, YAMLMixin):
     rationale: str
     optimized_query: str
 
 
-def sql_query_optimizer() -> OptimizedSQLQueryModel:
-    """Optimize the given SQL query"""
-
-
 def main():
-    init_dspy(max_tokens=3000)
+    init_dspy(max_tokens=3000, model="gpt-4")
 
     # result = invoke("What is the name of the album with the most tracks and count?", question_to_chinook_query)
 
-    result = call(sql_query_optimizer, poor_query)
+    result = OptimizedSQLQueryModel.to_inst(poor_query)
 
     print(result)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/test_openai_ror_cli.py` & `dspygen-2024.3.8/src/dspygen/experiments/done/test_openai_ror_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typer.testing import CliRunner
 
-from dspygen.experiments.openai_ror_cli import app
+from dspygen.experiments.done.openai_ror_cli import app
 
 runner = CliRunner()
 
 def test_create():
     result = runner.invoke(app, ["create"])
     assert result.exit_code == 0
     assert "This is the create command." in result.output  # Replace with specific expected output
```

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/weather_function_calling_asserts.py` & `dspygen-2024.3.8/src/dspygen/experiments/function_calling/weather_function_calling_asserts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dspygen.experiments.function_call import get_current_weather, get_n_day_weather_forecast
+from dspygen.experiments.function_calling.function_call import get_current_weather, get_n_day_weather_forecast
 from dspygen.modules.choose_function_module import choose_function_call
 from dspygen.modules.gen_keyword_arguments_module import gen_keyword_arguments_call
 from dspygen.utils.dspy_tools import init_dspy
 
 
 def chose_and_invoke(prompt, function_list):
     fn = choose_function_call(prompt=prompt, function_list=function_list)
```

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/weather_functions.exs` & `dspygen-2024.3.8/src/dspygen/experiments/function_calling/weather_functions.exs`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/experiments/workflow_engine.py` & `dspygen-2024.3.8/src/dspygen/workflow/workflow_engine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,69 @@
-from dspygen.modules.insight_tweet_module import insight_tweet_call
+from pydantic import Field
+
 from dspygen.rdddy.abstract_actor import AbstractActor
 from dspygen.rdddy.abstract_command import AbstractCommand
 from dspygen.rdddy.abstract_event import AbstractEvent
 from dspygen.rdddy.abstract_query import AbstractQuery
 from dspygen.rdddy.actor_system import ActorSystem
 from dspygen.utils.dspy_tools import init_dspy
+from dspygen.workflow.workflow_executor import execute_workflow
+from dspygen.workflow.workflow_models import Workflow
 
+from loguru import logger
 
 class StatusQuery(AbstractQuery):
     """Find out the status of the workflow engine."""
 
 
 class StartCommand(AbstractCommand):
     """Start the workflow."""
+    wf_path: str = Field(..., description="Path to the workflow YAML file.")
 
 
 class StopCommand(AbstractCommand):
     """Stop the workflow."""
 
 
 class StatusEvent(AbstractEvent):
     """Status has changed."""
 
 
 class JobCommand(AbstractCommand):
     tasks: list[str]
 
 
-class TweetEvent(AbstractEvent):
-    """Tweets has been generated."""
-
-
 class WorkflowEngine(AbstractActor):
     def __init__(self, actor_system, actor_id=None):
         super().__init__(actor_system, actor_id)
         self.status = "idle"
 
     async def handle_status(self, query: StatusQuery):
         print(f"Status: {self.status}")
 
     async def handle_start(self, command: StartCommand):
-        self.status = "waiting"
-        print("Starting workflow engine...")
+        if self.status != "idle":
+            print("Workflow engine is not idle.")
+            return
+
+        self.status = "loading"
+        print("Loading workflow from YAML...")
+        try:
+            await self.publish(StatusEvent(content=self.status))
+            print("Workflow is running...")
+            wf = Workflow.from_yaml(command.wf_path)
+            context = execute_workflow(wf)
+
+            await self.publish(StatusEvent(content=self.status))
+
+            # Optionally, use the context for further actions or status updates
+        except Exception as e:
+            logger.error(f"Failed to load or execute workflow: {e}")
+            self.status = "error"
+
         await self.publish(StatusEvent(content=self.status))
 
     async def handle_stop(self, command: StopCommand):
         self.status = "idle"
         print("Stop workflow engine...")
         await self.publish(StatusEvent(content=self.status))
 
@@ -53,31 +71,26 @@
         init_dspy()
 
         if self.status != "waiting":
             print("Not ready.")
             return
 
         for task in command.tasks:
-            text = insight_tweet_call(task)
-            await self.publish(TweetEvent(content=f"twitter-cli tweet='{text}'"))
+            print(task)
 
         print("Tasks done.")
         await self.publish(StopCommand())
 
 
-
-
 async def main():
     asys = ActorSystem()
     engine = await asys.actor_of(WorkflowEngine)
 
-    await asys.publish(StartCommand())
-    # await asys.publish(StatusQuery())
-    await asys.publish(JobCommand(tasks=["Elon Musk is a Lizard Person, prove me wrong?",
-                                         "I am the smartest all time. Thomas Edison Quote"]))
+    wf_path = "/Users/candacechatman/dev/dspygen/src/dspygen/workflow/data_analysis_workflow.yaml"
+    await asys.publish(StartCommand(wf_path=wf_path))
 
     while True:
         await asyncio.sleep(5)
 
 
 if __name__ == '__main__':
     import asyncio
```

### Comparing `dspygen-2024.3.7/src/dspygen/lm/groq_lm.py` & `dspygen-2024.3.8/src/dspygen/lm/groq_lm.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             ],
             model=self.kwargs.get("model", "mixtral-8x7b-32768"),
         )
         return [chat_completion.choices[0].message.content]
 
 
 def main():
-    # init_dspy(Groq, model="llama2-70b-4096", max_tokens=2000)
-    init_dspy(max_tokens=2000)
+    init_dspy(Groq, model="llama2-70b-4096", max_tokens=2000)
+    # init_dspy(max_tokens=2000)
     pred = dspy.Predict("prompt -> code")(prompt="Fast API CRUD endpoint for fire alarm global IoT network")
     print(pred.code)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `dspygen-2024.3.7/src/dspygen/models/BPMN.yaml` & `dspygen-2024.3.8/src/dspygen/models/BPMN.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/models/CMMN.yaml` & `dspygen-2024.3.8/src/dspygen/models/CMMN.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/models/bpm_plus_domain_models.py` & `dspygen-2024.3.8/src/dspygen/models/bpm_plus_domain_models.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/models/cmmn_shipping.yaml` & `dspygen-2024.3.8/src/dspygen/models/cmmn_shipping.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/models/dmn_shipping.yaml` & `dspygen-2024.3.8/src/dspygen/models/dmn_shipping.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/binary_output.py` & `dspygen-2024.3.8/src/dspygen/modules/binary_output_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/blog_module.py` & `dspygen-2024.3.8/src/dspygen/modules/blog_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     subject = dspy.InputField(desc="The main subject or topic for the blog article.")
 
     markdown_blog_article = dspy.OutputField(desc="Generated blog article in markdown format.", prefix="```markdown")
 
 
 class BlogModule(dspy.Module):
     """BlogModule"""
+    def __init__(self, *args, **kwargs):
+        super().__init__()
 
     def forward(self, subject):
         pred = dspy.ChainOfThought(BlogArticleGenerationSignature)
         result = pred(subject=subject).markdown_blog_article
         return result
```

### Comparing `dspygen-2024.3.7/src/dspygen/modules/book_appointment_module.py` & `dspygen-2024.3.8/src/dspygen/modules/book_appointment_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     def forward(self, requested_date, availability):
         pred = dspy.Predict("requested_date, availability -> is_booked")
         result = pred(requested_date=requested_date, availability=availability).is_booked
         return result
 
 
 def book_appointment_call(requested_date, availability):
+    # SQLModel, Chromadb
     book_appointment = BookAppointmentModule()
     return book_appointment.forward(requested_date=requested_date, availability=availability)
 
 
 @app.command()
 def call(requested_date, availability):
     """BookAppointmentModule"""
```

### Comparing `dspygen-2024.3.7/src/dspygen/modules/business_dev_consultant.py` & `dspygen-2024.3.8/src/dspygen/modules/business_dev_consultant.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 app = Typer()        
 
 
 class BusinessDevConsultantModule(dspy.Module):
     """BusinessDevConsultantModule"""
 
     def forward(self, prompt):
-        pred = dspy.Predict("prompt -> advice")
+        pred = dspy.ChainOfThought("prompt -> advice")
         result = pred(prompt=prompt).advice
         return result
 
 
 def business_dev_consultant_call(prompt):
     business_dev_consultant = BusinessDevConsultantModule()
     return business_dev_consultant.forward(prompt=prompt)
```

### Comparing `dspygen-2024.3.7/src/dspygen/modules/business_requirements.py` & `dspygen-2024.3.8/src/dspygen/modules/business_requirements.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/chat_bot_cli.py` & `dspygen-2024.3.8/src/dspygen/modules/chat_bot_cli.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/chat_bot_module.py` & `dspygen-2024.3.8/src/dspygen/modules/chat_bot_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/checker_module.py` & `dspygen-2024.3.8/src/dspygen/modules/checker_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/choose_function_module.py` & `dspygen-2024.3.8/src/dspygen/modules/choose_function_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 function_list parameters. The TODO comments indicate future plans for the code, including adding a streamlit
 component and a FastAPI route."""
 from typing import Callable
 
 import dspy
 from typer import Typer
 
-from dspygen.experiments.function_call import get_current_weather, get_n_day_weather_forecast
+from dspygen.experiments.function_calling.function_call import get_current_weather, get_n_day_weather_forecast
 from dspygen.utils.dspy_tools import init_dspy
 
 app = Typer()
 
 
 def function_to_dict(func: Callable) -> dict:
     output = {
```

### Comparing `dspygen-2024.3.7/src/dspygen/modules/cli_bot.py` & `dspygen-2024.3.8/src/dspygen/modules/cli_bot_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/cobol_to_python.py` & `dspygen-2024.3.8/src/dspygen/modules/cobol_to_python_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/dflss_module.py` & `dspygen-2024.3.8/src/dspygen/modules/dflss_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/file_name_module.py` & `dspygen-2024.3.8/src/dspygen/modules/file_name_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dspy
 import pyperclip
 from typer import Typer
 from inflection import underscore
 
 app = Typer(
-    help="Generate a file name from any text if no text is provided it will use clipboard."
+    help="Generate a file name from any text."
 )
 
 
 class FileContentToFileNameModule(dspy.Module):
     """Converts file content to a file name with extension"""
 
     def __init__(self, extension: str = None):
```

### Comparing `dspygen-2024.3.7/src/dspygen/modules/gen_cli_module.py` & `dspygen-2024.3.8/src/dspygen/modules/gen_cli_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/gen_keyword_arguments_module.py` & `dspygen-2024.3.8/src/dspygen/modules/gen_keyword_arguments_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import ast
 import inspect
 from typing import Any, Callable
 
 import dspy
 from typer import Typer
 
-from dspygen.experiments.function_call import get_current_weather, get_n_day_weather_forecast
+from dspygen.experiments.function_calling.function_call import get_current_weather, get_n_day_weather_forecast
 from dspygen.utils.dspy_tools import init_dspy
 
 
 class GenerateKeywordArgumentsSignature(dspy.Signature):
     """
     A Signature class designed to generate keyword arguments for a function call
     based on a given prompt and the function's signature.
```

### Comparing `dspygen-2024.3.7/src/dspygen/modules/gen_message.py` & `dspygen-2024.3.8/src/dspygen/modules/gen_message_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/gen_pydantic_instance_module.py` & `dspygen-2024.3.8/src/dspygen/modules/gen_pydantic_instance_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/gen_signature_module.py` & `dspygen-2024.3.8/src/dspygen/modules/gen_signature_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/get_selector.py` & `dspygen-2024.3.8/src/dspygen/modules/get_selector_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,37 +2,51 @@
 
 """
 import dspy
 from typer import Typer
 from dspygen.utils.dspy_tools import init_dspy
 
 
-app = Typer()        
+app = Typer()
+
+
+import dspy
+
+class SelectSingleElement(dspy.Signature):
+    """
+    Selects a single element from a list of elements that best matches the given prompt.
+    """
+    elements = dspy.InputField(desc="A list of elements.")
+    prompt = dspy.InputField(desc="A prompt used to match the most relevant element.")
+
+    selected_element = dspy.OutputField(desc="The css selector to use with Selenium.")
+
+
 
 
 class GetSelectorModule(dspy.Module):
     """GetSelectorModule"""
 
-    def forward(self, element_dicts, prompt):
-        pred = dspy.ChainOfThought("element_dicts, prompt -> selector_matching_element_and_prompt")
-        result = pred(element_dicts=element_dicts, prompt=prompt).selector_matching_element_and_prompt
+    def forward(self, elements, prompt):
+        pred = dspy.ChainOfThought(SelectSingleElement)
+        result = pred(elements=elements, prompt=prompt).selected_element
         return result
 
 
-def get_selector_call(element_dicts, prompt):
+def get_selector_call(elements, prompt):
     get_selector = GetSelectorModule()
-    return get_selector.forward(element_dicts=element_dicts, prompt=prompt)
+    return get_selector.forward(elements=elements, prompt=prompt)
 
 
 @app.command()
-def call(element_dicts, prompt):
+def call(elements, prompt):
     """GetSelectorModule"""
     init_dspy()
     
-    print(get_selector_call(element_dicts=element_dicts, prompt=prompt))
+    print(get_selector_call(elements=elements, prompt=prompt))
 
 
 from fastapi import APIRouter
 router = APIRouter()
 
 @router.post("/get_selector/")
 async def get_selector_route(data: dict):
@@ -57,12 +71,12 @@
 {'type': 'checkbox', 'id': 'p-variants-checkbox', 'role': 'button', 'aria-haspopup': 'true', 'data-event-name': 'ui.dropdown-p-variants', 'class': 'vector-dropdown-checkbox ', 'aria-label': 'Change language variant'}
 {'type': 'checkbox', 'id': 'vector-page-tools-dropdown-checkbox', 'role': 'button', 'aria-haspopup': 'true', 'data-event-name': 'ui.dropdown-vector-page-tools-dropdown', 'class': 'vector-dropdown-checkbox ', 'aria-label': 'Tools'}
 {'type': 'checkbox', 'id': 'vector-page-tools-dropdown-checkbox', 'role': 'button', 'aria-haspopup': 'true', 'data-event-name': 'ui.dropdown-vector-page-tools-dropdown', 'class': 'vector-dropdown-checkbox ', 'aria-label': 'Tools'}
 {'type': 'checkbox', 'id': 'p-lang-btn-checkbox', 'role': 'button', 'aria-haspopup': 'true', 'data-event-name': 'ui.dropdown-p-lang-btn', 'class': 'vector-dropdown-checkbox mw-interlanguage-selector', 'aria-label': 'Go to an article in another language. Available in 48 languages'}
 {'type': 'checkbox', 'id': 'p-lang-btn-checkbox', 'role': 'button', 'aria-haspopup': 'true', 'data-event-name': 'ui.dropdown-p-lang-btn', 'class': 'vector-dropdown-checkbox mw-interlanguage-selector', 'aria-label': 'Go to an article in another language. Available in 48 languages'}
 """
     prompt = "search box"
-    print(get_selector_call(element_dicts=element_dicts, prompt=prompt))
+    print(get_selector_call(elements=element_dicts, prompt=prompt))
     
 
 if __name__ == "__main__":
     main()
```

### Comparing `dspygen-2024.3.7/src/dspygen/modules/html_module.py` & `dspygen-2024.3.8/src/dspygen/modules/html_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/insight_tweet_module.py` & `dspygen-2024.3.8/src/dspygen/modules/insight_tweet_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/js_to_fast_api_module.py` & `dspygen-2024.3.8/src/dspygen/modules/js_to_fast_api_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/jsx_module.py` & `dspygen-2024.3.8/src/dspygen/modules/jsx_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/message_module.py` & `dspygen-2024.3.8/src/dspygen/modules/message_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/module_docstring_module.py` & `dspygen-2024.3.8/src/dspygen/modules/module_docstring_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/product_bot_module.py` & `dspygen-2024.3.8/src/dspygen/modules/product_bot_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/prompt_function_call_module.py` & `dspygen-2024.3.8/src/dspygen/modules/prompt_function_call_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/python_expert_module.py` & `dspygen-2024.3.8/src/dspygen/modules/python_expert_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/python_source_code_module.py` & `dspygen-2024.3.8/src/dspygen/modules/python_source_code_module.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 app = Typer()
 
 
 class PromptPep8PythonSourceCodeModule(dspy.Module):
     """Verbose Documentation for the DSPy Module"""
 
     def forward(self, prompt):
-        ignore_rules = "Ignore PEP 123"
-        pred = dspy.ChainOfThought("prompt, ignore_rules -> pep8_python_source_code")
-        result = pred(prompt=prompt, ingnore_rules=ignore_rules).pep8_python_source_code
+        pred = dspy.ChainOfThought("prompt -> pep8_python_source_code")
+        result = pred(prompt=prompt).pep8_python_source_code
         return result
 
 
 def python_source_code_call(prompt):
     prompt_pep8_python_source_code = PromptPep8PythonSourceCodeModule()
     return prompt_pep8_python_source_code.forward(prompt=prompt)
```

### Comparing `dspygen-2024.3.7/src/dspygen/modules/react_jsx_module.py` & `dspygen-2024.3.8/src/dspygen/modules/react_jsx_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typer import Typer
 
 
 app = Typer(help="Create React JSX source code.")
 
 
 class PromptReactJsxModule(dspy.Module):
+
     """This is a DSPy Module that converts a prompt into react_jsx"""
 
     def forward(self, prompt):
         pred = dspy.Predict("prompt -> react_jsx")
         result = pred(prompt=prompt).react_jsx
         return result
```

### Comparing `dspygen-2024.3.7/src/dspygen/modules/request_contract_module.py` & `dspygen-2024.3.8/src/dspygen/modules/request_contract_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/signature_factory.py` & `dspygen-2024.3.8/src/dspygen/modules/signature_factory.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/signature_renderer.py` & `dspygen-2024.3.8/src/dspygen/modules/signature_renderer.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/source_code_pep8_docs_module.py` & `dspygen-2024.3.8/src/dspygen/modules/source_code_pep8_docs_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/sql_query.py` & `dspygen-2024.3.8/src/dspygen/modules/sql_query_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/streamlit_bot.py` & `dspygen-2024.3.8/src/dspygen/modules/streamlit_bot_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/subject_destination_audience_newsletter_article_module.py` & `dspygen-2024.3.8/src/dspygen/modules/subject_destination_audience_newsletter_article_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/tax_return_agent.py` & `dspygen-2024.3.8/src/dspygen/modules/tax_return_agent.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/test.py` & `dspygen-2024.3.8/src/dspygen/modules/test.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/test_chat_bot_cli.py` & `dspygen-2024.3.8/src/dspygen/modules/test_chat_bot_cli.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/text_summary_module_module.py` & `dspygen-2024.3.8/src/dspygen/modules/text_summary_module_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/to_elixir_module.py` & `dspygen-2024.3.8/src/dspygen/modules/to_elixir_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/modules/usp_connect_ship_webhook.py` & `dspygen-2024.3.8/src/dspygen/modules/usp_connect_ship_webhook.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/pages/mqtt_page.py` & `dspygen-2024.3.8/src/dspygen/pages/mqtt_page.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/abstract_actor.py` & `dspygen-2024.3.8/src/dspygen/rdddy/abstract_actor.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/abstract_aggregate.py` & `dspygen-2024.3.8/src/dspygen/rdddy/abstract_aggregate.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/abstract_message.py` & `dspygen-2024.3.8/src/dspygen/rdddy/abstract_message.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,38 +8,33 @@
 
 
 class AbstractMessage(YAMLMixin, BaseModel):
     """Message class using Pydantic for data validation and serialization."""
 
     model_config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
 
-    actor_id: int = -1
-    content: Any = None
-    message_type: str = ""
+    actor_id: int = Field(default=-1, description="The ID of the actor that sent the message. -1 means it was published by the system.")
+    metadata: dict[str, Any] = Field(default_factory=dict, description="Metadata for the message.")
+    content: str | None = Field(default=None, description="The content of the message.")
+    message_type: str = Field(default="", description="The type of the message.")
 
     def __init__(self, **data):
         super().__init__(**data)
         # Calculate the relative import path at runtime
         self.message_type = self._calculate_import_path()
 
     def _calculate_import_path(self) -> str:
         """Calculate the relative import path of the class."""
         module = inspect.getmodule(self)
         relative_path = f"{module.__name__}.{self.__class__.__name__}"
         return relative_path
 
 
-
-from pydantic import BaseModel, Field
-
-
-
-
 class MessageList(YAMLMixin, BaseModel):
-    messages: list[AbstractMessage]
+    messages: list[AbstractMessage] = []
 
 
 class ExceptionMessage(AbstractMessage):
     """Generic exception message"""
 
 
 class TerminationMessage(AbstractMessage):
@@ -66,15 +61,15 @@
         return message_class(**data)
 
     @classmethod
     def create_messages_from_list(cls, data_list: list[dict]) -> list[T]:
         """Create a list of messages from a list of YAML data dictionaries.
 
         Parameters:
-        - data_list (List[dict]): A list of dictionaries containing message data.
+        - data_list (List[dict]): A list of dictionaries containing message  data.
 
         Returns:
         - List[Type[BaseModel]]: A list of appropriate message types.
         """
         messages = [cls.create_message(data) for data in data_list]
         return messages
```

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/abstract_policy.py` & `dspygen-2024.3.8/src/dspygen/rdddy/abstract_policy.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/abstract_repository.py` & `dspygen-2024.3.8/src/dspygen/rdddy/abstract_repository.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/abstract_saga.py` & `dspygen-2024.3.8/src/dspygen/rdddy/abstract_saga.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/actor_system.py` & `dspygen-2024.3.8/src/dspygen/rdddy/actor_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,25 +40,26 @@
 
 Usage:
 To use the ActorSystem, instantiate it within your application and use its methods to create actors and manage message passing. The system integrates seamlessly with the asyncio event loop, making it straightforward to incorporate into existing asynchronous applications.
 
 The actor_system.py module, guided by the AMCN, provides a robust foundation for developing actor-based systems within the RDDDY framework, ensuring that applications are built with a solid architectural foundation that promotes maintainability, scalability, and domain-driven design principles.
 """
 import asyncio
+import json
 from asyncio import Future
 from typing import TYPE_CHECKING, Optional, TypeVar, cast
 from paho.mqtt import client as mqtt_client
 
 import reactivex as rx
 from loguru import logger
 from paho.mqtt.enums import CallbackAPIVersion
 from reactivex import operators as ops
 from reactivex.scheduler.eventloop import AsyncIOScheduler
 
-from dspygen.rdddy.abstract_message import AbstractMessage
+from dspygen.rdddy.abstract_message import AbstractMessage, MessageFactory
 
 if TYPE_CHECKING:
     from dspygen.rdddy.abstract_actor import AbstractActor
 
 T = TypeVar("T", bound="AbstractActor")
 
 
@@ -102,28 +103,32 @@
             event_stream (Subject): A subject for publishing events within the actor system.
         """
         self.actors: dict[int, AbstractActor] = {}
         self.loop = loop if loop is not None else asyncio.get_event_loop()
         self.scheduler = AsyncIOScheduler(loop=self.loop)
         self.event_stream = rx.subject.Subject()
 
-        self.mqtt_client = mqtt_client.Client(CallbackAPIVersion.VERSION2)
-        self.mqtt_client.on_connect = self.on_connect
-        self.mqtt_client.on_message = self.on_message  # Define the callback for incoming messages
-        self.mqtt_client.connect(mqtt_broker, mqtt_port, 60)
-        self.mqtt_client.loop_start()
+        try:
+            self.mqtt_client = mqtt_client.Client(CallbackAPIVersion.VERSION2)
+            self.mqtt_client.on_connect = self.on_connect
+            self.mqtt_client.on_message = self.on_message  # Define the callback for incoming messages
+            self.mqtt_client.connect(mqtt_broker, mqtt_port, 60)
+            self.mqtt_client.loop_start()
+        except (ConnectionRefusedError, OSError) as e:
+            logger.error(f"Error connecting to MQTT Broker: {e}")
 
     def on_connect(self, client, userdata, flags, reason_code, properties):
         print("Connected to MQTT Broker.")
         client.subscribe("actor_system/publish")  # Subscribe to the topic
 
     def on_message(self, client, userdata, msg):
         print(f"Received message from topic {msg.topic}: {msg.payload}")
         # Deserialize the message payload into your internal message format
-        message = AbstractMessage.model_validate_json(msg.payload)  # Implement this method based on your message class
+        payload_dict = json.loads(msg.payload)
+        message = MessageFactory.create_message(payload_dict) # Implement this method based on your message class
         asyncio.run_coroutine_threadsafe(self.distribute_message(message), self.loop)
 
     async def distribute_message(self, message):
         # Prevent republishing to MQTT by directly invoking the local distribution logic
         self.event_stream.on_next(message)
         actors = list(self.actors.values())
         for actor in actors:
@@ -314,14 +319,32 @@
 
         Returns:
             AbstractActor: The actor object corresponding to the specified ID.
         """
         return cast(T, self.actors.get(actor_id))
 
 
+    async def shutdown(self):
+        """Shuts down the actor system and terminates all actors.
+
+        Preconditions (Pre):
+            - None
+
+        Transition (T):
+            - Terminates all actors within the actor system.
+            - Closes the event stream and scheduler.
+
+        Postconditions (Post):
+            - The actor system has been successfully shut down.
+        """
+        self.mqtt_client.loop_stop()
+        self.mqtt_client.disconnect()
+        logger.debug("Actor system shutdown complete.")
+
+
 import asyncio
 
 
 async def main():
     print("main")
     # await
```

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/browser/browser_domain.py` & `dspygen-2024.3.8/src/dspygen/rdddy/browser/browser_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dspygen.rdddy.abstract_event import AbstractEvent
 from dspygen.rdddy.abstract_message import *
 
 
 # Define commands and events
 class StartBrowserCommand(AbstractCommand):
     browser_id: str = "default"
-    custom_args: list[str] = None
+    custom_args: list[str] = []
 
 
 class BrowserStartedEvent(AbstractEvent):
     pass
 
 
 class StopBrowserCommand(AbstractCommand):
```

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/browser/browser_process_supervisor.py` & `dspygen-2024.3.8/src/dspygen/rdddy/browser/browser_process_supervisor.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 from dspygen.rdddy.abstract_actor import AbstractActor
 from dspygen.rdddy.actor_system import ActorSystem
 from dspygen.rdddy.browser.browser_domain import *
 from dspygen.rdddy.browser.browser_worker import BrowserWorker
 
 
+os.environ["PLAYWRIGHT_BROWSER"] = "/Applications/Google Chrome Canary.app/Contents/MacOS/Google Chrome Canary"
+
+
 class BrowserProcessSupervisor(AbstractActor):
     def __init__(self, actor_system):
         super().__init__(actor_system)
         self.processes: dict[str, Process] = {}  # Tracks browser processes by ID
         self.default_args = ["--remote-debugging-port=9222"]  # Default browser args
         self.health_check_running = False
 
@@ -28,16 +31,16 @@
         args = self.default_args if cmd.custom_args is None else cmd.custom_args
         self.processes[cmd.browser_id] = await asyncio.create_subprocess_exec(
             os.getenv("PLAYWRIGHT_BROWSER"),
             *args,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
         )
-        await asyncio.sleep(10)
-        # await self.start_health_check()
+        # await asyncio.sleep(10)
+        await self.start_health_check()
         logger.info(f"Started browser process with ID {cmd.browser_id}.")
 
     async def stop_browser_process(self, cmd: StopBrowserCommand):
         process = self.processes.pop(cmd.browser_id, None)
         if process:
             try:
                 process.terminate()
```

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/browser/browser_worker.py` & `dspygen-2024.3.8/src/dspygen/rdddy/browser/browser_worker.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/event_storm_domain_specification_model.py` & `dspygen-2024.3.8/src/dspygen/rdddy/event_storm_domain_specification_model.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/rdddy/event_storm_model.py` & `dspygen-2024.3.8/src/dspygen/rdddy/event_storm_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from pydantic import Field, BaseModel
 
-from dspygen.experiments.gen_pydantic_instance import instance
 from dspygen.rdddy.abstract_event import AbstractEvent
 from dspygen.utils.dspy_tools import init_dspy
 
 
 class EventStormingDomainSpecificationModel(BaseModel):
     """Integrates Event Storming with RDDDY and DFLSS to capture and analyze domain complexities through events, commands, and queries, using Hoare logic for correctness. It serves as a repository for interactions identified in Event Storming, enhancing system responsiveness and process efficiency. This model educates on designing and verifying systems aligned with domain requirements and operational excellence. CamelCase only. """
```

### Comparing `dspygen-2024.3.7/src/dspygen/subcommands/actor_cmd.py` & `dspygen-2024.3.8/src/dspygen/subcommands/actor_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     try:
         os.kill(pid, 0)  # No signal is sent, but error checking is still performed
     except OSError:
         return False
     else:
         return True
 
+
 @app.command(name="start")
 async def start_mqtt(broker_path: str = MOSQUITTO_BINARY, config_path: str = MOSQUITTO_CONF):
     """Starts the Mosquitto MQTT broker."""
     if os.path.exists(PID_FILE):
         with open(PID_FILE, 'r') as file:
             pid = int(file.read().strip())
             if process_is_running(pid):
@@ -85,9 +86,14 @@
 async def start_actor_system(message: str):
     """Starts the actor system with MQTT integration."""
     actor_system = ActorSystem()
 
     await actor_system.publish(AbstractCommand(content=message))
 
 
+@app.command(name="new")
+async def new_actor():
+    """Uses a Jinja template to generate a new actor."""
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `dspygen-2024.3.7/src/dspygen/subcommands/assert_cmd.py` & `dspygen-2024.3.8/src/dspygen/subcommands/assert_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/subcommands/browser_cmd.py` & `dspygen-2024.3.8/src/dspygen/subcommands/browser_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/subcommands/command_cmd.py` & `dspygen-2024.3.8/src/dspygen/subcommands/cmd_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/subcommands/help.txt` & `dspygen-2024.3.8/src/dspygen/subcommands/help.txt`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/subcommands/help_cmd.py` & `dspygen-2024.3.8/src/dspygen/subcommands/help_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/subcommands/lm_cmd.py` & `dspygen-2024.3.8/src/dspygen/subcommands/lm_cmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,17 +24,19 @@
     def __call__(self, prompt, only_completed=True, return_sorted=False, **kwargs):
         pass
         
 """
 
 
 @app.command(name="new")
-def new_lm():
+def new_lm(name: str = typer.Argument(...)):
     """Generates a new language model."""
-    typer.echo("Uses jinja and dspy module to create a language model.")
+    to = f"{lm_dir()}/"
+    source = render(lm_template, name=name, to=to + "{{ name | underscore }}_lm.py")
+    print(source)
 
 
 def main():
     print('main')
     name = "Groq"
     to = f"{lm_dir()}/"
     source = render(lm_template, name=name, to=to + "{{ name | underscore }}_lm.py")
```

### Comparing `dspygen-2024.3.7/src/dspygen/subcommands/module_cmd.py` & `dspygen-2024.3.8/src/dspygen/subcommands/module_cmd.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from importlib import import_module
 
 import os
 
 import inflection
 import typer
 
+from dspygen.dsl.dsl_pipeline_executor import execute_pipeline
 from dspygen.modules.gen_dspy_module import  DSPyModuleTemplate, SignatureDspyModuleModule
-from dspygen.modules.file_name_module import file_name_call
-from dspygen.modules.gen_pydantic_instance_module import gen_pydantic_instance_call
 from dspygen.utils.cli_tools import chatbot
 from dspygen.utils.dspy_tools import init_dspy
 from dspygen.utils.file_tools import dspy_modules_dir, source_dir, get_source
 
 app = typer.Typer(help="Generate DSPy Modules or call exist ones.")
 
 
@@ -24,19 +23,17 @@
 ):
     """Generate a new dspy.Module. Inputs and output will be static."""
     if len(inputs) == 0 or output is None:
         raise ValueError("Please provide a signature or input and output.")
 
     mdl = DSPyModuleTemplate(class_name=class_name, inputs=inputs.split(','), output=output)
 
-    print(mdl)
-
     source = SignatureDspyModuleModule().forward(mdl)
 
-    file_name = f"{inflection.underscore(class_name)}.py"
+    file_name = f"{inflection.underscore(class_name)}_module.py"
 
     with open(dspy_modules_dir() / file_name, "w") as file:
         file.write(source)
 
     print(source)
 
     print(f"Module saved to {dspy_modules_dir() / file_name}")
@@ -65,7 +62,9 @@
     load_commands()
 
 
 @app.command("help")
 def cli_help(question: str):
     """Answers the user questions with a helpful chatbot."""
     chatbot(question, get_source(__file__))
+
+
```

### Comparing `dspygen-2024.3.7/src/dspygen/subcommands/sig_cmd.py` & `dspygen-2024.3.8/src/dspygen/subcommands/sig_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/subcommands/temp_assert.py` & `dspygen-2024.3.8/src/dspygen/subcommands/temp_assert.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/__init__.py` & `dspygen-2024.3.8/src/dspygen/typetemp/__init__.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/environment/typed_environment.py` & `dspygen-2024.3.8/src/dspygen/typetemp/environment/typed_environment.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/environment/typed_native_environment.py` & `dspygen-2024.3.8/src/dspygen/typetemp/environment/typed_native_environment.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/extension/faker_extension.py` & `dspygen-2024.3.8/src/dspygen/typetemp/extension/faker_extension.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/extension/inflection_extension.py` & `dspygen-2024.3.8/src/dspygen/typetemp/extension/inflection_extension.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/functional.py` & `dspygen-2024.3.8/src/dspygen/typetemp/functional.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 
     rendered = template.render(**kwargs)
 
     if to:
         to_ = _env.from_string(to)
         rendered_to = to_.render(**kwargs)
 
+        # Check if the directory exists, if not create it
+        if not os.path.exists(os.path.dirname(rendered_to)):
+            os.makedirs(os.path.dirname(rendered_to))
+
         with open(rendered_to, "w") as file:
             file.write(rendered)
 
     return rendered
 
 
 def render_native(tmpl_str_or_path: str | Path, **kwargs) -> str:
```

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/template/async_render_mixin.py` & `dspygen-2024.3.8/src/dspygen/typetemp/template/async_render_mixin.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/template/dsl_project.py` & `dspygen-2024.3.8/src/dspygen/typetemp/template/dsl_project.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/template/render_funcs.py` & `dspygen-2024.3.8/src/dspygen/typetemp/template/render_funcs.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/template/render_mixin.py` & `dspygen-2024.3.8/src/dspygen/typetemp/template/render_mixin.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/template/smart_template.py` & `dspygen-2024.3.8/src/dspygen/typetemp/template/smart_template.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/template/typed_injector.py` & `dspygen-2024.3.8/src/dspygen/typetemp/template/typed_injector.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/template/typed_prompt.py` & `dspygen-2024.3.8/src/dspygen/typetemp/template/typed_prompt.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/template/typed_python_source.py` & `dspygen-2024.3.8/src/dspygen/typetemp/template/typed_python_source.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/typetemp/template/typed_template.py` & `dspygen-2024.3.8/src/dspygen/typetemp/template/typed_template.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/utils/complete.py` & `dspygen-2024.3.8/src/dspygen/utils/complete.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/utils/compression_tools.py` & `dspygen-2024.3.8/src/dspygen/utils/compression_tools.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/utils/create_prompts.py` & `dspygen-2024.3.8/src/dspygen/utils/create_prompts.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/utils/models.py` & `dspygen-2024.3.8/src/dspygen/utils/models.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.3.7/src/dspygen/utils/module_tools.py` & `dspygen-2024.3.8/src/dspygen/utils/module_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import types
 import inspect
 from typing import Callable
 
+
 def module_to_dict(module, include_docstring=True) -> dict:
     module_dict = {
         "module_name": module.__name__,
         "docstring": module.__doc__ if include_docstring else None,
         "functions": {},
         "classes": {}
     }
@@ -28,14 +29,15 @@
             for cname, cobj in obj.__dict__.items():
                 if isinstance(cobj, types.FunctionType) and inspect.getmodule(cobj) == module:
                     class_dict["methods"][cname] = function_to_dict(cobj)
             module_dict["classes"][name] = class_dict
 
     return module_dict
 
+
 def function_to_dict(func: Callable) -> dict:
     output = {
         "function_name": func.__name__,
         "docstring": func.__doc__,
         "keyword_arguments": {k: str(v) for k, v in func.__annotations__.items()},
     }
```

### Comparing `dspygen-2024.3.7/src/dspygen/utils/yaml_tools.py` & `dspygen-2024.3.8/src/dspygen/utils/yaml_tools.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,109 @@
-# Define a mixin for YAML serialization and deserialization
+# I have IMPLEMENTED your PerfectPythonProductionCode® AGI enterprise innovative and opinionated best practice
+# IMPLEMENTATION code of your requirements.
 import json
 import os
-from contextlib import contextmanager
-from typing import Any, Optional, TypeVar, Union
+from contextlib import contextmanager, asynccontextmanager
+from typing import Any, Optional, TypeVar, Union, Type
 
+import aiofiles
 import yaml
 from pydantic import BaseModel
 
 T = TypeVar("T", bound="YAMLMixin")
 
 
-# Define a mixin for YAML serialization and deserialization
 class YAMLMixin:
     def to_yaml(self: BaseModel, file_path: Optional[str] = None) -> str:
         yaml_content = yaml.dump(self.model_dump(), default_flow_style=False, width=1000)
         if file_path:
             with open(file_path, "w") as yaml_file:
                 yaml_file.write(yaml_content)
                 print(f"Wrote {file_path} to {yaml_content}")
         return yaml_content
-
+    
     @classmethod
     def from_yaml(cls: type["T"], file_path: str) -> "T":
         with open(file_path) as yaml_file:
             data = yaml.safe_load(yaml_file)
+        return cls.model_validate(data)
+
+    async def ato_yaml(self: BaseModel, file_path: Optional[str] = None) -> str:
+        """
+        Asynchronously serializes the Pydantic model to YAML and writes to a file.
+
+        Args:
+            file_path (Optional[str]): The file path to write the YAML content. If None, returns YAML string.
+
+        Returns:
+            str: The YAML content as a string.
+        """
+        yaml_content = yaml.dump(self.model_dump(), default_flow_style=False, width=1000)
+        if file_path:
+            async with aiofiles.open(file_path, "w") as yaml_file:
+                await yaml_file.write(yaml_content)
+        return yaml_content
+
+    @classmethod
+    async def afrom_yaml(cls: Type[T], file_path: str) -> T:
+        """
+        Asynchronously reads YAML content from a file and constructs an instance of the Pydantic model.
+
+        Args:
+            file_path (str): The file path from which to read the YAML content.
+
+        Returns:
+            T: An instance of the Pydantic model.
+        """
+        async with aiofiles.open(file_path, "r") as yaml_file:
+            data = yaml.safe_load(await yaml_file.read())
         return cls(**data)
 
     @classmethod
     @contextmanager
-    def context(cls: type[T], file_path: Optional[str] = None):
+    def io_context(cls: type[T], model_defaults=None, file_path: Optional[str] = None):
         """Context manager that automatically uses the subclass name as the filename."""
+        if model_defaults is None:
+            model_defaults = {}
+
         if file_path is None:
             filename = f"{cls.__name__}.yaml"
         else:
             filename = file_path
 
         absolute_path = os.path.abspath(filename)
 
-        try:
-            # Load from YAML if file exists
-            print(f"Loading {absolute_path}...")
-            instance = (
-                cls.from_yaml(absolute_path) if os.path.exists(absolute_path) else cls()
-            )
-            print(f"Instance loaded: {instance}")
-            yield instance
-            # Save to YAML
-            instance.to_yaml(absolute_path)
-            print("Saved as", absolute_path)
-        except Exception as e:
-            print(f"An error occurred: {e}")
+        # Load from YAML if file exists
+        instance = (
+            cls.from_yaml(absolute_path) if os.path.exists(absolute_path) else cls.model_validate(model_defaults)
+        )
+        yield instance
+        # Save to YAML
+        instance.to_yaml(absolute_path)
+
 
+    @classmethod
+    @asynccontextmanager
+    async def aio_context(cls: Type[T], model_defaults=None, file_path: Optional[str] = None):
+        if model_defaults is None:
+            model_defaults = {}
+
+        if file_path is None:
+            filename = f"{cls.__name__}.yaml"
+        else:
+            filename = file_path
+
+        absolute_path = os.path.abspath(filename)
+
+        instance = await cls.afrom_yaml(absolute_path) if os.path.exists(absolute_path) else cls.model_validate(model_defaults)
+
+        yield instance
+
+        await instance.ato_yaml(absolute_path)
 
-# I have IMPLEMENTED your PerfectPythonProductionCode® AGI enterprise innovative and opinionated best practice IMPLEMENTATION code of your requirements.
 
 
 def find_all_keys_in_file(filepath: str, target_key: str) -> list[Any]:
     """Find all occurrences of a key in a nested YAML-like dictionary or list from a YAML file and return the associated values.
 
     Parameters:
     - filepath (str): The path to the YAML file to be read.
@@ -104,24 +151,49 @@
         yaml_file.write(yaml_content)
     return yaml_content
 
 
 def from_yaml(model_cls: BaseModel, file_path: str) -> BaseModel:
     with open(file_path) as yaml_file:
         data = yaml.safe_load(yaml_file)
-    return model_cls(**data)
+    return model_cls.model_validate(data)
 
 
-if __name__ == "__main__":
+def main2():
     # Example usage: Assuming you have a YAML file named 'example.yaml' in the current directory
     # filepath = "example.yaml"
     # target_key = "definition"
     # found_definitions = find_all_keys_in_file(filepath, target_key)
     #
     # print(f"Found definitions in file {filepath}: {found_definitions}")
     # Example usage
     class MyData(BaseModel, YAMLMixin):
         my_attr: str = "Initial Value"
 
     with MyData.context() as data:
         print(f"Current attribute value: {data.my_attr}")
         data.my_attr = "Updated Value"
+
+def main():
+    class MyData(BaseModel, YAMLMixin):
+        my_attr: str
+
+    """Main function"""
+    with MyData.io_context({"my_attr": "Hello World"}) as data:
+        print(f"Current attribute value: {data.my_attr}")
+        data.my_attr = "Updated Value"
+
+
+import asyncio
+
+async def async_main():
+    class MyData(BaseModel, YAMLMixin):
+        my_attr: str
+
+    async with MyData.aio_context({"my_attr": "Hello World"}) as data:
+        print(f"Current attribute value: {data.my_attr}")
+        data.my_attr = "Updated Async Value"
+
+
+if __name__ == '__main__':
+    # asyncio.run(async_main())
+    main()
```

### Comparing `dspygen-2024.3.7/PKG-INFO` & `dspygen-2024.3.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 Metadata-Version: 2.1
 Name: dspygen
-Version: 2024.3.7
+Version: 2024.3.8
 Summary: A Ruby on Rails style framework for the DSPy (Demonstrate, Search, Predict) project for Language Models like GPT, BERT, and LLama.
 Home-page: https://github.com/seanchatmangpt/dspygen
 Author: Sean Chatman
 Author-email: info@chatmangpt.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
+Requires-Dist: anyio (>=4.3.0,<5.0.0)
 Requires-Dist: asyncer (>=0.0.5,<0.0.6)
+Requires-Dist: chromadb (>=0.4.24,<0.5.0)
 Requires-Dist: coloredlogs (>=15.0.1)
 Requires-Dist: dspy-ai (==2.3.1)
+Requires-Dist: ebooklib (>=0.18,<0.19)
 Requires-Dist: faker (>=23.2.1,<24.0.0)
 Requires-Dist: fastapi[all] (>=0.92.0)
 Requires-Dist: groq (>=0.4.1,<0.5.0)
 Requires-Dist: gunicorn (>=20.1.0)
+Requires-Dist: icontract (>=2.6.6,<3.0.0)
+Requires-Dist: ijson (>=3.2.3,<4.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: jinja2-ext (>=0.1,<0.2)
 Requires-Dist: jinja2-time (>=0.2.0,<0.3.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: munch (>=4.0.0,<5.0.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: paho-mqtt (>=2.0.0,<3.0.0)
+Requires-Dist: pandasql (>=0.7.3,<0.8.0)
 Requires-Dist: playwright (>=1.41.2,<2.0.0)
 Requires-Dist: poethepoet (>=0.20.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pydantic (>=1.10.7)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: pykka (>=4.0.2,<5.0.0)
+Requires-Dist: pypdf (>=4.1.0,<5.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: pytest-asyncio (>=0.23.5,<0.24.0)
+Requires-Dist: python-docx (>=1.1.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: reactivex (>=4.0.4,<5.0.0)
+Requires-Dist: sentify (>=0.7.4,<0.8.0)
+Requires-Dist: sqlmodel (>=0.0.16,<0.0.17)
 Requires-Dist: st-pages (>=0.4.5,<0.5.0)
 Requires-Dist: streamlit (>=1.19.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: typer[all] (>=0.9.0)
+Requires-Dist: tzlocal (>=5.2,<6.0)
 Requires-Dist: uvicorn[standard] (>=0.20.0)
 Project-URL: Repository, https://github.com/seanchatmangpt/dspygen
 Description-Content-Type: text/markdown
 
 [![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/user/my-package)
 
 # DSPyGen: Streamlining AI Development
```

