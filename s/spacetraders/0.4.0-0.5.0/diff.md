# Comparing `tmp/spacetraders-0.4.0.tar.gz` & `tmp/spacetraders-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetraders-0.4.0.tar", max compression
+gzip compressed data, was "spacetraders-0.5.0.tar", max compression
```

## Comparing `spacetraders-0.4.0.tar` & `spacetraders-0.5.0.tar`

### file list

```diff
@@ -1,208 +1,220 @@
--rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.4.0/README.md
--rw-r--r--   0        0        0      664 2023-05-15 19:26:39.587370 spacetraders-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      250 2023-05-15 19:23:16.207370 spacetraders-0.4.0/spacetraders/__init__.py
--rw-r--r--   0        0        0       47 2023-05-15 19:23:15.557370 spacetraders-0.4.0/spacetraders/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 19:23:15.607370 spacetraders-0.4.0/spacetraders/api/agents/__init__.py
--rw-r--r--   0        0        0     4139 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/agents/get_my_agent.py
--rw-r--r--   0        0        0        0 2023-05-15 19:23:15.607370 spacetraders-0.4.0/spacetraders/api/contracts/__init__.py
--rw-r--r--   0        0        0     4425 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/contracts/accept_contract.py
--rw-r--r--   0        0        0     5022 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/contracts/deliver_contract.py
--rw-r--r--   0        0        0     4437 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/api/contracts/fulfill_contract.py
--rw-r--r--   0        0        0     4420 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/contracts/get_contract.py
--rw-r--r--   0        0        0     4900 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/api/contracts/get_contracts.py
--rw-r--r--   0        0        0        0 2023-05-15 19:23:15.567370 spacetraders-0.4.0/spacetraders/api/default/__init__.py
--rw-r--r--   0        0        0     6960 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/default/register.py
--rw-r--r--   0        0        0        0 2023-05-15 19:23:15.607370 spacetraders-0.4.0/spacetraders/api/factions/__init__.py
--rw-r--r--   0        0        0     4427 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/factions/get_faction.py
--rw-r--r--   0        0        0     4853 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/factions/get_factions.py
--rw-r--r--   0        0        0        0 2023-05-15 19:23:15.617370 spacetraders-0.4.0/spacetraders/api/fleet/__init__.py
--rw-r--r--   0        0        0     4900 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/create_chart.py
--rw-r--r--   0        0        0     4550 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/create_ship_ship_scan.py
--rw-r--r--   0        0        0     4587 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/create_ship_system_scan.py
--rw-r--r--   0        0        0     4615 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
--rw-r--r--   0        0        0     5382 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/create_survey.py
--rw-r--r--   0        0        0     4961 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/dock_ship.py
--rw-r--r--   0        0        0     5217 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/extract_resources.py
--rw-r--r--   0        0        0     4373 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/get_my_ship.py
--rw-r--r--   0        0        0     4447 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/get_my_ship_cargo.py
--rw-r--r--   0        0        0     4871 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/get_my_ships.py
--rw-r--r--   0        0        0     5562 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/get_ship_cooldown.py
--rw-r--r--   0        0        0     4414 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/get_ship_nav.py
--rw-r--r--   0        0        0     4905 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/jettison.py
--rw-r--r--   0        0        0     5049 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/jump_ship.py
--rw-r--r--   0        0        0     5893 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/navigate_ship.py
--rw-r--r--   0        0        0     4954 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/orbit_ship.py
--rw-r--r--   0        0        0     5001 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/patch_ship_nav.py
--rw-r--r--   0        0        0     5192 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/purchase_cargo.py
--rw-r--r--   0        0        0     4680 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/purchase_ship.py
--rw-r--r--   0        0        0     4419 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/refuel_ship.py
--rw-r--r--   0        0        0     5010 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/sell_cargo.py
--rw-r--r--   0        0        0     5244 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/ship_refine.py
--rw-r--r--   0        0        0     5215 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/transfer_cargo.py
--rw-r--r--   0        0        0     5569 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/warp_ship.py
--rw-r--r--   0        0        0        0 2023-05-15 19:23:15.597370 spacetraders-0.4.0/spacetraders/api/systems/__init__.py
--rw-r--r--   0        0        0     4735 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/systems/get_jump_gate.py
--rw-r--r--   0        0        0     5121 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/systems/get_market.py
--rw-r--r--   0        0        0     4951 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/systems/get_shipyard.py
--rw-r--r--   0        0        0     4469 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/systems/get_system.py
--rw-r--r--   0        0        0     5421 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/systems/get_system_waypoints.py
--rw-r--r--   0        0        0     4877 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/systems/get_systems.py
--rw-r--r--   0        0        0     4710 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/systems/get_waypoint.py
--rw-r--r--   0        0        0     4384 2023-05-15 19:23:16.717370 spacetraders-0.4.0/spacetraders/client.py
--rw-r--r--   0        0        0      470 2023-05-15 19:23:16.507370 spacetraders-0.4.0/spacetraders/errors.py
--rw-r--r--   0        0        0    13081 2023-05-15 19:23:16.897370 spacetraders-0.4.0/spacetraders/models/__init__.py
--rw-r--r--   0        0        0     1269 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/accept_contract_response_200.py
--rw-r--r--   0        0        0     1299 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/accept_contract_response_200_data.py
--rw-r--r--   0        0        0     1460 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/agent.py
--rw-r--r--   0        0        0     1532 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/chart.py
--rw-r--r--   0        0        0     1709 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/connected_system.py
--rw-r--r--   0        0        0     1887 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/contract.py
--rw-r--r--   0        0        0     1712 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/contract_deliver_good.py
--rw-r--r--   0        0        0     1340 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/contract_payment.py
--rw-r--r--   0        0        0     1567 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/contract_terms.py
--rw-r--r--   0        0        0      201 2023-05-15 19:23:15.757370 spacetraders-0.4.0/spacetraders/models/contract_type.py
--rw-r--r--   0        0        0     1691 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/cooldown.py
--rw-r--r--   0        0        0     1251 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/create_chart_response_201.py
--rw-r--r--   0        0        0     1469 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/create_chart_response_201_data.py
--rw-r--r--   0        0        0     1304 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/create_ship_ship_scan_response_201.py
--rw-r--r--   0        0        0     1425 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
--rw-r--r--   0        0        0     1316 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/create_ship_system_scan_response_201.py
--rw-r--r--   0        0        0     1443 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/create_ship_system_scan_response_201_data.py
--rw-r--r--   0        0        0     1328 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
--rw-r--r--   0        0        0     1461 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
--rw-r--r--   0        0        0     1257 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/create_survey_response_201.py
--rw-r--r--   0        0        0     1398 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/create_survey_response_201_data.py
--rw-r--r--   0        0        0     1284 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/deliver_contract_json_body.py
--rw-r--r--   0        0        0     1275 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/deliver_contract_response_200.py
--rw-r--r--   0        0        0     1318 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/deliver_contract_response_200_data.py
--rw-r--r--   0        0        0     1292 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/dock_ship_dock_ship_200_response.py
--rw-r--r--   0        0        0     1227 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
--rw-r--r--   0        0        0     1368 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/extract_resources_json_body.py
--rw-r--r--   0        0        0     1281 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/extract_resources_response_201.py
--rw-r--r--   0        0        0     1532 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/extract_resources_response_201_data.py
--rw-r--r--   0        0        0     1261 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/extraction.py
--rw-r--r--   0        0        0     1250 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/extraction_yield.py
--rw-r--r--   0        0        0     1457 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/faction.py
--rw-r--r--   0        0        0     1421 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/faction_trait.py
--rw-r--r--   0        0        0     1869 2023-05-15 19:23:15.857370 spacetraders-0.4.0/spacetraders/models/faction_trait_symbol.py
--rw-r--r--   0        0        0     1275 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/fulfill_contract_response_200.py
--rw-r--r--   0        0        0     1301 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/fulfill_contract_response_200_data.py
--rw-r--r--   0        0        0     1175 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_contract_response_200.py
--rw-r--r--   0        0        0     1282 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_contracts_response_200.py
--rw-r--r--   0        0        0     1169 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/get_faction_response_200.py
--rw-r--r--   0        0        0     1276 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_factions_response_200.py
--rw-r--r--   0        0        0     1176 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_jump_gate_response_200.py
--rw-r--r--   0        0        0     1163 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/get_market_response_200.py
--rw-r--r--   0        0        0     1161 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/get_my_agent_response_200.py
--rw-r--r--   0        0        0     1186 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/get_my_ship_cargo_response_200.py
--rw-r--r--   0        0        0     1162 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/get_my_ship_response_200.py
--rw-r--r--   0        0        0     1262 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/get_my_ships_response_200.py
--rw-r--r--   0        0        0     1262 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_ship_cooldown_response_200.py
--rw-r--r--   0        0        0     1210 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_ship_nav_response_200.py
--rw-r--r--   0        0        0     1175 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/get_shipyard_response_200.py
--rw-r--r--   0        0        0     1163 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_system_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/get_system_waypoints_response_200.py
--rw-r--r--   0        0        0     1270 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/get_systems_response_200.py
--rw-r--r--   0        0        0     1266 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/get_waypoint_response_200.py
--rw-r--r--   0        0        0     1177 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/jettison_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/jettison_response_200.py
--rw-r--r--   0        0        0     1185 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/jettison_response_200_data.py
--rw-r--r--   0        0        0     1606 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/jump_gate.py
--rw-r--r--   0        0        0     1168 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/jump_ship_json_body.py
--rw-r--r--   0        0        0     1233 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/jump_ship_response_200.py
--rw-r--r--   0        0        0     1462 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/jump_ship_response_200_data.py
--rw-r--r--   0        0        0     2398 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/market.py
--rw-r--r--   0        0        0     1880 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/market_trade_good.py
--rw-r--r--   0        0        0      224 2023-05-15 19:23:15.757370 spacetraders-0.4.0/spacetraders/models/market_trade_good_supply.py
--rw-r--r--   0        0        0     2109 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/market_transaction.py
--rw-r--r--   0        0        0      170 2023-05-15 19:23:15.767370 spacetraders-0.4.0/spacetraders/models/market_transaction_type.py
--rw-r--r--   0        0        0     1206 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/meta.py
--rw-r--r--   0        0        0     1176 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/navigate_ship_json_body.py
--rw-r--r--   0        0        0     1257 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/navigate_ship_response_200.py
--rw-r--r--   0        0        0     1444 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/navigate_ship_response_200_data.py
--rw-r--r--   0        0        0     1304 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
--rw-r--r--   0        0        0     1231 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
--rw-r--r--   0        0        0     1420 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/patch_ship_nav_json_body.py
--rw-r--r--   0        0        0     1214 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/patch_ship_nav_response_200.py
--rw-r--r--   0        0        0     1352 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
--rw-r--r--   0        0        0     1484 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
--rw-r--r--   0        0        0     1211 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
--rw-r--r--   0        0        0     1333 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/purchase_ship_json_body.py
--rw-r--r--   0        0        0     1257 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/purchase_ship_response_201.py
--rw-r--r--   0        0        0     1447 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/purchase_ship_response_201_data.py
--rw-r--r--   0        0        0     1245 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/refuel_ship_response_200.py
--rw-r--r--   0        0        0     1397 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/refuel_ship_response_200_data.py
--rw-r--r--   0        0        0     1611 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/register_json_body.py
--rw-r--r--   0        0        0      244 2023-05-15 19:23:15.837370 spacetraders-0.4.0/spacetraders/models/register_json_body_faction.py
--rw-r--r--   0        0        0     1232 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/register_response_201.py
--rw-r--r--   0        0        0     1608 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/register_response_201_data.py
--rw-r--r--   0        0        0     2444 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/scanned_ship.py
--rw-r--r--   0        0        0     1144 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/scanned_ship_engine.py
--rw-r--r--   0        0        0     1141 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/scanned_ship_frame.py
--rw-r--r--   0        0        0     1149 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/scanned_ship_mounts_item.py
--rw-r--r--   0        0        0     1147 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/scanned_ship_reactor.py
--rw-r--r--   0        0        0     1492 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/scanned_system.py
--rw-r--r--   0        0        0     2293 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/scanned_waypoint.py
--rw-r--r--   0        0        0     1304 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
--rw-r--r--   0        0        0     1468 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
--rw-r--r--   0        0        0     1195 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_request.py
--rw-r--r--   0        0        0     3140 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship.py
--rw-r--r--   0        0        0     1484 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_cargo.py
--rw-r--r--   0        0        0     1510 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_cargo_item.py
--rw-r--r--   0        0        0     2248 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_crew.py
--rw-r--r--   0        0        0      167 2023-05-15 19:23:15.727370 spacetraders-0.4.0/spacetraders/models/ship_crew_rotation.py
--rw-r--r--   0        0        0     1883 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_engine.py
--rw-r--r--   0        0        0      319 2023-05-15 19:23:15.837370 spacetraders-0.4.0/spacetraders/models/ship_engine_symbol.py
--rw-r--r--   0        0        0     2278 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_frame.py
--rw-r--r--   0        0        0      694 2023-05-15 19:23:15.737370 spacetraders-0.4.0/spacetraders/models/ship_frame_symbol.py
--rw-r--r--   0        0        0     1586 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/ship_fuel.py
--rw-r--r--   0        0        0     1340 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_fuel_consumed.py
--rw-r--r--   0        0        0     1965 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/ship_module.py
--rw-r--r--   0        0        0     1033 2023-05-15 19:23:15.777370 spacetraders-0.4.0/spacetraders/models/ship_module_symbol.py
--rw-r--r--   0        0        0     1947 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_mount.py
--rw-r--r--   0        0        0      572 2023-05-15 19:23:15.837370 spacetraders-0.4.0/spacetraders/models/ship_mount_deposits_item.py
--rw-r--r--   0        0        0      854 2023-05-15 19:23:15.847370 spacetraders-0.4.0/spacetraders/models/ship_mount_symbol.py
--rw-r--r--   0        0        0     2114 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/ship_nav.py
--rw-r--r--   0        0        0      206 2023-05-15 19:23:15.747370 spacetraders-0.4.0/spacetraders/models/ship_nav_flight_mode.py
--rw-r--r--   0        0        0     1891 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_nav_route.py
--rw-r--r--   0        0        0     1497 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_nav_route_waypoint.py
--rw-r--r--   0        0        0      196 2023-05-15 19:23:15.767370 spacetraders-0.4.0/spacetraders/models/ship_nav_status.py
--rw-r--r--   0        0        0     1934 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_reactor.py
--rw-r--r--   0        0        0      344 2023-05-15 19:23:15.747370 spacetraders-0.4.0/spacetraders/models/ship_reactor_symbol.py
--rw-r--r--   0        0        0     1246 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/ship_refine_json_body.py
--rw-r--r--   0        0        0      330 2023-05-15 19:23:15.837370 spacetraders-0.4.0/spacetraders/models/ship_refine_json_body_produce.py
--rw-r--r--   0        0        0     1316 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response.py
--rw-r--r--   0        0        0     2047 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py
--rw-r--r--   0        0        0     1344 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
--rw-r--r--   0        0        0     1344 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
--rw-r--r--   0        0        0     1477 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/ship_registration.py
--rw-r--r--   0        0        0     1541 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_requirements.py
--rw-r--r--   0        0        0      479 2023-05-15 19:23:15.827370 spacetraders-0.4.0/spacetraders/models/ship_role.py
--rw-r--r--   0        0        0      549 2023-05-15 19:23:15.737370 spacetraders-0.4.0/spacetraders/models/ship_type.py
--rw-r--r--   0        0        0     2009 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/shipyard.py
--rw-r--r--   0        0        0     2498 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/shipyard_ship.py
--rw-r--r--   0        0        0     1225 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/shipyard_ship_types_item.py
--rw-r--r--   0        0        0     1698 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/shipyard_transaction.py
--rw-r--r--   0        0        0     2228 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/survey.py
--rw-r--r--   0        0        0     1209 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/survey_deposit.py
--rw-r--r--   0        0        0      181 2023-05-15 19:23:15.747370 spacetraders-0.4.0/spacetraders/models/survey_size.py
--rw-r--r--   0        0        0     1725 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/system.py
--rw-r--r--   0        0        0     1112 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/system_faction.py
--rw-r--r--   0        0        0      405 2023-05-15 19:23:15.747370 spacetraders-0.4.0/spacetraders/models/system_type.py
--rw-r--r--   0        0        0     1352 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/system_waypoint.py
--rw-r--r--   0        0        0     1299 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/trade_good.py
--rw-r--r--   0        0        0     4422 2023-05-15 19:23:15.827370 spacetraders-0.4.0/spacetraders/models/trade_symbol.py
--rw-r--r--   0        0        0     1352 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
--rw-r--r--   0        0        0     1221 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
--rw-r--r--   0        0        0     1304 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
--rw-r--r--   0        0        0     1168 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/warp_ship_json_body.py
--rw-r--r--   0        0        0     1233 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/warp_ship_response_200.py
--rw-r--r--   0        0        0     1436 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/warp_ship_response_200_data.py
--rw-r--r--   0        0        0     2279 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/waypoint.py
--rw-r--r--   0        0        0     1116 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/waypoint_faction.py
--rw-r--r--   0        0        0     1178 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/waypoint_orbital.py
--rw-r--r--   0        0        0     1427 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/waypoint_trait.py
--rw-r--r--   0        0        0     2200 2023-05-15 19:23:15.857370 spacetraders-0.4.0/spacetraders/models/waypoint_trait_symbol.py
--rw-r--r--   0        0        0      381 2023-05-15 19:23:15.747370 spacetraders-0.4.0/spacetraders/models/waypoint_type.py
--rw-r--r--   0        0        0     1341 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/types.py
--rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 spacetraders-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.5.0/README.md
+-rw-r--r--   0        0        0      664 2023-05-24 19:24:39.688239 spacetraders-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      250 2023-05-24 19:22:46.258239 spacetraders-0.5.0/spacetraders/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-24 19:22:45.628239 spacetraders-0.5.0/spacetraders/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 19:22:45.688239 spacetraders-0.5.0/spacetraders/api/agents/__init__.py
+-rw-r--r--   0        0        0     4139 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/agents/get_my_agent.py
+-rw-r--r--   0        0        0        0 2023-05-24 19:22:45.688239 spacetraders-0.5.0/spacetraders/api/contracts/__init__.py
+-rw-r--r--   0        0        0     4425 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/contracts/accept_contract.py
+-rw-r--r--   0        0        0     5022 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/contracts/deliver_contract.py
+-rw-r--r--   0        0        0     4437 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/contracts/fulfill_contract.py
+-rw-r--r--   0        0        0     4420 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/contracts/get_contract.py
+-rw-r--r--   0        0        0     4900 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/contracts/get_contracts.py
+-rw-r--r--   0        0        0        0 2023-05-24 19:22:45.638239 spacetraders-0.5.0/spacetraders/api/default/__init__.py
+-rw-r--r--   0        0        0     4069 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/default/get_status.py
+-rw-r--r--   0        0        0     6960 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/default/register.py
+-rw-r--r--   0        0        0        0 2023-05-24 19:22:45.688239 spacetraders-0.5.0/spacetraders/api/factions/__init__.py
+-rw-r--r--   0        0        0     4427 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/factions/get_faction.py
+-rw-r--r--   0        0        0     4853 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/factions/get_factions.py
+-rw-r--r--   0        0        0        0 2023-05-24 19:22:45.688239 spacetraders-0.5.0/spacetraders/api/fleet/__init__.py
+-rw-r--r--   0        0        0     4900 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/create_chart.py
+-rw-r--r--   0        0        0     4550 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/create_ship_ship_scan.py
+-rw-r--r--   0        0        0     4587 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/create_ship_system_scan.py
+-rw-r--r--   0        0        0     4615 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
+-rw-r--r--   0        0        0     5382 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/create_survey.py
+-rw-r--r--   0        0        0     4961 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/fleet/dock_ship.py
+-rw-r--r--   0        0        0     5217 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/fleet/extract_resources.py
+-rw-r--r--   0        0        0     4373 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/fleet/get_my_ship.py
+-rw-r--r--   0        0        0     4447 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/get_my_ship_cargo.py
+-rw-r--r--   0        0        0     4871 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/get_my_ships.py
+-rw-r--r--   0        0        0     5562 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/get_ship_cooldown.py
+-rw-r--r--   0        0        0     4414 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/get_ship_nav.py
+-rw-r--r--   0        0        0     4905 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/jettison.py
+-rw-r--r--   0        0        0     5343 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/fleet/jump_ship.py
+-rw-r--r--   0        0        0     5893 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/navigate_ship.py
+-rw-r--r--   0        0        0     4905 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/negotiate_contract.py
+-rw-r--r--   0        0        0     4954 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/orbit_ship.py
+-rw-r--r--   0        0        0     5001 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/patch_ship_nav.py
+-rw-r--r--   0        0        0     5192 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/purchase_cargo.py
+-rw-r--r--   0        0        0     4680 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/purchase_ship.py
+-rw-r--r--   0        0        0     4419 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/refuel_ship.py
+-rw-r--r--   0        0        0     5010 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/sell_cargo.py
+-rw-r--r--   0        0        0     5244 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/ship_refine.py
+-rw-r--r--   0        0        0     5215 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/transfer_cargo.py
+-rw-r--r--   0        0        0     5569 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/warp_ship.py
+-rw-r--r--   0        0        0        0 2023-05-24 19:22:45.678239 spacetraders-0.5.0/spacetraders/api/systems/__init__.py
+-rw-r--r--   0        0        0     4675 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/systems/get_jump_gate.py
+-rw-r--r--   0        0        0     5061 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/systems/get_market.py
+-rw-r--r--   0        0        0     4891 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/systems/get_shipyard.py
+-rw-r--r--   0        0        0     4409 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/systems/get_system.py
+-rw-r--r--   0        0        0     5421 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/systems/get_system_waypoints.py
+-rw-r--r--   0        0        0     4817 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/systems/get_systems.py
+-rw-r--r--   0        0        0     4650 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/systems/get_waypoint.py
+-rw-r--r--   0        0        0     4384 2023-05-24 19:22:46.688239 spacetraders-0.5.0/spacetraders/client.py
+-rw-r--r--   0        0        0      470 2023-05-24 19:22:46.578239 spacetraders-0.5.0/spacetraders/errors.py
+-rw-r--r--   0        0        0    14521 2023-05-24 19:22:46.838239 spacetraders-0.5.0/spacetraders/models/__init__.py
+-rw-r--r--   0        0        0     1269 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/accept_contract_response_200.py
+-rw-r--r--   0        0        0     1299 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/accept_contract_response_200_data.py
+-rw-r--r--   0        0        0     1587 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/agent.py
+-rw-r--r--   0        0        0     1532 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/chart.py
+-rw-r--r--   0        0        0     1709 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/connected_system.py
+-rw-r--r--   0        0        0     2160 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/contract.py
+-rw-r--r--   0        0        0     1712 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/contract_deliver_good.py
+-rw-r--r--   0        0        0     1340 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/contract_payment.py
+-rw-r--r--   0        0        0     1567 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/contract_terms.py
+-rw-r--r--   0        0        0      201 2023-05-24 19:22:45.828239 spacetraders-0.5.0/spacetraders/models/contract_type.py
+-rw-r--r--   0        0        0     1744 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/cooldown.py
+-rw-r--r--   0        0        0     1251 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/create_chart_response_201.py
+-rw-r--r--   0        0        0     1469 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/create_chart_response_201_data.py
+-rw-r--r--   0        0        0     1304 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/create_ship_ship_scan_response_201.py
+-rw-r--r--   0        0        0     1425 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
+-rw-r--r--   0        0        0     1316 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/create_ship_system_scan_response_201.py
+-rw-r--r--   0        0        0     1443 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/create_ship_system_scan_response_201_data.py
+-rw-r--r--   0        0        0     1328 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
+-rw-r--r--   0        0        0     1461 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
+-rw-r--r--   0        0        0     1257 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/create_survey_response_201.py
+-rw-r--r--   0        0        0     1398 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/create_survey_response_201_data.py
+-rw-r--r--   0        0        0     1284 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/deliver_contract_json_body.py
+-rw-r--r--   0        0        0     1275 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/deliver_contract_response_200.py
+-rw-r--r--   0        0        0     1318 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/deliver_contract_response_200_data.py
+-rw-r--r--   0        0        0     1292 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/dock_ship_dock_ship_200_response.py
+-rw-r--r--   0        0        0     1227 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
+-rw-r--r--   0        0        0     1368 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/extract_resources_json_body.py
+-rw-r--r--   0        0        0     1281 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/extract_resources_response_201.py
+-rw-r--r--   0        0        0     1532 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/extract_resources_response_201_data.py
+-rw-r--r--   0        0        0     1261 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/extraction.py
+-rw-r--r--   0        0        0     1250 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/extraction_yield.py
+-rw-r--r--   0        0        0     1604 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/faction.py
+-rw-r--r--   0        0        0     1421 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/faction_trait.py
+-rw-r--r--   0        0        0     1869 2023-05-24 19:22:45.938239 spacetraders-0.5.0/spacetraders/models/faction_trait_symbol.py
+-rw-r--r--   0        0        0     1275 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/fulfill_contract_response_200.py
+-rw-r--r--   0        0        0     1301 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/fulfill_contract_response_200_data.py
+-rw-r--r--   0        0        0     1175 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_contract_response_200.py
+-rw-r--r--   0        0        0     1282 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_contracts_response_200.py
+-rw-r--r--   0        0        0     1169 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/get_faction_response_200.py
+-rw-r--r--   0        0        0     1276 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/get_factions_response_200.py
+-rw-r--r--   0        0        0     1176 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_jump_gate_response_200.py
+-rw-r--r--   0        0        0     1163 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_market_response_200.py
+-rw-r--r--   0        0        0     1161 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_my_agent_response_200.py
+-rw-r--r--   0        0        0     1186 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_my_ship_cargo_response_200.py
+-rw-r--r--   0        0        0     1162 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/get_my_ship_response_200.py
+-rw-r--r--   0        0        0     1262 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_my_ships_response_200.py
+-rw-r--r--   0        0        0     1262 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_ship_cooldown_response_200.py
+-rw-r--r--   0        0        0     1210 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1175 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_shipyard_response_200.py
+-rw-r--r--   0        0        0     2640 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200.py
+-rw-r--r--   0        0        0     1213 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_announcements_item.py
+-rw-r--r--   0        0        0     1807 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_leaderboards.py
+-rw-r--r--   0        0        0     1264 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py
+-rw-r--r--   0        0        0     1289 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py
+-rw-r--r--   0        0        0     1191 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_links_item.py
+-rw-r--r--   0        0        0     1314 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_server_resets.py
+-rw-r--r--   0        0        0     1331 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_stats.py
+-rw-r--r--   0        0        0     1163 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_system_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_system_waypoints_response_200.py
+-rw-r--r--   0        0        0     1270 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/get_systems_response_200.py
+-rw-r--r--   0        0        0     1266 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_waypoint_response_200.py
+-rw-r--r--   0        0        0     1177 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/jettison_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/jettison_response_200.py
+-rw-r--r--   0        0        0     1185 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/jettison_response_200_data.py
+-rw-r--r--   0        0        0     1606 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/jump_gate.py
+-rw-r--r--   0        0        0     1168 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/jump_ship_json_body.py
+-rw-r--r--   0        0        0     1233 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/jump_ship_response_200.py
+-rw-r--r--   0        0        0     1462 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/jump_ship_response_200_data.py
+-rw-r--r--   0        0        0     2398 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/market.py
+-rw-r--r--   0        0        0     1880 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/market_trade_good.py
+-rw-r--r--   0        0        0      224 2023-05-24 19:22:45.828239 spacetraders-0.5.0/spacetraders/models/market_trade_good_supply.py
+-rw-r--r--   0        0        0     2109 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/market_transaction.py
+-rw-r--r--   0        0        0      170 2023-05-24 19:22:45.838239 spacetraders-0.5.0/spacetraders/models/market_transaction_type.py
+-rw-r--r--   0        0        0     1206 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/meta.py
+-rw-r--r--   0        0        0     1176 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/navigate_ship_json_body.py
+-rw-r--r--   0        0        0     1257 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/navigate_ship_response_200.py
+-rw-r--r--   0        0        0     1444 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/navigate_ship_response_200_data.py
+-rw-r--r--   0        0        0     1400 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py
+-rw-r--r--   0        0        0     1241 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py
+-rw-r--r--   0        0        0     1304 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
+-rw-r--r--   0        0        0     1231 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
+-rw-r--r--   0        0        0     1420 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/patch_ship_nav_json_body.py
+-rw-r--r--   0        0        0     1214 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/patch_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1352 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
+-rw-r--r--   0        0        0     1484 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1211 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
+-rw-r--r--   0        0        0     1333 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/purchase_ship_json_body.py
+-rw-r--r--   0        0        0     1257 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/purchase_ship_response_201.py
+-rw-r--r--   0        0        0     1447 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/purchase_ship_response_201_data.py
+-rw-r--r--   0        0        0     1245 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/refuel_ship_response_200.py
+-rw-r--r--   0        0        0     1562 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/refuel_ship_response_200_data.py
+-rw-r--r--   0        0        0     1611 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/register_json_body.py
+-rw-r--r--   0        0        0      244 2023-05-24 19:22:45.918239 spacetraders-0.5.0/spacetraders/models/register_json_body_faction.py
+-rw-r--r--   0        0        0     1232 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/register_response_201.py
+-rw-r--r--   0        0        0     1608 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/register_response_201_data.py
+-rw-r--r--   0        0        0     2444 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/scanned_ship.py
+-rw-r--r--   0        0        0     1144 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/scanned_ship_engine.py
+-rw-r--r--   0        0        0     1141 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/scanned_ship_frame.py
+-rw-r--r--   0        0        0     1149 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/scanned_ship_mounts_item.py
+-rw-r--r--   0        0        0     1147 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/scanned_ship_reactor.py
+-rw-r--r--   0        0        0     1492 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/scanned_system.py
+-rw-r--r--   0        0        0     2293 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/scanned_waypoint.py
+-rw-r--r--   0        0        0     1304 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
+-rw-r--r--   0        0        0     1468 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1195 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_request.py
+-rw-r--r--   0        0        0     3140 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship.py
+-rw-r--r--   0        0        0     1484 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_cargo.py
+-rw-r--r--   0        0        0     1510 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_cargo_item.py
+-rw-r--r--   0        0        0     2248 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_crew.py
+-rw-r--r--   0        0        0      167 2023-05-24 19:22:45.788239 spacetraders-0.5.0/spacetraders/models/ship_crew_rotation.py
+-rw-r--r--   0        0        0     1879 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_engine.py
+-rw-r--r--   0        0        0      319 2023-05-24 19:22:45.928239 spacetraders-0.5.0/spacetraders/models/ship_engine_symbol.py
+-rw-r--r--   0        0        0     2278 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_frame.py
+-rw-r--r--   0        0        0      694 2023-05-24 19:22:45.808239 spacetraders-0.5.0/spacetraders/models/ship_frame_symbol.py
+-rw-r--r--   0        0        0     1586 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/ship_fuel.py
+-rw-r--r--   0        0        0     1340 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/ship_fuel_consumed.py
+-rw-r--r--   0        0        0     1965 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/ship_module.py
+-rw-r--r--   0        0        0     1033 2023-05-24 19:22:45.848239 spacetraders-0.5.0/spacetraders/models/ship_module_symbol.py
+-rw-r--r--   0        0        0     1947 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_mount.py
+-rw-r--r--   0        0        0      572 2023-05-24 19:22:45.928239 spacetraders-0.5.0/spacetraders/models/ship_mount_deposits_item.py
+-rw-r--r--   0        0        0      854 2023-05-24 19:22:45.928239 spacetraders-0.5.0/spacetraders/models/ship_mount_symbol.py
+-rw-r--r--   0        0        0     2114 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/ship_nav.py
+-rw-r--r--   0        0        0      206 2023-05-24 19:22:45.818239 spacetraders-0.5.0/spacetraders/models/ship_nav_flight_mode.py
+-rw-r--r--   0        0        0     1891 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_nav_route.py
+-rw-r--r--   0        0        0     1497 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_nav_route_waypoint.py
+-rw-r--r--   0        0        0      196 2023-05-24 19:22:45.838239 spacetraders-0.5.0/spacetraders/models/ship_nav_status.py
+-rw-r--r--   0        0        0     1934 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/ship_reactor.py
+-rw-r--r--   0        0        0      344 2023-05-24 19:22:45.818239 spacetraders-0.5.0/spacetraders/models/ship_reactor_symbol.py
+-rw-r--r--   0        0        0     1246 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/ship_refine_json_body.py
+-rw-r--r--   0        0        0      330 2023-05-24 19:22:45.918239 spacetraders-0.5.0/spacetraders/models/ship_refine_json_body_produce.py
+-rw-r--r--   0        0        0     1316 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response.py
+-rw-r--r--   0        0        0     2047 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py
+-rw-r--r--   0        0        0     1344 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
+-rw-r--r--   0        0        0     1344 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
+-rw-r--r--   0        0        0     1477 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/ship_registration.py
+-rw-r--r--   0        0        0     1541 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_requirements.py
+-rw-r--r--   0        0        0      479 2023-05-24 19:22:45.898239 spacetraders-0.5.0/spacetraders/models/ship_role.py
+-rw-r--r--   0        0        0      549 2023-05-24 19:22:45.798239 spacetraders-0.5.0/spacetraders/models/ship_type.py
+-rw-r--r--   0        0        0     2009 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/shipyard.py
+-rw-r--r--   0        0        0     2498 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/shipyard_ship.py
+-rw-r--r--   0        0        0     1225 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/shipyard_ship_types_item.py
+-rw-r--r--   0        0        0     1698 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/shipyard_transaction.py
+-rw-r--r--   0        0        0     2228 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/survey.py
+-rw-r--r--   0        0        0     1209 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/survey_deposit.py
+-rw-r--r--   0        0        0      181 2023-05-24 19:22:45.818239 spacetraders-0.5.0/spacetraders/models/survey_size.py
+-rw-r--r--   0        0        0     1725 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/system.py
+-rw-r--r--   0        0        0     1112 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/system_faction.py
+-rw-r--r--   0        0        0      405 2023-05-24 19:22:45.818239 spacetraders-0.5.0/spacetraders/models/system_type.py
+-rw-r--r--   0        0        0     1352 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/system_waypoint.py
+-rw-r--r--   0        0        0     1299 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/trade_good.py
+-rw-r--r--   0        0        0     4422 2023-05-24 19:22:45.908239 spacetraders-0.5.0/spacetraders/models/trade_symbol.py
+-rw-r--r--   0        0        0     1352 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
+-rw-r--r--   0        0        0     1221 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
+-rw-r--r--   0        0        0     1304 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
+-rw-r--r--   0        0        0     1168 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/warp_ship_json_body.py
+-rw-r--r--   0        0        0     1233 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/warp_ship_response_200.py
+-rw-r--r--   0        0        0     1436 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/warp_ship_response_200_data.py
+-rw-r--r--   0        0        0     2279 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/waypoint.py
+-rw-r--r--   0        0        0     1116 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/waypoint_faction.py
+-rw-r--r--   0        0        0     1178 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/waypoint_orbital.py
+-rw-r--r--   0        0        0     1427 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/waypoint_trait.py
+-rw-r--r--   0        0        0     2200 2023-05-24 19:22:45.938239 spacetraders-0.5.0/spacetraders/models/waypoint_trait_symbol.py
+-rw-r--r--   0        0        0      381 2023-05-24 19:22:45.818239 spacetraders-0.5.0/spacetraders/models/waypoint_type.py
+-rw-r--r--   0        0        0     1341 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/types.py
+-rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 spacetraders-0.5.0/PKG-INFO
```

### Comparing `spacetraders-0.4.0/README.md` & `spacetraders-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/pyproject.toml` & `spacetraders-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacetraders"
-version = "0.4.0"
+version = "0.5.0"
 description = "Python API for Space Traders"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "spacetraders"}]
 
 [tool.poetry.dependencies]
```

### Comparing `spacetraders-0.4.0/spacetraders/api/agents/get_my_agent.py` & `spacetraders-0.5.0/spacetraders/api/agents/get_my_agent.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/contracts/accept_contract.py` & `spacetraders-0.5.0/spacetraders/api/contracts/accept_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/contracts/deliver_contract.py` & `spacetraders-0.5.0/spacetraders/api/contracts/deliver_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/contracts/fulfill_contract.py` & `spacetraders-0.5.0/spacetraders/api/contracts/fulfill_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/contracts/get_contract.py` & `spacetraders-0.5.0/spacetraders/api/contracts/get_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/contracts/get_contracts.py` & `spacetraders-0.5.0/spacetraders/api/contracts/get_contracts.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/default/register.py` & `spacetraders-0.5.0/spacetraders/api/default/register.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/factions/get_faction.py` & `spacetraders-0.5.0/spacetraders/api/factions/get_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/factions/get_factions.py` & `spacetraders-0.5.0/spacetraders/api/factions/get_factions.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/create_chart.py` & `spacetraders-0.5.0/spacetraders/api/fleet/create_chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/create_ship_ship_scan.py` & `spacetraders-0.5.0/spacetraders/api/fleet/create_ship_ship_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/create_ship_system_scan.py` & `spacetraders-0.5.0/spacetraders/api/fleet/create_ship_system_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/create_ship_waypoint_scan.py` & `spacetraders-0.5.0/spacetraders/api/fleet/create_ship_waypoint_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/create_survey.py` & `spacetraders-0.5.0/spacetraders/api/fleet/create_survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/dock_ship.py` & `spacetraders-0.5.0/spacetraders/api/fleet/dock_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/extract_resources.py` & `spacetraders-0.5.0/spacetraders/api/fleet/extract_resources.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/get_my_ship.py` & `spacetraders-0.5.0/spacetraders/api/fleet/get_my_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/get_my_ship_cargo.py` & `spacetraders-0.5.0/spacetraders/api/fleet/get_my_ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/get_my_ships.py` & `spacetraders-0.5.0/spacetraders/api/fleet/get_my_ships.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/get_ship_cooldown.py` & `spacetraders-0.5.0/spacetraders/api/fleet/get_ship_cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/get_ship_nav.py` & `spacetraders-0.5.0/spacetraders/api/fleet/get_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/jettison.py` & `spacetraders-0.5.0/spacetraders/api/fleet/jettison.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/jump_ship.py` & `spacetraders-0.5.0/spacetraders/api/fleet/jump_ship.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,16 +66,17 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: JumpShipJsonBody,
 ) -> Response[JumpShipResponse200]:
     """Jump Ship
 
-     Jump your ship instantly to a target system. Unlike other forms of navigation, jumping requires a
-    unit of antimatter.
+     Jump your ship instantly to a target system. When used while in orbit or docked to a jump gate
+    waypoint, any ship can use this command. When used elsewhere, jumping requires a jump drive unit and
+    consumes a unit of antimatter (which needs to be in your cargo).
 
     Args:
         ship_symbol (str):
         json_body (JumpShipJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -130,16 +131,17 @@
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     **json_body: JumpShipJsonBody,
 ) -> Response[JumpShipResponse200]:
     """Jump Ship
 
-     Jump your ship instantly to a target system. Unlike other forms of navigation, jumping requires a
-    unit of antimatter.
+     Jump your ship instantly to a target system. When used while in orbit or docked to a jump gate
+    waypoint, any ship can use this command. When used elsewhere, jumping requires a jump drive unit and
+    consumes a unit of antimatter (which needs to be in your cargo).
 
     Args:
         ship_symbol (str):
         json_body (JumpShipJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/navigate_ship.py` & `spacetraders-0.5.0/spacetraders/api/fleet/navigate_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/orbit_ship.py` & `spacetraders-0.5.0/spacetraders/api/fleet/orbit_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/patch_ship_nav.py` & `spacetraders-0.5.0/spacetraders/api/fleet/patch_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/purchase_cargo.py` & `spacetraders-0.5.0/spacetraders/api/fleet/purchase_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/purchase_ship.py` & `spacetraders-0.5.0/spacetraders/api/fleet/purchase_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/refuel_ship.py` & `spacetraders-0.5.0/spacetraders/api/fleet/refuel_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/sell_cargo.py` & `spacetraders-0.5.0/spacetraders/api/fleet/sell_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/ship_refine.py` & `spacetraders-0.5.0/spacetraders/api/fleet/ship_refine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/transfer_cargo.py` & `spacetraders-0.5.0/spacetraders/api/fleet/transfer_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/fleet/warp_ship.py` & `spacetraders-0.5.0/spacetraders/api/fleet/warp_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/systems/get_jump_gate.py` & `spacetraders-0.5.0/spacetraders/api/systems/get_jump_gate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import Client
 from ...models.get_jump_gate_response_200 import GetJumpGateResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/jump-gate".format(
         _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -57,15 +57,15 @@
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetJumpGateResponse200]:
     """Get Jump Gate
 
      Get jump gate details for a waypoint.
 
     Args:
@@ -118,15 +118,15 @@
     )
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetJumpGateResponse200]:
     """Get Jump Gate
 
      Get jump gate details for a waypoint.
 
     Args:
```

### Comparing `spacetraders-0.4.0/spacetraders/api/systems/get_market.py` & `spacetraders-0.5.0/spacetraders/api/systems/get_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import Client
 from ...models.get_market_response_200 import GetMarketResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/market".format(
         _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -57,15 +57,15 @@
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetMarketResponse200]:
     """Get Market
 
      Retrieve imports, exports and exchange data from a marketplace. Imports can be sold, exports can be
     purchased, and exchange goods can be purchased or sold. Send a ship to the waypoint to access trade
     good prices and recent transactions.
@@ -120,15 +120,15 @@
     )
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetMarketResponse200]:
     """Get Market
 
      Retrieve imports, exports and exchange data from a marketplace. Imports can be sold, exports can be
     purchased, and exchange goods can be purchased or sold. Send a ship to the waypoint to access trade
     good prices and recent transactions.
```

### Comparing `spacetraders-0.4.0/spacetraders/api/systems/get_shipyard.py` & `spacetraders-0.5.0/spacetraders/api/systems/get_shipyard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import Client
 from ...models.get_shipyard_response_200 import GetShipyardResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/shipyard".format(
         _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -57,15 +57,15 @@
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetShipyardResponse200]:
     """Get Shipyard
 
      Get the shipyard for a waypoint. Send a ship to the waypoint to access ships that are currently
     available for purchase and recent transactions.
 
@@ -119,15 +119,15 @@
     )
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetShipyardResponse200]:
     """Get Shipyard
 
      Get the shipyard for a waypoint. Send a ship to the waypoint to access ships that are currently
     available for purchase and recent transactions.
```

### Comparing `spacetraders-0.4.0/spacetraders/api/systems/get_system.py` & `spacetraders-0.5.0/spacetraders/api/systems/get_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import Client
 from ...models.get_system_response_200 import GetSystemResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str = "X1-OE",
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}".format(
         _client.base_url, systemSymbol=system_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -55,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     system_symbol: str = "X1-OE",
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetSystemResponse200]:
     """Get System
 
      Get the details of a system.
 
     Args:
@@ -113,15 +113,15 @@
         )
     )
 
 
 async def asyncio_detailed(
     system_symbol: str = "X1-OE",
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetSystemResponse200]:
     """Get System
 
      Get the details of a system.
 
     Args:
```

### Comparing `spacetraders-0.4.0/spacetraders/api/systems/get_system_waypoints.py` & `spacetraders-0.5.0/spacetraders/api/systems/get_system_waypoints.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/api/systems/get_systems.py` & `spacetraders-0.5.0/spacetraders/api/systems/get_systems.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import Client
 from ...models.get_systems_response_200 import GetSystemsResponse200
 from ...types import UNSET, ApiError, Error, Response, Unset
 
 
 def _get_kwargs(
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Dict[str, Any]:
     url = "{}/systems".format(_client.base_url)
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -61,15 +61,15 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetSystemsResponse200]:
     """List Systems
 
      Return a list of all systems.
@@ -122,15 +122,15 @@
             headers=resp.headers,
         )
     )
 
 
 async def asyncio_detailed(
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetSystemsResponse200]:
     """List Systems
 
      Return a list of all systems.
```

### Comparing `spacetraders-0.4.0/spacetraders/api/systems/get_waypoint.py` & `spacetraders-0.5.0/spacetraders/api/systems/get_waypoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import Client
 from ...models.get_waypoint_response_200 import GetWaypointResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}".format(
         _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -57,15 +57,15 @@
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetWaypointResponse200]:
     """Get Waypoint
 
      View the details of a waypoint.
 
     Args:
@@ -118,15 +118,15 @@
     )
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: AuthenticatedClient,
+    _client: Client,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetWaypointResponse200]:
     """Get Waypoint
 
      View the details of a waypoint.
 
     Args:
```

### Comparing `spacetraders-0.4.0/spacetraders/client.py` & `spacetraders-0.5.0/spacetraders/client.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/__init__.py` & `spacetraders-0.5.0/spacetraders/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,14 +49,28 @@
 from .get_my_agent_response_200 import GetMyAgentResponse200
 from .get_my_ship_cargo_response_200 import GetMyShipCargoResponse200
 from .get_my_ship_response_200 import GetMyShipResponse200
 from .get_my_ships_response_200 import GetMyShipsResponse200
 from .get_ship_cooldown_response_200 import GetShipCooldownResponse200
 from .get_ship_nav_response_200 import GetShipNavResponse200
 from .get_shipyard_response_200 import GetShipyardResponse200
+from .get_status_response_200 import GetStatusResponse200
+from .get_status_response_200_announcements_item import (
+    GetStatusResponse200AnnouncementsItem,
+)
+from .get_status_response_200_leaderboards import GetStatusResponse200Leaderboards
+from .get_status_response_200_leaderboards_most_credits_item import (
+    GetStatusResponse200LeaderboardsMostCreditsItem,
+)
+from .get_status_response_200_leaderboards_most_submitted_charts_item import (
+    GetStatusResponse200LeaderboardsMostSubmittedChartsItem,
+)
+from .get_status_response_200_links_item import GetStatusResponse200LinksItem
+from .get_status_response_200_server_resets import GetStatusResponse200ServerResets
+from .get_status_response_200_stats import GetStatusResponse200Stats
 from .get_system_response_200 import GetSystemResponse200
 from .get_system_waypoints_response_200 import GetSystemWaypointsResponse200
 from .get_systems_response_200 import GetSystemsResponse200
 from .get_waypoint_response_200 import GetWaypointResponse200
 from .jettison_json_body import JettisonJsonBody
 from .jettison_response_200 import JettisonResponse200
 from .jettison_response_200_data import JettisonResponse200Data
@@ -69,14 +83,20 @@
 from .market_trade_good_supply import MarketTradeGoodSupply
 from .market_transaction import MarketTransaction
 from .market_transaction_type import MarketTransactionType
 from .meta import Meta
 from .navigate_ship_json_body import NavigateShipJsonBody
 from .navigate_ship_response_200 import NavigateShipResponse200
 from .navigate_ship_response_200_data import NavigateShipResponse200Data
+from .negotiate_contract_negotiate_contract_200_response import (
+    NegotiateContractNegotiateContract200Response,
+)
+from .negotiate_contract_negotiate_contract_200_response_data import (
+    NegotiateContractNegotiateContract200ResponseData,
+)
 from .orbit_ship_orbit_ship_200_response import OrbitShipOrbitShip200Response
 from .orbit_ship_orbit_ship_200_response_data import OrbitShipOrbitShip200ResponseData
 from .patch_ship_nav_json_body import PatchShipNavJsonBody
 from .patch_ship_nav_response_200 import PatchShipNavResponse200
 from .purchase_cargo_purchase_cargo_201_response import (
     PurchaseCargoPurchaseCargo201Response,
 )
@@ -218,14 +238,22 @@
     "GetMyAgentResponse200",
     "GetMyShipCargoResponse200",
     "GetMyShipResponse200",
     "GetMyShipsResponse200",
     "GetShipCooldownResponse200",
     "GetShipNavResponse200",
     "GetShipyardResponse200",
+    "GetStatusResponse200",
+    "GetStatusResponse200AnnouncementsItem",
+    "GetStatusResponse200Leaderboards",
+    "GetStatusResponse200LeaderboardsMostCreditsItem",
+    "GetStatusResponse200LeaderboardsMostSubmittedChartsItem",
+    "GetStatusResponse200LinksItem",
+    "GetStatusResponse200ServerResets",
+    "GetStatusResponse200Stats",
     "GetSystemResponse200",
     "GetSystemsResponse200",
     "GetSystemWaypointsResponse200",
     "GetWaypointResponse200",
     "JettisonJsonBody",
     "JettisonResponse200",
     "JettisonResponse200Data",
@@ -238,14 +266,16 @@
     "MarketTradeGoodSupply",
     "MarketTransaction",
     "MarketTransactionType",
     "Meta",
     "NavigateShipJsonBody",
     "NavigateShipResponse200",
     "NavigateShipResponse200Data",
+    "NegotiateContractNegotiateContract200Response",
+    "NegotiateContractNegotiateContract200ResponseData",
     "OrbitShipOrbitShip200Response",
     "OrbitShipOrbitShip200ResponseData",
     "PatchShipNavJsonBody",
     "PatchShipNavResponse200",
     "PurchaseCargoPurchaseCargo201Response",
     "PurchaseCargoPurchaseCargo201ResponseData",
     "PurchaseCargoPurchaseCargoRequest",
```

### Comparing `spacetraders-0.4.0/spacetraders/models/accept_contract_response_200.py` & `spacetraders-0.5.0/spacetraders/models/accept_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/accept_contract_response_200_data.py` & `spacetraders-0.5.0/spacetraders/models/accept_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/agent.py` & `spacetraders-0.5.0/spacetraders/models/scanned_ship_frame.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,31 +5,25 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="Agent")
+T = TypeVar("T", bound="ScannedShipFrame")
 
 
-class Agent(BaseModel):
-    """
+class ScannedShipFrame(BaseModel):
+    """The frame of the ship.
+
     Attributes:
-        account_id (str):
         symbol (str):
-        headquarters (str): The headquarters of the agent.
-        credits_ (int): The number of credits the agent has available. Credits can be negative if funds have been
-            overdrawn.
     """
 
-    account_id: str = Field(alias="accountId")
     symbol: str = Field(alias="symbol")
-    headquarters: str = Field(alias="headquarters")
-    credits_: int = Field(alias="credits")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/chart.py` & `spacetraders-0.5.0/spacetraders/models/chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/connected_system.py` & `spacetraders-0.5.0/spacetraders/models/connected_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/contract.py` & `spacetraders-0.5.0/spacetraders/models/scanned_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-import datetime
 from typing import (
     Any,
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.contract_terms import ContractTerms
-from ..models.contract_type import ContractType
+from ..models.system_type import SystemType
 from ..types import Unset
 
-T = TypeVar("T", bound="Contract")
+T = TypeVar("T", bound="ScannedSystem")
 
 
-class Contract(BaseModel):
+class ScannedSystem(BaseModel):
     """
     Attributes:
-        id (str):
-        faction_symbol (str): The symbol of the faction that this contract is for.
-        type (ContractType):
-        terms (ContractTerms):
-        accepted (bool): Whether the contract has been accepted by the agent
-        fulfilled (bool): Whether the contract has been fulfilled
-        expiration (datetime.datetime): The time at which the contract expires
+        symbol (str):
+        sector_symbol (str):
+        type (SystemType): The type of waypoint.
+        x (int):
+        y (int):
+        distance (int):
     """
 
-    id: str = Field(alias="id")
-    faction_symbol: str = Field(alias="factionSymbol")
-    type: ContractType = Field(alias="type")
-    terms: "ContractTerms" = Field(alias="terms")
-    expiration: datetime.datetime = Field(alias="expiration")
-    accepted: bool = Field(False, alias="accepted")
-    fulfilled: bool = Field(False, alias="fulfilled")
+    symbol: str = Field(alias="symbol")
+    sector_symbol: str = Field(alias="sectorSymbol")
+    type: SystemType = Field(alias="type")
+    x: int = Field(alias="x")
+    y: int = Field(alias="y")
+    distance: int = Field(alias="distance")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/contract_deliver_good.py` & `spacetraders-0.5.0/spacetraders/models/contract_deliver_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/contract_payment.py` & `spacetraders-0.5.0/spacetraders/models/contract_payment.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/contract_terms.py` & `spacetraders-0.5.0/spacetraders/models/contract_terms.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/cooldown.py` & `spacetraders-0.5.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,29 @@
-import datetime
 from typing import (
     Any,
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
+from ..models.ship_nav import ShipNav
 from ..types import Unset
 
-T = TypeVar("T", bound="Cooldown")
+T = TypeVar("T", bound="OrbitShipOrbitShip200ResponseData")
 
 
-class Cooldown(BaseModel):
-    """A cooldown is a period of time in which a ship cannot perform certain actions.
-
+class OrbitShipOrbitShip200ResponseData(BaseModel):
+    """
     Attributes:
-        ship_symbol (str): The symbol of the ship that is on cooldown
-        total_seconds (int): The total duration of the cooldown in seconds
-        remaining_seconds (int): The remaining duration of the cooldown in seconds
-        expiration (datetime.datetime): The date and time when the cooldown expires in ISO 8601 format
+        nav (ShipNav): The navigation information of the ship.
     """
 
-    ship_symbol: str = Field(alias="shipSymbol")
-    total_seconds: int = Field(alias="totalSeconds")
-    remaining_seconds: int = Field(alias="remainingSeconds")
-    expiration: datetime.datetime = Field(alias="expiration")
+    nav: "ShipNav" = Field(alias="nav")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/create_chart_response_201.py` & `spacetraders-0.5.0/spacetraders/models/create_chart_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/create_chart_response_201_data.py` & `spacetraders-0.5.0/spacetraders/models/create_chart_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/create_ship_ship_scan_response_201.py` & `spacetraders-0.5.0/spacetraders/models/create_ship_ship_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/create_ship_ship_scan_response_201_data.py` & `spacetraders-0.5.0/spacetraders/models/create_ship_ship_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/create_ship_system_scan_response_201.py` & `spacetraders-0.5.0/spacetraders/models/create_ship_system_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/create_ship_system_scan_response_201_data.py` & `spacetraders-0.5.0/spacetraders/models/create_ship_system_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/create_ship_waypoint_scan_response_201.py` & `spacetraders-0.5.0/spacetraders/models/create_ship_waypoint_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py` & `spacetraders-0.5.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/create_survey_response_201.py` & `spacetraders-0.5.0/spacetraders/models/create_survey_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/create_survey_response_201_data.py` & `spacetraders-0.5.0/spacetraders/models/create_survey_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/deliver_contract_json_body.py` & `spacetraders-0.5.0/spacetraders/models/deliver_contract_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/deliver_contract_response_200.py` & `spacetraders-0.5.0/spacetraders/models/deliver_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/deliver_contract_response_200_data.py` & `spacetraders-0.5.0/spacetraders/models/deliver_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/dock_ship_dock_ship_200_response.py` & `spacetraders-0.5.0/spacetraders/models/dock_ship_dock_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py` & `spacetraders-0.5.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/extract_resources_json_body.py` & `spacetraders-0.5.0/spacetraders/models/extract_resources_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/extract_resources_response_201.py` & `spacetraders-0.5.0/spacetraders/models/extract_resources_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/extract_resources_response_201_data.py` & `spacetraders-0.5.0/spacetraders/models/extract_resources_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/extraction.py` & `spacetraders-0.5.0/spacetraders/models/extraction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/extraction_yield.py` & `spacetraders-0.5.0/spacetraders/models/extraction_yield.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/faction.py` & `spacetraders-0.5.0/spacetraders/models/jettison_json_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,35 +3,28 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.faction_trait import FactionTrait
 from ..types import Unset
 
-T = TypeVar("T", bound="Faction")
+T = TypeVar("T", bound="JettisonJsonBody")
 
 
-class Faction(BaseModel):
+class JettisonJsonBody(BaseModel):
     """
     Attributes:
         symbol (str):
-        name (str):
-        description (str):
-        headquarters (str):
-        traits (List['FactionTrait']):
+        units (int):
     """
 
     symbol: str = Field(alias="symbol")
-    name: str = Field(alias="name")
-    description: str = Field(alias="description")
-    headquarters: str = Field(alias="headquarters")
-    traits: List["FactionTrait"] = Field(alias="traits")
+    units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/faction_trait.py` & `spacetraders-0.5.0/spacetraders/models/faction_trait.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/faction_trait_symbol.py` & `spacetraders-0.5.0/spacetraders/models/faction_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/fulfill_contract_response_200.py` & `spacetraders-0.5.0/spacetraders/models/fulfill_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/fulfill_contract_response_200_data.py` & `spacetraders-0.5.0/spacetraders/models/fulfill_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_contract_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_contracts_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_contracts_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_faction_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_faction_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_factions_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_factions_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_jump_gate_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_jump_gate_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_market_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_market_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_my_agent_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_my_agent_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_my_ship_cargo_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_my_ship_cargo_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_my_ship_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_my_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_my_ships_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_my_ships_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_ship_cooldown_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_ship_cooldown_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_ship_nav_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_shipyard_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_shipyard_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_system_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_system_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_system_waypoints_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_system_waypoints_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_systems_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_systems_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/get_waypoint_response_200.py` & `spacetraders-0.5.0/spacetraders/models/get_waypoint_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/jettison_json_body.py` & `spacetraders-0.5.0/spacetraders/models/waypoint_faction.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,26 +5,24 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="JettisonJsonBody")
+T = TypeVar("T", bound="WaypointFaction")
 
 
-class JettisonJsonBody(BaseModel):
+class WaypointFaction(BaseModel):
     """
     Attributes:
         symbol (str):
-        units (int):
     """
 
     symbol: str = Field(alias="symbol")
-    units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/jettison_response_200.py` & `spacetraders-0.5.0/spacetraders/models/jettison_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/jettison_response_200_data.py` & `spacetraders-0.5.0/spacetraders/models/jettison_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/jump_gate.py` & `spacetraders-0.5.0/spacetraders/models/jump_gate.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/jump_ship_json_body.py` & `spacetraders-0.5.0/spacetraders/models/jump_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/jump_ship_response_200.py` & `spacetraders-0.5.0/spacetraders/models/jump_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/jump_ship_response_200_data.py` & `spacetraders-0.5.0/spacetraders/models/jump_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/market.py` & `spacetraders-0.5.0/spacetraders/models/market.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/market_trade_good.py` & `spacetraders-0.5.0/spacetraders/models/market_trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/market_transaction.py` & `spacetraders-0.5.0/spacetraders/models/market_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/meta.py` & `spacetraders-0.5.0/spacetraders/models/meta.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/navigate_ship_json_body.py` & `spacetraders-0.5.0/spacetraders/models/navigate_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/navigate_ship_response_200.py` & `spacetraders-0.5.0/spacetraders/models/navigate_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/navigate_ship_response_200_data.py` & `spacetraders-0.5.0/spacetraders/models/navigate_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py` & `spacetraders-0.5.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py` & `spacetraders-0.5.0/spacetraders/models/survey_deposit.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,27 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.ship_nav import ShipNav
 from ..types import Unset
 
-T = TypeVar("T", bound="OrbitShipOrbitShip200ResponseData")
+T = TypeVar("T", bound="SurveyDeposit")
 
 
-class OrbitShipOrbitShip200ResponseData(BaseModel):
-    """
+class SurveyDeposit(BaseModel):
+    """A surveyed deposit of a mineral or resource available for extraction.
+
     Attributes:
-        nav (ShipNav): The navigation information of the ship.
+        symbol (str): The symbol of the deposit.
     """
 
-    nav: "ShipNav" = Field(alias="nav")
+    symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/patch_ship_nav_json_body.py` & `spacetraders-0.5.0/spacetraders/models/patch_ship_nav_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/patch_ship_nav_response_200.py` & `spacetraders-0.5.0/spacetraders/models/patch_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py` & `spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py` & `spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py` & `spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/purchase_ship_json_body.py` & `spacetraders-0.5.0/spacetraders/models/purchase_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/purchase_ship_response_201.py` & `spacetraders-0.5.0/spacetraders/models/purchase_ship_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/purchase_ship_response_201_data.py` & `spacetraders-0.5.0/spacetraders/models/purchase_ship_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/refuel_ship_response_200.py` & `spacetraders-0.5.0/spacetraders/models/refuel_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/refuel_ship_response_200_data.py` & `spacetraders-0.5.0/spacetraders/models/warp_ship_response_200_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,31 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.agent import Agent
 from ..models.ship_fuel import ShipFuel
+from ..models.ship_nav import ShipNav
 from ..types import Unset
 
-T = TypeVar("T", bound="RefuelShipResponse200Data")
+T = TypeVar("T", bound="WarpShipResponse200Data")
 
 
-class RefuelShipResponse200Data(BaseModel):
+class WarpShipResponse200Data(BaseModel):
     """
     Attributes:
-        agent (Agent):
         fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
             or action.
+        nav (ShipNav): The navigation information of the ship.
     """
 
-    agent: "Agent" = Field(alias="agent")
     fuel: "ShipFuel" = Field(alias="fuel")
+    nav: "ShipNav" = Field(alias="nav")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/register_json_body.py` & `spacetraders-0.5.0/spacetraders/models/register_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/register_response_201.py` & `spacetraders-0.5.0/spacetraders/models/register_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/register_response_201_data.py` & `spacetraders-0.5.0/spacetraders/models/register_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/scanned_ship.py` & `spacetraders-0.5.0/spacetraders/models/scanned_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/scanned_ship_engine.py` & `spacetraders-0.5.0/spacetraders/models/scanned_ship_engine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/scanned_ship_frame.py` & `spacetraders-0.5.0/spacetraders/models/waypoint_orbital.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,19 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="ScannedShipFrame")
+T = TypeVar("T", bound="WaypointOrbital")
 
 
-class ScannedShipFrame(BaseModel):
-    """The frame of the ship.
+class WaypointOrbital(BaseModel):
+    """An orbital is another waypoint that orbits a parent waypoint.
 
     Attributes:
         symbol (str):
     """
 
     symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
```

### Comparing `spacetraders-0.4.0/spacetraders/models/scanned_ship_mounts_item.py` & `spacetraders-0.5.0/spacetraders/models/scanned_ship_mounts_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/scanned_ship_reactor.py` & `spacetraders-0.5.0/spacetraders/models/scanned_ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/scanned_system.py` & `spacetraders-0.5.0/spacetraders/models/ship_nav_route_waypoint.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,37 +3,36 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.system_type import SystemType
+from ..models.waypoint_type import WaypointType
 from ..types import Unset
 
-T = TypeVar("T", bound="ScannedSystem")
+T = TypeVar("T", bound="ShipNavRouteWaypoint")
 
 
-class ScannedSystem(BaseModel):
-    """
+class ShipNavRouteWaypoint(BaseModel):
+    """The destination or departure of a ships nav route.
+
     Attributes:
         symbol (str):
-        sector_symbol (str):
-        type (SystemType): The type of waypoint.
+        type (WaypointType): The type of waypoint.
+        system_symbol (str):
         x (int):
         y (int):
-        distance (int):
     """
 
     symbol: str = Field(alias="symbol")
-    sector_symbol: str = Field(alias="sectorSymbol")
-    type: SystemType = Field(alias="type")
+    type: WaypointType = Field(alias="type")
+    system_symbol: str = Field(alias="systemSymbol")
     x: int = Field(alias="x")
     y: int = Field(alias="y")
-    distance: int = Field(alias="distance")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/scanned_waypoint.py` & `spacetraders-0.5.0/spacetraders/models/scanned_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py` & `spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py` & `spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_request.py` & `spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship.py` & `spacetraders-0.5.0/spacetraders/models/ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_cargo.py` & `spacetraders-0.5.0/spacetraders/models/ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_cargo_item.py` & `spacetraders-0.5.0/spacetraders/models/ship_cargo_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_crew.py` & `spacetraders-0.5.0/spacetraders/models/ship_crew.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_engine.py` & `spacetraders-0.5.0/spacetraders/models/ship_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 class ShipEngine(BaseModel):
     """The engine determines how quickly a ship travels between waypoints.
 
     Attributes:
         symbol (ShipEngineSymbol):
         name (str):
         description (str):
-        speed (float):
+        speed (int):
         requirements (ShipRequirements): The requirements for installation on a ship
         condition (Union[Unset, int]): Condition is a range of 0 to 100 where 0 is completely worn out and 100 is brand
             new.
     """
 
     symbol: ShipEngineSymbol = Field(alias="symbol")
     name: str = Field(alias="name")
     description: str = Field(alias="description")
-    speed: float = Field(alias="speed")
+    speed: int = Field(alias="speed")
     requirements: "ShipRequirements" = Field(alias="requirements")
     condition: Union[Unset, int] = Field(UNSET, alias="condition")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_frame.py` & `spacetraders-0.5.0/spacetraders/models/ship_frame.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_frame_symbol.py` & `spacetraders-0.5.0/spacetraders/models/ship_frame_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_fuel.py` & `spacetraders-0.5.0/spacetraders/models/ship_fuel.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_fuel_consumed.py` & `spacetraders-0.5.0/spacetraders/models/ship_fuel_consumed.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_module.py` & `spacetraders-0.5.0/spacetraders/models/ship_module.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_module_symbol.py` & `spacetraders-0.5.0/spacetraders/models/ship_module_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_mount.py` & `spacetraders-0.5.0/spacetraders/models/ship_mount.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_mount_deposits_item.py` & `spacetraders-0.5.0/spacetraders/models/ship_mount_deposits_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_mount_symbol.py` & `spacetraders-0.5.0/spacetraders/models/ship_mount_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_nav.py` & `spacetraders-0.5.0/spacetraders/models/ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_nav_route.py` & `spacetraders-0.5.0/spacetraders/models/ship_nav_route.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_nav_route_waypoint.py` & `spacetraders-0.5.0/spacetraders/models/system_waypoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,31 +6,28 @@
 )
 
 from pydantic import BaseModel, Field
 
 from ..models.waypoint_type import WaypointType
 from ..types import Unset
 
-T = TypeVar("T", bound="ShipNavRouteWaypoint")
+T = TypeVar("T", bound="SystemWaypoint")
 
 
-class ShipNavRouteWaypoint(BaseModel):
-    """The destination or departure of a ships nav route.
-
+class SystemWaypoint(BaseModel):
+    """
     Attributes:
         symbol (str):
         type (WaypointType): The type of waypoint.
-        system_symbol (str):
         x (int):
         y (int):
     """
 
     symbol: str = Field(alias="symbol")
     type: WaypointType = Field(alias="type")
-    system_symbol: str = Field(alias="systemSymbol")
     x: int = Field(alias="x")
     y: int = Field(alias="y")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_reactor.py` & `spacetraders-0.5.0/spacetraders/models/ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_refine_json_body.py` & `spacetraders-0.5.0/spacetraders/models/ship_refine_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response.py` & `spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py` & `spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py` & `spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py` & `spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_registration.py` & `spacetraders-0.5.0/spacetraders/models/ship_registration.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_requirements.py` & `spacetraders-0.5.0/spacetraders/models/ship_requirements.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/ship_type.py` & `spacetraders-0.5.0/spacetraders/models/ship_type.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/shipyard.py` & `spacetraders-0.5.0/spacetraders/models/shipyard.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/shipyard_ship.py` & `spacetraders-0.5.0/spacetraders/models/shipyard_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/shipyard_ship_types_item.py` & `spacetraders-0.5.0/spacetraders/models/shipyard_ship_types_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/shipyard_transaction.py` & `spacetraders-0.5.0/spacetraders/models/shipyard_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/survey.py` & `spacetraders-0.5.0/spacetraders/models/survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/survey_deposit.py` & `spacetraders-0.5.0/spacetraders/models/system_faction.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,22 +5,21 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="SurveyDeposit")
+T = TypeVar("T", bound="SystemFaction")
 
 
-class SurveyDeposit(BaseModel):
-    """A surveyed deposit of a mineral or resource available for extraction.
-
+class SystemFaction(BaseModel):
+    """
     Attributes:
-        symbol (str): The symbol of the deposit.
+        symbol (str):
     """
 
     symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `spacetraders-0.4.0/spacetraders/models/system.py` & `spacetraders-0.5.0/spacetraders/models/system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/system_faction.py` & `spacetraders-0.5.0/spacetraders/models/warp_ship_json_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,24 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="SystemFaction")
+T = TypeVar("T", bound="WarpShipJsonBody")
 
 
-class SystemFaction(BaseModel):
+class WarpShipJsonBody(BaseModel):
     """
     Attributes:
-        symbol (str):
+        waypoint_symbol (str): The target destination.
     """
 
-    symbol: str = Field(alias="symbol")
+    waypoint_symbol: str = Field(alias="waypointSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/system_waypoint.py` & `spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,33 +3,30 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.waypoint_type import WaypointType
 from ..types import Unset
 
-T = TypeVar("T", bound="SystemWaypoint")
+T = TypeVar("T", bound="TransferCargoTransferCargoRequest")
 
 
-class SystemWaypoint(BaseModel):
+class TransferCargoTransferCargoRequest(BaseModel):
     """
     Attributes:
-        symbol (str):
-        type (WaypointType): The type of waypoint.
-        x (int):
-        y (int):
+        trade_symbol (str):
+        units (int):
+        ship_symbol (str):
     """
 
-    symbol: str = Field(alias="symbol")
-    type: WaypointType = Field(alias="type")
-    x: int = Field(alias="x")
-    y: int = Field(alias="y")
+    trade_symbol: str = Field(alias="tradeSymbol")
+    units: int = Field(alias="units")
+    ship_symbol: str = Field(alias="shipSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/trade_good.py` & `spacetraders-0.5.0/spacetraders/models/trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/trade_symbol.py` & `spacetraders-0.5.0/spacetraders/models/trade_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py` & `spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py` & `spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py` & `spacetraders-0.5.0/spacetraders/models/get_status_response_200_stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,30 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="TransferCargoTransferCargoRequest")
+T = TypeVar("T", bound="GetStatusResponse200Stats")
 
 
-class TransferCargoTransferCargoRequest(BaseModel):
+class GetStatusResponse200Stats(BaseModel):
     """
     Attributes:
-        trade_symbol (str):
-        units (int):
-        ship_symbol (str):
+        agents (int):
+        ships (int):
+        systems (int):
+        waypoints (int):
     """
 
-    trade_symbol: str = Field(alias="tradeSymbol")
-    units: int = Field(alias="units")
-    ship_symbol: str = Field(alias="shipSymbol")
+    agents: int = Field(alias="agents")
+    ships: int = Field(alias="ships")
+    systems: int = Field(alias="systems")
+    waypoints: int = Field(alias="waypoints")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/warp_ship_json_body.py` & `spacetraders-0.5.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,26 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="WarpShipJsonBody")
+T = TypeVar("T", bound="GetStatusResponse200LeaderboardsMostCreditsItem")
 
 
-class WarpShipJsonBody(BaseModel):
+class GetStatusResponse200LeaderboardsMostCreditsItem(BaseModel):
     """
     Attributes:
-        waypoint_symbol (str): The target destination.
+        agent_symbol (str):
+        credits_ (int):
     """
 
-    waypoint_symbol: str = Field(alias="waypointSymbol")
+    agent_symbol: str = Field(alias="agentSymbol")
+    credits_: int = Field(alias="credits")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/warp_ship_response_200.py` & `spacetraders-0.5.0/spacetraders/models/warp_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/warp_ship_response_200_data.py` & `spacetraders-0.5.0/spacetraders/models/waypoint_trait.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,31 +3,31 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.ship_fuel import ShipFuel
-from ..models.ship_nav import ShipNav
+from ..models.waypoint_trait_symbol import WaypointTraitSymbol
 from ..types import Unset
 
-T = TypeVar("T", bound="WarpShipResponse200Data")
+T = TypeVar("T", bound="WaypointTrait")
 
 
-class WarpShipResponse200Data(BaseModel):
+class WaypointTrait(BaseModel):
     """
     Attributes:
-        fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
-            or action.
-        nav (ShipNav): The navigation information of the ship.
+        symbol (WaypointTraitSymbol): The unique identifier of the trait.
+        name (str): The name of the trait.
+        description (str): A description of the trait.
     """
 
-    fuel: "ShipFuel" = Field(alias="fuel")
-    nav: "ShipNav" = Field(alias="nav")
+    symbol: WaypointTraitSymbol = Field(alias="symbol")
+    name: str = Field(alias="name")
+    description: str = Field(alias="description")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/waypoint.py` & `spacetraders-0.5.0/spacetraders/models/waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/models/waypoint_faction.py` & `spacetraders-0.5.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,26 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="WaypointFaction")
+T = TypeVar("T", bound="GetStatusResponse200LeaderboardsMostSubmittedChartsItem")
 
 
-class WaypointFaction(BaseModel):
+class GetStatusResponse200LeaderboardsMostSubmittedChartsItem(BaseModel):
     """
     Attributes:
-        symbol (str):
+        agent_symbol (str):
+        chart_count (int):
     """
 
-    symbol: str = Field(alias="symbol")
+    agent_symbol: str = Field(alias="agentSymbol")
+    chart_count: int = Field(alias="chartCount")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/waypoint_orbital.py` & `spacetraders-0.5.0/spacetraders/models/get_status_response_200_server_resets.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,25 +5,26 @@
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
 from ..types import Unset
 
-T = TypeVar("T", bound="WaypointOrbital")
+T = TypeVar("T", bound="GetStatusResponse200ServerResets")
 
 
-class WaypointOrbital(BaseModel):
-    """An orbital is another waypoint that orbits a parent waypoint.
-
+class GetStatusResponse200ServerResets(BaseModel):
+    """
     Attributes:
-        symbol (str):
+        next_ (str): The date and time when the game server will reset.
+        frequency (str): How often we intend to reset the game server.
     """
 
-    symbol: str = Field(alias="symbol")
+    next_: str = Field(alias="next")
+    frequency: str = Field(alias="frequency")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/waypoint_trait.py` & `spacetraders-0.5.0/spacetraders/models/faction.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,31 +3,37 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.waypoint_trait_symbol import WaypointTraitSymbol
+from ..models.faction_trait import FactionTrait
 from ..types import Unset
 
-T = TypeVar("T", bound="WaypointTrait")
+T = TypeVar("T", bound="Faction")
 
 
-class WaypointTrait(BaseModel):
+class Faction(BaseModel):
     """
     Attributes:
-        symbol (WaypointTraitSymbol): The unique identifier of the trait.
-        name (str): The name of the trait.
-        description (str): A description of the trait.
+        symbol (str):
+        name (str):
+        description (str):
+        headquarters (str):
+        traits (List['FactionTrait']):
+        is_recruiting (bool): Whether or not the faction is currently recruiting new agents.
     """
 
-    symbol: WaypointTraitSymbol = Field(alias="symbol")
+    symbol: str = Field(alias="symbol")
     name: str = Field(alias="name")
     description: str = Field(alias="description")
+    headquarters: str = Field(alias="headquarters")
+    traits: List["FactionTrait"] = Field(alias="traits")
+    is_recruiting: bool = Field(alias="isRecruiting")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.4.0/spacetraders/models/waypoint_trait_symbol.py` & `spacetraders-0.5.0/spacetraders/models/waypoint_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/spacetraders/types.py` & `spacetraders-0.5.0/spacetraders/types.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.4.0/PKG-INFO` & `spacetraders-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetraders
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python API for Space Traders
 License: Apache-2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

