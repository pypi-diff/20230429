# Comparing `tmp/gridworks_atn-0.2.3.tar.gz` & `tmp/gridworks_atn-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_atn-0.2.3.tar", max compression
+gzip compressed data, was "gridworks_atn-0.2.4.tar", max compression
```

## Comparing `gridworks_atn-0.2.3.tar` & `gridworks_atn-0.2.4.tar`

### file list

```diff
@@ -1,117 +1,110 @@
--rw-r--r--   0        0        0     1065 2023-03-01 11:32:48.320980 gridworks_atn-0.2.3/LICENSE
--rw-r--r--   0        0        0     3002 2023-03-01 11:32:48.320980 gridworks_atn-0.2.3/README.md
--rw-r--r--   0        0        0     2116 2023-03-01 11:33:08.657070 gridworks_atn-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      336 2023-03-01 11:32:48.340980 gridworks_atn-0.2.3/src/gwatn/__init__.py
--rw-r--r--   0        0        0      226 2023-03-01 11:32:48.340980 gridworks_atn-0.2.3/src/gwatn/__main__.py
--rw-r--r--   0        0        0     7480 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/api_types.py
--rw-r--r--   0        0        0      593 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/api_types_hack.py
--rw-r--r--   0        0        0    17350 2023-03-01 11:33:08.657070 gridworks_atn-0.2.3/src/gwatn/atn_actor_base.py
--rw-r--r--   0        0        0     4840 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/atn_utils.py
--rw-r--r--   0        0        0     4871 2023-03-01 11:33:08.657070 gridworks_atn-0.2.3/src/gwatn/config.py
--rw-r--r--   0        0        0        0 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/csv_makers/__init__.py
--rw-r--r--   0        0        0     1152 2023-03-01 11:33:08.657070 gridworks_atn-0.2.3/src/gwatn/csv_makers/codec.py
--rw-r--r--   0        0        0    14863 2023-03-01 11:33:08.657070 gridworks_atn-0.2.3/src/gwatn/csv_makers/scada_report_a.py
--rw-r--r--   0        0        0     6148 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/data_classes/.DS_Store
--rw-r--r--   0        0        0      202 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/data_classes/__init__.py
--rw-r--r--   0        0        0    23507 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/data_classes/base_g_node.py
--rw-r--r--   0        0        0      583 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/data_classes/d_edge.py
--rw-r--r--   0        0        0     7812 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/data_classes/d_graph.py
--rw-r--r--   0        0        0     1559 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/data_classes/d_node.py
--rw-r--r--   0        0        0     5366 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/data_classes/g_node.py
--rw-r--r--   0        0        0     6791 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/data_classes/g_node_instance.py
--rw-r--r--   0        0        0      734 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/data_classes/gps_point.py
--rw-r--r--   0        0        0     2482 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/data_classes/market_type.py
--rw-r--r--   0        0        0     1494 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/data_classes/supervisor_container.py
--rw-r--r--   0        0        0    14450 2023-03-01 11:33:08.657070 gridworks_atn-0.2.3/src/gwatn/demo_methods.py
--rw-r--r--   0        0        0      276 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/dev_utils/__init__.py
--rw-r--r--   0        0        0     1792 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/dev_utils/dev_discoverer.py
--rw-r--r--   0        0        0    11883 2023-03-01 11:33:08.657070 gridworks_atn-0.2.3/src/gwatn/dev_utils/dev_ta_owner.py
--rw-r--r--   0        0        0    10994 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/dev_utils/dev_validator.py
--rw-r--r--   0        0        0     1171 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/dev_utils/make_plants.py
--rw-r--r--   0        0        0    11409 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/dispatch_contract.py
--rw-r--r--   0        0        0    12463 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/dispatch_contract_artifacts/application.json
--rw-r--r--   0        0        0     5229 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/dispatch_contract_artifacts/approval.teal
--rw-r--r--   0        0        0       40 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/dispatch_contract_artifacts/clear.teal
--rw-r--r--   0        0        0     3937 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/dispatch_contract_artifacts/contract.json
--rw-r--r--   0        0        0     2172 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/__init__.py
--rw-r--r--   0        0        0      932 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/actor_class.py
--rw-r--r--   0        0        0      673 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/algo_cert_type.py
--rw-r--r--   0        0        0      638 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/atn_spaceheat_strategy_name.py
--rw-r--r--   0        0        0      990 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/core_g_node_role.py
--rw-r--r--   0        0        0      700 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/distribution_tariff.py
--rw-r--r--   0        0        0      598 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/emitter_pump_feedback_model.py
--rw-r--r--   0        0        0      614 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/energy_supply_type.py
--rw-r--r--   0        0        0     2149 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/g_node_role.py
--rw-r--r--   0        0        0      992 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/g_node_status.py
--rw-r--r--   0        0        0      933 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/gni_status.py
--rw-r--r--   0        0        0      870 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/local_comm_interface.py
--rw-r--r--   0        0        0     1908 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/make_model.py
--rw-r--r--   0        0        0      563 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/market_price_unit.py
--rw-r--r--   0        0        0      590 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/market_quantity_unit.py
--rw-r--r--   0        0        0     1394 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/market_type_name.py
--rw-r--r--   0        0        0     1326 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/message_category.py
--rw-r--r--   0        0        0     1189 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/message_category_symbol.py
--rw-r--r--   0        0        0      928 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/mixing_valve_feedback_model.py
--rw-r--r--   0        0        0      626 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/recognized_currency_unit.py
--rw-r--r--   0        0        0      570 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/recognized_temperature_unit.py
--rw-r--r--   0        0        0     1590 2023-03-01 11:32:48.344980 gridworks_atn-0.2.3/src/gwatn/enums/role.py
--rw-r--r--   0        0        0     1331 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/enums/strategy_name.py
--rw-r--r--   0        0        0     1081 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/enums/supervisor_container_status.py
--rw-r--r--   0        0        0     1197 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/enums/telemetry_name.py
--rw-r--r--   0        0        0      832 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/enums/unit.py
--rw-r--r--   0        0        0      795 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/enums/universe_type.py
--rw-r--r--   0        0        0        0 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/py.typed
--rw-r--r--   0        0        0     7945 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/python_ta_daemon.json
--rw-r--r--   0        0        0    12518 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/python_ta_daemon.py
--rw-r--r--   0        0        0    26857 2023-03-01 11:33:08.657070 gridworks_atn-0.2.3/src/gwatn/scada_actor.py
--rw-r--r--   0        0        0     1391 2023-03-01 11:33:08.657070 gridworks_atn-0.2.3/src/gwatn/simple_atn_actor.py
--rw-r--r--   0        0        0     3169 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/ta_daemon_rest_api.py
--rw-r--r--   0        0        0      460 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/ta_validator_rest_api.py
--rw-r--r--   0        0        0    44071 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/two_channel_actor_base.py
--rw-r--r--   0        0        0     7833 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/types/__init__.py
--rw-r--r--   0        0        0     7780 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/types/accepted_bid.py
--rw-r--r--   0        0        0    20134 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/types/atn_bid.py
--rw-r--r--   0        0        0    34181 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/types/atn_params_heatpumpwithbooststore.py
--rw-r--r--   0        0        0     7953 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/types/atn_params_report_heatpumpwithbooststore.py
--rw-r--r--   0        0        0    20209 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/types/base_g_node_gt.py
--rw-r--r--   0        0        0     8221 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/types/basegnode_scada_create.py
--rw-r--r--   0        0        0    11106 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/types/csv_distp_sync.py
--rw-r--r--   0        0        0    11354 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/types/csv_eprt_sync.py
--rw-r--r--   0        0        0    11280 2023-03-01 11:32:48.348980 gridworks_atn-0.2.3/src/gwatn/types/csv_heat_profile.py
--rw-r--r--   0        0        0    21761 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/csv_weather_forecast_sync.py
--rw-r--r--   0        0        0     9785 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/discoverycert_algo_create.py
--rw-r--r--   0        0        0     7659 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/dispatch_contract_confirmed_heatpumpwithbooststore.py
--rw-r--r--   0        0        0    38712 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/flo_params_heatpumpwithbooststore.py
--rw-r--r--   0        0        0    24382 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/g_node_gt.py
--rw-r--r--   0        0        0    15767 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/g_node_instance_gt.py
--rw-r--r--   0        0        0     8106 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0     6718 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/gw_cert_id.py
--rw-r--r--   0        0        0     3501 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/heartbeat_a.py
--rw-r--r--   0        0        0     4539 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/heartbeat_algo_audit.py
--rw-r--r--   0        0        0     8524 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/heartbeat_b.py
--rw-r--r--   0        0        0     5919 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/initial_tadeed_algo_create.py
--rw-r--r--   0        0        0     7420 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/initial_tadeed_algo_optin.py
--rw-r--r--   0        0        0     8742 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/initial_tadeed_algo_transfer.py
--rw-r--r--   0        0        0     7959 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/join_dispatch_contract.py
--rw-r--r--   0        0        0    12341 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/latest_price.py
--rw-r--r--   0        0        0     4928 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/market_slot.py
--rw-r--r--   0        0        0    17073 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/market_type_gt.py
--rw-r--r--   0        0        0     5294 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/new_tadeed_algo_optin.py
--rw-r--r--   0        0        0     5196 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/new_tadeed_send.py
--rw-r--r--   0        0        0     5024 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/old_tadeed_algo_return.py
--rw-r--r--   0        0        0     8361 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/price_quantity.py
--rw-r--r--   0        0        0     2392 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/price_quantity_unitless.py
--rw-r--r--   0        0        0     5580 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/ready.py
--rw-r--r--   0        0        0     4904 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/scada_cert_transfer.py
--rw-r--r--   0        0        0     6545 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/sim_scada_driver_report.py
--rw-r--r--   0        0        0     8097 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/sim_timestep.py
--rw-r--r--   0        0        0     3120 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/sla_enter.py
--rw-r--r--   0        0        0     7390 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/snapshot_heatpumpwithbooststore.py
--rw-r--r--   0        0        0     6080 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/super_starter.py
--rw-r--r--   0        0        0    12065 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/supervisor_container_gt.py
--rw-r--r--   0        0        0     4001 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/tadeed_specs_hack.py
--rw-r--r--   0        0        0     8981 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/tavalidatorcert_algo_create.py
--rw-r--r--   0        0        0    10763 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/tavalidatorcert_algo_transfer.py
--rw-r--r--   0        0        0     5142 2023-03-01 11:32:48.352980 gridworks_atn-0.2.3/src/gwatn/types/terminalasset_certify_hack.py
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 gridworks_atn-0.2.3/setup.py
--rw-r--r--   0        0        0     4041 1970-01-01 00:00:00.000000 gridworks_atn-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-29 18:36:00.003173 gridworks_atn-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3002 2023-04-29 18:36:00.003173 gridworks_atn-0.2.4/README.md
+-rw-r--r--   0        0        0     2150 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      336 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/__init__.py
+-rw-r--r--   0        0        0      226 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/__main__.py
+-rw-r--r--   0        0        0     7480 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/api_types.py
+-rw-r--r--   0        0        0    21829 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/atn_actor_base.py
+-rw-r--r--   0        0        0     4840 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/atn_utils.py
+-rw-r--r--   0        0        0     4871 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/config.py
+-rw-r--r--   0        0        0     6148 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/.DS_Store
+-rw-r--r--   0        0        0      202 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/__init__.py
+-rw-r--r--   0        0        0    23507 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/base_g_node.py
+-rw-r--r--   0        0        0      583 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/d_edge.py
+-rw-r--r--   0        0        0     7812 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/d_graph.py
+-rw-r--r--   0        0        0     1559 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/d_node.py
+-rw-r--r--   0        0        0     5366 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/g_node.py
+-rw-r--r--   0        0        0     6791 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/g_node_instance.py
+-rw-r--r--   0        0        0      734 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/gps_point.py
+-rw-r--r--   0        0        0     2482 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/market_type.py
+-rw-r--r--   0        0        0     1494 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/supervisor_container.py
+-rw-r--r--   0        0        0    14466 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/demo_methods.py
+-rw-r--r--   0        0        0      276 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dev_utils/__init__.py
+-rw-r--r--   0        0        0     1792 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_discoverer.py
+-rw-r--r--   0        0        0    11883 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_ta_owner.py
+-rw-r--r--   0        0        0    10994 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_validator.py
+-rw-r--r--   0        0        0     1171 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dev_utils/make_plants.py
+-rw-r--r--   0        0        0    11409 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dispatch_contract.py
+-rw-r--r--   0        0        0    12463 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/application.json
+-rw-r--r--   0        0        0     5229 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/approval.teal
+-rw-r--r--   0        0        0       40 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/clear.teal
+-rw-r--r--   0        0        0     3937 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/contract.json
+-rw-r--r--   0        0        0     2116 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/enums/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/algo_cert_type.py
+-rw-r--r--   0        0        0      638 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/atn_spaceheat_strategy_name.py
+-rw-r--r--   0        0        0      990 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/core_g_node_role.py
+-rw-r--r--   0        0        0      700 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/distribution_tariff.py
+-rw-r--r--   0        0        0      598 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/emitter_pump_feedback_model.py
+-rw-r--r--   0        0        0      614 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/energy_supply_type.py
+-rw-r--r--   0        0        0     2246 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/enums/g_node_role.py
+-rw-r--r--   0        0        0      992 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/g_node_status.py
+-rw-r--r--   0        0        0      933 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/gni_status.py
+-rw-r--r--   0        0        0      563 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/market_price_unit.py
+-rw-r--r--   0        0        0      590 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/market_quantity_unit.py
+-rw-r--r--   0        0        0     1394 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/market_type_name.py
+-rw-r--r--   0        0        0     1326 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/message_category.py
+-rw-r--r--   0        0        0     1189 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/message_category_symbol.py
+-rw-r--r--   0        0        0      928 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/mixing_valve_feedback_model.py
+-rw-r--r--   0        0        0      626 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/recognized_currency_unit.py
+-rw-r--r--   0        0        0      570 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/recognized_temperature_unit.py
+-rw-r--r--   0        0        0     1331 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/strategy_name.py
+-rw-r--r--   0        0        0     1081 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/supervisor_container_status.py
+-rw-r--r--   0        0        0     1918 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/enums/telemetry_name.py
+-rw-r--r--   0        0        0      795 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/universe_type.py
+-rw-r--r--   0        0        0     6718 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/freedom_hack.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/py.typed
+-rw-r--r--   0        0        0     7945 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/python_ta_daemon.json
+-rw-r--r--   0        0        0    12518 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/python_ta_daemon.py
+-rw-r--r--   0        0        0    26857 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/scada_actor.py
+-rw-r--r--   0        0        0      834 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/scada_codec.py
+-rw-r--r--   0        0        0     4870 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/simple_atn_actor.py
+-rw-r--r--   0        0        0     3169 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/ta_daemon_rest_api.py
+-rw-r--r--   0        0        0      460 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/ta_validator_rest_api.py
+-rw-r--r--   0        0        0    47761 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/two_channel_actor_base.py
+-rw-r--r--   0        0        0    13293 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/types/__init__.py
+-rw-r--r--   0        0        0     7780 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/accepted_bid.py
+-rw-r--r--   0        0        0    20134 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/atn_bid.py
+-rw-r--r--   0        0        0    34181 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/atn_params_heatpumpwithbooststore.py
+-rw-r--r--   0        0        0     7953 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/atn_params_report_heatpumpwithbooststore.py
+-rw-r--r--   0        0        0    20209 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/base_g_node_gt.py
+-rw-r--r--   0        0        0     8221 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/basegnode_scada_create.py
+-rw-r--r--   0        0        0    11106 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/csv_distp_sync.py
+-rw-r--r--   0        0        0    11354 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/csv_eprt_sync.py
+-rw-r--r--   0        0        0    11280 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/csv_heat_profile.py
+-rw-r--r--   0        0        0    21761 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/csv_weather_forecast_sync.py
+-rw-r--r--   0        0        0     1067 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/types/data_channel.py
+-rw-r--r--   0        0        0     9785 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/discoverycert_algo_create.py
+-rw-r--r--   0        0        0     7659 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/dispatch_contract_confirmed_heatpumpwithbooststore.py
+-rw-r--r--   0        0        0    38712 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/flo_params_heatpumpwithbooststore.py
+-rw-r--r--   0        0        0    24513 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/types/g_node_gt.py
+-rw-r--r--   0        0        0    15767 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/g_node_instance_gt.py
+-rw-r--r--   0        0        0     8106 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0     6718 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/gw_cert_id.py
+-rw-r--r--   0        0        0     3501 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/heartbeat_a.py
+-rw-r--r--   0        0        0     4539 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/heartbeat_algo_audit.py
+-rw-r--r--   0        0        0     8767 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/types/heartbeat_b.py
+-rw-r--r--   0        0        0     5919 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_create.py
+-rw-r--r--   0        0        0     7420 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     8742 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_transfer.py
+-rw-r--r--   0        0        0     7959 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/join_dispatch_contract.py
+-rw-r--r--   0        0        0    12341 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/latest_price.py
+-rw-r--r--   0        0        0     4928 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/market_slot.py
+-rw-r--r--   0        0        0    17073 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/market_type_gt.py
+-rw-r--r--   0        0        0     5294 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/new_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     5196 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/new_tadeed_send.py
+-rw-r--r--   0        0        0     5024 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/old_tadeed_algo_return.py
+-rw-r--r--   0        0        0     8361 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/price_quantity.py
+-rw-r--r--   0        0        0     2392 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/price_quantity_unitless.py
+-rw-r--r--   0        0        0     5580 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/ready.py
+-rw-r--r--   0        0        0     4904 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/scada_cert_transfer.py
+-rw-r--r--   0        0        0     6545 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/sim_scada_driver_report.py
+-rw-r--r--   0        0        0     8097 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/sim_timestep.py
+-rw-r--r--   0        0        0     3120 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/sla_enter.py
+-rw-r--r--   0        0        0     7390 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/snapshot_heatpumpwithbooststore.py
+-rw-r--r--   0        0        0     6080 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/super_starter.py
+-rw-r--r--   0        0        0    12065 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/supervisor_container_gt.py
+-rw-r--r--   0        0        0     4001 2023-04-29 18:36:00.023173 gridworks_atn-0.2.4/src/gwatn/types/tadeed_specs_hack.py
+-rw-r--r--   0        0        0     8981 2023-04-29 18:36:00.023173 gridworks_atn-0.2.4/src/gwatn/types/tavalidatorcert_algo_create.py
+-rw-r--r--   0        0        0    10763 2023-04-29 18:36:00.023173 gridworks_atn-0.2.4/src/gwatn/types/tavalidatorcert_algo_transfer.py
+-rw-r--r--   0        0        0     5142 2023-04-29 18:36:00.023173 gridworks_atn-0.2.4/src/gwatn/types/terminalasset_certify_hack.py
+-rw-r--r--   0        0        0     4053 1970-01-01 00:00:00.000000 gridworks_atn-0.2.4/PKG-INFO
```

### Comparing `gridworks_atn-0.2.3/LICENSE` & `gridworks_atn-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/README.md` & `gridworks_atn-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/pyproject.toml` & `gridworks_atn-0.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-atn"
-version = "0.2.3"
+version = "0.2.4"
 description = "Gridworks Atn Spaceheat"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "None"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-atn"
 repository = "https://github.com/thegridelectric/gridworks-atn"
 documentation = "https://gridworks-atn.readthedocs.io"
@@ -16,17 +16,17 @@
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/thegridelectric/gridworks-atn/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-gridworks = "^0.1.4"
-gridworks-protocol = "^0.2.6"
-boto3 = "^1.26.3"
+gridworks = "^0.2.1"
+gridworks-protocol = "^0.4.5"
+gridworks-proactor = "^0.1.8"
 paho-mqtt = "^1.6.1"
 
 types-requests = "^2.28.11.2"
 numpy = "^1.23.4"
 
 
 
@@ -51,14 +51,15 @@
 safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 myst-parser = {version = ">=0.16.1"}
+xlsxwriter = "^3.0.9"
 
 [tool.poetry.scripts]
 gridworks-atn = "gwatn.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.17.0"
 rich = "^12.6.0"
```

### Comparing `gridworks_atn-0.2.3/src/gwatn/api_types.py` & `gridworks_atn-0.2.4/src/gwatn/api_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         "flo.params.heatpumpwithbooststore": "000",
         "g.node.gt": "002",
         "g.node.instance.gt": "000",
         "gt.dispatch.boolean": "110",
         "gw.cert.id": "000",
         "heartbeat.a": "100",
         "heartbeat.algo.audit": "000",
-        "heartbeat.b": "000",
+        "heartbeat.b": "001",
         "initial.tadeed.algo.create": "000",
         "initial.tadeed.algo.optin": "002",
         "initial.tadeed.algo.transfer": "000",
         "join.dispatch.contract": "000",
         "latest.price": "000",
         "market.slot": "000",
         "market.type.gt": "000",
@@ -168,15 +168,15 @@
         "flo.params.heatpumpwithbooststore.000": "Active",
         "g.node.gt.002": "Pending",
         "g.node.instance.gt.000": "Pending",
         "gt.dispatch.boolean.110": "Pending",
         "gw.cert.id.000": "Active",
         "heartbeat.a.100": "Pending",
         "heartbeat.algo.audit.000": "Pending",
-        "heartbeat.b.000": "Pending",
+        "heartbeat.b.001": "Pending",
         "initial.tadeed.algo.create.000": "Active",
         "initial.tadeed.algo.optin.002": "Active",
         "initial.tadeed.algo.transfer.000": "Active",
         "join.dispatch.contract.000": "Active",
         "latest.price.000": "Pending",
         "market.slot.000": "Pending",
         "market.type.gt.000": "Pending",
```

### Comparing `gridworks_atn-0.2.3/src/gwatn/atn_actor_base.py` & `gridworks_atn-0.2.4/src/gwatn/atn_actor_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,118 +2,142 @@
 import functools
 import logging
 import random
 import time
 import uuid
 from abc import abstractmethod
 from typing import Optional
+from typing import cast
 from typing import no_type_check
 
 import gridworks.algo_utils as algo_utils
 import pendulum
 from algosdk.atomic_transaction_composer import TransactionWithSigner
 from algosdk.future.transaction import *
 from algosdk.v2client.algod import AlgodClient
 from beaker.client import ApplicationClient
 from gridworks.algo_utils import BasicAccount
 from gridworks.enums import GNodeRole
 from gridworks.message import as_enum
+from gwproto.message import Message as ScadaMessage
+from gwproto.messages import Ack
+from gwproto.messages import GtShStatusEvent
+from gwproto.messages import PeerActiveEvent
+from gwproto.messages import Ping as GridworksPing
+from gwproto.messages import SnapshotSpaceheatEvent
 from pydantic import BaseModel
 
 from gwatn.config import AtnSettings
 from gwatn.dispatch_contract import DispatchContract
 from gwatn.enums import AlgoCertType
 from gwatn.enums import MessageCategorySymbol
 from gwatn.enums import UniverseType
 from gwatn.two_channel_actor_base import TwoChannelActorBase
 from gwatn.types import AtnParamsHeatpumpwithbooststore as AtnParams
 from gwatn.types import (
     DispatchContractConfirmedHeatpumpwithbooststore_Maker as DispatchContractConfirmed_Maker,
 )
+from gwatn.types import GtShStatus
 from gwatn.types import GwCertId
 from gwatn.types import GwCertId_Maker
 from gwatn.types import HeartbeatA
 from gwatn.types import HeartbeatA_Maker
 from gwatn.types import HeartbeatB
 from gwatn.types import HeartbeatB_Maker
 from gwatn.types import JoinDispatchContract
 from gwatn.types import JoinDispatchContract_Maker
 from gwatn.types import LatestPrice
 from gwatn.types import LatestPrice_Maker
+from gwatn.types import PowerWatts
 from gwatn.types import SimTimestep
 from gwatn.types import SimTimestep_Maker
+from gwatn.types import SnapshotSpaceheat
 
 
 LOG_FORMAT = (
     "%(levelname) -10s %(sasctime)s %(name) -30s %(funcName) "
     "-35s %(lineno) -5d: %(message)s"
 )
 LOGGER = logging.getLogger(__name__)
 
 
 class HbStatus(BaseModel):
     LastHeartbeatReceivedMs: int
     AtnLastHex: str = "0"
     ScadaLastHex: str = "0"
+    # To see beaker issue an ABI complaint:
+    # ScadaLastHex: Optional[str] = None
+    #
+    # This will create an HbStatus with ScadaLastHex of None
+    # when the Atn is initialized.
 
 
 def dummy_atn_params() -> AtnParams:
     return AtnParams(
         SliceDurationMinutes=60,
         FloSlices=48,
         GNodeAlias="d1.isone.dummy.ta",
         GNodeInstanceId="00000000-0000-0000-0000-000000000000",
         TypeName="atn.params.heatpumpwithbooststore",
         Version="000",
     )
 
 
 class AtnActorBase(TwoChannelActorBase):
-    def __init__(self, settings: AtnSettings):
+    def __init__(self, settings: AtnSettings, use_algo: bool = False):
         super().__init__(settings=settings)
         self.settings: AtnSettings = settings
         self.scada_gni_id = settings.scada_gni_id
-        self.acct: BasicAccount = BasicAccount(settings.sk.get_secret_value())
-        self.client: AlgodClient = AlgodClient(
-            settings.algo_api_secrets.algod_token.get_secret_value(),
-            settings.public.algod_address,
-        )
-        if algo_utils.algos(self.acct.addr) < 5:
-            raise Exception(
-                f"Insufficiently funded. Make sure atn has at least 5 algos"
-            )
-        # TODO: move this into spaceheat along with join_dispatch_contract_received
-        self.atn_params: AtnParams = dummy_atn_params()
-        self.sp = self.client.suggested_params()
-        self.sp.flat_fee = True
-        self.sp.fee = 2000
-        # this is initialized with the AppId provided by the SCADA
-        self.dc_app_id: Optional[int] = None
-        self.dc_client: Optional[ApplicationClient] = None
-        self.check_for_dispatch_contract()
-        self.universe_type = as_enum(
-            self.settings.universe_type_value, UniverseType, UniverseType.default()
-        )
-        self.trading_rights_id: Optional[GwCertId] = None
-        self.update_trading_rights()
-        self.hb_status = HbStatus(LastHeartbeatReceivedMs=int(time.time() * 1000))
         self._time: float = self.get_initial_time_s()
 
+        if use_algo is True:
+            self.acct: BasicAccount = BasicAccount(settings.sk.get_secret_value())
+            self.client: AlgodClient = AlgodClient(
+                settings.algo_api_secrets.algod_token.get_secret_value(),
+                settings.public.algod_address,
+            )
+            if algo_utils.algos(self.acct.addr) < 5:
+                raise Exception(
+                    f"Insufficiently funded. Make sure atn has at least 5 algos"
+                )
+            # TODO: move this into spaceheat along with join_dispatch_contract_received
+            self.atn_params: AtnParams = dummy_atn_params()
+            self.sp = self.client.suggested_params()
+            self.sp.flat_fee = True
+            self.sp.fee = 2000
+            # this is initialized with the AppId provided by the SCADA
+            self.dc_app_id: Optional[int] = None
+            self.dc_client: Optional[ApplicationClient] = None
+            self.check_for_dispatch_contract()
+            self.universe_type = as_enum(
+                self.settings.universe_type_value, UniverseType, UniverseType.default()
+            )
+            self.trading_rights_id: Optional[GwCertId] = None
+            self.update_trading_rights()
+            self.hb_status = HbStatus(LastHeartbeatReceivedMs=int(time.time() * 1000))
+
     def local_rabbit_startup(self) -> None:
         rjb = MessageCategorySymbol.rjb.value
         tc_alias_lrh = self.settings.time_coordinator_alias.replace(".", "-")
         binding = f"{rjb}.{tc_alias_lrh}.timecoordinator.sim-timestep"
 
         cb = functools.partial(self.on_timecoordinator_bindok, binding=binding)
         self._consume_channel.queue_bind(
             self.queue_name, "timecoordinatormic_tx", routing_key=binding, callback=cb
         )
         LOGGER.info(
             f"Queue {self.queue_name} bound to timecoordinatormic_tx with {binding} "
         )
+        scada_alias_lrh = self.scada_alias.replace(".", "-")
+        binding = f"gw.{scada_alias_lrh}.#"
+        cb = functools.partial(self.on_scada_bindok, binding=binding)
+        self._consume_channel.queue_bind(
+            self.queue_name, "amq.topic", routing_key=binding, callback=cb
+        )
+        LOGGER.info(f"Queue {self.queue_name} bound to amq.topic with {binding} ")
         pong = HeartbeatA_Maker(
             my_hex=str(random.choice("0123456789abcdef")), your_last_hex="0"
         ).tuple
         self.send_message(
             payload=pong,
             to_role=GNodeRole.Supervisor,
             to_g_node_alias=self.settings.my_super_alias,
@@ -127,14 +151,18 @@
     def strategy_rabbit_startup(self) -> None:
         pass
 
     @no_type_check
     def on_timecoordinator_bindok(self, _unused_frame, binding) -> None:
         LOGGER.info(f"Queue {self.queue_name} bound with {binding}")
 
+    @no_type_check
+    def on_scada_bindok(self, _unused_frame, binding) -> None:
+        LOGGER.info(f"Queue {self.queue_name} bound with {binding}")
+
     def time(self) -> float:
         if self.universe_type == UniverseType.Dev:
             return self._time
         else:
             return time.time()
 
     def get_initial_time_s(self) -> float:
@@ -146,14 +174,91 @@
     def prepare_for_death(self) -> None:
         self.actor_main_stopped = True
 
     ########################
     ## Receives
     ########################
 
+    def route_scada_message(self, from_alias: str, message: ScadaMessage) -> None:
+        """Routes messages from the SCADA to methods that should be overwritten
+        in derived class"""
+
+        # if message.Header.Src != self.scada_alias:
+        #     LOGGER.info(
+        #         f"Ignoring scada message from {message.Header.Src}. My scada is {self.scada_alias}"
+        #     )
+        #     LOGGER.info(f"{message}")
+        #     return
+        if message.Header.AckRequired == True:
+            payload = Ack(AckMessageID=message.Header.MessageId)
+            self.send_scada_message(payload)
+
+        path_dbg = 0
+        match message.Payload:
+            case GridworksPing():
+                self._process_gridworks_ping_from_scada(
+                    cast(GridworksPing, message.Payload)
+                )
+            case GtShStatusEvent():
+                self._process_gt_sh_status_event_from_scada(
+                    cast(GtShStatusEvent, message.Payload)
+                )
+            case PeerActiveEvent():
+                self._process_peer_active_event_from_scada(
+                    cast(PeerActiveEvent, message.Payload)
+                )
+            case SnapshotSpaceheatEvent():
+                self._process_snapshot_spaceheat_event_from_scada(
+                    cast(SnapshotSpaceheatEvent, message.Payload)
+                )
+            case PowerWatts():
+                self._process_power_watts_from_scada(cast(PowerWatts, message.Payload))
+
+            case SnapshotSpaceheat():
+                self._process_snapshot_spaceheat_from_scada(
+                    cast(SnapshotSpaceheat, message.Payload)
+                )
+
+    @abstractmethod
+    def _process_gridworks_ping_from_scada(self, payload: GridworksPing) -> None:
+        """Atn has received gridworks.ping message from its SCADA"""
+        raise NotImplementedError
+
+    @abstractmethod
+    def _process_peer_active_event_from_scada(self, payload: PeerActiveEvent) -> None:
+        """Atn has received gridworks.event.comm.peer.active message from its SCADA"""
+        raise NotImplementedError
+
+    def _process_gt_sh_status_event_from_scada(self, payload: GtShStatusEvent) -> None:
+        """Atn has received gridworks.event.gt.sh.status message from its SCADA"""
+        gt_sh_status = payload.status
+        self._process_gt_sh_status_from_scada(payload=gt_sh_status)
+
+    def _process_snapshot_spaceheat_event_from_scada(
+        self, payload: SnapshotSpaceheatEvent
+    ) -> None:
+        """Atn has received  gridworks.event.snapshot.spaceheat message from its SCADA"""
+        snapshot_spaceheat = payload.snap
+        self._process_snapshot_spaceheat_from_scada(payload=snapshot_spaceheat)
+
+    @abstractmethod
+    def _process_gt_sh_status_from_scada(self, payload: GtShStatus) -> None:
+        """Atn has received gt.sh.status message from its SCADA"""
+        raise NotImplementedError
+
+    @abstractmethod
+    def _process_power_watts_from_scada(self, payload: PowerWatts) -> None:
+        """Atn has received power.watts message from its SCADA"""
+        raise NotImplementedError
+
+    @abstractmethod
+    def _process_snapshot_spaceheat_from_scada(self, payload: SnapshotSpaceheat):
+        """Atn has received a snapshot.sspaceheat message from the SCADA"""
+        raise NotImplementedError
+
     def route_message(
         self, from_alias: str, from_role: GNodeRole, payload: HeartbeatA
     ) -> None:
         self.payload = payload
         if payload.TypeName == HeartbeatA_Maker.type_name:
             if from_role != GNodeRole.Supervisor:
                 LOGGER.info(
@@ -232,15 +337,15 @@
             return
         self.hb_status.LastHeartbeatReceivedMs = int(time.time() * 1000)
         self.hb_status.ScadaLastHex = ping.MyHex
         self.hb_status.AtnLastHex = str(random.choice("0123456789abcdef"))
         LOGGER.info(f"Got {ping.MyHex}")
         # Does not send back. Atn waits for the DispatchContract's expected
         # one minute before sending.
-        print(f"Got heartbeat from scada: {ping}")
+        # print(f"Got heartbeat from scada: {ping}")
 
     def hb_to_scada(self):
         """Checks that Atn is in Dispatch Contract, sends a HeartbeatB to Scada,
         and then reports to DispatchContract"""
         if not self.in_dispatch_contract():
             LOGGER.info("Not sending hb to Scada - not in DispatchContract yet")
         ping = HeartbeatB_Maker(
@@ -252,15 +357,15 @@
             send_time_unix_ms=int(1000 * time.time()),
         ).tuple
         self.send_message(
             payload=ping,
             to_role=GNodeRole.Scada,
             to_g_node_alias=self.scada_alias,
         )
-        LOGGER.info(f"Sent hb {ping}")
+        LOGGER.info(f"Sent  {ping.MyHex}")
         # report to DispatchContract
         ptxn = PaymentTxn(self.acct.addr, self.sp, self.dc_client.app_addr, 1000)
         self.dc_client.call(
             DispatchContract.heartbeat_algo_audit,
             signed_proof=TransactionWithSigner(ptxn, self.acct.as_signer()),
             heartbeat=ping.as_dict(),
         )
@@ -313,18 +418,16 @@
 
         """
         if self.in_dispatch_contract():
             LOGGER.warning(
                 f"Ignoring JoinDispatchContract - already in dispatch contract {self.dc_app_id}"
             )
             return
-        self.g_node_instance_id = str(uuid.uuid4())
         self.scada_gni_id = payload.FromGNodeInstanceId
         with open(".env", "a") as file:
-            file.write(f'ATN_G_NODE_INSTANCE_ID="{self.g_node_instance_id}"\n')
             file.write(f'ATN_SCADA_GNI_ID="{payload.FromGNodeInstanceId}"\n')
         self.dc_client = ApplicationClient(
             client=self.client,
             app=DispatchContract(),
             signer=self.acct.as_signer(),
             app_id=payload.DispatchContractAppId,
         )
```

### Comparing `gridworks_atn-0.2.3/src/gwatn/atn_utils.py` & `gridworks_atn-0.2.4/src/gwatn/atn_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/config.py` & `gridworks_atn-0.2.4/src/gwatn/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/data_classes/.DS_Store` & `gridworks_atn-0.2.4/src/gwatn/data_classes/.DS_Store`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/data_classes/base_g_node.py` & `gridworks_atn-0.2.4/src/gwatn/data_classes/base_g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/data_classes/d_edge.py` & `gridworks_atn-0.2.4/src/gwatn/data_classes/d_edge.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/data_classes/d_graph.py` & `gridworks_atn-0.2.4/src/gwatn/data_classes/d_graph.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/data_classes/d_node.py` & `gridworks_atn-0.2.4/src/gwatn/data_classes/d_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/data_classes/g_node.py` & `gridworks_atn-0.2.4/src/gwatn/data_classes/g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/data_classes/g_node_instance.py` & `gridworks_atn-0.2.4/src/gwatn/data_classes/g_node_instance.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/data_classes/gps_point.py` & `gridworks_atn-0.2.4/src/gwatn/data_classes/gps_point.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/data_classes/market_type.py` & `gridworks_atn-0.2.4/src/gwatn/data_classes/market_type.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/data_classes/supervisor_container.py` & `gridworks_atn-0.2.4/src/gwatn/data_classes/supervisor_container.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/demo_methods.py` & `gridworks_atn-0.2.4/src/gwatn/demo_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -379,36 +379,36 @@
     print("")
     print("")
     print("Certifying MollyMetermaid as a TaValidator")
     print("")
     print("")
     time.sleep(2)
 
-    print("")
-    print("")
-    print("Starting up Molly Metermaid's Validator API")
-    print("")
-    print("")
-    time.sleep(2)
-    cmd = "docker compose -f docker-api.yml up -d"
-    subprocess.run(cmd.split())
+    # print("")
+    # print("")
+    # print("Starting up Molly Metermaid's Validator API")
+    # print("")
+    # print("")
+    # time.sleep(2)
+    # cmd = "docker compose -f docker-api.yml up -d"
+    # subprocess.run(cmd.split())
 
-    print("Verify that it works by inspecting http://localhost:8001/docs")
-    print("")
-    print("")
+    # print("Verify that it works by inspecting http://localhost:8001/docs")
+    # print("")
+    # print("")
 
-    time.sleep(2)
-    print("This also started up the API half of the MarketMaker.")
-    print("Verify that it is working:")
+    # time.sleep(2)
+    # print("This also started up the API half of the MarketMaker.")
+    # print("Verify that it is working:")
 
-    print("- http://localhost:7997/ shows market maker information")
-    print(
-        "- http://localhost:7997/get-time/, which should be 0 unix time, but will show the time"
-    )
-    print(" of the simulation once that starts")
+    # print("- http://localhost:7997/ shows market maker information")
+    # print(
+    #     "- http://localhost:7997/get-time/, which should be 0 unix time, but will show the time"
+    # )
+    # print(" of the simulation once that starts")
 
     rr = certify_molly_metermaid()
 
     pprint(rr)
     if rr.HttpStatusCode > 200:
         raise Exception("Stopping demo due to errors")
 
@@ -497,28 +497,26 @@
     print("")
     print("")
     time.sleep(2)
     input("HIT RETURN TO CONTINUE")
     print("")
     print("")
     print(
-        "In fact the AtomicTNodes do not exist yet. Go to http://d1-1.electricity.works:15672/#/queues"
+        "In fact the AtomicTNodes and SCADAS do not exist yet. Go to http://d1-1.electricity.works:15672/#/queues"
     )
     print("")
     print("")
     time.sleep(1)
     print("Username and password are the same:")
     print("")
     print("smqPublic")
     print("")
     print("")
     time.sleep(1)
-    print(
-        "You will only see the dummy queues, the world d1-Fxxx, and the market maker ...keene.F-xxx"
-    )
+    print("When they do, you will see queues representing AtomicTNodes and SCADAS ")
     # input("To start the atn actors (and time coordinator) in a docker instance, HIT RETURN")
     # )
     # print("")
     # print("")
     # print("It takes about 5 seconds for them to shop up. Look for them at")
     # print("http://d1-1.electricity.works:15672/#/queues")
     # print(
```

### Comparing `gridworks_atn-0.2.3/src/gwatn/dev_utils/dev_discoverer.py` & `gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_discoverer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/dev_utils/dev_ta_owner.py` & `gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_ta_owner.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/dev_utils/dev_validator.py` & `gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_validator.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/dev_utils/make_plants.py` & `gridworks_atn-0.2.4/src/gwatn/dev_utils/make_plants.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/dispatch_contract.py` & `gridworks_atn-0.2.4/src/gwatn/dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/dispatch_contract_artifacts/application.json` & `gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/application.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/dispatch_contract_artifacts/approval.teal` & `gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/approval.teal`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/dispatch_contract_artifacts/contract.json` & `gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/contract.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/__init__.py` & `gridworks_atn-0.2.4/src/gwatn/enums/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """ GwSchema Enums used in gwatn """
-from gwatn.enums.actor_class import ActorClass
+from gwproto.enums import ActorClass
+from gwproto.enums import LocalCommInterface
+from gwproto.enums import MakeModel
+from gwproto.enums import Role
+from gwproto.enums import TelemetryName
+from gwproto.enums import Unit
+
 from gwatn.enums.algo_cert_type import AlgoCertType
 from gwatn.enums.atn_spaceheat_strategy_name import AtnSpaceheatStrategyName
 from gwatn.enums.core_g_node_role import CoreGNodeRole
 from gwatn.enums.distribution_tariff import DistributionTariff
 from gwatn.enums.emitter_pump_feedback_model import EmitterPumpFeedbackModel
 from gwatn.enums.energy_supply_type import EnergySupplyType
 from gwatn.enums.g_node_role import GNodeRole
 from gwatn.enums.g_node_status import GNodeStatus
 from gwatn.enums.gni_status import GniStatus
-from gwatn.enums.local_comm_interface import LocalCommInterface
-from gwatn.enums.make_model import MakeModel
 from gwatn.enums.market_price_unit import MarketPriceUnit
 from gwatn.enums.market_quantity_unit import MarketQuantityUnit
 from gwatn.enums.market_type_name import MarketTypeName
 from gwatn.enums.message_category import MessageCategory
 from gwatn.enums.message_category_symbol import MessageCategorySymbol
 from gwatn.enums.mixing_valve_feedback_model import MixingValveFeedbackModel
 from gwatn.enums.recognized_currency_unit import RecognizedCurrencyUnit
 from gwatn.enums.recognized_temperature_unit import RecognizedTemperatureUnit
-from gwatn.enums.role import Role
 from gwatn.enums.strategy_name import StrategyName
 from gwatn.enums.supervisor_container_status import SupervisorContainerStatus
-from gwatn.enums.telemetry_name import TelemetryName
-from gwatn.enums.unit import Unit
 from gwatn.enums.universe_type import UniverseType
 
 
 __all__ = [
     "AlgoCertType",
     "AtnSpaceheatStrategyName",
     "CoreGNodeRole",
```

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/algo_cert_type.py` & `gridworks_atn-0.2.4/src/gwatn/enums/algo_cert_type.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/atn_spaceheat_strategy_name.py` & `gridworks_atn-0.2.4/src/gwatn/enums/atn_spaceheat_strategy_name.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/core_g_node_role.py` & `gridworks_atn-0.2.4/src/gwatn/enums/core_g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/distribution_tariff.py` & `gridworks_atn-0.2.4/src/gwatn/enums/distribution_tariff.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/emitter_pump_feedback_model.py` & `gridworks_atn-0.2.4/src/gwatn/enums/emitter_pump_feedback_model.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/energy_supply_type.py` & `gridworks_atn-0.2.4/src/gwatn/enums/energy_supply_type.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/g_node_role.py` & `gridworks_atn-0.2.4/src/gwatn/enums/g_node_role.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,22 +20,24 @@
       * World: Adminstrative GNode responsible for managing and authorizing instances
       * TimeCoordinator: Responsible for managing time in simulations
       * Supervisor: Responsible for GNode actors running in a container
       * Scada: GNode associated to the device and code that directly monitors and actuates a Transactive Device
       * PriceService: Provides price forecasts for markets run by MarketMakers
       * WeatherService: Provides weather forecasts
       * AggregatedTNode: An aggregation of AtomicTNodes
+      * Persister: Responsible for acking events with delivery guarantees
     """
 
     GNode = auto()
     TerminalAsset = auto()
     Scada = auto()
     PriceService = auto()
     WeatherService = auto()
     AggregatedTNode = auto()
+    Persister = auto()
     AtomicTNode = auto()
     MarketMaker = auto()
     AtomicMeteringNode = auto()
     ConductorTopologyNode = auto()
     InterconnectionComponent = auto()
     World = auto()
     TimeCoordinator = auto()
```

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/g_node_status.py` & `gridworks_atn-0.2.4/src/gwatn/enums/g_node_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/gni_status.py` & `gridworks_atn-0.2.4/src/gwatn/enums/gni_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/local_comm_interface.py` & `gridworks_atn-0.2.4/src/gwatn/enums/message_category_symbol.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 from enum import auto
 from typing import List
 
 from fastapi_utils.enums import StrEnum
 
 
-class LocalCommInterface(StrEnum):
+class MessageCategorySymbol(StrEnum):
     """
-    Categorization of in-house comm mechanisms for SCADA
+    Shorthand symbols for MessageCategory000 Enum, used in meta-data like routing keys
 
     Choices and descriptions:
 
-      * Analog_4_20_mA:
-      * RS232:
-      * I2C:
-      * Wifi:
-      * SimRabbit:
-      * Unknown:
-      * Ethernet:
-      * OneWire:
-      * RS485:
+      * unknown: Default value
+      * rj: Serialized Json message sent on the world rabbit broker from one GNode actor to another
+      * rjb: Serailized Json message broadcast on the world rabbit broker by a GNode actor
+      * s: GwSerial protocol message sent on the world rabbit broker
+      * gw: Serialized Json message following MQTT topic format, sent on the world rabbit broker
+      * post: REST API post
+      * postack: REST API post response
+      * get: REST API GET
     """
 
-    ANALOG_4_20_MA = auto()
-    RS232 = auto()
-    I2C = auto()
-    WIFI = auto()
-    SIMRABBIT = auto()
-    UNKNOWN = auto()
-    ETHERNET = auto()
-    ONEWIRE = auto()
-    RS485 = auto()
+    unknown = auto()
+    rj = auto()
+    rjb = auto()
+    s = auto()
+    gw = auto()
+    post = auto()
+    postack = auto()
+    get = auto()
 
     @classmethod
-    def default(cls) -> "LocalCommInterface":
+    def default(cls) -> "MessageCategorySymbol":
         """
-        Returns default value UNKNOWN
+        Returns default value unknown
         """
-        return cls.UNKNOWN
+        return cls.unknown
 
     @classmethod
     def values(cls) -> List[str]:
         """
         Returns enum choices
         """
         return [elt.value for elt in cls]
```

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/market_price_unit.py` & `gridworks_atn-0.2.4/src/gwatn/enums/market_price_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/market_quantity_unit.py` & `gridworks_atn-0.2.4/src/gwatn/enums/market_quantity_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/market_type_name.py` & `gridworks_atn-0.2.4/src/gwatn/enums/market_type_name.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/message_category.py` & `gridworks_atn-0.2.4/src/gwatn/enums/message_category.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/mixing_valve_feedback_model.py` & `gridworks_atn-0.2.4/src/gwatn/enums/mixing_valve_feedback_model.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/recognized_currency_unit.py` & `gridworks_atn-0.2.4/src/gwatn/enums/recognized_currency_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/recognized_temperature_unit.py` & `gridworks_atn-0.2.4/src/gwatn/enums/recognized_temperature_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/strategy_name.py` & `gridworks_atn-0.2.4/src/gwatn/enums/strategy_name.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/supervisor_container_status.py` & `gridworks_atn-0.2.4/src/gwatn/enums/supervisor_container_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/enums/unit.py` & `gridworks_atn-0.2.4/src/gwatn/enums/universe_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,34 @@
 from enum import auto
 from typing import List
 
 from fastapi_utils.enums import StrEnum
 
 
-class Unit(StrEnum):
+class UniverseType(StrEnum):
     """
-    Specifies the physical unit of sensed data reported by SCADA
+    Allows for multiple GridWorks, in particular for development and shared simulations. [More Info](https://gridworks.readthedocs.io/en/latest/universe.html).
 
     Choices and descriptions:
 
-      * Unknown:
-      * Unitless:
-      * W:
-      * Celcius:
-      * Fahrenheit:
-      * Gpm:
-      * Wh:
-      * AmpsRms:
-      * VoltsRms:
+      * Dev: Simulation running on a single computer.
+      * Hybrid: Anything goes.
+      * Production: Money at stake.
     """
 
-    Unknown = auto()
-    Unitless = auto()
-    W = auto()
-    Celcius = auto()
-    Fahrenheit = auto()
-    Gpm = auto()
-    Wh = auto()
-    AmpsRms = auto()
-    VoltsRms = auto()
+    Dev = auto()
+    Hybrid = auto()
+    Production = auto()
 
     @classmethod
-    def default(cls) -> "Unit":
+    def default(cls) -> "UniverseType":
         """
-        Returns default value Unknown
+        Returns default value Dev
         """
-        return cls.Unknown
+        return cls.Dev
 
     @classmethod
     def values(cls) -> List[str]:
         """
         Returns enum choices
         """
         return [elt.value for elt in cls]
```

### Comparing `gridworks_atn-0.2.3/src/gwatn/python_ta_daemon.json` & `gridworks_atn-0.2.4/src/gwatn/python_ta_daemon.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/python_ta_daemon.py` & `gridworks_atn-0.2.4/src/gwatn/python_ta_daemon.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/scada_actor.py` & `gridworks_atn-0.2.4/src/gwatn/scada_actor.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/ta_daemon_rest_api.py` & `gridworks_atn-0.2.4/src/gwatn/ta_daemon_rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/two_channel_actor_base.py` & `gridworks_atn-0.2.4/src/gwatn/two_channel_actor_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,40 @@
 import time
 import uuid
 from abc import ABC
 from abc import abstractmethod
 from enum import auto
 from typing import Dict
 from typing import Optional
+from typing import TypeVar
 from typing import no_type_check
 
 import gridworks.property_format as property_format
 import gridworks.utils as utils
 import pika  # type: ignore
 from fastapi_utils.enums import StrEnum
 from gridworks.enums import GNodeRole
 from gridworks.errors import SchemaError
+from gwproto.message import Message as ScadaMessage
+from gwproto.messages import Ack
+from pydantic import ValidationError
 
 import gwatn.api_types as api_types
 from gwatn.config import AtnSettings
 from gwatn.enums import MessageCategory
 from gwatn.enums import MessageCategorySymbol
 from gwatn.enums import UniverseType
+from gwatn.scada_codec import ScadaCodec
 from gwatn.types import HeartbeatA
 from gwatn.types import HeartbeatA_Maker
 
 
+PayloadT = TypeVar("PayloadT")
+
+
 class RabbitRole(StrEnum):
     atomictnode = auto()
     marketmaker = auto()
     scada = auto()
     supervisor = auto()
     timecoordinator = auto()
     world = auto()
@@ -69,35 +77,49 @@
     UNKNOWN_ROUTING_KEY_TYPE = "UnknownRoutingKeyType"
     UNHANDLED_ROUTING_KEY_TYPE = "UnhandledRoutingKeyType"
     UNKNOWN_MESSAGE_CATEGORY_SYMBOL = "UnknownMessageCategorySymbol"
     UNKNOWN_TYPE_NAME = "UnknownTypeName"
     FROM_GNODE_DECODING_PROBLEM = "FromGNodeDecodingProblem"
     UNKONWN_GNODE = "UnknownGNode"
     TO_DIRECT_ROUTING = "ToDirectRouting"
+    GWPROTO_DECODING_PROBLEM = "GwprotoDecodingProblem"
 
 
 BACKOFF_NUMBER = 16
 
 LOG_FORMAT = (
     "%(levelname) -10s %(asctime)s %(name) -30s %(funcName) "
     "-35s %(lineno) -5d: %(message)s"
 )
 LOGGER = logging.getLogger(__name__)
 
 LOGGER.setLevel(logging.WARNING)
 
+import json
+from typing import List
+
+from pydantic import BaseModel
+
+
+class DbgMsg(BaseModel):
+    RoutingKey: str
+    MessageType: bytes
+    MessageTuple: ScadaMessage
+
 
 class TwoChannelActorBase(ABC):
     SHUTDOWN_INTERVAL = 0.1
 
     def __init__(
         self,
         settings: AtnSettings,
         api_type_maker_by_name: Dict[str, HeartbeatA_Maker] = api_types.TypeMakerByName,
     ):
+        self.scada_codec = ScadaCodec()
+        self.dbg_messages: List[DbgMsg] = []
         self.api_type_maker_by_name = api_type_maker_by_name
         self.latest_routing_key: Optional[str] = None
         self.shutting_down: bool = False
         self.alias: str = settings.g_node_alias
         self.g_node_instance_id: str = settings.g_node_instance_id
         self.g_node_role: GNodeRole = GNodeRole(settings.g_node_role_value)
         self.rabbit_role: RabbitRole = RabbitRolebyRole[self.g_node_role]
@@ -188,18 +210,54 @@
         is the message that was sent.
         :param pika.channel.Channel _unused_channel: The channel object
         :param pika.Spec.Basic.Deliver: basic_deliver method
         :param pika.Spec.BasicProperties: properties
         :param bytes body: The message body
         """
         self.latest_routing_key = basic_deliver.routing_key
-        LOGGER.debug(
+        routing_key: str = basic_deliver.routing_key
+
+        LOGGER.info(
             f"{self.alias}: Got {basic_deliver.routing_key} with delivery tag {basic_deliver.delivery_tag}"
         )
         self.acknowledge_message(basic_deliver.delivery_tag)
+        msg_category = self.message_category_from_routing_key(routing_key)
+
+        try:
+            from_alias = self.from_alias_from_routing_key(routing_key)
+        except SchemaError as e:
+            self._latest_on_message_diagnostic = (
+                OnReceiveMessageDiagnostic.FROM_GNODE_DECODING_PROBLEM
+            )
+            LOGGER.warning(
+                f"IGNORING MESSAGE. {self._latest_on_message_diagnostic}: {e}"
+            )
+            return
+
+        if msg_category == MessageCategory.MqttJsonBroadcast:
+            try:
+                message = self.scada_codec.decode(topic="gw", payload=body)
+            except ValidationError as e:
+                self._latest_on_message_diagnostic = (
+                    OnReceiveMessageDiagnostic.GWPROTO_DECODING_PROBLEM
+                )
+                LOGGER.warning(
+                    f"IGNORING MESSAGE. {self._latest_on_message_diagnostic}: {e}"
+                )
+                return
+            self.dbg_messages.append(
+                DbgMsg(
+                    RoutingKey=basic_deliver.routing_key,
+                    MessageType=body,
+                    MessageTuple=message,
+                )
+            )
+            self.route_scada_message(from_alias=from_alias, message=message)
+            return
+
         try:
             type_name = self.get_payload_type_name(basic_deliver)
         except SchemaError:
             return
         self.type_name = type_name
 
         if type_name not in self.api_type_maker_by_name.keys():
@@ -215,26 +273,14 @@
             payload = self.api_type_maker_by_name[type_name].type_to_tuple(body)
         except Exception as e:
             LOGGER.warning(
                 f"TypeName for incoming message claimed to be {type_name}, but was not true! Failed to make a {self.api_type_maker_by_name[type_name].tuple}"
             )
             return
 
-        routing_key: str = basic_deliver.routing_key
-
-        try:
-            from_alias = self.from_alias_from_routing_key(routing_key)
-        except SchemaError as e:
-            self._latest_on_message_diagnostic = (
-                OnReceiveMessageDiagnostic.FROM_GNODE_DECODING_PROBLEM
-            )
-            LOGGER.warning(
-                f"IGNORING MESSAGE. {self._latest_on_message_diagnostic}: {e}"
-            )
-            return
         try:
             from_role = self.from_role_from_routing_key(routing_key)
         except SchemaError as e:
             self._latest_on_message_diagnostic = (
                 OnReceiveMessageDiagnostic.FROM_GNODE_DECODING_PROBLEM
             )
             LOGGER.warning(
@@ -253,14 +299,56 @@
 
     @abstractmethod
     def route_message(
         self, from_alias: str, from_role: GNodeRole, payload: HeartbeatA
     ) -> None:
         raise NotImplementedError
 
+    def route_scada_message(self, from_alias: str, message: ScadaMessage) -> None:
+        """This router should be overwritten by derived class"""
+        ...
+
+    @no_type_check
+    def send_scada_message(
+        self, payload: PayloadT, ack_required: bool = False
+    ) -> OnSendMessageDiagnostic:
+        """Publish an MqttBroadcast message to the SCADA partner
+
+        Args: message: A ScadaMessage (TypeName gw)
+        """
+        message_id = str(uuid.uuid4())
+        message = ScadaMessage(
+            Src=self.alias,
+            Payload=payload,
+            AckRequired=ack_required,
+            MessageId=message_id,
+        )
+        message_as_type = self.scada_codec.encode(message)
+        routing_key = self.scada_routing_key(payload=payload)
+        publish_exchange = "amq.topic"
+        properties = pika.BasicProperties(
+            reply_to=self.queue_name,
+            app_id=self.alias,
+            type=MessageCategory.MqttJsonBroadcast,
+            correlation_id=message_id,
+        )
+
+        try:
+            self._publish_channel.basic_publish(
+                exchange=publish_exchange,
+                routing_key=routing_key,
+                body=message_as_type,
+                properties=properties,
+            )
+            LOGGER.info(f" [x] Sent {payload.TypeName} w routing key {routing_key}")
+            return OnSendMessageDiagnostic.MESSAGE_SENT
+        except BaseException:
+            LOGGER.exception("Problem publishing scada message")
+            return OnSendMessageDiagnostic.UNKNOWN_ERROR
+
     @no_type_check
     def send_message(
         self,
         payload: HeartbeatA,
         message_category: MessageCategory = MessageCategory.RabbitJsonDirect,
         to_role: Optional[GNodeRole] = None,
         to_g_node_alias: Optional[str] = None,
@@ -284,38 +372,45 @@
         """
 
         if self._stopping:
             return OnSendMessageDiagnostic.STOPPING_SO_NOT_SENDING
         if self._stopped:
             return OnSendMessageDiagnostic.STOPPED_SO_NOT_SENDING
 
+        if message_category == MessageCategory.MqttJsonBroadcast:
+            raise Exception(
+                f"Use send_scada_message to send messages to SCADA: {payload}"
+            )
+
         if "MessageId" in payload.as_dict():
             correlation_id = payload.MessageId
         else:
             correlation_id = str(uuid.uuid4())
 
+        properties = pika.BasicProperties(
+            reply_to=self.queue_name,
+            app_id=self.alias,
+            type=message_category,
+            correlation_id=correlation_id,
+        )
+
+        publish_exchange = self._publish_exchange
         if message_category is MessageCategory.RabbitJsonDirect:
             if not isinstance(to_role, GNodeRole):
                 raise Exception("Must include to_role for a direct message")
             if not property_format.is_left_right_dot(to_g_node_alias):
                 raise Exception(
                     f"to_g_node_alias must have LrdAliasFormat. Got {to_g_node_alias}"
                 )
             routing_key = self.direct_routing_key(
                 to_role=to_role,
                 payload=payload,
                 to_g_node_alias=to_g_node_alias,
             )
 
-            properties = pika.BasicProperties(
-                reply_to=self.queue_name,
-                app_id=self.alias,
-                type=message_category.RabbitJsonDirect,
-                correlation_id=correlation_id,
-            )
         elif message_category is MessageCategory.RabbitJsonBroadcast:
             routing_key = self.broadcast_routing_key(
                 payload=payload, radio_channel=radio_channel
             )
             properties = pika.BasicProperties(
                 reply_to=self.queue_name,
                 app_id=self.alias,
@@ -330,15 +425,15 @@
             return OnSendMessageDiagnostic.CHANNEL_NOT_OPEN
         if not self._publish_channel.is_open:
             LOGGER.error(f"Publish channel not open so not sending {routing_key}")
             return OnSendMessageDiagnostic.CHANNEL_NOT_OPEN
 
         try:
             self._publish_channel.basic_publish(
-                exchange=self._publish_exchange,
+                exchange=publish_exchange,
                 routing_key=routing_key,
                 body=payload.as_type(),
                 properties=properties,
             )
             LOGGER.debug(f" [x] Sent {payload.TypeName} w routing key {routing_key}")
             return OnSendMessageDiagnostic.MESSAGE_SENT
 
@@ -923,60 +1018,51 @@
         else:
             if not property_format.is_left_right_dot(radio_channel):
                 raise Exception(
                     f"radio_channel must have LrdAliasFormat. Got {radio_channel}"
                 )
             return f"{msg_type}.{from_alias_lrh}.{from_role}.{type_name_lrh}.{radio_channel}"
 
+    def scada_routing_key(self, payload: Ack) -> str:
+        if self.g_node_role != GNodeRole.AtomicTNode:
+            raise Exception(f"Only send messages to SCADA if role is AtomicTNode!")
+        msg_type = MessageCategorySymbol.gw.value
+        from_alias_lrh = self.alias.replace(".", "-")
+        type_name_lrh = payload.TypeName.replace(".", "-")
+
+        scada_routing_key = f"{msg_type}.{from_alias_lrh}.{type_name_lrh}"
+        return scada_routing_key
+
     def direct_routing_key(
         self, to_role: GNodeRole, payload: HeartbeatA, to_g_node_alias: str
     ) -> str:
         msg_type = MessageCategorySymbol.rj.value
         from_lrh_alias = self.alias.replace(".", "-")
         from_role = self.rabbit_role.value
         to_role_val = RabbitRolebyRole[to_role].value
         to_lrh_alias = to_g_node_alias.replace(".", "-")
         type_name_lrh = payload.TypeName.replace(".", "-")
 
         direct_routing_key = f"{msg_type}.{from_lrh_alias}.{from_role}.{type_name_lrh}.{to_role_val}.{to_lrh_alias}"
         return direct_routing_key
 
-    def type_name_from_routing_key(
-        self,
-        routing_key: str,
-    ) -> str:
-        """Returns the type alias of the message given the routing key. Raises a SchemaError
-        exception if there is a problem decoding the type alias, or if it does not have
-        the appropriate left-right-dot format.
+    def message_category_from_routing_key(self, routing_key: str) -> MessageCategory:
+        """Returns the MessageCategory of the message given the routing key.
 
-        For all the GNode Registry messages, this involves json dumping the payload
-        and looking for the TypeName dict key. However, in GridWorks World registries
-        where the participating entities represent TerminalAssets, AtomicTNodes, and
-        other operational actors in the electric grid model, there are a couple edge patterns
-        of routing key where the TypeName is a substring of the routing key itself.
-
-        The decision to embed the routing key INSIDE the body for the main set of
-        messages has to do with the length limit of 255 for rabbit routing keys, and
-        the desire to include both the FromGNodeAlias and the ToGNodeAlias in that key.
+        Raises a SchemaError exception if there is a problem decoding the MessageCategory
 
         Args:
-            routing_key (str): This is the basic_deliver.routing_key string
-            in a rabbit message
+           routing_key (str): This is the basic_deliver.routing_key string
+           in a rabbit message
 
         Returns:
-            str: the TypeName of the payload, in Lrd format
+           MessageCategory: the MessageCategory, as enum
         """
         routing_key_words = routing_key.split(".")
-        if len(routing_key_words) < 4:
-            self._latest_on_message_diagnostic = (
-                OnReceiveMessageDiagnostic.UNKNOWN_ROUTING_KEY_TYPE
-            )
-            raise SchemaError(f"Routing key {routing_key} must have at least 3 words!")
         msg_category_symbol_value = routing_key_words[0]
-        type_name_lrh = routing_key_words[3]
 
         try:
             msg_category_symbol = MessageCategorySymbol(msg_category_symbol_value)
         except ValueError:
             self._latest_on_message_diagnostic = (
                 OnReceiveMessageDiagnostic.UNKNOWN_MESSAGE_CATEGORY_SYMBOL
             )
@@ -992,14 +1078,37 @@
         if msg_category not in allowable_categories:
             self._latest_on_message_diagnostic = (
                 OnReceiveMessageDiagnostic.UNHANDLED_ROUTING_KEY_TYPE
             )
             raise SchemaError(
                 f"Rabbit messages do not handle {msg_category_symbol.value}"
             )
+        return msg_category
+
+    def type_name_from_routing_key(
+        self,
+        routing_key: str,
+    ) -> str:
+        """Returns the TypeName of the message given the routing key. Raises a SchemaError
+        exception if there is a problem decoding the TypeName, or if it does not have
+        the appropriate left-right-dot format.
+
+        Args:
+            routing_key (str): This is the basic_deliver.routing_key string
+            in a rabbit message
+
+        Returns:
+            str: the TypeName of the payload, in Lrd format
+        """
+        routing_key_words = routing_key.split(".")
+        msg_category = self.message_category_from_routing_key(routing_key)
+        if msg_category == MessageCategory.MqttJsonBroadcast:
+            type_name_lrh = routing_key_words[2]
+        else:
+            type_name_lrh = routing_key_words[3]
 
         if not property_format.is_lrh_alias_format(type_name_lrh):
             self._latest_on_message_diagnostic = (
                 OnReceiveMessageDiagnostic.TYPE_NAME_DECODING_PROBLEM
             )
             raise SchemaError(
                 f"TypeName {type_name_lrh} in {routing_key} message not lrh_alias_format!"
@@ -1036,14 +1145,19 @@
 
         Raises:
             SchemaError: Error in message construction
 
         Returns:
             GNodeRole: GNodeRole of the actor that sent the message
         """
+        msg_category = self.message_category_from_routing_key(routing_key)
+        if msg_category == MessageCategory.MqttJsonBroadcast:
+            raise Exception(
+                "MqttJsonBroadcast does not contain FromRole in routing key"
+            )
         routing_key_words = routing_key.split(".")
         try:
             from_g_node_rabbit_role = routing_key_words[2]
         except:
             raise SchemaError(f"{routing_key} must have at least three words!")
         try:
             rabbit_role = RabbitRole(from_g_node_rabbit_role)
```

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/accepted_bid.py` & `gridworks_atn-0.2.4/src/gwatn/types/accepted_bid.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/atn_bid.py` & `gridworks_atn-0.2.4/src/gwatn/types/atn_bid.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/atn_params_heatpumpwithbooststore.py` & `gridworks_atn-0.2.4/src/gwatn/types/atn_params_heatpumpwithbooststore.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/atn_params_report_heatpumpwithbooststore.py` & `gridworks_atn-0.2.4/src/gwatn/types/atn_params_report_heatpumpwithbooststore.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/base_g_node_gt.py` & `gridworks_atn-0.2.4/src/gwatn/types/base_g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/basegnode_scada_create.py` & `gridworks_atn-0.2.4/src/gwatn/types/basegnode_scada_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/csv_distp_sync.py` & `gridworks_atn-0.2.4/src/gwatn/types/csv_distp_sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/csv_eprt_sync.py` & `gridworks_atn-0.2.4/src/gwatn/types/csv_eprt_sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/csv_heat_profile.py` & `gridworks_atn-0.2.4/src/gwatn/types/csv_heat_profile.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/csv_weather_forecast_sync.py` & `gridworks_atn-0.2.4/src/gwatn/types/csv_weather_forecast_sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/discoverycert_algo_create.py` & `gridworks_atn-0.2.4/src/gwatn/types/discoverycert_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/dispatch_contract_confirmed_heatpumpwithbooststore.py` & `gridworks_atn-0.2.4/src/gwatn/types/dispatch_contract_confirmed_heatpumpwithbooststore.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/flo_params_heatpumpwithbooststore.py` & `gridworks_atn-0.2.4/src/gwatn/types/flo_params_heatpumpwithbooststore.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/g_node_gt.py` & `gridworks_atn-0.2.4/src/gwatn/types/g_node_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         "3901c7d2",
         "c499943c",
         "88112a93",
         "674ad859",
         "2161739f",
         "1dce1efd",
         "db57d184",
+        "07f28817",
     ]
 
     @classmethod
     def is_symbol(cls, candidate: str) -> bool:
         if candidate in cls.symbols:
             return True
         return False
@@ -56,14 +57,15 @@
     World = auto()
     TimeCoordinator = auto()
     Supervisor = auto()
     Scada = auto()
     PriceService = auto()
     WeatherService = auto()
     AggregatedTNode = auto()
+    Persister = auto()
 
     @classmethod
     def default(cls) -> "GNodeRole000":
         return cls.GNode
 
     @classmethod
     def values(cls) -> List[str]:
@@ -96,14 +98,15 @@
         "3901c7d2": GNodeRole000.World,
         "c499943c": GNodeRole000.TimeCoordinator,
         "88112a93": GNodeRole000.Supervisor,
         "674ad859": GNodeRole000.Scada,
         "2161739f": GNodeRole000.PriceService,
         "1dce1efd": GNodeRole000.WeatherService,
         "db57d184": GNodeRole000.AggregatedTNode,
+        "07f28817": GNodeRole000.Persister,
     }
 
     versioned_enum_to_type_dict: Dict[GNodeRole000, str] = {
         GNodeRole000.GNode: "00000000",
         GNodeRole000.TerminalAsset: "bdeaa0b1",
         GNodeRole000.AtomicTNode: "8021dcad",
         GNodeRole000.MarketMaker: "304890c5",
@@ -113,14 +116,15 @@
         GNodeRole000.World: "3901c7d2",
         GNodeRole000.TimeCoordinator: "c499943c",
         GNodeRole000.Supervisor: "88112a93",
         GNodeRole000.Scada: "674ad859",
         GNodeRole000.PriceService: "2161739f",
         GNodeRole000.WeatherService: "1dce1efd",
         GNodeRole000.AggregatedTNode: "db57d184",
+        GNodeRole000.Persister: "07f28817",
     }
 
 
 class GNodeStatus100SchemaEnum:
     enum_name: str = "g.node.status.100"
     symbols: List[str] = [
         "00000000",
```

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/g_node_instance_gt.py` & `gridworks_atn-0.2.4/src/gwatn/types/g_node_instance_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/gt_dispatch_boolean.py` & `gridworks_atn-0.2.4/src/gwatn/types/gt_dispatch_boolean.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/gw_cert_id.py` & `gridworks_atn-0.2.4/src/gwatn/types/gw_cert_id.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/heartbeat_a.py` & `gridworks_atn-0.2.4/src/gwatn/types/heartbeat_a.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/heartbeat_algo_audit.py` & `gridworks_atn-0.2.4/src/gwatn/types/heartbeat_algo_audit.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/heartbeat_b.py` & `gridworks_atn-0.2.4/src/gwatn/types/heartbeat_b.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-"""Type heartbeat.b, version 000"""
+"""Type heartbeat.b, version 001"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
+from typing import Optional
 
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 
@@ -108,26 +109,26 @@
     FromGNodeInstanceId: str = Field(
         title="My GNodeInstanceId",
     )
     MyHex: str = Field(
         title="Hex character getting sent",
         default="0",
     )
-    YourLastHex: str = Field(
-        title="Last hex character received from heartbeat partner",
-        default="0",
+    YourLastHex: Optional[str] = Field(
+        title="Last hex character received from heartbeat partner. If the heartbeat initiator wants to start the sequence over, it does not include this.",
+        default=None,
     )
     LastReceivedTimeUnixMs: int = Field(
         title="Time YourLastHex was received on my clock",
     )
     SendTimeUnixMs: int = Field(
         title="Time this message is made and sent on my clock",
     )
     TypeName: Literal["heartbeat.b"] = "heartbeat.b"
-    Version: str = "000"
+    Version: str = "001"
 
     @validator("FromGNodeAlias")
     def _check_from_g_node_alias(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
         except ValueError as e:
             raise ValueError(
@@ -150,15 +151,17 @@
         try:
             check_is_hex_char(v)
         except ValueError as e:
             raise ValueError(f"MyHex failed HexChar format validation: {e}")
         return v
 
     @validator("YourLastHex")
-    def _check_your_last_hex(cls, v: str) -> str:
+    def _check_your_last_hex(cls, v: Optional[str]) -> Optional[str]:
+        if v is None:
+            return v
         try:
             check_is_hex_char(v)
         except ValueError as e:
             raise ValueError(f"YourLastHex failed HexChar format validation: {e}")
         return v
 
     @validator("LastReceivedTimeUnixMs")
@@ -179,30 +182,32 @@
             raise ValueError(
                 f"SendTimeUnixMs failed ReasonableUnixTimeMs format validation: {e}"
             )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
+        if d["YourLastHex"] is None:
+            del d["YourLastHex"]
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
 
 class HeartbeatB_Maker:
     type_name = "heartbeat.b"
-    version = "000"
+    version = "001"
 
     def __init__(
         self,
         from_g_node_alias: str,
         from_g_node_instance_id: str,
         my_hex: str,
-        your_last_hex: str,
+        your_last_hex: Optional[str],
         last_received_time_unix_ms: int,
         send_time_unix_ms: int,
     ):
         self.tuple = HeartbeatB(
             FromGNodeAlias=from_g_node_alias,
             FromGNodeInstanceId=from_g_node_instance_id,
             MyHex=my_hex,
@@ -238,15 +243,15 @@
         if "FromGNodeAlias" not in d2.keys():
             raise SchemaError(f"dict {d2} missing FromGNodeAlias")
         if "FromGNodeInstanceId" not in d2.keys():
             raise SchemaError(f"dict {d2} missing FromGNodeInstanceId")
         if "MyHex" not in d2.keys():
             raise SchemaError(f"dict {d2} missing MyHex")
         if "YourLastHex" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing YourLastHex")
+            d2["YourLastHex"] = None
         if "LastReceivedTimeUnixMs" not in d2.keys():
             raise SchemaError(f"dict {d2} missing LastReceivedTimeUnixMs")
         if "SendTimeUnixMs" not in d2.keys():
             raise SchemaError(f"dict {d2} missing SendTimeUnixMs")
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
@@ -254,9 +259,9 @@
             FromGNodeAlias=d2["FromGNodeAlias"],
             FromGNodeInstanceId=d2["FromGNodeInstanceId"],
             MyHex=d2["MyHex"],
             YourLastHex=d2["YourLastHex"],
             LastReceivedTimeUnixMs=d2["LastReceivedTimeUnixMs"],
             SendTimeUnixMs=d2["SendTimeUnixMs"],
             TypeName=d2["TypeName"],
-            Version="000",
+            Version="001",
         )
```

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/initial_tadeed_algo_create.py` & `gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/initial_tadeed_algo_optin.py` & `gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_optin.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/initial_tadeed_algo_transfer.py` & `gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/join_dispatch_contract.py` & `gridworks_atn-0.2.4/src/gwatn/types/join_dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/latest_price.py` & `gridworks_atn-0.2.4/src/gwatn/types/latest_price.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/market_slot.py` & `gridworks_atn-0.2.4/src/gwatn/types/market_slot.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/market_type_gt.py` & `gridworks_atn-0.2.4/src/gwatn/types/market_type_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/new_tadeed_algo_optin.py` & `gridworks_atn-0.2.4/src/gwatn/types/new_tadeed_algo_optin.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/new_tadeed_send.py` & `gridworks_atn-0.2.4/src/gwatn/types/new_tadeed_send.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/old_tadeed_algo_return.py` & `gridworks_atn-0.2.4/src/gwatn/types/old_tadeed_algo_return.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/price_quantity.py` & `gridworks_atn-0.2.4/src/gwatn/types/price_quantity.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/price_quantity_unitless.py` & `gridworks_atn-0.2.4/src/gwatn/types/price_quantity_unitless.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/ready.py` & `gridworks_atn-0.2.4/src/gwatn/types/ready.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/scada_cert_transfer.py` & `gridworks_atn-0.2.4/src/gwatn/types/scada_cert_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/sim_scada_driver_report.py` & `gridworks_atn-0.2.4/src/gwatn/types/sim_scada_driver_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/sim_timestep.py` & `gridworks_atn-0.2.4/src/gwatn/types/sim_timestep.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/sla_enter.py` & `gridworks_atn-0.2.4/src/gwatn/types/sla_enter.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/snapshot_heatpumpwithbooststore.py` & `gridworks_atn-0.2.4/src/gwatn/types/snapshot_heatpumpwithbooststore.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/super_starter.py` & `gridworks_atn-0.2.4/src/gwatn/types/super_starter.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/supervisor_container_gt.py` & `gridworks_atn-0.2.4/src/gwatn/types/supervisor_container_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/tadeed_specs_hack.py` & `gridworks_atn-0.2.4/src/gwatn/types/tadeed_specs_hack.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/tavalidatorcert_algo_create.py` & `gridworks_atn-0.2.4/src/gwatn/types/tavalidatorcert_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/tavalidatorcert_algo_transfer.py` & `gridworks_atn-0.2.4/src/gwatn/types/tavalidatorcert_algo_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/src/gwatn/types/terminalasset_certify_hack.py` & `gridworks_atn-0.2.4/src/gwatn/types/terminalasset_certify_hack.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.3/setup.py` & `gridworks_atn-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gridworks-atn
+Version: 0.2.4
+Summary: Gridworks Atn Spaceheat
+Home-page: https://github.com/thegridelectric/gridworks-atn
+License: None
+Author: Jessica Millar
+Author-email: jmillar@gridworks-consulting.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: gridworks (>=0.2.1,<0.3.0)
+Requires-Dist: gridworks-proactor (>=0.1.8,<0.2.0)
+Requires-Dist: gridworks-protocol (>=0.4.5,<0.5.0)
+Requires-Dist: numpy (>=1.23.4,<2.0.0)
+Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
+Requires-Dist: types-requests (>=2.28.11.2,<3.0.0.0)
+Project-URL: Changelog, https://github.com/thegridelectric/gridworks-atn/releases
+Project-URL: Documentation, https://gridworks-atn.readthedocs.io
+Project-URL: Repository, https://github.com/thegridelectric/gridworks-atn
+Description-Content-Type: text/markdown
+
+# Gridworks Atn
+
+[![PyPI](https://img.shields.io/pypi/v/gridworks-atn.svg)][pypi_]
+[![Status](https://img.shields.io/pypi/status/gridworks-atn.svg)][status]
+[![Python Version](https://img.shields.io/pypi/pyversions/gridworks-atn)][python version]
+[![License](https://img.shields.io/pypi/l/gridworks-atn)][license]
+
+[![Read the documentation at https://gridworks-atn.readthedocs.io/](https://img.shields.io/readthedocs/gridworks/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/thegridelectric/gridworks-atn/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/thegridelectric/gridworks-atn/branch/main/graph/badge.svg)][codecov]
+
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi_]: https://pypi.org/project/gridworks-atn/
+[status]: https://pypi.org/project/gridworks-atn/
+[python version]: https://pypi.org/project/gridworks-atn
+[read the docs]: https://gridworks-atn.readthedocs.io/
+[tests]: https://github.com/thegridelectric/gridworks-atn/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-atn
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
+
+This is the [GridWorks](https://gridworks.readthedocs.io/) Python SDK for building Atomic Transactive Nodes, or
+[AtomicTNodes](https://gridworks.readthedocs.io/en/latest/atomic-t-node.html>).
+
+AtomicTNodes are the most fun and interesting GridWorks actors to design and build. They are what make electrical devices
+_transactive_. More specifically, each AtomicTNode is dedicated to the job of operating its very own
+[Transactive Device](https://gridworks.readthedocs.io/en/latest/transactive-device.html), and simultaneously bidding on its behalf into electricity markets.
+
+To learn about using this SDK, visit the [Gridworks Atn docs](https://gridworks-atn.readthedocs.io/en/latest/). To explore the rest of GridWorks, visit the [GridWorks docs](https://gridworks.readthedocs.io/en/latest/).
+
+## License
+
+Distributed under the terms of the [MIT license][license],
+**Gridworks Atn** is free and open source software.
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+## Credits
+
+This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+
+[@cjolowicz]: https://github.com/cjolowicz
+[pypi]: https://pypi.org/
+[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[file an issue]: https://github.com/thegridelectric/gridworks-atn/issues
+[pip]: https://pip.pypa.io/
+
+<!-- github-only -->
+
+[license]: https://github.com/thegridelectric/gridworks-atn/blob/main/LICENSE
+[contributor guide]: https://github.com/thegridelectric/gridworks-atn/blob/main/CONTRIBUTING.md
+[command-line reference]: https://gridworks-atn.readthedocs.io/en/latest/usage.html
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['gwatn',
- 'gwatn.csv_makers',
- 'gwatn.data_classes',
- 'gwatn.dev_utils',
- 'gwatn.enums',
- 'gwatn.types']
-
-package_data = \
-{'': ['*'], 'gwatn': ['dispatch_contract_artifacts/*']}
-
-install_requires = \
-['boto3>=1.26.3,<2.0.0',
- 'gridworks-protocol>=0.2.6,<0.3.0',
- 'gridworks>=0.1.4,<0.2.0',
- 'numpy>=1.23.4,<2.0.0',
- 'paho-mqtt>=1.6.1,<2.0.0',
- 'types-requests>=2.28.11.2,<3.0.0.0']
-
-entry_points = \
-{'console_scripts': ['gridworks-atn = gwatn.__main__:main']}
-
-setup_kwargs = {
-    'name': 'gridworks-atn',
-    'version': '0.2.3',
-    'description': 'Gridworks Atn Spaceheat',
-    'long_description': "# Gridworks Atn\n\n[![PyPI](https://img.shields.io/pypi/v/gridworks-atn.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/gridworks-atn.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/gridworks-atn)][python version]\n[![License](https://img.shields.io/pypi/l/gridworks-atn)][license]\n\n[![Read the documentation at https://gridworks-atn.readthedocs.io/](https://img.shields.io/readthedocs/gridworks/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/thegridelectric/gridworks-atn/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/thegridelectric/gridworks-atn/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/gridworks-atn/\n[status]: https://pypi.org/project/gridworks-atn/\n[python version]: https://pypi.org/project/gridworks-atn\n[read the docs]: https://gridworks-atn.readthedocs.io/\n[tests]: https://github.com/thegridelectric/gridworks-atn/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-atn\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nThis is the [GridWorks](https://gridworks.readthedocs.io/) Python SDK for building Atomic Transactive Nodes, or\n[AtomicTNodes](https://gridworks.readthedocs.io/en/latest/atomic-t-node.html>).\n\nAtomicTNodes are the most fun and interesting GridWorks actors to design and build. They are what make electrical devices\n_transactive_. More specifically, each AtomicTNode is dedicated to the job of operating its very own\n[Transactive Device](https://gridworks.readthedocs.io/en/latest/transactive-device.html), and simultaneously bidding on its behalf into electricity markets.\n\nTo learn about using this SDK, visit the [Gridworks Atn docs](https://gridworks-atn.readthedocs.io/en/latest/). To explore the rest of GridWorks, visit the [GridWorks docs](https://gridworks.readthedocs.io/en/latest/).\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n**Gridworks Atn** is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/thegridelectric/gridworks-atn/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/thegridelectric/gridworks-atn/blob/main/LICENSE\n[contributor guide]: https://github.com/thegridelectric/gridworks-atn/blob/main/CONTRIBUTING.md\n[command-line reference]: https://gridworks-atn.readthedocs.io/en/latest/usage.html\n",
-    'author': 'Jessica Millar',
-    'author_email': 'jmillar@gridworks-consulting.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/thegridelectric/gridworks-atn',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

