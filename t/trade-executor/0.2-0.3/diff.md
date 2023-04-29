# Comparing `tmp/trade_executor-0.2.tar.gz` & `tmp/trade_executor-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trade_executor-0.2.tar", max compression
+gzip compressed data, was "trade_executor-0.3.tar", max compression
```

## Comparing `trade_executor-0.2.tar` & `trade_executor-0.3.tar`

### file list

```diff
@@ -1,126 +1,190 @@
--rw-r--r--   0        0        0      710 2022-09-17 18:24:10.572197 trade_executor-0.2/LICENSE.txt
--rw-r--r--   0        0        0     1981 2022-11-25 17:45:04.518105 trade_executor-0.2/README.md
--rw-r--r--   0        0        0     3792 2022-11-28 09:47:08.852763 trade_executor-0.2/pyproject.toml
--rw-r--r--   0        0        0       97 2022-09-17 18:24:10.606247 trade_executor-0.2/tradeexecutor/__init__.py
--rw-r--r--   0        0        0       41 2022-09-17 18:24:10.606327 trade_executor-0.2/tradeexecutor/analysis/__init__.py
--rw-r--r--   0        0        0    28800 2022-11-27 13:41:03.992838 trade_executor-0.2/tradeexecutor/analysis/trade_analyser.py
--rw-r--r--   0        0        0       25 2022-09-17 18:24:10.606561 trade_executor-0.2/tradeexecutor/backtest/__init__.py
--rw-r--r--   0        0        0     6809 2022-11-18 13:52:33.056824 trade_executor-0.2/tradeexecutor/backtest/backtest_execution.py
--rw-r--r--   0        0        0     5814 2022-11-25 17:30:18.071927 trade_executor-0.2/tradeexecutor/backtest/backtest_pricing.py
--rw-r--r--   0        0        0    12163 2022-09-17 18:24:10.606870 trade_executor-0.2/tradeexecutor/backtest/backtest_routing.py
--rw-r--r--   0        0        0    17714 2022-11-25 11:55:17.980323 trade_executor-0.2/tradeexecutor/backtest/backtest_runner.py
--rw-r--r--   0        0        0     1707 2022-11-25 08:55:40.766235 trade_executor-0.2/tradeexecutor/backtest/backtest_sync.py
--rw-r--r--   0        0        0     1329 2022-11-25 17:30:18.072125 trade_executor-0.2/tradeexecutor/backtest/backtest_valuation.py
--rw-r--r--   0        0        0     1348 2022-11-25 08:55:40.766380 trade_executor-0.2/tradeexecutor/backtest/data_preload.py
--rw-r--r--   0        0        0     1340 2022-09-17 18:24:10.607253 trade_executor-0.2/tradeexecutor/backtest/simulated_wallet.py
--rw-r--r--   0        0        0       32 2022-09-17 18:24:10.607338 trade_executor-0.2/tradeexecutor/cli/__init__.py
--rw-r--r--   0        0        0     2861 2022-09-17 18:24:10.607406 trade_executor-0.2/tradeexecutor/cli/approval.py
--rw-r--r--   0        0        0     7891 2022-09-17 18:24:10.607491 trade_executor-0.2/tradeexecutor/cli/discord_handler.py
--rw-r--r--   0        0        0      948 2022-09-27 22:04:00.138372 trade_executor-0.2/tradeexecutor/cli/env.py
--rwxr-xr-x   0        0        0     1019 2022-09-27 22:04:00.138432 trade_executor-0.2/tradeexecutor/cli/latest_release.py
--rw-r--r--   0        0        0     6676 2022-11-27 21:50:07.792106 trade_executor-0.2/tradeexecutor/cli/log.py
--rw-r--r--   0        0        0    25034 2022-11-28 09:47:39.662057 trade_executor-0.2/tradeexecutor/cli/loop.py
--rw-r--r--   0        0        0    35869 2022-11-28 07:51:22.436900 trade_executor-0.2/tradeexecutor/cli/main.py
--rw-r--r--   0        0        0     3776 2022-11-27 21:08:34.143842 trade_executor-0.2/tradeexecutor/cli/prepare_docker_env.py
--rw-r--r--   0        0        0      419 2022-11-25 08:55:40.767818 trade_executor-0.2/tradeexecutor/cli/result.py
--rw-r--r--   0        0        0     3885 2022-11-27 21:08:34.144004 trade_executor-0.2/tradeexecutor/cli/testtrade.py
--rw-r--r--   0        0        0      301 2022-09-17 18:24:10.608046 trade_executor-0.2/tradeexecutor/ethereum/__init__.py
--rw-r--r--   0        0        0   564330 2022-09-17 18:24:10.608984 trade_executor-0.2/tradeexecutor/ethereum/abi/uniswap/erc20.json
--rw-r--r--   0        0        0     7715 2022-09-17 18:24:10.609069 trade_executor-0.2/tradeexecutor/ethereum/abi/uniswap/factory.json
--rw-r--r--   0        0        0    29729 2022-09-17 18:24:10.609167 trade_executor-0.2/tradeexecutor/ethereum/abi/uniswap/pair.json
--rw-r--r--   0        0        0    14169 2022-09-17 18:24:10.609252 trade_executor-0.2/tradeexecutor/ethereum/abi/uniswap/uniswap_erc20.json
--rw-r--r--   0        0        0     4725 2022-11-26 12:40:47.994129 trade_executor-0.2/tradeexecutor/ethereum/default_routes.py
--rw-r--r--   0        0        0    17854 2022-11-25 08:55:40.768463 trade_executor-0.2/tradeexecutor/ethereum/execution.py
--rw-r--r--   0        0        0     1180 2022-11-27 21:08:34.144336 trade_executor-0.2/tradeexecutor/ethereum/hot_wallet_sync.py
--rw-r--r--   0        0        0     6662 2022-11-27 21:08:34.144642 trade_executor-0.2/tradeexecutor/ethereum/tx.py
--rw-r--r--   0        0        0     4786 2022-11-26 12:40:47.994333 trade_executor-0.2/tradeexecutor/ethereum/uniswap_v2_execution.py
--rw-r--r--   0        0        0     8367 2022-10-14 08:35:46.843062 trade_executor-0.2/tradeexecutor/ethereum/uniswap_v2_execution_v0.py
--rw-r--r--   0        0        0     7217 2022-09-27 22:04:00.139234 trade_executor-0.2/tradeexecutor/ethereum/uniswap_v2_live_pricing.py
--rw-r--r--   0        0        0    25909 2022-11-26 12:40:47.994635 trade_executor-0.2/tradeexecutor/ethereum/uniswap_v2_routing.py
--rw-r--r--   0        0        0     1656 2022-09-17 18:24:10.610205 trade_executor-0.2/tradeexecutor/ethereum/uniswap_v2_valuation.py
--rw-r--r--   0        0        0     1564 2022-09-17 18:24:10.610274 trade_executor-0.2/tradeexecutor/ethereum/uniswap_v2_valuation_v0.py
--rw-r--r--   0        0        0     2443 2022-10-04 09:12:05.546281 trade_executor-0.2/tradeexecutor/ethereum/universe.py
--rw-r--r--   0        0        0     2945 2022-09-17 18:24:10.610420 trade_executor-0.2/tradeexecutor/ethereum/wallet.py
--rw-r--r--   0        0        0     6227 2022-11-27 21:08:34.144898 trade_executor-0.2/tradeexecutor/ethereum/web3config.py
--rw-r--r--   0        0        0       52 2022-09-17 18:24:10.610503 trade_executor-0.2/tradeexecutor/monkeypatch/__init__.py
--rw-r--r--   0        0        0     1169 2022-09-17 18:24:10.610582 trade_executor-0.2/tradeexecutor/monkeypatch/dataclasses_json.py
--rw-r--r--   0        0        0      786 2022-09-17 18:24:10.610676 trade_executor-0.2/tradeexecutor/state/__init__.py
--rw-r--r--   0        0        0     6550 2022-10-25 09:30:48.069731 trade_executor-0.2/tradeexecutor/state/blockhain_transaction.py
--rw-r--r--   0        0        0     1627 2022-09-17 18:24:10.610832 trade_executor-0.2/tradeexecutor/state/freeze.py
--rw-r--r--   0        0        0     4962 2022-09-27 22:04:00.139345 trade_executor-0.2/tradeexecutor/state/identifier.py
--rw-r--r--   0        0        0      897 2022-09-17 18:24:10.610965 trade_executor-0.2/tradeexecutor/state/metadata.py
--rw-r--r--   0        0        0    16885 2022-11-27 21:08:34.145350 trade_executor-0.2/tradeexecutor/state/portfolio.py
--rw-r--r--   0        0        0    16621 2022-11-27 21:08:34.145746 trade_executor-0.2/tradeexecutor/state/position.py
--rw-r--r--   0        0        0     1748 2022-09-17 18:24:10.611223 trade_executor-0.2/tradeexecutor/state/reserve.py
--rw-r--r--   0        0        0      494 2022-09-17 18:24:10.611273 trade_executor-0.2/tradeexecutor/state/revaluation.py
--rw-r--r--   0        0        0     9309 2022-11-27 21:08:34.145990 trade_executor-0.2/tradeexecutor/state/state.py
--rw-r--r--   0        0        0     4680 2022-11-28 09:47:39.662886 trade_executor-0.2/tradeexecutor/state/statistics.py
--rw-r--r--   0        0        0     3610 2022-11-25 17:30:18.074219 trade_executor-0.2/tradeexecutor/state/store.py
--rw-r--r--   0        0        0     1736 2022-09-17 18:24:10.611663 trade_executor-0.2/tradeexecutor/state/sync.py
--rw-r--r--   0        0        0    14610 2022-11-27 21:08:34.146242 trade_executor-0.2/tradeexecutor/state/trade.py
--rw-r--r--   0        0        0     1085 2022-09-17 18:24:10.611820 trade_executor-0.2/tradeexecutor/state/types.py
--rw-r--r--   0        0        0     2836 2022-11-27 13:41:03.993224 trade_executor-0.2/tradeexecutor/state/validator.py
--rw-r--r--   0        0        0     4376 2022-11-27 13:02:58.437065 trade_executor-0.2/tradeexecutor/state/visualisation.py
--rw-r--r--   0        0        0     4856 2022-11-28 09:47:39.663919 trade_executor-0.2/tradeexecutor/statistics/core.py
--rw-r--r--   0        0        0      493 2022-09-17 18:24:10.612058 trade_executor-0.2/tradeexecutor/strategy/__init__.py
--rw-r--r--   0        0        0     1590 2022-09-17 18:24:10.612123 trade_executor-0.2/tradeexecutor/strategy/approval.py
--rw-r--r--   0        0        0     4846 2022-11-25 11:55:17.981100 trade_executor-0.2/tradeexecutor/strategy/bootstrap.py
--rw-r--r--   0        0        0     5729 2022-11-25 17:55:22.846017 trade_executor-0.2/tradeexecutor/strategy/cycle.py
--rw-r--r--   0        0        0     1553 2022-11-26 12:40:47.994923 trade_executor-0.2/tradeexecutor/strategy/default_routing_options.py
--rw-r--r--   0        0        0     1536 2022-11-25 08:55:40.770669 trade_executor-0.2/tradeexecutor/strategy/description.py
--rw-r--r--   0        0        0      403 2022-09-17 18:24:10.612429 trade_executor-0.2/tradeexecutor/strategy/dummy.py
--rw-r--r--   0        0        0     3642 2022-11-28 09:47:39.664289 trade_executor-0.2/tradeexecutor/strategy/execution_context.py
--rw-r--r--   0        0        0     3975 2022-11-27 21:08:34.146467 trade_executor-0.2/tradeexecutor/strategy/execution_model.py
--rw-r--r--   0        0        0     1980 2022-11-25 11:55:17.981391 trade_executor-0.2/tradeexecutor/strategy/factory.py
--rw-r--r--   0        0        0     3811 2022-09-17 18:24:10.612722 trade_executor-0.2/tradeexecutor/strategy/output.py
--rw-r--r--   0        0        0       92 2022-09-17 18:24:10.612799 trade_executor-0.2/tradeexecutor/strategy/pandas_trader/__init__.py
--rw-r--r--   0        0        0    15166 2022-11-27 21:08:34.146693 trade_executor-0.2/tradeexecutor/strategy/pandas_trader/position_manager.py
--rw-r--r--   0        0        0     4912 2022-09-27 22:04:00.140815 trade_executor-0.2/tradeexecutor/strategy/pandas_trader/rebalance.py
--rw-r--r--   0        0        0     2851 2022-09-17 18:24:10.613053 trade_executor-0.2/tradeexecutor/strategy/pandas_trader/runner.py
--rw-r--r--   0        0        0     1986 2022-09-17 18:24:10.613123 trade_executor-0.2/tradeexecutor/strategy/pandas_trader/trade_decision.py
--rw-r--r--   0        0        0     2804 2022-09-17 18:24:10.613184 trade_executor-0.2/tradeexecutor/strategy/pricing_model.py
--rw-r--r--   0        0        0      345 2022-09-27 22:04:00.141002 trade_executor-0.2/tradeexecutor/strategy/qstrader/__init__.py
--rw-r--r--   0        0        0      872 2022-09-17 18:24:10.613322 trade_executor-0.2/tradeexecutor/strategy/qstrader/alpha_model.py
--rw-r--r--   0        0        0     6943 2022-09-17 18:24:10.613405 trade_executor-0.2/tradeexecutor/strategy/qstrader/order_sizer.py
--rw-r--r--   0        0        0    11319 2022-11-25 17:30:18.074950 trade_executor-0.2/tradeexecutor/strategy/qstrader/portfolio_construction_model.py
--rw-r--r--   0        0        0     7282 2022-09-17 18:24:10.613548 trade_executor-0.2/tradeexecutor/strategy/qstrader/runner.py
--rw-r--r--   0        0        0      484 2022-09-17 18:24:10.613604 trade_executor-0.2/tradeexecutor/strategy/reserve_currency.py
--rw-r--r--   0        0        0     2988 2022-11-26 12:40:47.995250 trade_executor-0.2/tradeexecutor/strategy/routing.py
--rw-r--r--   0        0        0    15405 2022-11-25 08:55:40.771440 trade_executor-0.2/tradeexecutor/strategy/runner.py
--rw-r--r--   0        0        0     2323 2022-11-25 08:55:40.771706 trade_executor-0.2/tradeexecutor/strategy/stoploss.py
--rw-r--r--   0        0        0    15906 2022-11-25 17:30:18.075245 trade_executor-0.2/tradeexecutor/strategy/strategy_module.py
--rw-r--r--   0        0        0      805 2022-09-17 18:24:10.613980 trade_executor-0.2/tradeexecutor/strategy/strategy_type.py
--rw-r--r--   0        0        0    35559 2022-11-25 08:55:40.772391 trade_executor-0.2/tradeexecutor/strategy/trading_strategy_universe.py
--rw-r--r--   0        0        0     4656 2022-11-27 21:08:34.146971 trade_executor-0.2/tradeexecutor/strategy/universe_model.py
--rw-r--r--   0        0        0     1937 2022-11-25 17:30:18.075410 trade_executor-0.2/tradeexecutor/strategy/valuation.py
--rw-r--r--   0        0        0       27 2022-09-17 18:24:10.614374 trade_executor-0.2/tradeexecutor/testing/__init__.py
--rw-r--r--   0        0        0     4508 2022-09-17 18:24:10.614437 trade_executor-0.2/tradeexecutor/testing/backtest_trader.py
--rw-r--r--   0        0        0     3831 2022-09-17 18:24:10.614506 trade_executor-0.2/tradeexecutor/testing/dummy_trader.py
--rw-r--r--   0        0        0     6214 2022-09-17 18:24:10.614578 trade_executor-0.2/tradeexecutor/testing/ethereumtrader.py
--rw-r--r--   0        0        0     1729 2022-09-27 22:04:00.141899 trade_executor-0.2/tradeexecutor/testing/pairuniversetrader.py
--rw-r--r--   0        0        0     4327 2022-11-03 19:58:38.021311 trade_executor-0.2/tradeexecutor/testing/simulated_execution_loop.py
--rw-r--r--   0        0        0     3020 2022-09-27 22:04:00.141960 trade_executor-0.2/tradeexecutor/testing/simulated_trader.py
--rw-r--r--   0        0        0      251 2022-09-17 18:24:10.614799 trade_executor-0.2/tradeexecutor/testing/synthetic_ethereum_data.py
--rw-r--r--   0        0        0     2150 2022-09-27 22:04:00.142060 trade_executor-0.2/tradeexecutor/testing/synthetic_exchange_data.py
--rw-r--r--   0        0        0     3528 2022-09-27 22:04:00.142154 trade_executor-0.2/tradeexecutor/testing/synthetic_price_data.py
--rw-r--r--   0        0        0       53 2022-09-17 18:24:10.614999 trade_executor-0.2/tradeexecutor/utils/__init__.py
--rw-r--r--   0        0        0      522 2022-11-03 19:58:38.021547 trade_executor-0.2/tradeexecutor/utils/blockchain.py
--rw-r--r--   0        0        0      397 2022-09-17 18:24:10.615052 trade_executor-0.2/tradeexecutor/utils/dataclass.py
--rw-r--r--   0        0        0      296 2022-09-27 22:04:00.142204 trade_executor-0.2/tradeexecutor/utils/format.py
--rw-r--r--   0        0        0      305 2022-11-26 12:40:47.995503 trade_executor-0.2/tradeexecutor/utils/fullname.py
--rw-r--r--   0        0        0      423 2022-09-17 18:24:10.615153 trade_executor-0.2/tradeexecutor/utils/price.py
--rw-r--r--   0        0        0      823 2022-09-17 18:24:10.615210 trade_executor-0.2/tradeexecutor/utils/timer.py
--rw-r--r--   0        0        0     1533 2022-11-27 13:49:33.281955 trade_executor-0.2/tradeexecutor/utils/timestamp.py
--rw-r--r--   0        0        0       52 2022-09-27 22:04:00.142342 trade_executor-0.2/tradeexecutor/utils/typing.py
--rw-r--r--   0        0        0      937 2022-11-25 08:55:40.772781 trade_executor-0.2/tradeexecutor/utils/url.py
--rw-r--r--   0        0        0       40 2022-09-17 18:24:10.615462 trade_executor-0.2/tradeexecutor/visual/__init__.py
--rw-r--r--   0        0        0     4698 2022-11-18 14:00:02.999857 trade_executor-0.2/tradeexecutor/visual/benchmark.py
--rw-r--r--   0        0        0    10037 2022-11-26 12:40:47.995978 trade_executor-0.2/tradeexecutor/visual/single_pair.py
--rw-r--r--   0        0        0       41 2022-09-17 18:24:10.615753 trade_executor-0.2/tradeexecutor/webhook/__init__.py
--rw-r--r--   0        0        0     2347 2022-11-25 08:55:40.773012 trade_executor-0.2/tradeexecutor/webhook/api.py
--rw-r--r--   0        0        0     4495 2022-11-21 12:02:46.391603 trade_executor-0.2/tradeexecutor/webhook/app.py
--rw-r--r--   0        0        0     2102 2022-09-17 18:24:10.615966 trade_executor-0.2/tradeexecutor/webhook/error.py
--rw-r--r--   0        0        0      580 2022-09-17 18:24:10.616036 trade_executor-0.2/tradeexecutor/webhook/events.py
--rw-r--r--   0        0        0     2281 2022-09-17 18:24:10.616128 trade_executor-0.2/tradeexecutor/webhook/server.py
--rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 trade_executor-0.2/setup.py
--rw-r--r--   0        0        0     4038 1970-01-01 00:00:00.000000 trade_executor-0.2/PKG-INFO
+-rw-r--r--   0        0        0      710 2022-09-17 18:24:10.572197 trade_executor-0.3/LICENSE.txt
+-rw-r--r--   0        0        0     3567 2023-04-29 18:51:35.713290 trade_executor-0.3/README.md
+-rw-r--r--   0        0        0     4325 2023-04-29 18:52:03.816004 trade_executor-0.3/pyproject.toml
+-rw-r--r--   0        0        0       97 2022-09-17 18:24:10.606247 trade_executor-0.3/tradeexecutor/__init__.py
+-rw-r--r--   0        0        0       41 2022-09-17 18:24:10.606327 trade_executor-0.3/tradeexecutor/analysis/__init__.py
+-rw-r--r--   0        0        0    13177 2023-04-18 22:44:56.796954 trade_executor-0.3/tradeexecutor/analysis/alpha_model_analyser.py
+-rw-r--r--   0        0        0     2397 2023-04-18 22:44:56.797137 trade_executor-0.3/tradeexecutor/analysis/fee_analyser.py
+-rw-r--r--   0        0        0     3453 2023-04-26 10:26:00.672498 trade_executor-0.3/tradeexecutor/analysis/multipair.py
+-rw-r--r--   0        0        0    34698 2023-04-27 14:18:53.814254 trade_executor-0.3/tradeexecutor/analysis/trade_analyser.py
+-rw-r--r--   0        0        0       25 2022-09-17 18:24:10.606561 trade_executor-0.3/tradeexecutor/backtest/__init__.py
+-rw-r--r--   0        0        0    10490 2023-03-01 15:19:10.070659 trade_executor-0.3/tradeexecutor/backtest/backtest_execution.py
+-rw-r--r--   0        0        0     9676 2023-04-19 08:31:31.383285 trade_executor-0.3/tradeexecutor/backtest/backtest_pricing.py
+-rw-r--r--   0        0        0     8770 2023-03-27 22:48:02.291644 trade_executor-0.3/tradeexecutor/backtest/backtest_routing.py
+-rw-r--r--   0        0        0    21150 2023-04-18 22:44:56.797973 trade_executor-0.3/tradeexecutor/backtest/backtest_runner.py
+-rw-r--r--   0        0        0     4160 2023-04-17 20:22:44.629814 trade_executor-0.3/tradeexecutor/backtest/backtest_sync.py
+-rw-r--r--   0        0        0     1295 2023-04-17 20:22:44.630044 trade_executor-0.3/tradeexecutor/backtest/backtest_valuation.py
+-rw-r--r--   0        0        0     1624 2023-04-17 20:22:44.630303 trade_executor-0.3/tradeexecutor/backtest/data_preload.py
+-rw-r--r--   0        0        0     6116 2023-04-29 18:17:15.959752 trade_executor-0.3/tradeexecutor/backtest/grid_search.py
+-rw-r--r--   0        0        0     1286 2023-04-29 13:51:44.486537 trade_executor-0.3/tradeexecutor/backtest/notebook.py
+-rw-r--r--   0        0        0     1340 2022-09-17 18:24:10.607253 trade_executor-0.3/tradeexecutor/backtest/simulated_wallet.py
+-rw-r--r--   0        0        0       32 2022-09-17 18:24:10.607338 trade_executor-0.3/tradeexecutor/cli/__init__.py
+-rw-r--r--   0        0        0     2861 2022-09-17 18:24:10.607406 trade_executor-0.3/tradeexecutor/cli/approval.py
+-rw-r--r--   0        0        0     8941 2023-04-17 20:22:44.630559 trade_executor-0.3/tradeexecutor/cli/bootstrap.py
+-rw-r--r--   0        0        0       42 2023-02-11 09:28:14.539908 trade_executor-0.3/tradeexecutor/cli/commands/__init__.py
+-rw-r--r--   0        0        0      708 2023-04-17 20:22:44.630840 trade_executor-0.3/tradeexecutor/cli/commands/app.py
+-rw-r--r--   0        0        0     3243 2023-04-17 20:22:44.631010 trade_executor-0.3/tradeexecutor/cli/commands/check_universe.py
+-rw-r--r--   0        0        0     7823 2023-04-17 20:22:44.631276 trade_executor-0.3/tradeexecutor/cli/commands/check_wallet.py
+-rw-r--r--   0        0        0     8236 2023-04-17 20:22:44.631560 trade_executor-0.3/tradeexecutor/cli/commands/console.py
+-rw-r--r--   0        0        0     4603 2023-04-23 21:04:11.835267 trade_executor-0.3/tradeexecutor/cli/commands/enzyme_asset_list.py
+-rw-r--r--   0        0        0     6016 2023-04-27 14:18:53.814491 trade_executor-0.3/tradeexecutor/cli/commands/enzyme_deploy_vault.py
+-rw-r--r--   0        0        0      174 2023-02-11 09:28:14.541002 trade_executor-0.3/tradeexecutor/cli/commands/hello.py
+-rw-r--r--   0        0        0     3501 2023-04-17 20:22:44.631707 trade_executor-0.3/tradeexecutor/cli/commands/init.py
+-rw-r--r--   0        0        0     5600 2023-04-17 20:22:44.632017 trade_executor-0.3/tradeexecutor/cli/commands/perform_test_trade.py
+-rw-r--r--   0        0        0     5663 2023-04-17 20:22:44.632283 trade_executor-0.3/tradeexecutor/cli/commands/repair.py
+-rw-r--r--   0        0        0     2490 2023-04-17 20:22:44.632468 trade_executor-0.3/tradeexecutor/cli/commands/shared_options.py
+-rw-r--r--   0        0        0    22014 2023-04-17 20:22:44.632768 trade_executor-0.3/tradeexecutor/cli/commands/start.py
+-rw-r--r--   0        0        0      503 2023-04-27 14:18:53.814711 trade_executor-0.3/tradeexecutor/cli/commands/version.py
+-rw-r--r--   0        0        0     1666 2023-02-11 09:28:14.542248 trade_executor-0.3/tradeexecutor/cli/discord.py
+-rw-r--r--   0        0        0      949 2023-04-05 19:42:46.629653 trade_executor-0.3/tradeexecutor/cli/env.py
+-rwxr-xr-x   0        0        0     1019 2022-09-27 22:04:00.138432 trade_executor-0.3/tradeexecutor/cli/latest_release.py
+-rw-r--r--   0        0        0     8184 2023-04-17 20:22:44.633035 trade_executor-0.3/tradeexecutor/cli/log.py
+-rw-r--r--   0        0        0    39180 2023-04-18 22:44:56.798314 trade_executor-0.3/tradeexecutor/cli/loop.py
+-rw-r--r--   0        0        0      802 2023-04-27 14:18:53.814892 trade_executor-0.3/tradeexecutor/cli/main.py
+-rw-r--r--   0        0        0      419 2023-02-11 09:28:14.543579 trade_executor-0.3/tradeexecutor/cli/result.py
+-rw-r--r--   0        0        0     3890 2023-04-17 20:22:44.633896 trade_executor-0.3/tradeexecutor/cli/testtrade.py
+-rw-r--r--   0        0        0     1443 2023-02-11 09:28:14.543960 trade_executor-0.3/tradeexecutor/cli/version_info.py
+-rw-r--r--   0        0        0     5865 2023-02-11 09:28:14.544139 trade_executor-0.3/tradeexecutor/cli/watchdog.py
+-rw-r--r--   0        0        0      301 2022-09-17 18:24:10.608046 trade_executor-0.3/tradeexecutor/ethereum/__init__.py
+-rw-r--r--   0        0        0   564330 2022-09-17 18:24:10.608984 trade_executor-0.3/tradeexecutor/ethereum/abi/uniswap/erc20.json
+-rw-r--r--   0        0        0     7715 2022-09-17 18:24:10.609069 trade_executor-0.3/tradeexecutor/ethereum/abi/uniswap/factory.json
+-rw-r--r--   0        0        0    29729 2022-09-17 18:24:10.609167 trade_executor-0.3/tradeexecutor/ethereum/abi/uniswap/pair.json
+-rw-r--r--   0        0        0    14169 2022-09-17 18:24:10.609252 trade_executor-0.3/tradeexecutor/ethereum/abi/uniswap/uniswap_erc20.json
+-rw-r--r--   0        0        0       33 2023-04-03 10:43:31.167215 trade_executor-0.3/tradeexecutor/ethereum/enzyme/__init__.py
+-rw-r--r--   0        0        0     3830 2023-04-26 10:26:00.673243 trade_executor-0.3/tradeexecutor/ethereum/enzyme/asset.py
+-rw-r--r--   0        0        0    22496 2023-04-26 10:26:00.673462 trade_executor-0.3/tradeexecutor/ethereum/enzyme/polygon_assets.json
+-rw-r--r--   0        0        0     5037 2023-04-17 20:22:44.634137 trade_executor-0.3/tradeexecutor/ethereum/enzyme/tx.py
+-rw-r--r--   0        0        0    14261 2023-04-17 20:22:44.634412 trade_executor-0.3/tradeexecutor/ethereum/enzyme/vault.py
+-rw-r--r--   0        0        0     7167 2023-02-20 22:42:50.588911 trade_executor-0.3/tradeexecutor/ethereum/eth_pricing_model.py
+-rw-r--r--   0        0        0     1933 2023-02-20 22:42:50.589011 trade_executor-0.3/tradeexecutor/ethereum/eth_valuation.py
+-rw-r--r--   0        0        0     2786 2023-04-17 20:22:44.634643 trade_executor-0.3/tradeexecutor/ethereum/ethereumtrader.py
+-rw-r--r--   0        0        0    30773 2023-04-17 20:22:44.634977 trade_executor-0.3/tradeexecutor/ethereum/execution.py
+-rw-r--r--   0        0        0     3309 2023-04-17 20:22:44.635211 trade_executor-0.3/tradeexecutor/ethereum/hot_wallet_sync_model.py
+-rw-r--r--   0        0        0    30228 2023-04-17 20:22:44.635510 trade_executor-0.3/tradeexecutor/ethereum/routing_data.py
+-rw-r--r--   0        0        0    16356 2023-04-17 20:22:44.635780 trade_executor-0.3/tradeexecutor/ethereum/routing_model.py
+-rw-r--r--   0        0        0    11490 2023-04-05 15:52:50.981652 trade_executor-0.3/tradeexecutor/ethereum/routing_state.py
+-rw-r--r--   0        0        0     1076 2023-04-03 10:43:31.167817 trade_executor-0.3/tradeexecutor/ethereum/token.py
+-rw-r--r--   0        0        0    10349 2023-04-17 20:22:44.636035 trade_executor-0.3/tradeexecutor/ethereum/tx.py
+-rw-r--r--   0        0        0        0 2023-04-17 20:22:44.636079 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v2/__init__.py
+-rw-r--r--   0        0        0     3756 2023-04-17 20:22:44.636329 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v2/uniswap_v2_execution.py
+-rw-r--r--   0        0        0    13652 2023-04-17 20:22:44.636543 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v2/uniswap_v2_execution_v0.py
+-rw-r--r--   0        0        0     9230 2023-04-17 20:22:44.636776 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v2/uniswap_v2_live_pricing.py
+-rw-r--r--   0        0        0    11949 2023-04-17 20:22:44.636981 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v2/uniswap_v2_routing.py
+-rw-r--r--   0        0        0     1436 2023-04-17 20:22:44.637176 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v2/uniswap_v2_valuation.py
+-rw-r--r--   0        0        0     1484 2023-04-17 20:22:44.637443 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v2/uniswap_v2_valuation_v0.py
+-rw-r--r--   0        0        0        0 2023-04-17 20:22:44.637474 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v3/__init__.py
+-rw-r--r--   0        0        0     3904 2023-04-17 20:22:44.637655 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v3/uniswap_v3_execution.py
+-rw-r--r--   0        0        0     9509 2023-04-17 20:22:44.637831 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v3/uniswap_v3_live_pricing.py
+-rw-r--r--   0        0        0    10352 2023-04-17 20:22:44.638014 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v3/uniswap_v3_routing.py
+-rw-r--r--   0        0        0     1444 2023-04-17 20:22:44.638124 trade_executor-0.3/tradeexecutor/ethereum/uniswap_v3/uniswap_v3_valuation.py
+-rw-r--r--   0        0        0     2711 2023-04-03 10:49:23.985602 trade_executor-0.3/tradeexecutor/ethereum/universe.py
+-rw-r--r--   0        0        0     2949 2023-03-29 23:06:10.369664 trade_executor-0.3/tradeexecutor/ethereum/wallet.py
+-rw-r--r--   0        0        0     7793 2023-04-17 20:22:44.638362 trade_executor-0.3/tradeexecutor/ethereum/web3config.py
+-rw-r--r--   0        0        0       52 2022-09-17 18:24:10.610503 trade_executor-0.3/tradeexecutor/monkeypatch/__init__.py
+-rw-r--r--   0        0        0     2663 2023-03-27 22:48:02.294474 trade_executor-0.3/tradeexecutor/monkeypatch/dataclasses_json.py
+-rw-r--r--   0        0        0     2583 2023-04-27 14:18:53.815057 trade_executor-0.3/tradeexecutor/monkeypatch/web3.py
+-rw-r--r--   0        0        0      786 2022-09-17 18:24:10.610676 trade_executor-0.3/tradeexecutor/state/__init__.py
+-rw-r--r--   0        0        0     3482 2023-04-05 19:42:46.629974 trade_executor-0.3/tradeexecutor/state/balance_update.py
+-rw-r--r--   0        0        0    10094 2023-04-17 20:22:44.638627 trade_executor-0.3/tradeexecutor/state/blockhain_transaction.py
+-rw-r--r--   0        0        0     2605 2023-04-18 22:44:56.798387 trade_executor-0.3/tradeexecutor/state/crossover.py
+-rw-r--r--   0        0        0     1699 2023-03-27 22:48:02.295359 trade_executor-0.3/tradeexecutor/state/freeze.py
+-rw-r--r--   0        0        0     8137 2023-04-03 10:43:31.167973 trade_executor-0.3/tradeexecutor/state/identifier.py
+-rw-r--r--   0        0        0     1273 2023-02-11 09:28:14.548960 trade_executor-0.3/tradeexecutor/state/metadata.py
+-rw-r--r--   0        0        0    26673 2023-04-26 10:26:00.673778 trade_executor-0.3/tradeexecutor/state/portfolio.py
+-rw-r--r--   0        0        0    33798 2023-04-26 10:26:00.674091 trade_executor-0.3/tradeexecutor/state/position.py
+-rw-r--r--   0        0        0     8573 2023-03-27 22:48:02.295812 trade_executor-0.3/tradeexecutor/state/repair.py
+-rw-r--r--   0        0        0     2604 2023-04-05 19:41:43.993823 trade_executor-0.3/tradeexecutor/state/reserve.py
+-rw-r--r--   0        0        0      494 2022-09-17 18:24:10.611273 trade_executor-0.3/tradeexecutor/state/revaluation.py
+-rw-r--r--   0        0        0    15820 2023-04-04 14:26:18.195994 trade_executor-0.3/tradeexecutor/state/state.py
+-rw-r--r--   0        0        0     8370 2023-04-11 10:44:48.563418 trade_executor-0.3/tradeexecutor/state/statistics.py
+-rw-r--r--   0        0        0     4035 2023-02-11 09:28:14.550569 trade_executor-0.3/tradeexecutor/state/store.py
+-rw-r--r--   0        0        0     3599 2023-04-05 19:43:14.740729 trade_executor-0.3/tradeexecutor/state/sync.py
+-rw-r--r--   0        0        0    28466 2023-04-18 22:44:56.799039 trade_executor-0.3/tradeexecutor/state/trade.py
+-rw-r--r--   0        0        0     1507 2023-04-23 21:04:11.835837 trade_executor-0.3/tradeexecutor/state/types.py
+-rw-r--r--   0        0        0     1469 2023-03-27 22:48:02.296336 trade_executor-0.3/tradeexecutor/state/uptime.py
+-rw-r--r--   0        0        0     3631 2023-03-27 22:48:02.296435 trade_executor-0.3/tradeexecutor/state/validator.py
+-rw-r--r--   0        0        0    12481 2023-04-18 22:44:56.799229 trade_executor-0.3/tradeexecutor/state/visualisation.py
+-rw-r--r--   0        0        0     4856 2023-02-11 09:28:14.552334 trade_executor-0.3/tradeexecutor/statistics/core.py
+-rw-r--r--   0        0        0     3578 2023-04-18 22:44:56.799477 trade_executor-0.3/tradeexecutor/statistics/summary.py
+-rw-r--r--   0        0        0      493 2022-09-17 18:24:10.612058 trade_executor-0.3/tradeexecutor/strategy/__init__.py
+-rw-r--r--   0        0        0    22214 2023-04-26 10:26:00.674455 trade_executor-0.3/tradeexecutor/strategy/alpha_model.py
+-rw-r--r--   0        0        0     1590 2022-09-17 18:24:10.612123 trade_executor-0.3/tradeexecutor/strategy/approval.py
+-rw-r--r--   0        0        0     5806 2023-04-17 20:22:44.639974 trade_executor-0.3/tradeexecutor/strategy/bootstrap.py
+-rw-r--r--   0        0        0     6830 2023-04-22 22:02:18.444378 trade_executor-0.3/tradeexecutor/strategy/cycle.py
+-rw-r--r--   0        0        0     5251 2023-02-27 11:44:34.864502 trade_executor-0.3/tradeexecutor/strategy/default_routing_options.py
+-rw-r--r--   0        0        0     1742 2023-02-11 09:28:14.554287 trade_executor-0.3/tradeexecutor/strategy/description.py
+-rw-r--r--   0        0        0     3066 2023-02-11 09:28:14.554588 trade_executor-0.3/tradeexecutor/strategy/dummy.py
+-rw-r--r--   0        0        0     3923 2023-04-17 20:22:44.640344 trade_executor-0.3/tradeexecutor/strategy/execution_context.py
+-rw-r--r--   0        0        0     5231 2023-04-17 20:22:44.640596 trade_executor-0.3/tradeexecutor/strategy/execution_model.py
+-rw-r--r--   0        0        0     2000 2023-04-17 20:22:44.640785 trade_executor-0.3/tradeexecutor/strategy/factory.py
+-rw-r--r--   0        0        0     3815 2023-02-11 09:28:14.555767 trade_executor-0.3/tradeexecutor/strategy/output.py
+-rw-r--r--   0        0        0       92 2022-09-17 18:24:10.612799 trade_executor-0.3/tradeexecutor/strategy/pandas_trader/__init__.py
+-rw-r--r--   0        0        0     9595 2023-02-11 09:28:14.555984 trade_executor-0.3/tradeexecutor/strategy/pandas_trader/decision_trigger.py
+-rw-r--r--   0        0        0    27205 2023-04-26 10:26:00.674779 trade_executor-0.3/tradeexecutor/strategy/pandas_trader/position_manager.py
+-rw-r--r--   0        0        0     4682 2023-04-18 22:44:56.800419 trade_executor-0.3/tradeexecutor/strategy/pandas_trader/rebalance.py
+-rw-r--r--   0        0        0     7476 2023-04-17 20:22:44.641440 trade_executor-0.3/tradeexecutor/strategy/pandas_trader/runner.py
+-rw-r--r--   0        0        0     1986 2022-09-17 18:24:10.613123 trade_executor-0.3/tradeexecutor/strategy/pandas_trader/trade_decision.py
+-rw-r--r--   0        0        0     4589 2023-04-18 22:44:56.800639 trade_executor-0.3/tradeexecutor/strategy/pricing_model.py
+-rw-r--r--   0        0        0      345 2023-02-11 09:28:14.563067 trade_executor-0.3/tradeexecutor/strategy/qstrader/__init__.py
+-rw-r--r--   0        0        0      872 2022-09-17 18:24:10.613322 trade_executor-0.3/tradeexecutor/strategy/qstrader/alpha_model.py
+-rw-r--r--   0        0        0     6999 2023-02-11 09:28:14.563237 trade_executor-0.3/tradeexecutor/strategy/qstrader/order_sizer.py
+-rw-r--r--   0        0        0    11396 2023-02-11 09:28:14.563563 trade_executor-0.3/tradeexecutor/strategy/qstrader/portfolio_construction_model.py
+-rw-r--r--   0        0        0     7431 2023-02-11 09:28:14.563811 trade_executor-0.3/tradeexecutor/strategy/qstrader/runner.py
+-rw-r--r--   0        0        0      625 2023-02-11 09:28:14.564065 trade_executor-0.3/tradeexecutor/strategy/reserve_currency.py
+-rw-r--r--   0        0        0     4660 2023-04-23 21:04:11.835990 trade_executor-0.3/tradeexecutor/strategy/reverse_universe.py
+-rw-r--r--   0        0        0     9041 2023-04-17 20:22:44.641724 trade_executor-0.3/tradeexecutor/strategy/routing.py
+-rw-r--r--   0        0        0    17440 2023-04-04 08:50:41.338097 trade_executor-0.3/tradeexecutor/strategy/routing_model_base.py
+-rw-r--r--   0        0        0     6370 2023-04-04 14:26:18.196529 trade_executor-0.3/tradeexecutor/strategy/run_state.py
+-rw-r--r--   0        0        0    20498 2023-04-17 20:22:44.642157 trade_executor-0.3/tradeexecutor/strategy/runner.py
+-rw-r--r--   0        0        0     5616 2023-04-19 08:31:31.384992 trade_executor-0.3/tradeexecutor/strategy/stop_loss.py
+-rw-r--r--   0        0        0      680 2023-02-11 09:28:14.565922 trade_executor-0.3/tradeexecutor/strategy/strategy_cycle_trigger.py
+-rw-r--r--   0        0        0    16199 2023-02-11 09:31:57.788498 trade_executor-0.3/tradeexecutor/strategy/strategy_module.py
+-rw-r--r--   0        0        0      805 2022-09-17 18:24:10.613980 trade_executor-0.3/tradeexecutor/strategy/strategy_type.py
+-rw-r--r--   0        0        0     3122 2023-02-11 09:28:14.566499 trade_executor-0.3/tradeexecutor/strategy/summary.py
+-rw-r--r--   0        0        0     3488 2023-04-17 20:22:44.642410 trade_executor-0.3/tradeexecutor/strategy/sync_model.py
+-rw-r--r--   0        0        0     6260 2023-04-18 22:44:56.800822 trade_executor-0.3/tradeexecutor/strategy/trade_pricing.py
+-rw-r--r--   0        0        0    54547 2023-04-27 21:52:41.945333 trade_executor-0.3/tradeexecutor/strategy/trading_strategy_universe.py
+-rw-r--r--   0        0        0     4756 2023-04-10 09:52:55.168918 trade_executor-0.3/tradeexecutor/strategy/universe_model.py
+-rw-r--r--   0        0        0     2090 2023-02-20 22:42:50.593623 trade_executor-0.3/tradeexecutor/strategy/valuation.py
+-rw-r--r--   0        0        0     3351 2023-02-28 20:33:59.927859 trade_executor-0.3/tradeexecutor/strategy/weighting.py
+-rw-r--r--   0        0        0       27 2022-09-17 18:24:10.614374 trade_executor-0.3/tradeexecutor/testing/__init__.py
+-rw-r--r--   0        0        0     5743 2023-02-20 22:42:50.593951 trade_executor-0.3/tradeexecutor/testing/backtest_trader.py
+-rw-r--r--   0        0        0     3932 2023-02-28 15:24:43.085624 trade_executor-0.3/tradeexecutor/testing/dummy_trader.py
+-rw-r--r--   0        0        0     2973 2023-04-03 10:43:31.169677 trade_executor-0.3/tradeexecutor/testing/dummy_wallet.py
+-rw-r--r--   0        0        0     8220 2023-04-17 20:22:44.643040 trade_executor-0.3/tradeexecutor/testing/ethereumtrader_uniswap_v2.py
+-rw-r--r--   0        0        0     6824 2023-04-17 20:22:44.643205 trade_executor-0.3/tradeexecutor/testing/ethereumtrader_uniswap_v3.py
+-rw-r--r--   0        0        0     1823 2023-04-17 20:22:44.643424 trade_executor-0.3/tradeexecutor/testing/pairuniversetrader.py
+-rw-r--r--   0        0        0      743 2023-04-05 15:52:50.983178 trade_executor-0.3/tradeexecutor/testing/pytest_helpers.py
+-rw-r--r--   0        0        0     8367 2023-04-17 20:22:44.643592 trade_executor-0.3/tradeexecutor/testing/simulated_execution_loop.py
+-rw-r--r--   0        0        0     3160 2023-04-17 20:22:44.643836 trade_executor-0.3/tradeexecutor/testing/simulated_trader.py
+-rw-r--r--   0        0        0      251 2022-09-17 18:24:10.614799 trade_executor-0.3/tradeexecutor/testing/synthetic_ethereum_data.py
+-rw-r--r--   0        0        0     2289 2023-02-11 09:28:14.568672 trade_executor-0.3/tradeexecutor/testing/synthetic_exchange_data.py
+-rw-r--r--   0        0        0     3528 2022-09-27 22:04:00.142154 trade_executor-0.3/tradeexecutor/testing/synthetic_price_data.py
+-rw-r--r--   0        0        0       53 2022-09-17 18:24:10.614999 trade_executor-0.3/tradeexecutor/utils/__init__.py
+-rw-r--r--   0        0        0     1602 2023-03-01 15:19:10.075435 trade_executor-0.3/tradeexecutor/utils/accuracy.py
+-rw-r--r--   0        0        0      522 2023-02-11 09:28:14.568893 trade_executor-0.3/tradeexecutor/utils/blockchain.py
+-rw-r--r--   0        0        0      397 2022-09-17 18:24:10.615052 trade_executor-0.3/tradeexecutor/utils/dataclass.py
+-rw-r--r--   0        0        0      296 2022-09-27 22:04:00.142204 trade_executor-0.3/tradeexecutor/utils/format.py
+-rw-r--r--   0        0        0      305 2023-02-11 09:28:14.569164 trade_executor-0.3/tradeexecutor/utils/fullname.py
+-rw-r--r--   0        0        0      423 2022-09-17 18:24:10.615153 trade_executor-0.3/tradeexecutor/utils/price.py
+-rw-r--r--   0        0        0     1560 2023-02-14 13:41:36.646227 trade_executor-0.3/tradeexecutor/utils/python_module_loader.py
+-rw-r--r--   0        0        0     2433 2023-02-11 09:28:14.569385 trade_executor-0.3/tradeexecutor/utils/ring_buffer_logging_handler.py
+-rw-r--r--   0        0        0      823 2022-09-17 18:24:10.615210 trade_executor-0.3/tradeexecutor/utils/timer.py
+-rw-r--r--   0        0        0     2088 2023-03-27 22:48:02.297114 trade_executor-0.3/tradeexecutor/utils/timestamp.py
+-rw-r--r--   0        0        0       52 2022-09-27 22:04:00.142342 trade_executor-0.3/tradeexecutor/utils/typing.py
+-rw-r--r--   0        0        0      937 2023-02-11 09:28:14.569861 trade_executor-0.3/tradeexecutor/utils/url.py
+-rw-r--r--   0        0        0       40 2022-09-17 18:24:10.615462 trade_executor-0.3/tradeexecutor/visual/__init__.py
+-rw-r--r--   0        0        0     7499 2023-04-27 14:18:55.726044 trade_executor-0.3/tradeexecutor/visual/benchmark.py
+-rw-r--r--   0        0        0     6780 2023-04-26 10:26:00.675228 trade_executor-0.3/tradeexecutor/visual/equity_curve.py
+-rw-r--r--   0        0        0      773 2023-02-11 09:28:14.570376 trade_executor-0.3/tradeexecutor/visual/image_output.py
+-rw-r--r--   0        0        0    30883 2023-04-27 14:19:19.910062 trade_executor-0.3/tradeexecutor/visual/single_pair.py
+-rw-r--r--   0        0        0     1862 2023-02-11 09:28:14.570847 trade_executor-0.3/tradeexecutor/visual/strategy_state.py
+-rw-r--r--   0        0        0     5775 2023-04-18 22:44:56.801680 trade_executor-0.3/tradeexecutor/visual/technical_indicator.py
+-rw-r--r--   0        0        0       41 2022-09-17 18:24:10.615753 trade_executor-0.3/tradeexecutor/webhook/__init__.py
+-rw-r--r--   0        0        0     6381 2023-03-27 22:48:02.298073 trade_executor-0.3/tradeexecutor/webhook/api.py
+-rw-r--r--   0        0        0     4719 2023-02-11 09:28:14.571333 trade_executor-0.3/tradeexecutor/webhook/app.py
+-rw-r--r--   0        0        0     2102 2022-12-07 17:17:25.926302 trade_executor-0.3/tradeexecutor/webhook/error.py
+-rw-r--r--   0        0        0      580 2022-09-17 18:24:10.616036 trade_executor-0.3/tradeexecutor/webhook/events.py
+-rw-r--r--   0        0        0     2164 2023-02-11 09:28:14.571572 trade_executor-0.3/tradeexecutor/webhook/server.py
+-rw-r--r--   0        0        0     6351 1970-01-01 00:00:00.000000 trade_executor-0.3/setup.py
+-rw-r--r--   0        0        0     5890 1970-01-01 00:00:00.000000 trade_executor-0.3/PKG-INFO
```

### Comparing `trade_executor-0.2/LICENSE.txt` & `trade_executor-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/pyproject.toml` & `trade_executor-0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,86 @@
 [tool.poetry]
 name = "trade-executor"
-version = "0.2"
-description = "Trading strategy execution and backtesting"
+version = "0.3"
+description = "Algorithmic trading backtesting and execution engine for decentralised finance"
 authors = ["Mikko Ohtamaa <mikko@tradingstrategy.ai>"]
 homepage = "https://tradingstrategy.ai"
 repository = "https://github.com/tradingstrategy-ai/trade-executor"
 license = "APGL"
 readme = "README.md"
-keywords = ["algorithmic trading", "ethereum", "cryptocurrency", "uniswap", "quantitative finance", "binance", "blockchain", "pancakeswap", "polygon", "web3"]
+keywords = ["algorithmic trading", "ethereum", "cryptocurrency", "uniswap", "quantitative finance", "binance", "coinbase", "pancakeswap"]
 packages = [
     { include = "tradeexecutor" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 
 # Use these during development
 # web3-ethereum-defi = {path = "deps/web3-ethereum-defi", develop = true}
 # trading-strategy = {path = "deps/trading-strategy", develop = true}
 requests = "^2.27.1"
-web3 = "^5.26.0"
-web3-ethereum-defi = "^0.11.1"
-trading-strategy = "0.8.5"
+web3-ethereum-defi = "0.18.3"
+trading-strategy = "0.14"
 matplotlib = "^3.6.0"
 jupyterlab = "^3.5.0"
 pandas-ta = "^0.3.14-beta.0"
-tqdm-loggable = "^0.1.1"
+tqdm-loggable = "0.1.3"
 
 # tqdm progress bar doesn't show up in VScode Jupyter with ipywidgets>=8
 # https://github.com/microsoft/vscode-jupyter/issues/11014
 ipywidgets = ">=7.0,<8.0"
 
 #
 # Execution deps
 #
 typer = {version="^0.4.0", optional = true}
 colorama = {version="^0.4.4", optional = true}
 coloredlogs = {version="^15.0.1", optional = true}
 prompt-toolkit = {version = "^3.0.31", optional = true}
 APScheduler = {version="^3.9.1", optional = true}
-python-logstash-tradingstrategy = {version="^0.5.0", optional = true}
+#python-logstash-tradingstrategy = {version="^0.5.0", optional = true}
+python-logstash-tradingstrategy = "0.5.1"
 python-logging-discord-handler = {version="^0.1.3", optional = true}
 python-dotenv = {version="^0.21.0", optional = true}
+kaleido = {version="0.2.1", optional = true}
 
 #
 # Web server deps
 #
 pyramid = {version="^2.0", optional = true}
-pyramid-openapi3 = {version="^0.13", optional = true}
+pyramid-openapi3 = {version="^0.16.0", optional = true}
 waitress = {version="^2.0.0", optional = true}
 WebTest = {version="^3.0.0", optional = true}
+# python-openapi3 incompatible with newer versions
+openapi-core = {version = "<0.17", optional = true}
+
 
 #
 # Legacy strategy deps
 #
 trading-strategy-qstrader = {version="^0.5",  optional = true}
 
 #
+# quantstats package for generating
+# advanced statistical reports
+#
+quantstats = {version="^0.0.59", optional = true}
+
+#
 # This package is to be used in various environemnts
 # - Execution oracles (makes trades)
 # - Client side Python within a browser
 # - Web server
 #
 # Note: in the future execution may exist without a web server,
 # e.g. in-browser  bots.
 #
 tqdm = "^4.64.1"
+tblib = "^1.7.0"
 [tool.poetry.extras]
 
 # Legacy strats
 qstrader = ["trading-strategy-qstrader"]
 
 # Only needed when running live trades
 execution = [
@@ -77,30 +88,40 @@
     "python-logstash-tradingstrategy",
     "APScheduler",
     "typer",
     "colorama",
     "coloredlogs",
     "prompt-toolkit",
     "python-dotenv",
-    "setuptools"
+    "setuptools",
+    "kaleido"
 ]
 
 # These dependencies are not neededon the client side code
 web-server = [
     "pyramid",
     "WebTest",
+    "openapi-core",
     "pyramid-openapi3",
     "waitress"
 ]
 
+data = ["web3-ethereum-defi"]
+
+# for generating advanced statistical reports
+quantstats = ["quantstats"]
+
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
+pytest = "^7.2.2"
 ipdb = "^0.13.9"
 flaky = "^3.7.0"
 
+[tool.poetry.group.dev.dependencies]
+pytest-reverse = "^1.5.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 trade-executor = 'tradeexecutor.cli.main:app'
 get-latest-release = 'tradeexecutor.cli.latest_release:main'
```

### Comparing `trade_executor-0.2/tradeexecutor/analysis/trade_analyser.py` & `trade_executor-0.3/tradeexecutor/strategy/pandas_trader/position_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,804 +1,707 @@
-"""Analyze the trade performance of algorithm.
+"""Positions open and closing management."""
 
-Calculate success/fail rate of trades and plot success distribution.
+import datetime
+from decimal import Decimal
+from typing import List, Optional, Union
+import logging
 
-Example analysis include:
+import pandas as pd
 
-- Table: Summary of all trades
+from tradeexecutor.state.identifier import AssetIdentifier, TradingPairIdentifier
+from tradeexecutor.state.portfolio import Portfolio
+from tradeexecutor.state.position import TradingPosition
+from tradeexecutor.state.state import State
+from tradeexecutor.state.trade import TradeType, TradeExecution
+from tradeexecutor.state.types import USDollarAmount, Percent
+from tradeexecutor.strategy.pricing_model import PricingModel
+from tradingstrategy.candle import CandleSampleUnavailable
+from tradingstrategy.pair import DEXPair
+from tradingstrategy.universe import Universe
+from tradeexecutor.strategy.trading_strategy_universe import translate_trading_pair, TradingStrategyUniverse
 
-- Graph: Trade won/lost distribution
+logger = logging.getLogger(__name__)
 
-- Timeline: Analysis of each individual trades made
 
-.. note ::
+class NoSingleOpenPositionException(Exception):
+    """Raised if getting the single position of the current portfolio is not successful."""
 
-    A lot of this code has been lifted off from trading-strategy package
-    where it had to deal with different trading frameworks.
-    It could be simplified greatly now.
 
-"""
-import datetime
-import enum
-import logging
-from dataclasses import dataclass, field
-from typing import List, Dict, Iterable, Optional, Tuple, Callable, Set
+class PositionManager:
+    """An utility class to open and close new trade positions.
 
-import numpy as np
-import pandas as pd
-from dataclasses_json import dataclass_json, Exclude, config
+    `PositionManager` hides away the complex logic reason about trades.
+    It is designed to be used in a trading strategy's `decide_trades()` function
+    as an utility class to generate trades a list of :py:class:`TradeExecution`
+    objects.
 
-from tradeexecutor.state.portfolio import Portfolio
-from tradeexecutor.state.trade import TradeExecution, TradeType
-from tradeexecutor.utils.format import calculate_percentage
-from tradeexecutor.utils.timestamp import json_encode_timedelta, json_decode_timedelta
-
-from tradingstrategy.exchange import Exchange
-from tradingstrategy.pair import PandasPairUniverse
-from tradingstrategy.types import PrimaryKey, USDollarAmount
-from tradingstrategy.utils.format import format_value, format_price, format_duration_days_hours_mins, \
-    format_percent_2_decimals
-from tradingstrategy.utils.summarydataframe import as_dollar, as_integer, create_summary_table, as_percent, as_duration
+    It offers a simple interface for trading for people who are used to
+    TradingView's :term:`Pine Script` or similar limited trade scripting environment.
 
-logger = logging.getLogger(__name__)
+    PositionManager helps about
 
+    - How to have up-to-date price information
 
-@dataclass
-class SpotTrade:
-    """Track spot trades to construct position performance.
+    - Setting take profit/stop loss parameters for positions
 
-    For sells, quantity is negative.
-    """
+    - Converting between US dollar prices, crypto prices
+
+    - Converting between quantity and value of a trade
 
-    #: Internal running counter to uniquely label all trades in trade analysis
-    trade_id: PrimaryKey
+    - Caring whether we have an existing position open for the trading pair already
 
-    #: Trading pair for this trade
-    pair_id: PrimaryKey
+    - Shortcut methods for trading strategies that trade only a single trading pair
 
-    #: When this trade was made, the backtes simulation thick
-    timestamp: pd.Timestamp
+    `PositionManager` takes the price feed and current execution state as an input and
+    produces the execution instructions to change positions.
 
-    #: Asset price at buy in
-    price: USDollarAmount
+    Below are some recipes how to use position manager.
 
-    #: How much we bought the asset. Negative value for sells.
-    quantity: float
+    Position manager is usually instiated at your `decide_trades` function as the following:
 
-    #: How much fees we paid to the exchange
-    commission: USDollarAmount
+    .. code-block:: python
 
-    #: How much we lost against the midprice due to the slippage
-    slippage: USDollarAmount
+        from typing import List, Dict
 
-    #: Any hints applied for this trade why it was performed
-    trade_type: Optional[TradeType] = None
+        from tradeexecutor.state.visualisation import PlotKind
+        from tradeexecutor.state.trade import TradeExecution
+        from tradeexecutor.strategy.pricing_model import PricingModel
+        from tradeexecutor.strategy.pandas_trader.position_manager import PositionManager
+        from tradeexecutor.state.state import State
+        from tradingstrategy.universe import Universe
 
-    #: Internal state dump of the algorithm when this trade was made.
-    #: This is mostly useful when doing the trade analysis try to understand
-    #: why some trades were made.
-    #: It also allows you to reconstruct the portfolio state over the time.
-    state_details: Optional[Dict] = None
 
-    def is_buy(self):
-        return self.quantity > 0
+        def decide_trades(
+                timestamp: pd.Timestamp,
+                universe: Universe,
+                state: State,
+                pricing_model: PricingModel,
+                cycle_debug_data: Dict) -> List[TradeExecution]:
 
-    def is_sell(self):
-        return self.quantity < 0
+            # Create a position manager helper class that allows us easily to create
+            # opening/closing trades for different positions
+            position_manager = PositionManager(timestamp, universe, state, pricing_model)
 
-    @property
-    def value(self) -> USDollarAmount:
-        return abs(self.price * float(self.quantity))
 
+    How to check if you have an open position using :py:meth:`is_any_open`
+    and then open a new position:
 
-@dataclass
-class TradePosition:
-    """How a particular asset traded.
+    .. code-block:: python
 
-    Each asset can have multiple entries (buys) and exits (sells)
+        # List of any trades we decide on this cycle.
+        # Because the strategy is simple, there can be
+        # only zero (do nothing) or 1 (open or close) trades
+        # decides
+        trades = []
 
-    For a simple strategies there can be only one or two trades per position.
+        if not position_manager.is_any_open():
+            buy_amount = cash * position_size
+            trades += position_manager.open_1x_long(pair, buy_amount)
 
-    * Enter (buy)
+        return trades
+
+    How to check the entry price and open quantity of your latest position.
+    See also :py:class:`decimal.Decimal` about arbitrary precision decimal numbers
+    in Python.
+
+    .. code-block:: python
+
+        # Will throw an exception if there is no position open
+        current_position = position_manager.get_current_position()
+
+        # Quantity is the open amount in tokens.
+        # This is expressed in Python Decimal class,
+        # because Ethereum token balances are accurate up to 18 decimals
+        # and this kind of accuracy cannot be expressed in floating point numbers.
+        quantity = current_position.get_quantity()
+        assert quantity == Decimal('0.03045760003971992547285959728')
+
+        # The current price is the price of the trading pair
+        # that was recorded on the last price feed sync.
+        # This is a 64-bit floating point, as the current price
+        # is always approximation based on market conditions.
+        price = current_position.get_current_price()
+        assert price == 1641.6263899583264
+
+        # The opening price is the price of the first trade
+        # that was made for this position. This is the actual
+        # executed price of the trade, expressed as floating
+        # point for the convenience.
+        price = current_position.get_opening_price()
+        assert price == 1641.6263899583264
 
-    * Exit (sell optionally)
     """
 
-    #: List of all trades done for this position
-    trades: List[SpotTrade] = field(default_factory=list)
+    def __init__(self,
+                 timestamp: Union[datetime.datetime, pd.Timestamp],
+                 universe: Universe,
+                 state: State,
+                 pricing_model: PricingModel,
+                 default_slippage_tolerance=0.01,  # Slippage tole
+                 ):
+
+        """Create a new PositionManager instance.
+        
+        Call within `decide_trades` function.
+        
+        :param timestamp: 
+            The timestamp of the current strategy cycle
+            
+        :param universe: 
+            Trading universe of available assets
+        
+        :param state: 
+            Current state of the trade execution
+            
+        :param pricing_model:
+            The model to estimate prices for any trades
+         
+        :param default_slippage_tolerance: 
+            Slippage tolerance parameter set for any trades if not overriden trade-by-trade basis.
+            
+        """
+
+        assert pricing_model, "pricing_model is needed in order to know buy/sell price of new positions"
+        assert isinstance(universe, Universe), f"Got {universe} {type(universe)}"
 
-    #: Closing the position could be deducted from the trades themselves,
-    #: but we cache it by hand to speed up processing
-    opened_at: Optional[pd.Timestamp] = None
+        if isinstance(timestamp, pd.Timestamp):
+            timestamp = timestamp.to_pydatetime().replace(tzinfo=None)
 
-    #: Closing the position could be deducted from the trades themselves,
-    #: but we cache it by hand to speed up processing
-    closed_at: Optional[pd.Timestamp] = None
+        self.timestamp = timestamp
+        self.universe = universe
+        self.state = state
+        self.pricing_model = pricing_model
+        self.default_slippage_tolerance = default_slippage_tolerance
 
-    def __eq__(self, other: "TradePosition"):
-        """Trade positions are unique by opening timestamp and pair id.]
+        reserve_currency, reserve_price = state.portfolio.get_default_reserve()
 
-        We assume there cannot be a position opened for the same asset at the same time twice.
+        self.reserve_currency = reserve_currency
+
+    def is_any_open(self) -> bool:
+        """Do we have any positions open."""
+        return len(self.state.portfolio.open_positions) > 0
+
+    def get_current_position(self) -> TradingPosition:
+        """Get the current single position.
+
+        This is a shortcut function for trading strategies
+        that operate only a single trading pair and a single position.
+
+        :return:
+            Currently open trading position
+
+        :raise NoSingleOpenPositionError:
+            If you do not have a position open or there are multiple positions open.
         """
-        return self.position_id == other.position_id
 
-    def __hash__(self):
-        """Allows easily create index (hash map) of all positions"""
-        return hash((self.position_id))
+        open_positions = self.state.portfolio.open_positions
+
+        if len(open_positions) == 0:
+            raise NoSingleOpenPositionException(f"No positions open at {self.timestamp}")
 
-    @property
-    def position_id(self) -> PrimaryKey:
-        """Position id is the same as the opening trade id."""
-        return self.trades[0].trade_id
+        if len(open_positions) > 1:
+            raise NoSingleOpenPositionException(f"Multiple positions ({len(open_positions)}) open at {self.timestamp}")
 
-    @property
-    def pair_id(self) -> PrimaryKey:
-        """Position id is the same as the opening trade id."""
-        return self.trades[0].pair_id
+        return next(iter(open_positions.values()))
 
-    @property
-    def duration(self) -> Optional[datetime.timedelta]:
-        """How long this position was held.
+    def get_current_position_for_pair(self, pair: TradingPairIdentifier) -> Optional[TradingPosition]:
+        """Get the current open position for a specific trading pair.
+
+        :return:
+            Currently open trading position.
+
+            If there is no open position return None.
 
-        :return: None if the position is still open
         """
-        if not self.is_closed():
-            return None
-        return self.closed_at - self.opened_at
+        return self.state.portfolio.get_position_by_trading_pair(pair)
 
-    def is_open(self):
-        return self.closed_at is None
+    def get_last_closed_position(self) -> Optional[TradingPosition]:
+        """Get the position that was last closed.
 
-    def is_closed(self):
-        return not self.is_open()
+        If multiple positions are closed at the same time,
+        return a random position.
 
-    @property
-    def open_quantity(self) -> float:
-        return sum([t.quantity for t in self.trades])
-
-    @property
-    def open_value(self) -> float:
-        """The current value of this open position, with the price at the time of opening."""
-        assert self.is_open()
-        return sum([t.value for t in self.trades])
-
-    @property
-    def open_price(self) -> float:
-        """At what price we opened this position.
-
-        Supports only simple enter/exit positions.
-        """
-        return self.get_first_entry_price()
-
-    def get_first_entry_price(self) -> float:
-        """What was the price when the first entry buy for this position was made.
-        """
-        buys = list(self.buys)
-        return buys[0].price
-
-    def get_last_exit_price(self) -> float:
-        """What was the time when the last sell for this position was executd.
-        """
-        sells = list(self.sells)
-        return sells[-1].price
-        assert len(sells) == 1
-
-    @property
-    def close_price(self) -> float:
-        """At what price we exited this position.
-
-        Supports only simple enter/exit positions.
-        """
-        return self.get_last_exit_price()
-
-    @property
-    def buys(self) -> Iterable[SpotTrade]:
-        return [t for t in self.trades if t.is_buy()]
-
-    @property
-    def sells(self) -> Iterable[SpotTrade]:
-        return [t for t in self.trades if t.is_sell()]
-
-    @property
-    def buy_value(self) -> USDollarAmount:
-        return sum([t.value - t.commission for t in self.trades if t.is_buy()])
-
-    @property
-    def sell_value(self) -> USDollarAmount:
-        return sum([t.value - t.commission for t in self.trades if t.is_sell()])
-
-    @property
-    def realised_profit(self) -> USDollarAmount:
-        """Calculated life-time profit over this position."""
-        assert not self.is_open()
-        return -sum([float(t.quantity) * t.price - t.commission for t in self.trades])
-
-    @property
-    def realised_profit_percent(self) -> float:
-        """Calculated life-time profit over this position."""
-        assert not self.is_open()
-        buy_value = self.buy_value
-        sell_value = self.sell_value
-        return sell_value / buy_value - 1
-
-    def is_win(self):
-        """Did we win this trade."""
-        assert not self.is_open()
-        return self.realised_profit > 0
-
-    def is_lose(self):
-        assert not self.is_open()
-        return self.realised_profit < 0
-
-    def is_stop_loss(self) -> bool:
-        """Was stop loss triggered for this position"""
-        for t in self.trades:
-            if t.trade_type == TradeType.stop_loss:
-                return True
-        return False
-
-    def is_take_profit(self) -> bool:
-        """Was trake profit triggered for this position"""
-        for t in self.trades:
-            if t.trade_type == TradeType.take_profit:
-                return True
-        return False
-
-    def add_trade(self, t: SpotTrade):
-        if self.trades:
-            last_trade = self.trades[-1]
-            assert t.timestamp >= last_trade.timestamp, f"Tried to do trades in wrong order. Last: {last_trade}, got {t}"
-        self.trades.append(t)
-
-    def can_trade_close_position(self, t: SpotTrade):
-        assert self.is_open()
-        if not t.is_sell():
-            return False
-        open_quantity = self.open_quantity
-        closing_quantity = -t.quantity
-        assert closing_quantity <= open_quantity, "Cannot sell more than we have in balance sheet"
-        return closing_quantity == open_quantity
-
-    def get_max_size(self) -> USDollarAmount:
-        """Get the largest size of this position over the time"""
-        cur_size = 0
-        max_size = 0
-
-        if len(self.trades) > 2:
-            logger.warning("Position has %d trades so this method might produce wrong result")
-
-        for t in self.trades:
-            cur_size = t.value
-            max_size = max(cur_size, max_size)
-        return max_size
-
-    def get_trade_count(self) -> int:
-        """How many individual trades was done to manage this position."""
-        return len(self.trades)
-
-
-@dataclass
-class AssetTradeHistory:
-    """How a particular asset traded.
+        Example:
 
-    Each position can have increments or decrements.
-    When position is decreased to zero, it is considered closed, and a new buy open a new position.
-    """
-    positions: List[TradePosition] = field(default_factory=list)
+        .. code-block:: python
 
-    def get_first_opened_at(self) -> Optional[pd.Timestamp]:
-        if self.positions:
-            return self.positions[0].opened_at
-        return None
-
-    def get_last_closed_at(self) -> Optional[pd.Timestamp]:
-        for position in reversed(self.positions):
-            if not position.is_open():
-                return position.closed_at
-
-        return None
-
-    def add_trade(self, t: SpotTrade):
-        """Adds a new trade to the asset history.
-
-        If there is an open position the trade is added against this,
-        otherwise a new position is opened for tracking.
-        """
-        current_position = None
-        if self.positions:
-            if self.positions[-1].is_open():
-                current_position = self.positions[-1]
-
-        if current_position:
-            if current_position.can_trade_close_position(t):
-                # Close the existing position
-                current_position.closed_at = t.timestamp
-                current_position.add_trade(t)
-                assert current_position.open_quantity == 0
+            last_position = position_manager.get_last_closed_position()
+            if last_position:
+                ago = timestamp - last_position.closed_at
+                print(f"Last position was closed {ago}")
             else:
-                # Add to the existing position
-                current_position.add_trade(t)
-        else:
-            # Open new position
-            new_position = TradePosition(opened_at=t.timestamp)
-            new_position.add_trade(t)
-            self.positions.append(new_position)
-
-
-@dataclass_json
-@dataclass
-class TradeSummary:
-    """Some generic statistics over all the trades"""
-    won: int
-    lost: int
-    zero_loss: int
-    stop_losses: int
-    undecided: int
-    realised_profit: USDollarAmount
-    open_value: USDollarAmount
-    uninvested_cash: USDollarAmount
-
-    initial_cash: USDollarAmount
-    extra_return: USDollarAmount
-    duration: datetime.timedelta = field(metadata=config(
-        encoder=json_encode_timedelta,
-        decoder=json_decode_timedelta,
-    ))
-
-    average_winning_trade_profit_pc: float
-    average_losing_trade_loss_pc: float
-    biggest_winning_trade_pc: Optional[float]
-    biggest_losing_trade_pc: Optional[float]
-
-    average_duration_of_winning_trades: datetime.timedelta = field(metadata=config(
-        encoder=json_encode_timedelta,
-        decoder=json_decode_timedelta,
-    ))
-    average_duration_of_losing_trades: datetime.timedelta = field(metadata=config(
-        encoder=json_encode_timedelta,
-        decoder=json_decode_timedelta,
-    ))
-
-    total_trades: int = field(init=False)
-    win_percent: float = field(init=False)
-    return_percent: float = field(init=False)
-    annualised_return_percent: float = field(init=False)
-    all_stop_loss_percent: float = field(init=False)
-    lost_stop_loss_percent: float = field(init=False)
-    average_net_profit: USDollarAmount = field(init=False)
-    end_value: USDollarAmount = field(init=False)
-
-    def __post_init__(self):
-
-        self.total_trades = self.won + self.lost + self.zero_loss
-        self.win_percent = calculate_percentage(self.won, self.total_trades)
-        self.return_percent = calculate_percentage(self.realised_profit, self.initial_cash)
-        self.annualised_return_percent = calculate_percentage(self.return_percent * datetime.timedelta(days=365),
-                                                              self.duration) if self.return_percent else None
-        self.all_stop_loss_percent = calculate_percentage(self.stop_losses, self.total_trades)
-        self.lost_stop_loss_percent = calculate_percentage(self.stop_losses, self.lost)
-        self.average_net_profit = self.realised_profit / self.total_trades if self.total_trades else None
-        self.end_value = self.open_value + self.uninvested_cash
-
-    def to_dataframe(self) -> pd.DataFrame:
-        """Creates a human-readable Pandas dataframe table from the object."""
-        human_data = {
-            "Trading period length": as_duration(self.duration),
-            "Return %": as_percent(self.return_percent),
-            "Annualised return %": as_percent(self.annualised_return_percent),
-            "Cash at start": as_dollar(self.initial_cash),
-            "Value at end": as_dollar(self.end_value),
-            "Trade win percent": as_percent(self.win_percent),
-            "Total trades done": as_integer(self.total_trades),
-            "Won trades": as_integer(self.won),
-            "Lost trades": as_integer(self.lost),
-            "Stop losses triggered": as_integer(self.stop_losses),
-            "Stop loss % of all": as_percent(self.all_stop_loss_percent),
-            "Stop loss % of lost": as_percent(self.lost_stop_loss_percent),
-            "Zero profit trades": as_integer(self.zero_loss),
-            "Positions open at the end": as_integer(self.undecided),
-            "Realised profit and loss": as_dollar(self.realised_profit),
-            "Portfolio unrealised value": as_dollar(self.open_value),
-            "Extra returns on lending pool interest": as_dollar(self.extra_return),
-            "Cash left at the end": as_dollar(self.uninvested_cash),
-            "Average winning trade profit %": as_percent(self.average_winning_trade_profit_pc),
-            "Average losing trade loss %": as_percent(self.average_losing_trade_loss_pc),
-            "Biggest winning trade %": as_percent(self.biggest_winning_trade_pc),
-            "Biggest losing trade %": as_percent(self.biggest_losing_trade_pc),
-            "Average duration of winning trades": as_duration(self.average_duration_of_winning_trades),
-            "Average duration of losing trades": as_duration(self.average_duration_of_losing_trades)
-        }
-        return create_summary_table(human_data)
-
-
-@dataclass
-class TradeAnalysis:
-    """Analysis of trades in a portfolio."""
-
-    portfolio: Portfolio
-
-    #: How a particular asset traded. Asset id -> Asset history mapping
-    asset_histories: Dict[object, AssetTradeHistory] = field(default_factory=dict)
-
-    def get_first_opened_at(self) -> Optional[pd.Timestamp]:
-        def all_opens():
-            for history in self.asset_histories.values():
-                yield history.get_first_opened_at()
-
-        return min(all_opens())
-
-    def get_last_closed_at(self) -> Optional[pd.Timestamp]:
-        def all_closes():
-            for history in self.asset_histories.values():
-                closed = history.get_last_closed_at()
-                if closed:
-                    yield closed
-
-        return max(all_closes())
-
-    def get_all_positions(self) -> Iterable[Tuple[PrimaryKey, TradePosition]]:
-        """Return open and closed positions over all traded assets."""
-        for pair_id, history in self.asset_histories.items():
-            for position in history.positions:
-                yield pair_id, position
-
-    def get_open_positions(self) -> Iterable[Tuple[PrimaryKey, TradePosition]]:
-        """Return open and closed positions over all traded assets."""
-        for pair_id, history in self.asset_histories.items():
-            for position in history.positions:
-                if position.is_open():
-                    yield pair_id, position
-
-    def calculate_summary_statistics(self) -> TradeSummary:
-        """Calculate some statistics how our trades went."""
-
-        initial_cash = self.portfolio.get_initial_deposit()
-
-        uninvested_cash = self.portfolio.get_current_cash()
-
-        # EthLisbon hack
-        extra_return = 0
-
-        duration = datetime.timedelta(0)
-
-        winning_trades = []
-        losing_trades = []
-        winning_trades_duration = []
-        losing_trades_duration = []
-        biggest_winning_trade_pc = None
-        biggest_losing_trade_pc = None
-        average_duration_of_losing_trades = datetime.timedelta(0)
-        average_duration_of_winning_trades = datetime.timedelta(0)
-
-        first_trade, last_trade = self.portfolio.get_first_and_last_executed_trade()
-        if first_trade and first_trade != last_trade:
-            duration = last_trade.executed_at - first_trade.executed_at
-
-        won = lost = zero_loss = stop_losses = undecided = 0
-        open_value: USDollarAmount = 0
-        profit: USDollarAmount = 0
-        for pair_id, position in self.get_all_positions():
-            if position.is_open():
-                open_value += position.open_value
-                undecided += 1
-                continue
-
-            if position.is_stop_loss():
-                stop_losses += 1
-
-            if position.is_win():
-                won += 1
-                winning_trades.append(position.realised_profit_percent)
-                winning_trades_duration.append(position.duration)
-
-
-            elif position.is_lose():
-                lost += 1
-                losing_trades.append(position.realised_profit_percent)
-                losing_trades_duration.append(position.duration)
+                print("Strategy has not decided any position before")
 
-            else:
-                # Any profit exactly balances out loss in slippage and commission
-                zero_loss += 1
+        :return:
 
-            profit += position.realised_profit
+            None if the strategy has not closed any positions
+        """
+        closed_positions = self.state.portfolio.closed_positions
 
-        if len(winning_trades) > 0:
-            average_winning_trade_profit_pc = float(np.mean(winning_trades))
-        else:
-            average_winning_trade_profit_pc = 0
+        if len(closed_positions) == 0:
+            return None
 
-        if len(losing_trades) > 0:
-            average_losing_trade_loss_pc = float(np.mean(losing_trades))
-        else:
-            average_losing_trade_loss_pc = 0
+        return max(closed_positions.values(), key=lambda c: c.closed_at)
 
-        if winning_trades:
-            biggest_winning_trade_pc = max(winning_trades)
+    def get_current_portfolio(self) -> Portfolio:
+        """Return the active portfolio of the strategy."""
+        return self.state.portfolio
+
+    def get_trading_pair(self, pair_id: int) -> TradingPairIdentifier:
+        """Get a trading pair identifier by its internal id.
+
+        Note that internal integer ids are not stable over
+        multiple trade cycles and might be reset.
+        Always use (chain id, smart contract) for persistent
+        pair identifier.
 
-        if losing_trades:
-            biggest_losing_trade_pc = min(losing_trades)
+        :return:
+            Trading pair information
+        """
+        dex_pair = self.universe.pairs.get_pair_by_id(pair_id)
+        return translate_trading_pair(dex_pair)
 
-        if winning_trades_duration:
-            average_duration_of_winning_trades = np.mean(winning_trades_duration).to_pytimedelta()
-
-        if losing_trades_duration:
-            average_duration_of_losing_trades = np.mean(losing_trades_duration).to_pytimedelta()
-
-        return TradeSummary(
-            won=won,
-            lost=lost,
-            zero_loss=zero_loss,
-            stop_losses=stop_losses,
-            undecided=undecided,
-            realised_profit=profit + extra_return,
-            open_value=open_value,
-            uninvested_cash=uninvested_cash,
-            initial_cash=initial_cash,
-            extra_return=extra_return,
-            duration=duration,
-            average_winning_trade_profit_pc=average_winning_trade_profit_pc,
-            average_losing_trade_loss_pc=average_losing_trade_loss_pc,
-            biggest_winning_trade_pc=biggest_winning_trade_pc,
-            biggest_losing_trade_pc=biggest_losing_trade_pc,
-            average_duration_of_winning_trades=average_duration_of_winning_trades,
-            average_duration_of_losing_trades=average_duration_of_losing_trades,
-        )
+    def get_pair_fee(self,
+                     pair: Optional[TradingPairIdentifier] = None,
+                     ) -> Optional[float]:
+        """Estimate the trading/LP fees for a trading pair.
 
-    def create_timeline(self) -> pd.DataFrame:
-        """Create a timeline feed how we traded over a course of time.
+        This information can come either from the exchange itself (Uni v2 compatibles),
+        or from the trading pair (Uni v3).
 
-        Note: We assume each position has only one enter and exit event, not position increases over the lifetime.
+        The return value is used to fill the
+        fee values for any newly opened trades.
 
-        :return: DataFrame with timestamp and timeline_event columns
+        :param pair:
+            Trading pair for which we want to have the fee.
+
+            Can be left empty if the underlying exchange is always
+            offering the same fee.
+
+        :return:
+            The estimated trading fee, expressed as %.
+
+            Returns None if the fee information is not available.
+            This can be different from zero fees.
         """
+        return self.pricing_model.get_pair_fee(self.timestamp, pair)
 
-        def gen_events():
-            for pair_id, position in self.get_all_positions():
-                yield (position.position_id, position)
+    def open_1x_long(self,
+                     pair: Union[DEXPair, TradingPairIdentifier],
+                     value: USDollarAmount,
+                     take_profit_pct: Optional[float] = None,
+                     stop_loss_pct: Optional[float] = None,
+                     trailing_stop_loss_pct: Optional[float] = None,
+                     notes: Optional[str] = None,
+                     slippage_tolerance: Optional[float] = None,
+                     ) -> List[TradeExecution]:
+        """Open a long.
+
+        - For simple buy and hold trades
+
+        - Open a spot market buy.
+
+        - Checks that there is not existing position - cannot increase position
+
+        :param pair:
+            Trading pair where we take the position
+
+        :param value:
+            How large position to open, in US dollar terms
+
+        :param take_profit_pct:
+            If set, set the position take profit relative
+            to the current market price.
+            1.0 is the current market price.
+            If asset opening price is $1000, take_profit_pct=1.05
+            will sell the asset when price reaches $1050.
+
+        :param stop_loss_pct:
+            If set, set the position to trigger stop loss relative to
+            the current market price.
+            1.0 is the current market price.
+            If asset opening price is $1000, stop_loss_pct=0.95
+            will sell the asset when price reaches 950.
+
+        :param notes:
+            Human readable notes for this trade
+
+        :param slippage_tolerance:
+            Slippage tolerance for this trade.
+
+            Use :py:attr:`default_slippage_tolerance` if not set.
+
+        :return:
+            A list of new trades.
+            Opening a position may general several trades for complex DeFi positions,
+            though usually the result contains only a single trade.
 
-        df = pd.DataFrame(gen_events(), columns=["position_id", "position"])
-        return df
+        """
 
+        # Translate DEXPair object to the trading pair model
+        if isinstance(pair, DEXPair):
+            executor_pair = translate_trading_pair(pair)
+        else:
+            executor_pair = pair
 
-class TimelineRowStylingMode(enum.Enum):
-    #: Style using Pandas background_gradient
-    gradient = "gradient"
+        # Convert amount of reserve currency to the decimal
+        # so we can have exact numbers from this point forward
+        if type(value) == float:
+            value = Decimal(value)
+
+        price_structure = self.pricing_model.get_buy_price(self.timestamp, executor_pair, value)
+
+        assert type(price_structure.mid_price) == float
+
+        reserve_asset, reserve_price = self.state.portfolio.get_default_reserve()
+
+        slippage_tolerance = slippage_tolerance or self.default_slippage_tolerance
+
+        position, trade, created = self.state.create_trade(
+            self.timestamp,
+            pair=executor_pair,
+            quantity=None,
+            reserve=Decimal(value),
+            assumed_price=price_structure.price,
+            trade_type=TradeType.rebalance,
+            reserve_currency=self.reserve_currency,
+            reserve_currency_price=reserve_price,
+            lp_fees_estimated=price_structure.get_total_lp_fees(),
+            pair_fee=price_structure.get_fee_percentage(),
+            planned_mid_price=price_structure.mid_price,
+            price_structure=price_structure,
+            slippage_tolerance=slippage_tolerance,
+        )
 
-    #: Simple
-    #: Profit = green, loss = red
-    simple = "simple"
+        assert created, f"There was conflicting open position for pair: {executor_pair}"
 
+        if take_profit_pct:
+            position.take_profit = price_structure.mid_price * take_profit_pct
 
-class TimelineStyler:
-    """Style the expanded trades timeline table.
+        if stop_loss_pct:
+            position.stop_loss = price_structure.mid_price * stop_loss_pct
 
-    Give HTML hints for DataFrame how it should be rendered
-    in the notebook output.
-    """
+        if trailing_stop_loss_pct:
+            assert stop_loss_pct is None, "You cannot give both stop_loss_pct and trailing_stop_loss_pct"
+            position.stop_loss = price_structure.mid_price * trailing_stop_loss_pct
+            position.trailing_stop_loss_pct = trailing_stop_loss_pct
 
-    def __init__(self,
-                 row_styling: TimelineRowStylingMode,
-                 hidden_columns: List[str],
-                 vmin: float,
-                 vmax: float,
-                 ):
-        self.row_styling = row_styling
-        self.hidden_columns = hidden_columns
-        self.vmin = vmin
-        self.vmax = vmax
+        if notes:
+            position.notes = notes
+            trade.notes = notes
 
-    def colour_timelime_row_simple(self, row: pd.Series) -> pd.Series:
-        """Set colour for each timeline row based on its profit.
+        self.state.visualisation.add_message(
+            self.timestamp,
+            f"Opened 1x long on {pair}, position value {value} USD")
 
-        - +/- 5% colouring
+        return [trade]
 
-        - More information: https://stackoverflow.com/a/49745352/315168
+    def adjust_position(self,
+                        pair: TradingPairIdentifier,
+                        dollar_delta: USDollarAmount,
+                        quantity_delta: Optional[float],
+                        weight: float,
+                        stop_loss: Optional[Percent] = None,
+                        take_profit: Optional[Percent] = None,
+                        trailing_stop_loss: Optional[Percent] = None,
+                        slippage_tolerance: Optional[float] = None,
+                        override_stop_loss=False,
+                        ) -> List[TradeExecution]:
+        """Adjust holdings for a certain position.
 
-        - CSS colours: https://htmlcolorcodes.com/color-names/
-        """
+        Used to rebalance positions.
 
-        pnl_raw = row["PnL % raw"]
+        A new position is opened if no existing position is open.
+        If everything is sold, the old position is closed
 
-        if pnl_raw < -0.05:
-            return pd.Series('background-color: Salmon', row.index)
-        elif pnl_raw < 0:
-            return pd.Series('background-color: LightSalmon', row.index)
-        elif pnl_raw > 0.05:
-            return pd.Series('background-color: LawnGreen', row.index)
-        else:
-            return pd.Series('background-color: PaleGreen', row.index)
+        If the rebalance is sell (`dollar_amount_delta` is negative),
+        then calculate the quantity of the asset to sell based
+        on the latest available market price on the position.
+
+        This method is called by :py:func:`~tradeexecutor.strategy.pandas_trades.rebalance.rebalance_portfolio`.
+
+        .. warning ::
+
+            Adjust position cannot be used to close an existing position, because
+            epsilons in quantity math. Use :py:meth:`close_position` for this.
+
+        :param pair:
+            Trading pair which position we adjust
+
+        :param dollar_delta:
+            How much we want to increase/decrease the position in US dollar terms.
+
+        :param quantity_delta:
+            How much we want to increase/decrease the position in the asset unit terms.
 
-    def __call__(self, df: pd.DataFrame):
-        """Applies styles on a dataframe
+            Used only when decreasing existing positions (selling).
 
-        :param df:
-            Dataframe as returned by :py:func`expand_timeline`.
+        :param weight:
+            What is the weight of the asset in the new target portfolio 0....1.
+            Currently only used to detect condition "sell all" instead of
+            trying to match quantity/price conversion.
+
+        :param stop_loss:
+            Set the stop loss for the position.
+
+            Use 0...1 based on the current mid price.
+            E.g. 0.98 = 2% stop loss under the current mid price.
+
+            Sets the initial stop loss. If you want to override
+            this for an existing position you need to use `override_stop_loss` parameter.
+
+        :param take_profit:
+            Set the take profit for the position.
+
+            Use 0...1 based on the current mid price.
+            E.g. 1.02 = 2% take profit over the current mid-price.
+
+        :param slippage_tolerance:
+            Slippage tolerance for this trade.
+
+            Use :py:attr:`default_slippage_tolerance` if not set.
+
+        :param override_stop_loss:
+            If not set and a position has already stop loss set, do not modify it.
+
+        :return:
+            List of trades to be executed to get to the desired
+            position level.
         """
-        # Create a Pandas Styler with multiple styling options applied
+        assert dollar_delta != 0
+        assert weight <= 1, f"Target weight cannot be over one: {weight}"
+        assert weight >= 0, f"Target weight cannot be negative: {weight}"
+
         try:
-            styles = df.style \
-                .hide(axis="index") \
-                .hide(axis="columns", subset=self.hidden_columns)
-        except KeyError:
-            # The input df was empty (no trades)
-            styles = df.style
-
-        # Don't let the text inside a cell to wrap
-        styles = styles.set_table_styles({
-            "Opened at": [{'selector': 'td', 'props': [('white-space', 'nowrap')]}],
-            "Exchange": [{'selector': 'td', 'props': [('white-space', 'nowrap')]}],
-        })
-
-        if self.row_styling == TimelineRowStylingMode.gradient:
-            # Dynamically color the background of trade outcome coluns # https://pandas.pydata.org/docs/reference/api/pandas.io.formats.style.Styler.background_gradient.html
-            # TODO: This gradient styling is confusing
-            # get rid of it long term
-            styles = styles.background_gradient(
-                axis=0,
-                gmap=df['PnL % raw'],
-                cmap='RdYlGn',
-                vmin=self.vmin,  # We can only lose 100% of our money on position
-                vmax=self.vmax)  # 50% profit is 21.5 position. Assume this is the max success color we can hit over
+            if dollar_delta > 0:
+                price_structure = self.pricing_model.get_buy_price(self.timestamp, pair, dollar_delta)
+            else:
+                price_structure = self.pricing_model.get_sell_price(self.timestamp, pair, abs(quantity_delta))
+
+        except CandleSampleUnavailable as e:
+            # Backtesting cannot fetch price for an asset,
+            # probably not enough data and the pair is trading early?
+            data_delay_tolerance = getattr(self.pricing_model, "data_delay_tolerance", None)
+            raise CandleSampleUnavailable(
+                f"Could not fetch price for {pair} at {self.timestamp}\n"
+                f"\n"
+                f"This is usually due to sparse candle data - trades have not been made or the blockchain was halted during the price look-up period.\n"
+                f"Because there are no trades we cannot determine what was the correct asset price using {data_delay_tolerance} data tolerance delay.\n"
+                f"\n"
+                f"You can work around this by checking that any trading pair candles are fresh enough in your decide_trades() function\n"
+                f"or increase the parameter in BacktestSimplePricingModel(data_delay_tolerance) or run_backtest_inline(data_delay_tolerance)\n"
+            ) from e
+
+        price = price_structure.price
+
+        reserve_asset, reserve_price = self.state.portfolio.get_default_reserve()
+
+        slippage_tolerance = slippage_tolerance or self.default_slippage_tolerance
+
+        if dollar_delta > 0:
+            # Buy
+            position, trade, created = self.state.create_trade(
+                self.timestamp,
+                pair=pair,
+                quantity=None,
+                reserve=Decimal(dollar_delta),
+                assumed_price=price,
+                trade_type=TradeType.rebalance,
+                reserve_currency=self.reserve_currency,
+                reserve_currency_price=reserve_price,
+                planned_mid_price=price_structure.mid_price,
+                lp_fees_estimated=price_structure.get_total_lp_fees(),
+                pair_fee=price_structure.get_fee_percentage(),
+                slippage_tolerance=slippage_tolerance,
+            )
         else:
-            styles = styles.apply(self.colour_timelime_row_simple, axis=1)
+            # Sell
+            # Convert dollar amount to quantity of the last known price
 
-        return styles
+            assert quantity_delta is not None
+            assert quantity_delta < 0, f"Received non-negative sell quantity {quantity_delta} for {pair}"
 
+            position = self.state.portfolio.get_position_by_trading_pair(pair)
+            assert position is not None, f"Assumed {pair} has open position because of attempt sell at {dollar_delta} USD adjust"
 
-def expand_timeline(
-        exchanges: Set[Exchange],
-        pair_universe: PandasPairUniverse,
-        timeline: pd.DataFrame,
-        vmin=-0.3,
-        vmax=0.2,
-        timestamp_format="%Y-%m-%d",
-        hidden_columns=["Id", "PnL % raw"],
-        row_styling_mode=TimelineRowStylingMode.simple,
-) -> Tuple[pd.DataFrame, TimelineStyler]:
-    """Expand trade history timeline to human readable table.
+            position, trade, created = self.state.create_trade(
+                self.timestamp,
+                pair=pair,
+                quantity=Decimal(quantity_delta),
+                reserve=None,
+                assumed_price=price_structure.price,
+                trade_type=TradeType.rebalance,
+                reserve_currency=self.reserve_currency,
+                reserve_currency_price=reserve_price,
+                planned_mid_price=price_structure.mid_price,
+                lp_fees_estimated=price_structure.get_total_lp_fees(),
+                slippage_tolerance=slippage_tolerance,
+                price_structure=price_structure,
+            )
 
-    This will the outputting much easier in Python Notebooks.
+        assert trade.lp_fees_estimated > 0, f"LP fees estimated: {trade.lp_fees_estimated} - {trade}"
 
-    Currently does not incrementing/decreasing positions gradually.
+        # Update stop loss for this position
+        if stop_loss:
 
-    Instaqd of applying styles or returning a styled dataframe, we return a callable that applies the styles.
-    This is because of Pandas issue https://github.com/pandas-dev/pandas/issues/40675 - hidden indexes, columns,
-    etc. are not exported.
+            assert stop_loss < 1, f"Got stop loss {stop_loss}"
 
-    :param exchanges: Needed for exchange metadata
+            if position.stop_loss:
+                # Update existing stop loss
+                if override_stop_loss:
+                    position.stop_loss = price_structure.mid_price * stop_loss
+                else:
+                    # Do not override existing stop loss set earlier
+                    pass
+            else:
+                # Set the initial stop loss
+                position.stop_loss = price_structure.mid_price * stop_loss
 
-    :param pair_universe: Needed for trading pair metadata
+        if trailing_stop_loss:
+            assert trailing_stop_loss < 1, f"Got trailing_stop_loss {trailing_stop_loss}"
+            if not position.stop_loss:
+                position.stop_loss = price_structure.mid_price * trailing_stop_loss
+            position.trailing_stop_loss_pct = trailing_stop_loss
 
-    :param vmax: Trade success % to have the extreme green color.
+        if take_profit:
+            assert take_profit > 1, f"Got take profit {take_profit}"
+            position.take_profit = price_structure.mid_price * take_profit
 
-    :param vmin: The % of lost capital on the trade to have the extreme red color.
+        return [trade]
 
-    :param timestamp_format: How to format Opened at column, as passed to `strftime()`
+    def close_position(self,
+                       position: TradingPosition,
+                       trade_type: TradeType=TradeType.rebalance,
+                       notes: Optional[str] = None,
+                       trades_as_list=False,
+                       slippage_tolerance: Optional[float] = None,
+                       ) -> Optional[TradeExecution] | List[TradeExecution]:
+        """Close a single position.
 
-    :param hidden_columns: Hide columns in the output table
+        The position may already have piled up selling trades.
+        In this case calling `close_position()` again on the same position
+        does nothing and `None` is returned.
 
-    :return: DataFrame with human=readable position win/loss information, having DF indexed by timestamps and a styler function
-    """
+        :param position:
+            Position to be closed
 
-    exchange_map = {e.exchange_id: e for e in exchanges}
+        :param trade_type:
+            What's the reason to close the position
 
-    # https://stackoverflow.com/a/52363890/315168
-    def expander(row):
-        position: TradePosition = row["position"]
-        # timestamp = row.name  # ???
-        pair_id = position.pair_id
-        pair_info = pair_universe.get_pair_by_id(pair_id)
-        exchange = exchange_map.get(pair_info.exchange_id)
-        if not exchange:
-            raise RuntimeError(f"No exchange for id {pair_info.exchange_id}, pair {pair_info}")
-
-        if position.is_stop_loss():
-            remarks = "SL"
-        elif position.is_take_profit():
-            remarks = "TP"
-        else:
-            remarks = ""
+        :param notes:
+            Human readable notes for this trade
 
-        r = {
-            # "timestamp": timestamp,
-            "Id": position.position_id,
-            "Remarks": remarks,
-            "Opened at": position.opened_at.strftime(timestamp_format),
-            "Duration": format_duration_days_hours_mins(position.duration) if position.duration else np.nan,
-            "Exchange": exchange.name,
-            "Base asset": pair_info.base_token_symbol,
-            "Quote asset": pair_info.quote_token_symbol,
-            "Position max size": format_value(position.get_max_size()),
-            "PnL USD": format_value(position.realised_profit) if position.is_closed() else np.nan,
-            "PnL %": format_percent_2_decimals(position.realised_profit_percent) if position.is_closed() else np.nan,
-            "PnL % raw": position.realised_profit_percent if position.is_closed() else 0,
-            "Open price USD": format_price(position.open_price),
-            "Close price USD": format_price(position.close_price) if position.is_closed() else np.nan,
-            "Trade count": position.get_trade_count(),
-        }
-        return r
-
-    applied_df = timeline.apply(expander, axis='columns', result_type='expand')
-
-    if len(applied_df) > 0:
-        # https://stackoverflow.com/a/52720936/315168
-        applied_df \
-            .sort_values(by=['Id'], ascending=[True], inplace=True)
-
-    # Get rid of NaN labels
-    # https://stackoverflow.com/a/28390992/315168
-    applied_df.fillna('', inplace=True)
-
-    styling = TimelineStyler(
-        row_styling=row_styling_mode,
-        hidden_columns=hidden_columns,
-        vmin=vmin,
-        vmax=vmax,
-    )
-
-    return applied_df, styling
+        :param trades_as_list:
+            A migration parameter for the future signature where we are
+            always returning a list of trades.
 
+        :param slippage_tolerance:
+            Slippage tolerance for this trade.
 
-def build_trade_analysis(portfolio: Portfolio) -> TradeAnalysis:
-    """Build a trade analysis from list of positions.
+            Use :py:attr:`default_slippage_tolerance` if not set.
 
-    - Read positions from backtesting or live state
+        :return:
+            Get list of trades needed to close this position.
 
-    - Create TradeAnalysis instance that can be used to display Jupyter notebook
-      data on the performance
-    """
+            If `trades_as_list` is `False`.
+            A trade that will close the position fully.
+            If there is nothing left to close, return None.
+
+            Otherwise return list of trades.
 
-    histories = {}
+        """
 
-    positions = list(portfolio.get_all_positions())
+        assert position.is_long(), "Only long supported for now"
+        assert position.is_open(), f"Tried to close already closed position {position}"
 
-    # Sort positions based on their id
-    # because open, closed and frozen positions might be in a mixed order
-    positions = sorted(positions, key=lambda p: p.position_id)
-
-    # Each Backtrader Trade instance presents a position
-    # Trade instances contain TradeHistory entries that present change to this position
-    # with Order instances attached
-    for position in positions:
+        quantity_left = position.get_live_quantity()
+
+        if quantity_left == 0:
+            # We have already generated closing trades for this position
+            # earlier
+            logger.warning("Tried to close position that has enough selling trades to sent it to zero: %s", position)
+            return None
 
         pair = position.pair
-        pair_id = pair.internal_id
-        assert type(pair_id) == int
+        quantity = quantity_left
+        price_structure = self.pricing_model.get_sell_price(self.timestamp, pair, quantity=quantity)
 
-        trade: TradeExecution
+        reserve_asset, reserve_price = self.state.portfolio.get_default_reserve()
 
-        trades = list(position.trades.values())
+        slippage_tolerance = slippage_tolerance or self.default_slippage_tolerance
 
-        for trade in trades:
+        position2, trade, created = self.state.create_trade(
+            self.timestamp,
+            pair,
+            -quantity,  # Negative quantity = sell all
+            None,
+            price_structure.price,
+            trade_type,
+            reserve_asset,
+            reserve_price,  # TODO: Harcoded stablecoin USD exchange rate
+            notes=notes,
+            pair_fee=price_structure.get_fee_percentage(),
+            lp_fees_estimated=price_structure.get_total_lp_fees(),
+            planned_mid_price=price_structure.mid_price,
+            position=position,
+            slippage_tolerance=slippage_tolerance,
+            price_structure=price_structure,
+        )
+        assert position == position2, f"Somehow messed up the close_position() trade.\n" \
+                                      f"Original position: {position}.\n" \
+                                      f"Trade's position: {position2}.\n" \
+                                      f"Trade: {trade}\n" \
+                                      f"Quantity left: {quantity_left}\n" \
+                                      f"Price structure: {price_structure}\n" \
+                                      f"Reserve asset: {reserve_asset}\n"
 
-            history = histories.get(pair_id)
-            if not history:
-                history = histories[pair_id] = AssetTradeHistory()
-
-            # filter out failed trade
-            if trade.executed_at is None:
-                continue
-
-            # Internally negative quantities are for sells
-            quantity = trade.executed_quantity
-            timestamp = pd.Timestamp(trade.executed_at)
-            price = trade.executed_price
-
-            # print("Got event", event, status)
-            assert quantity != 0, f"Got bad quantity for {trade}"
-            # import ipdb ; ipdb.set_trace()
-            assert price > 0, f"Got invalid trade {trade}"
-
-            spot_trade = SpotTrade(
-                pair_id=pair_id,
-                trade_id=trade.trade_id,
-                timestamp=timestamp,
-                price=price,
-                quantity=quantity,
-                commission=0,
-                slippage=0,  # TODO
-                trade_type=trade.trade_type,
-            )
-            history.add_trade(spot_trade)
+        if trades_as_list:
+            return [trade]
+        else:
+            # TODO: Old path - will be removed in the future versions
+            return trade
+
+    def close_all(self) -> List[TradeExecution]:
+        """Close all open positions.
+
+        :return:
+            List of trades that will close existing positions
+        """
+        assert self.is_any_open(), "No positions to close"
 
-    return TradeAnalysis(portfolio, asset_histories=histories)
+        position: TradingPosition
+        trades = []
+        for position in self.state.portfolio.open_positions.values():
+            trade = self.close_position(position)
+            if trade:
+                trades.append(trade)
+
+        return trades
+
+    def estimate_asset_quantity(
+            self,
+            pair: TradingPairIdentifier,
+            dollar_amount: USDollarAmount,
+    ) -> float:
+        """Convert dollar amount to the quantity of a token.
+        
+        Use the market mid-price of the timestamp.
+
+        :param pair:
+            Trading pair of which base pair we estimate.
+
+        :param dollar_amount:
+            Get the asset quantity for this many dollars.
+
+        :return:
+            Asset quantity.
+
+            The sign of the asset quantity is the same as the sign of `dollar_amount` parameter.
+
+            We return as float, because the exact quantity is never known due the price fluctuations and slippage.
+
+        """
+        assert dollar_amount, f"Got dollar amount: {dollar_amount}"
+        timestamp = self.timestamp
+        pricing_model = self.pricing_model
+        price = pricing_model.get_mid_price(timestamp, pair)
+        return float(dollar_amount / price)
```

### Comparing `trade_executor-0.2/tradeexecutor/backtest/backtest_routing.py` & `trade_executor-0.3/tradeexecutor/ethereum/uniswap_v2/uniswap_v2_routing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,288 +1,318 @@
-"""Find routes between historical pairs."""
-
+"""Route trades to different Uniswap v2 like exchanges."""
 import logging
-from collections import defaultdict
-from decimal import Decimal
 from typing import Dict, Set, List, Optional, Tuple
 
-from eth_typing import HexAddress, ChecksumAddress
+from eth_defi.tx import AssetDelta
+from tradeexecutor.state.types import BPS
+from tradingstrategy.chain import ChainId
 from web3 import Web3
-from web3.contract import Contract
+from web3.exceptions import ContractLogicError
+from web3.exceptions import ContractLogicError
 
-from eth_defi.abi import get_deployed_contract
-from eth_defi.gas import estimate_gas_fees
-from eth_defi.token import fetch_erc20_details
 from eth_defi.uniswap_v2.deployment import UniswapV2Deployment, fetch_deployment
 from eth_defi.uniswap_v2.swap import swap_with_slippage_protection
-from tradeexecutor.backtest.simulated_wallet import SimulatedWallet
-from tradeexecutor.ethereum.execution import get_token_for_asset
-from tradeexecutor.ethereum.tx import TransactionBuilder
-from tradeexecutor.state.blockhain_transaction import BlockchainTransaction
+
+from tradeexecutor.ethereum.tx import HotWalletTransactionBuilder
 from tradeexecutor.state.identifier import TradingPairIdentifier, AssetIdentifier
-from tradeexecutor.state.trade import TradeExecution
-from tradeexecutor.strategy.routing import RoutingModel, RoutingState, CannotRouteTrade
-from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse, translate_trading_pair, \
-    translate_token
+from tradeexecutor.state.blockhain_transaction import BlockchainTransaction
 from tradingstrategy.pair import PandasPairUniverse
 
 from tradeexecutor.strategy.universe_model import StrategyExecutionUniverse
-
-
+from tradeexecutor.ethereum.routing_state import (
+    EthereumRoutingState, 
+    route_tokens, # don't remove forwarded import
+    OutOfBalance, # don't remove forwarded import
+    get_base_quote,
+    get_base_quote_intermediary
+)
+from tradeexecutor.ethereum.routing_model import EthereumRoutingModel
+ 
 logger = logging.getLogger(__name__)
 
 
-class OutOfBalance(Exception):
-    """Did not have enough tokens"""
-
-
-class BacktestRoutingState(RoutingState):
+class UniswapV2RoutingState(EthereumRoutingState):
 
     def __init__(self,
                  pair_universe: PandasPairUniverse,
-                 wallet: SimulatedWallet,
-                 ):
-        self.pair_universe = pair_universe
-        self.wallet = wallet
+                 tx_builder: Optional[HotWalletTransactionBuilder] = None,
+                 web3: Optional[Web3] = None,
+                 swap_gas_limit=2_000_000):
+        super().__init__(pair_universe=pair_universe,
+                         tx_builder=tx_builder,
+                         swap_gas_limit=swap_gas_limit,
+                         web3=web3)
+    
+    def __repr__(self):
+        return f"<UniswapV2RoutingState Tx builder: {self.tx_builder} web3: {self.web3}>"
+    
+    def get_uniswap_for_pair(self, factory_router_map: dict, target_pair: TradingPairIdentifier) -> UniswapV2Deployment:
+        """Get a router for a trading pair."""
+        return get_uniswap_for_pair(self.web3, factory_router_map, target_pair)
+    
+    def trade_on_router_two_way(self,
+            uniswap: UniswapV2Deployment,
+            target_pair: TradingPairIdentifier,
+            reserve_asset: AssetIdentifier,
+            reserve_amount: int,
+            max_slippage: float,
+            check_balances: False,
+            asset_deltas: Optional[List[AssetDelta]] = None,
+        ):
+        """Prepare the actual swap. Same for Uniswap V2 and V3.
 
-    def is_route_approved(self, router_address: str):
-        return router_address in self.approved_routes
+        :param check_balances:
+            Check on-chain balances that the account has enough tokens
+            and raise exception if not.
+        """
 
-    def mark_router_approved(self, token_address, router_address):
-        self.approved_routes[router_address].add(token_address)
+        base_token, quote_token = get_base_quote(self.web3, target_pair, reserve_asset)
 
-    def check_has_enough_tokens(
-            self,
-            token: AssetIdentifier,
-            amount: Decimal,
-    ):
-        """Check we have enough buy side tokens to do a trade."""
-        balance = self.wallet.get_balance(token.address)
-        if balance < amount:
-            raise OutOfBalance(f"SimulatedWallet does not have enough {token} tokens to trade. Need {amount}, has {balance}")
+        if check_balances:
+            self.check_has_enough_tokens(quote_token, reserve_amount)
+        
+        if target_pair.fee:
+            bps_fee = target_pair.fee * 10_000
+            bound_swap_func = swap_with_slippage_protection(
+                uniswap,
+                recipient_address=self.tx_builder.get_token_delivery_address(),
+                base_token=base_token,
+                quote_token=quote_token,
+                amount_in=reserve_amount,
+                max_slippage=max_slippage * 100,  # In BPS
+                fee=bps_fee
+            )
+        else:
+            logger.warning("Pair supplied without fee, using default fee")
+            
+            bound_swap_func = swap_with_slippage_protection(
+                uniswap,
+                recipient_address=self.tx_builder.get_token_delivery_address(),
+                base_token=base_token,
+                quote_token=quote_token,
+                amount_in=reserve_amount,
+                max_slippage=max_slippage * 100,  # In BPS
+            )
+        
+        return self.create_signed_transaction(
+            uniswap.router,
+            bound_swap_func,
+            self.swap_gas_limit,
+            asset_deltas,
+        )
 
-    def create_trade(self,
+    def trade_on_router_three_way(self,
+            uniswap: UniswapV2Deployment,
             target_pair: TradingPairIdentifier,
+            intermediary_pair: TradingPairIdentifier,
             reserve_asset: AssetIdentifier,
-            reserve_amount: Decimal,
+            reserve_amount: int,
             max_slippage: float,
-            check_balances: False):
-        """Prepare the actual swap.
+            check_balances: False,
+            asset_deltas: Optional[List[AssetDelta]] = None):
+        """Prepare the actual swap for three way trade.
 
         :param check_balances:
             Check on-chain balances that the account has enough tokens
             and raise exception if not.
         """
 
-        if reserve_asset == target_pair.quote:
-            # Buy with e.g. BUSD
-            base_token = get_token_for_asset(web3, target_pair.base)
-            quote_token = get_token_for_asset(web3, target_pair.quote)
-        elif reserve_asset == target_pair.base:
-            # Sell, flip the direction
-            base_token = get_token_for_asset(web3, target_pair.quote)
-            quote_token = get_token_for_asset(web3, target_pair.base)
-        else:
-            raise RuntimeError(f"Cannot trade {target_pair}")
+        self.validate_pairs(target_pair, intermediary_pair)
+
+        self.validate_exchange(target_pair, intermediary_pair)
+        self.validate_exchange(target_pair, intermediary_pair)
+
+        base_token, quote_token, intermediary_token = get_base_quote_intermediary(self.web3,target_pair, intermediary_pair, reserve_asset)
 
         if check_balances:
             self.check_has_enough_tokens(quote_token, reserve_amount)
 
-        tx = self.create_simulated_trade(target_pair, max)
+        assert target_pair.fee == intermediary_pair.fee, "Uniswap V2 pairs should all have the same fee"
+        
+        if target_pair.fee:
+            bps_fee = target_pair.fee * 10_000
+            bound_swap_func = swap_with_slippage_protection(
+                uniswap,
+                recipient_address=self.tx_builder.get_token_delivery_address(),
+                base_token=base_token,
+                quote_token=quote_token,
+                amount_in=reserve_amount,
+                max_slippage=max_slippage * 100,  # In BPS,
+                intermediate_token=intermediary_token,
+                fee = bps_fee
+            )
+        else:
+            logger.warning("Pair supplied without fee, using default fee")
+            
+            bound_swap_func = swap_with_slippage_protection(
+                uniswap,
+                recipient_address=self.tx_builder.get_token_delivery_address(),
+                base_token=base_token,
+                quote_token=quote_token,
+                amount_in=reserve_amount,
+                max_slippage=max_slippage * 100,  # In BPS,
+                intermediate_token=intermediary_token,
+            )
+
+        tx = self.tx_builder.sign_transaction(
+            uniswap.router,
+            bound_swap_func,
+            self.swap_gas_limit,
+            asset_deltas
+        )
         return [tx]
 
 
-class BacktestRoutingModel(RoutingModel):
+class UniswapV2SimpleRoutingModel(EthereumRoutingModel):
     """A simple router that does not optimise the trade execution cost.
 
     - Able to trade on multiple exchanges
 
     - Able to three-way trades through predefined intermediary hops,
       either on the exchange itself or some outside exchange
     """
 
     def __init__(self,
                  factory_router_map: Dict[str, Tuple[str, Optional[str]]],
                  allowed_intermediary_pairs: Dict[str, str],
                  reserve_token_address: str,
+                 chain_id: Optional[ChainId] = None,
+                 trading_fee: Optional[BPS] = None # TODO remove
                  ):
         """
         :param factory_router_map:
             Defines router smart contracts to be used with each DEX.
             Each Uniswap v2 is uniquely identified by its factory contract.
             Addresses always lowercase.
 
+            Map of factory address -> (router address, init code hash tuple)
+
         :param allowed_intermediary_pairs:
 
             Quote token address -> pair smart contract address mapping.
 
             Because we hold our reserves only in one currecy e.g. BUSD
             and we want to trade e.g. Cake/BNB pairs, we need to whitelist
             BNB as an allowed intermediary token.
             This makes it possible to do BUSD -> BNB -> Cake trade.
             This set is the list of pair smart contract addresses that
             are allowed to be used as a hop.
 
+        :param trading_fee:
+            Trading fee express as float bps.
+
+            This is the LP fee applied to all swaps.
+
+        :param chain_id:
+            Store the chain id for which these routes were generated for.
+
         :param reserve_token_address:
             Token address of our reserve currency.
             Relevent for buy/sell routing.
             Lowercase.
         """
 
-        assert type(factory_router_map) == dict
-        assert type(allowed_intermediary_pairs) == dict
-        assert type(reserve_token_address) == str
-
-        assert reserve_token_address.lower() == reserve_token_address
-
-        # Convert all key addresses to lowercase to
-        # avoid mix up with Ethereum address checksums
-        self.factory_router_map = {k.lower(): v for k, v in factory_router_map.items()}
-        self.allowed_intermediary_pairs = {k.lower(): v.lower() for k, v in allowed_intermediary_pairs.items()}
-        self.reserve_token_address = reserve_token_address
-
-    def get_reserve_asset(self, pair_universe: PandasPairUniverse) -> AssetIdentifier:
-        """Translate our reserve token address tok an asset description."""
-        assert pair_universe is not None, "Pair universe missing"
-        reserve_token = pair_universe.get_token(self.reserve_token_address)
-        assert reserve_token, f"Pair universe does not contain our reserve asset {self.reserve_token_address}"
-        return translate_token(reserve_token)
-
-    def trade(self,
-              routing_state: BacktestRoutingState,
-              target_pair: TradingPairIdentifier,
-              reserve_asset: AssetIdentifier,
-              reserve_asset_amount: Decimal,  # Raw amount of the reserve asset
-              max_slippage: float=0.01,
-              check_balances=False,
-              intermediary_pair: Optional[TradingPairIdentifier] = None,
-              ) -> List[BlockchainTransaction]:
-        """
+        super().__init__(allowed_intermediary_pairs, reserve_token_address, chain_id)
 
-        :param routing_state:
-        :param target_pair:
-        :param reserve_asset:
-        :param reserve_asset_amount:
-        :param max_slippage:
-            Max slippage per trade. 0.01 is 1%.
-        :param check_balances:
-            Check on-chain balances that the account has enough tokens
-            and raise exception if not.
-        :param intermediary_pair:
-            If the trade needs to be routed through a intermediary pool, e.g.
-            BUSD -> BNB -> Cake.
-        :return:
-            List of prepared transactions to make this trade.
-            These transactions, like approve() may relate to the earlier
-            transactions in the `routing_state`.
-        """
+        assert type(factory_router_map) == dict
+        self.factory_router_map = self.convert_address_dict_to_lower(factory_router_map)
+        
+        # TODO remove trading_fee
+        if trading_fee is not None:
+            assert trading_fee >= 0, f"Got fee: {trading_fee}"
+            assert trading_fee <= 1, f"Got fee: {trading_fee}"
 
-        assert type(reserve_asset_amount) == int
-        assert max_slippage is not None, "Max slippage must be given"
-        assert type(max_slippage) == float
-        assert reserve_asset_amount > 0, f"For sells, switch reserve_asset to different token. Got target_pair: {target_pair}, reserve_asset: {reserve_asset}, amount: {reserve_asset_amount}"
-
-        # Our reserves match directly the asset on trading pair
-        # -> we can do one leg trade
-        if not intermediary_pair:
-            if target_pair.quote == reserve_asset or target_pair.base == reserve_asset:
-                return self.routing_state.create_and_complete_trade(
-                    target_pair,
-                    reserve_asset,
-                    reserve_asset_amount,
-                    max_slippage=max_slippage,
-                    check_balances=check_balances,
-                )
-            raise RuntimeError(f"Do not how to trade reserve {reserve_asset} with {target_pair}")
-        else:
+        self.trading_fee = trading_fee
 
-            assert intermediary_pair.pool_address.lower() in self.allowed_intermediary_pairs.values(), f"Does not how to trade a pair. Got intermediary pair {intermediary_pair} that is not allowed, allowed intermediary pairs are {self.allowed_intermediary_pairs}"
+    def get_default_trading_fee(self) -> Optional[float]:
+        return self.trading_fee
 
-            return self.routing_state.create_and_complete_trade(
-                target_pair,
-                reserve_asset,
-                reserve_asset_amount,
-                max_slippage=max_slippage,
-                check_balances=check_balances,
-                intermediary_pair=intermediary_pair,
-            )
+    def create_routing_state(self,
+                             universe: StrategyExecutionUniverse,
+                             execution_details: dict) -> UniswapV2RoutingState:
+        """Create a new routing state for this cycle.
 
-    def route_pair(self, pair_universe: PandasPairUniverse, trading_pair: TradingPairIdentifier) \
-            -> Tuple[TradingPairIdentifier, Optional[TradingPairIdentifier]]:
-        """Return Uniswap routing information (path components) for a trading pair.
+        - Connect routing to web3 and hot wallet
 
-        For three-way pairs, figure out the intermedia step.
+        - Read on-chain data on what gas fee we are going to use
 
-        :return:
-            (router address, target pair, intermediate pair) tuple
+        - Setup transaction builder based on this information
         """
 
-        assert isinstance(trading_pair, TradingPairIdentifier)
-
-        reserve_asset = self.get_reserve_asset(pair_universe)
-
-        # We can directly do a two-way trade
-        if trading_pair.quote == reserve_asset:
-            return trading_pair, None
-
-        # Only issue for legacy code
-        assert pair_universe, "PairUniverse must be given so that we know how to route three way trades"
-
-        # Try to find a mid-hop pool for the trade
-        intermediate_pair_contract_address = self.allowed_intermediary_pairs.get(trading_pair.quote.address.lower())
+        return super().create_routing_state(universe, execution_details, UniswapV2RoutingState)
 
-        if not intermediate_pair_contract_address:
-            raise CannotRouteTrade(f"Does not know how to trade pair {trading_pair} - supported intermediate tokens are {list(self.allowed_intermediary_pairs.keys())}")
-
-        dex_pair = pair_universe.get_pair_by_smart_contract(intermediate_pair_contract_address)
-        assert dex_pair is not None, f"Pair universe did not contain pair for a pair contract address {intermediate_pair_contract_address}, quote token is {trading_pair.quote}"
-
-        intermediate_pair = translate_trading_pair(dex_pair)
-        if not intermediate_pair:
-            raise CannotRouteTrade(f"Universe does not have a trading pair with smart contract address {intermediate_pair_contract_address}")
-
-        return trading_pair, intermediate_pair
-
-    def setup_internal(self, routing_state: RoutingState, trade: TradeExecution):
-        """Simulate trade braodcast and mark it as success."""
-
-        # 2. Capital allocation
-        nonce, tx_hash = routing_state.wallet.fetch_nonce_and_tx_hash()
-
-        trade.blockchain_transactions = [
-            BlockchainTransaction(
-                nonce=nonce,
-                tx_hash=tx_hash,
-            )
-        ]
-
-    def setup_trades(self,
-                     routing_state: BacktestRoutingState,
-                     trades: List[TradeExecution],
-                     check_balances=False):
-        """Strategy and live execution connection.
-
-        Turns abstract strategy trades to real blockchain transactions.
-
-        - Modifies TradeExecution objects in place and associates a blockchain transaction for each
-
-        - Signs tranactions from the hot wallet and broadcasts them to the network
-
-        :param check_balances:
-            Check that the wallet has enough reserves to perform the trades
-            before executing them. Because we are selling before buying.
-            sometimes we do no know this until the sell tx has been completed.
-
-        :param max_slippage:
-            Max slippaeg tolerated per trade. 0.01 is 1%.
+    def perform_preflight_checks_and_logging(self,
+        pair_universe: PandasPairUniverse):
+        """"Checks the integrity of the routing.
 
+        - Called from check-wallet to see our routing and balances are good
         """
-        for t in trades:
-            self.setup_internal(routing_state, t)
 
-    def create_routing_state(self,
-                     universe: TradingStrategyUniverse,
-                     execution_details: dict) -> BacktestRoutingState:
-        """Create a new routing state for this cycle."""
-        assert isinstance(universe, TradingStrategyUniverse)
-        wallet = execution_details["wallet"]
-        return BacktestRoutingState(universe.universe.pairs, wallet)
+        logger.info("Routing details")
+        for factory, router in self.factory_router_map.items():
+            logger.info("  Factory %s uses router %s", factory, router[0])
+
+        self.reserve_asset_logging(pair_universe)
+        
+    def make_direct_trade(
+        self, 
+        routing_state: EthereumRoutingState,
+        target_pair: TradingPairIdentifier,
+        reserve_asset: AssetIdentifier,
+        reserve_amount: int,
+        max_slippage: float,
+        check_balances=False,
+        asset_deltas: Optional[List[AssetDelta]] = None,
+    ) -> List[BlockchainTransaction]:
+        
+        return super().make_direct_trade(
+            routing_state,
+            target_pair,
+            reserve_asset,
+            reserve_amount,
+            max_slippage,
+            self.factory_router_map,
+            check_balances,
+            asset_deltas=asset_deltas,
+        )
+    
+    def make_multihop_trade(
+        self,
+        routing_state: EthereumRoutingState,
+        target_pair: TradingPairIdentifier,
+        intermediary_pair: TradingPairIdentifier,
+        reserve_asset: AssetIdentifier,
+        reserve_amount: int,
+        max_slippage: float,
+        check_balances=False,
+        asset_deltas: Optional[List[AssetDelta]] = None,
+    ) -> List[BlockchainTransaction]:
+        
+        return super().make_multihop_trade(
+            routing_state,
+            target_pair,
+            intermediary_pair,
+            reserve_asset,
+            reserve_amount,
+            max_slippage,
+            self.factory_router_map,
+            check_balances,
+            asset_deltas=asset_deltas,
+        )
+    
+    
+        
+def get_uniswap_for_pair(web3: Web3, factory_router_map: dict, target_pair: TradingPairIdentifier) -> UniswapV2Deployment:
+    """Get a router for a trading pair."""
+    assert target_pair.exchange_address, f"Exchange address missing for {target_pair}"
+    factory_address = Web3.to_checksum_address(target_pair.exchange_address)
+    router_address, init_code_hash = factory_router_map[factory_address.lower()]
+
+    try:
+        return fetch_deployment(
+            web3,
+            factory_address,
+            Web3.to_checksum_address(router_address),
+            init_code_hash=init_code_hash,
+        )
+    except ContractLogicError as e:
+        raise RuntimeError(f"Could not fetch deployment data for router address {router_address} (factory {factory_address}) - data is likely wrong") from e
```

### Comparing `trade_executor-0.2/tradeexecutor/backtest/backtest_runner.py` & `trade_executor-0.3/tradeexecutor/backtest/backtest_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,37 +4,40 @@
 from contextlib import AbstractContextManager
 from dataclasses import dataclass
 from decimal import Decimal
 from pathlib import Path
 from queue import Queue
 from typing import Optional, Callable, Tuple
 
+import pandas as pd
+
 from tradeexecutor.backtest.backtest_execution import BacktestExecutionModel
 from tradeexecutor.backtest.backtest_pricing import BacktestSimplePricingModel
 from tradeexecutor.backtest.backtest_routing import BacktestRoutingModel
-from tradeexecutor.backtest.backtest_sync import BacktestSyncer
+from tradeexecutor.backtest.backtest_sync import BacktestSyncer, BacktestSyncModel
 from tradeexecutor.backtest.backtest_valuation import BacktestValuationModel
 from tradeexecutor.backtest.simulated_wallet import SimulatedWallet
 from tradeexecutor.cli.log import setup_notebook_logging
 from tradeexecutor.cli.loop import ExecutionLoop
-from tradeexecutor.ethereum.default_routes import get_routing_model, get_backtest_routing_model
+from tradeexecutor.ethereum.routing_data import get_routing_model, get_backtest_routing_model
 from tradeexecutor.state.state import State
 from tradeexecutor.state.store import NoneStore
 from tradeexecutor.strategy.approval import UncheckedApprovalModel, ApprovalModel
 from tradeexecutor.strategy.cycle import CycleDuration
 from tradeexecutor.strategy.description import StrategyExecutionDescription
 from tradeexecutor.strategy.execution_context import ExecutionContext, ExecutionMode
 from tradeexecutor.strategy.pandas_trader.runner import PandasTraderRunner
 from tradeexecutor.strategy.strategy_module import parse_strategy_module,  \
     DecideTradesProtocol, CreateTradingUniverseProtocol, CURRENT_ENGINE_VERSION
 from tradeexecutor.strategy.reserve_currency import ReserveCurrency
 from tradeexecutor.strategy.default_routing_options import TradeRouting
 from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse,  \
     DefaultTradingStrategyUniverseModel
 from tradeexecutor.strategy.universe_model import StaticUniverseModel, UniverseOptions
+from tradeexecutor.utils.accuracy import setup_decimal_accuracy
 from tradeexecutor.utils.timer import timed_task
 from tradingstrategy.client import Client
 from tradingstrategy.timebucket import TimeBucket
 
 
 @dataclass
 class BacktestSetup:
@@ -53,15 +56,15 @@
     cycle_duration: Optional[CycleDuration]
     universe: Optional[TradingStrategyUniverse]
     wallet: SimulatedWallet
     state: State
     pricing_model: Optional[BacktestSimplePricingModel]
     routing_model: Optional[BacktestRoutingModel]
     execution_model: BacktestExecutionModel
-    sync_method: BacktestSyncer
+    sync_model: BacktestSyncModel
 
     trading_strategy_engine_version: str
     trade_routing: TradeRouting
     reserve_currency: ReserveCurrency
     decide_trades: DecideTradesProtocol
     create_trading_universe: Optional[CreateTradingUniverseProtocol]
 
@@ -73,15 +76,15 @@
     # strategy_module: StrategyModuleInformation
 
     def backtest_static_universe_strategy_factory(
             self,
             *ignore,
             execution_model: BacktestExecutionModel,
             execution_context: ExecutionContext,
-            sync_method: BacktestSyncer,
+            sync_model: BacktestSyncModel,
             pricing_model_factory: Callable,
             valuation_model_factory: Callable,
             client: Client,
             timed_task_context_manager: AbstractContextManager,
             approval_model: ApprovalModel,
             **kwargs) -> StrategyExecutionDescription:
         """Create a strategy description and runner based on backtest parameters in this setup."""
@@ -99,18 +102,19 @@
             routing_model = get_backtest_routing_model(trade_routing, self.reserve_currency)
 
         runner = PandasTraderRunner(
             timed_task_context_manager=timed_task_context_manager,
             execution_model=execution_model,
             approval_model=approval_model,
             valuation_model_factory=valuation_model_factory,
-            sync_method=sync_method,
+            sync_model=sync_model,
             pricing_model_factory=pricing_model_factory,
             routing_model=routing_model,
             decide_trades=self.decide_trades,
+            execution_context=execution_context,
         )
 
         if self.universe:
             # Trading universe is set by unit tests
             universe_model = StaticUniverseModel(self.universe)
         else:
             # Trading universe is loaded by the strategy script
@@ -134,45 +138,50 @@
         cycle_duration: CycleDuration,
         initial_deposit: int,
         universe: TradingStrategyUniverse,
         routing_model: BacktestRoutingModel,
         max_slippage=0.01,
         validate_strategy_module=False,
         candle_time_frame: Optional[TimeBucket]=None,
+        allow_missing_fees=False,
     ):
     """High-level entry point for setting up a single backtest for a predefined universe.
 
     The trading universe creation from the strategy is skipped,
     instead of you can pass your own universe e.g. synthetic universe.
     This is useful for running backtests against synthetic universes.
 
     :param cycle_duration:
         Override the default strategy cycle duration
 
+    :param allow_missing_fees:
+        Legacy workaround
+
     :param candle_time_frame:
         Override the default strategy candle time bucket
 
     """
 
     assert initial_deposit > 0
 
     wallet = SimulatedWallet()
 
-    deposit_syncer = BacktestSyncer(wallet, Decimal(initial_deposit))
+    # deposit_syncer = BacktestSyncer(wallet, Decimal(initial_deposit))
+    sync_model = BacktestSyncModel(wallet, Decimal(initial_deposit))
 
     # Create the initial state
     state = State()
-    events = deposit_syncer(state.portfolio, start_at, universe.reserve_assets)
-    assert len(events) == 1
-    token, usd_exchange_rate = state.portfolio.get_default_reserve_currency()
+    events = sync_model.sync_treasury(start_at, state, universe.reserve_assets)
+    # assert len(events) == 1
+    token, usd_exchange_rate = state.portfolio.get_default_reserve()
     assert usd_exchange_rate == 1
     assert state.portfolio.get_current_cash() == initial_deposit
 
     # Set up execution and pricing
-    pricing_model = BacktestSimplePricingModel(universe.universe.candles, routing_model)
+    pricing_model = BacktestSimplePricingModel(universe.universe.candles, routing_model, allow_missing_fees=allow_missing_fees)
     execution_model = BacktestExecutionModel(wallet, max_slippage)
 
     # Load strategy Python file
     strategy_mod_exports: dict = runpy.run_path(strategy_path)
     strategy_module = parse_strategy_module(strategy_mod_exports)
 
     if validate_strategy_module:
@@ -188,15 +197,15 @@
         universe_options=universe_options,
         wallet=wallet,
         state=state,
         universe=universe,
         pricing_model=pricing_model,
         execution_model=execution_model,
         routing_model=routing_model,
-        sync_method=deposit_syncer,
+        sync_model=sync_model,
         decide_trades=strategy_module.decide_trades,
         create_trading_universe=None,
         reserve_currency=strategy_module.reserve_currency,
         trade_routing=strategy_module.trade_routing,
         trading_strategy_engine_version=strategy_module.trading_strategy_engine_version,
     )
 
@@ -222,15 +231,16 @@
         Override the default strategy candle time bucket
     """
 
     assert isinstance(strategy_path, Path), f"Got {strategy_path}"
     assert initial_deposit > 0
 
     wallet = SimulatedWallet()
-    deposit_syncer = BacktestSyncer(wallet, Decimal(initial_deposit))
+    # deposit_syncer = BacktestSyncer(wallet, Decimal(initial_deposit))
+    sync_model = BacktestSyncModel(wallet, Decimal(initial_deposit))
 
     execution_model = BacktestExecutionModel(wallet, max_slippage)
 
     # Load strategy Python file
     strategy_mod_exports: dict = runpy.run_path(strategy_path)
     strategy_module = parse_strategy_module(strategy_mod_exports)
 
@@ -245,63 +255,83 @@
         universe_options=universe_options,
         wallet=wallet,
         state=State(),
         universe=None,
         pricing_model=None,  # Will be set up later
         execution_model=execution_model,
         routing_model=None, # Will be set up later
-        sync_method=deposit_syncer,
+        sync_model=sync_model,
         decide_trades=strategy_module.decide_trades,
         create_trading_universe=strategy_module.create_trading_universe,
         reserve_currency=strategy_module.reserve_currency,
         trade_routing=strategy_module.trade_routing,
         trading_strategy_engine_version=strategy_module.trading_strategy_engine_version,
     )
 
 
 def run_backtest(
         setup: BacktestSetup,
-        client: Optional[Client]=None) -> Tuple[State, TradingStrategyUniverse, dict]:
+        client: Optional[Client]=None,
+        allow_missing_fees=False,
+) -> Tuple[State, TradingStrategyUniverse, dict]:
     """Run a strategy backtest.
 
     Loads strategy file, construct trading universe is real data
     downloaded with Trading Strategy client.
 
+    :param allow_missing_fees:
+        Legacy workaround
+
     :return:
         Tuple(the final state of the backtest, trading universe, debug dump)
     """
 
     # State is pristine and not used yet
     assert len(list(setup.state.portfolio.get_all_trades())) == 0
 
     # Create empty state for this backtest
     store = NoneStore(setup.state)
 
     # Captured in teh callback
     backtest_universe: TradingStrategyUniverse = None
 
-    def pricing_model_factory(execution_model, universe, routing_model):
+    def pricing_model_factory(execution_model, universe: TradingStrategyUniverse, routing_model):
         if setup.pricing_model:
             # Use pricing model given inline
             return setup.pricing_model
 
-        # Construct a backtest pricing model
-        return BacktestSimplePricingModel(universe, routing_model)
+        return BacktestSimplePricingModel(
+            universe,
+            routing_model,
+            data_delay_tolerance=guess_data_delay_tolerance(universe),
+            allow_missing_fees=allow_missing_fees,
+        )
 
     def valuation_model_factory(pricing_model):
         return BacktestValuationModel(pricing_model)
 
     if not setup.universe:
-        def backtest_setup(state: State, universe: TradingStrategyUniverse, deposit_syncer: BacktestSyncer):
+        def backtest_setup(state: State, universe: TradingStrategyUniverse, sync_model: BacktestSyncModel):
+            # Use strategy script create_trading_universe() hook to construct the universe
             # Called on the first cycle. Only if the universe is not predefined.
             # Create the initial state of the execution.
             nonlocal backtest_universe
-            events = deposit_syncer(state.portfolio, setup.start_at, universe.reserve_assets)
-            assert len(events) == 1, f"Did not get 1 initial backtest deposit event, got {len(events)} events"
-            token, usd_exchange_rate = state.portfolio.get_default_reserve_currency()
+
+            # Mark backtest stop loss data being available,
+            # after create_trading_universe() has loaded it
+            if universe.has_stop_loss_data():
+                setup.execution_model.stop_loss_data_available = True
+
+            #events = deposit_syncer(state.portfolio, setup.start_at, universe.reserve_assets)
+            #assert len(events) == 1, f"Did not get 1 initial backtest deposit event, got {len(events)} events.\nMake sure you did not call backtest_setup() twice?"
+
+            events = sync_model.sync_treasury(setup.start_at, state, list(universe.reserve_assets))
+            # assert len(events) == 1, f"Did not get 1 initial backtest deposit event, got {len(events)} events.\nMake sure you did not call backtest_setup() twice?"
+
+            token, usd_exchange_rate = state.portfolio.get_default_reserve()
             assert usd_exchange_rate == 1
             backtest_universe = universe
     else:
         backtest_universe = setup.universe
         def backtest_setup(state: State, universe: TradingStrategyUniverse, deposit_syncer: BacktestSyncer):
             pass
 
@@ -311,29 +341,30 @@
     )
 
     main_loop = ExecutionLoop(
         name=setup.name,
         command_queue=Queue(),
         execution_model=setup.execution_model,
         execution_context=execution_context,
-        sync_method=setup.sync_method,
+        sync_model=setup.sync_model,
         approval_model=UncheckedApprovalModel(),
         pricing_model_factory=pricing_model_factory,
         valuation_model_factory=valuation_model_factory,
         store=store,
         client=client,
         strategy_factory=setup.backtest_static_universe_strategy_factory,
         cycle_duration=setup.cycle_duration,
         stats_refresh_frequency=None,
         position_trigger_check_frequency=None,
         max_data_delay=None,
         debug_dump_file=None,
         backtest_start=setup.start_at,
         backtest_end=setup.end_at,
         backtest_setup=backtest_setup,
+        backtest_candle_time_frame_override=setup.universe_options.candle_time_bucket_override,
         tick_offset=datetime.timedelta(seconds=1),
         trade_immediately=True,
     )
 
     debug_dump = main_loop.run()
 
     return setup.state, backtest_universe, debug_dump
@@ -345,22 +376,24 @@
     end_at: datetime.datetime,
     client: Optional[Client],
     decide_trades: DecideTradesProtocol,
     cycle_duration: CycleDuration,
     initial_deposit: float,
     reserve_currency: ReserveCurrency,
     trade_routing: Optional[TradeRouting],
-    create_trading_universe: Optional[CreateTradingUniverseProtocol]=None,
-    universe: Optional[TradingStrategyUniverse]=None,
-    routing_model: Optional[BacktestRoutingModel]=None,
+    create_trading_universe: Optional[CreateTradingUniverseProtocol] = None,
+    universe: Optional[TradingStrategyUniverse] = None,
+    routing_model: Optional[BacktestRoutingModel] = None,
     max_slippage=0.01,
-    candle_time_frame: Optional[TimeBucket]=None,
+    candle_time_frame: Optional[TimeBucket] = None,
     log_level=logging.WARNING,
     data_preload=True,
+    data_delay_tolerance: Optional[pd.Timedelta] = None,
     name: str="backtest",
+    allow_missing_fees=False,
 ) -> Tuple[State, TradingStrategyUniverse, dict]:
     """Run backtests for given decide_trades and create_trading_universe functions.
 
     Does not load strategy from a separate .py file.
     Useful for running strategies directly from notebooks.
 
     :param name:
@@ -410,14 +443,33 @@
     :param log_level:
         Python logging level to display log messages during the backtest run.
 
     :param data_preload:
         Before the backtesting begins, load and cache datasets
         with nice progress bar to the user.
 
+    :param data_delay_tolerance:
+        What is the maximum hours/days lookup we allow in the backtesting when we ask for the latest price of an asset.
+
+        The asset price fetch might fail due to sparse candle data - trades have not been made or the blockchain was halted during the price look-up period.
+        Because there are no trades we cannot determine what was the correct asset price using {data_delay_tolerance} data tolerance delay.
+
+        The default value `None` tries to guess the value based on the univerity candle timeframe,
+        but often this guess is incorrect as only analysing every pair data gives a correct answer.
+
+        The workarounds include ignoring assets in your backtest that might not have price data (look up they have enough valid candles
+        at the decide_trades timestamp) or simply increasing this parameter.
+
+        This parameter is passed to :py:class:`tradeexecutor.backtest.backtest_pricing.BacktestSimplePricingModel`.
+
+    :param allow_missing_fees:
+        Allow synthetic data to lack fee information.
+
+        Only set in legacy backtests.
+
     :return:
         tuple (State of a completely executed strategy, trading strategy universe, debug dump dict)
     """
 
     if ignore:
         # https://www.python.org/dev/peps/pep-3102/
         raise TypeError("Only keyword arguments accepted")
@@ -426,31 +478,44 @@
     assert isinstance(end_at, datetime.datetime)
     assert initial_deposit > 0
 
     # Setup our special logging level if not done yet.
     # (Not done when called from notebook)
     setup_notebook_logging(log_level)
 
+    # Make sure no rounding bugs
+    setup_decimal_accuracy()
+
     wallet = SimulatedWallet()
-    deposit_syncer = BacktestSyncer(wallet, Decimal(initial_deposit))
+    # deposit_syncer = BacktestSyncer(wallet, Decimal(initial_deposit))
+    sync_model = BacktestSyncModel(wallet, Decimal(initial_deposit))
 
     stop_loss_data_available = universe.has_stop_loss_data() if universe else False
 
     execution_model = BacktestExecutionModel(
         wallet,
         max_slippage,
         stop_loss_data_available=stop_loss_data_available,
     )
 
     if universe:
         if not routing_model:
             assert trade_routing, "You just give either routing_mode or trade_routing"
             assert reserve_currency, "Reserve current must be given to generate routing model"
             routing_model = get_backtest_routing_model(trade_routing, reserve_currency)
-        pricing_model = BacktestSimplePricingModel(universe.universe.candles, routing_model)
+
+        if data_delay_tolerance is None:
+            data_delay_tolerance = guess_data_delay_tolerance(universe)
+
+        pricing_model = BacktestSimplePricingModel(
+            universe.universe.candles,
+            routing_model,
+            data_delay_tolerance=data_delay_tolerance,
+            allow_missing_fees=allow_missing_fees,
+        )
     else:
         assert create_trading_universe, "Must give create_trading_universe if no universe given"
         pricing_model = None
 
     universe_options = UniverseOptions(
         candle_time_bucket_override=candle_time_frame,
     )
@@ -462,19 +527,33 @@
         universe_options=universe_options,
         wallet=wallet,
         state=State(name=name),
         universe=universe,
         pricing_model=pricing_model,  # Will be set up later
         execution_model=execution_model,
         routing_model=routing_model,  # Use given routing model if available
-        sync_method=deposit_syncer,
+        sync_model=sync_model,
         decide_trades=decide_trades,
         create_trading_universe=create_trading_universe,
         reserve_currency=reserve_currency,
         trade_routing=trade_routing,
         trading_strategy_engine_version=CURRENT_ENGINE_VERSION,
         name=name,
         data_preload=data_preload,
     )
 
-    return run_backtest(backtest_setup, client)
+    return run_backtest(backtest_setup, client, allow_missing_fees=True)
+
+
+def guess_data_delay_tolerance(universe: TradingStrategyUniverse) -> pd.Timedelta:
+    """Try to dynamically be flexible with the backtesting pricing look up.
+
+    This could work around some data quality issues or early historical data.
+    """
+    if universe.universe.time_bucket == TimeBucket.d7:
+        data_delay_tolerance = pd.Timedelta("9d")
+    else:
+        data_delay_tolerance = pd.Timedelta("2d")
+
+    return data_delay_tolerance
+
```

### Comparing `trade_executor-0.2/tradeexecutor/backtest/backtest_valuation.py` & `trade_executor-0.3/tradeexecutor/backtest/backtest_valuation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import datetime
 from typing import Tuple
 
 from tradeexecutor.backtest.backtest_pricing import BacktestSimplePricingModel
-from tradeexecutor.ethereum.uniswap_v2_live_pricing import UniswapV2LivePricing
 from tradeexecutor.state.position import TradingPosition
 from tradeexecutor.state.types import USDollarAmount
 from tradeexecutor.strategy.valuation import ValuationModel
 
 
 class BacktestValuationModel(ValuationModel):
-    """Re-value assets based on their on-chain backtest dataset price."""
+    """Re-value assets based on their on-chain backtest dataset price.
+
+    Each asset is valued at its market sell price estimation.
+    """
 
     def __init__(self, pricing_model: BacktestSimplePricingModel):
         assert pricing_model, "pricing_model missing"
         self.pricing_model = pricing_model
 
     def __call__(self,
                  ts: datetime.datetime,
                  position: TradingPosition) -> Tuple[datetime.datetime, USDollarAmount]:
 
         assert isinstance(ts, datetime.datetime)
-        assert ts.minute == 0, f"Timestamp sanity check failed {ts}"
-        assert ts.second == 0, f"Timestamp sanity check failed {ts}"
+        assert ts.second == 0, f"Timestamp sanity check failed, does not have even seconds: {ts}"
 
         pair = position.pair
 
         assert position.is_long(), "Short not supported"
         quantity = position.get_quantity()
-        price = self.pricing_model.get_sell_price(ts, pair, quantity)
-        return ts, float(price)
+        trade_price = self.pricing_model.get_sell_price(ts, pair, quantity)
+        return ts, float(trade_price.price)
 
 
 def backtest_valuation_factory(pricing_model):
     return BacktestValuationModel(pricing_model)
```

### Comparing `trade_executor-0.2/tradeexecutor/backtest/data_preload.py` & `trade_executor-0.3/tradeexecutor/backtest/data_preload.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 """Backtesting dataset load progress baring."""
 
 from typing import Optional, Callable
 
 import pandas as pd
 
-from tradingstrategy.client import Client
+from tradeexecutor.strategy.strategy_module import CreateTradingUniverseProtocol
+from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse
+from tradingstrategy.client import Client, BaseClient
 from tradingstrategy.environment.jupyter import download_with_tqdm_progress_bar
 
 from tradeexecutor.strategy.execution_context import ExecutionMode, ExecutionContext
 from tradeexecutor.strategy.universe_model import UniverseOptions
 from tradeexecutor.utils.timer import timed_task
 
 
 def preload_data(
-        client: Client,
-        create_trading_universe: Callable,
+        client: BaseClient,
+        create_trading_universe: CreateTradingUniverseProtocol,
         universe_options: UniverseOptions,
-):
+) -> TradingStrategyUniverse:
     """Show nice progress bar for setting up data fees for backtesting trading universe.
 
     - We trigger call to `create_trading_universe` before the actual backtesting begins
 
     - The client is in a mode that it will display dataset download progress bars.
       We do not display these progress bars by default, as it could a bit noisy.
     """
 
     # Switch to the progress bar downloader
     # TODO: Make this cleaner
-    client.transport.download_func = download_with_tqdm_progress_bar
+    if isinstance(client, Client):
+        client.transport.download_func = download_with_tqdm_progress_bar
 
     execution_context = ExecutionContext(
         mode=ExecutionMode.data_preload,
         timed_task_context_manager=timed_task,
     )
 
-    create_trading_universe(
+    return create_trading_universe(
         pd.Timestamp.now(),
         client,
         execution_context,
         universe_options=universe_options,
     )
```

### Comparing `trade_executor-0.2/tradeexecutor/backtest/simulated_wallet.py` & `trade_executor-0.3/tradeexecutor/backtest/simulated_wallet.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/cli/approval.py` & `trade_executor-0.3/tradeexecutor/cli/approval.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/cli/env.py` & `trade_executor-0.3/tradeexecutor/cli/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,12 +30,12 @@
         envvar = p.envvar
         if envvar:
             # Option --help does not have envvar, etc.
             result.append(
                 EnvVarDescription(
                     envvar,
                     p.help,
-                    p.type,
+                    p.cause,
                 )
             )
 
     return result
```

### Comparing `trade_executor-0.2/tradeexecutor/cli/latest_release.py` & `trade_executor-0.3/tradeexecutor/cli/latest_release.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/cli/main.py` & `trade_executor-0.3/tradeexecutor/cli/loop.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,810 +1,975 @@
-"""Command-line entry point for the daemon build on the top of Typer."""
-import datetime
+"""Trade executor main loop."""
+
 import logging
-import os.path
-from decimal import Decimal
+import datetime
+import pickle
+import random
 from pathlib import Path
 from queue import Queue
-from typing import Optional, Callable, Tuple
-from importlib.metadata import version
+from typing import Optional, Callable, List, cast, Tuple
 
-import typer
-from tradingstrategy.chain import ChainId
-from tradingstrategy.timebucket import TimeBucket
+import pandas as pd
+from apscheduler.events import EVENT_JOB_ERROR
 
-from web3 import Web3
+from tradeexecutor.cli.watchdog import create_watchdog_registry, register_worker, mark_alive, start_background_watchdog, \
+    WatchdogMode
+from tradeexecutor.statistics.summary import calculate_summary_statistics
+from tradeexecutor.strategy.pandas_trader.decision_trigger import wait_for_universe_data_availability_jsonl
+from tradeexecutor.strategy.routing import RoutingModel
+from tradeexecutor.strategy.run_state import RunState
+from tradeexecutor.strategy.strategy_cycle_trigger import StrategyCycleTrigger
+
+try:
+    from apscheduler.executors.pool import ThreadPoolExecutor
+    from apscheduler.schedulers.blocking import BlockingScheduler
+except ImportError:
+    # apscheduler is only required in live trading
+    pass
+
+try:
+    from tqdm_loggable.auto import tqdm
+except ImportError:
+    # tqdm_loggable is only available at the live execution,
+    # but fallback to normal TQDM auto mode
+    from tqdm.auto import tqdm
 
-from eth_defi.balances import fetch_erc20_balances_by_token_list
-from eth_defi.gas import GasPriceMethod
-from eth_defi.token import fetch_erc20_details
-from eth_defi.hotwallet import HotWallet
-
-from tradeexecutor.backtest.backtest_execution import BacktestExecutionModel
-from tradeexecutor.backtest.backtest_pricing import backtest_pricing_factory
-from tradeexecutor.backtest.backtest_sync import BacktestSyncer
-from tradeexecutor.backtest.backtest_valuation import backtest_valuation_factory
-from tradeexecutor.backtest.simulated_wallet import SimulatedWallet
-from tradeexecutor.cli.result import display_backtesting_results
-from tradeexecutor.cli.testtrade import make_test_trade
-from tradeexecutor.ethereum.web3config import Web3Config
-from tradeexecutor.state.metadata import Metadata
+from tradeexecutor.backtest.backtest_pricing import BacktestSimplePricingModel
 from tradeexecutor.state.state import State
+from tradeexecutor.state.store import StateStore
+from tradeexecutor.strategy.sync_model import SyncMethodV0, SyncModel
+from tradeexecutor.state.trade import TradeExecution
+from tradeexecutor.state.validator import validate_state_serialisation
+from tradeexecutor.statistics.core import update_statistics
+from tradeexecutor.strategy.approval import ApprovalModel
 from tradeexecutor.strategy.description import StrategyExecutionDescription
-from tradeexecutor.strategy.cycle import CycleDuration
-from tradeexecutor.cli.approval import CLIApprovalModel
-from tradeexecutor.cli.loop import ExecutionLoop
-from tradeexecutor.ethereum.hot_wallet_sync import EthereumHotWalletReserveSyncer
-from tradeexecutor.ethereum.uniswap_v2_execution import UniswapV2ExecutionModel
-from tradeexecutor.ethereum.uniswap_v2_valuation import uniswap_v2_sell_valuation_factory
-from tradeexecutor.monkeypatch.dataclasses_json import patch_dataclasses_json
-from tradeexecutor.ethereum.uniswap_v2_live_pricing import uniswap_v2_live_pricing_factory
-from tradeexecutor.state.store import JSONFileStore, StateStore, NoneStore
-from tradeexecutor.strategy.approval import ApprovalType, UncheckedApprovalModel, ApprovalModel
-from tradeexecutor.strategy.bootstrap import import_strategy_file, make_factory_from_strategy_mod
-from tradeexecutor.strategy.dummy import DummyExecutionModel
+from tradeexecutor.strategy.execution_model import ExecutionModel
 from tradeexecutor.strategy.execution_context import ExecutionMode, ExecutionContext
-from tradeexecutor.strategy.execution_model import TradeExecutionType, ExecutionModel
-from tradeexecutor.cli.log import setup_logging, setup_discord_logging, setup_logstash_logging
-from tradeexecutor.strategy.strategy_module import read_strategy_module, StrategyModuleInformation
-from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverseModel
-from tradeexecutor.strategy.universe_model import UniverseOptions
-from tradeexecutor.utils.fullname import get_object_full_name
-from tradeexecutor.utils.timer import timed_task
-from tradeexecutor.webhook.server import create_webhook_server
-from tradingstrategy.client import Client
+from tradeexecutor.strategy.factory import StrategyFactory
+from tradeexecutor.strategy.pricing_model import PricingModelFactory
+from tradeexecutor.strategy.runner import StrategyRunner
+from tradeexecutor.strategy.cycle import CycleDuration, snap_to_next_tick, snap_to_previous_tick, round_datetime_up
+from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse
+from tradeexecutor.strategy.universe_model import UniverseModel, StrategyExecutionUniverse, UniverseOptions
+from tradeexecutor.strategy.valuation import ValuationModelFactory
+from tradingstrategy.client import Client, BaseClient
+from tradingstrategy.timebucket import TimeBucket
 
-app = typer.Typer()
 
+logger = logging.getLogger(__name__)
 
-TRADE_EXECUTOR_VERSION = version('trade-executor')
 
+class LiveSchedulingTaskFailed(Exception):
+    """Main loop dies uncleanly.
 
-logger: Optional[logging.Logger] = None
+    Any of live trading looop scheduled tasks can die with an exception.
+    Raise this and wrap the underlying exception if we need to crash the trading loop.
+    """
 
 
-def validate_executor_id(id: str):
-    """Check that given executor id is good.
+class ExecutionLoop:
+    """Live or backtesting trade execution loop.
 
-    No spaces.
+    This is the main loop of any strategy execution.
 
-    - Will be used in filenames
+    - Run scheduled tasks for different areas (trade cycle, position revaluation, stop loss triggers)
 
-    - Will be used in URLs
+    - Call :py:class:`ExecutionModel` to perform ticking through the strategy
 
-    :raise AssertionError:
-        If the user gives us non-id like id
+    - Manage the persistent state of the strategy
     """
 
-    assert id, f"EXECUTOR_ID must be given so that executor instances can be identified"
-    assert " " not in id, f"Bad EXECUTOR_ID: {id}"
+    def __init__(
+            self,
+            *ignore,
+            name: str,
+            command_queue: Queue,
+            execution_model: ExecutionModel,
+            execution_context: ExecutionContext,
+            sync_model: SyncModel,
+            approval_model: ApprovalModel,
+            pricing_model_factory: PricingModelFactory,
+            valuation_model_factory: ValuationModelFactory,
+            store: StateStore,
+            client: Optional[BaseClient],
+            strategy_factory: Optional[StrategyFactory],
+            cycle_duration: CycleDuration,
+            stats_refresh_frequency: Optional[datetime.timedelta],
+            position_trigger_check_frequency: Optional[datetime.timedelta],
+            max_data_delay: Optional[datetime.timedelta] = None,
+            reset=False,
+            max_cycles: Optional[int] = None,
+            debug_dump_file: Optional[Path] = None,
+            backtest_start: Optional[datetime.datetime] = None,
+            backtest_end: Optional[datetime.datetime] = None,
+            backtest_setup: Optional[Callable[[State], None]] = None,
+            backtest_candle_time_frame_override: Optional[TimeBucket] = None,
+            backtest_stop_loss_time_frame_override: Optional[TimeBucket] = None,
+            stop_loss_check_frequency: Optional[TimeBucket] = None,
+            tick_offset: datetime.timedelta=datetime.timedelta(minutes=0),
+            trade_immediately=False,
+            run_state: Optional[RunState]=None,
+            strategy_cycle_trigger: StrategyCycleTrigger = StrategyCycleTrigger.cycle_offset,
+            routing_model: Optional[RoutingModel] = None,
+    ):
+        """See main.py for details."""
 
+        if ignore:
+            # https://www.python.org/dev/peps/pep-3102/
+            raise TypeError("Only keyword arguments accepted")
 
-def create_web3_config(
-    json_rpc_binance,
-    json_rpc_polygon,
-    json_rpc_avalanche,
-    json_rpc_ethereum,
-    gas_price_method: Optional[GasPriceMethod]=None,
-) -> Optional[Web3Config]:
-    """Create Web3 connection to the live node we are executing against.
+        assert isinstance(sync_model, SyncModel)
+        self.sync_model = sync_model
 
-    :return web3:
-        Connect to any passed JSON RPC URL
+        self.cycle_duration = cycle_duration
+        self.stop_loss_check_frequency = stop_loss_check_frequency
+        self.strategy_factory = strategy_factory
+        self.reset = reset
+        self.routing_model = routing_model
 
-    """
-    web3config = Web3Config.setup_from_environment(
-        gas_price_method,
-        json_rpc_ethereum=json_rpc_ethereum,
-        json_rpc_binance=json_rpc_binance,
-        json_rpc_polygon=json_rpc_polygon,
-        json_rpc_avalanche=json_rpc_avalanche,
-    )
-    return web3config
-
-
-def create_trade_execution_model(
-        execution_type: TradeExecutionType,
-        private_key: str,
-        web3config: Web3Config,
-        confirmation_timeout: datetime.timedelta,
-        confirmation_block_count: int,
-        max_slippage: float,
-        min_balance_threshold: Optional[Decimal],
-):
-    """Set up the execution mode for the command line client."""
-
-    if execution_type == TradeExecutionType.dummy:
-        return DummyExecutionModel()
-    elif execution_type == TradeExecutionType.uniswap_v2_hot_wallet:
-        assert private_key, "Private key is needed for live trading"
-        web3 = web3config.get_default()
-        hot_wallet = HotWallet.from_private_key(private_key)
-        sync_method = EthereumHotWalletReserveSyncer(web3, hot_wallet.address)
-        execution_model = UniswapV2ExecutionModel(
-            web3,
-            hot_wallet,
-            confirmation_timeout=confirmation_timeout,
-            confirmation_block_count=confirmation_block_count,
-            max_slippage=max_slippage,
-            min_balance_threshold=min_balance_threshold,
+        args = locals().copy()
+        args.pop("self")
+
+        assert "execution_context" in args, "execution_context required"
+
+        # TODO: Spell out individual variables for type hinting support
+        self.__dict__.update(args)
+
+        self.timed_task_context_manager = self.execution_context.timed_task_context_manager
+
+        self.runner: Optional[StrategyRunner] = None
+        self.universe_model: Optional[UniverseModel] = None
+        self.strategy_cycle_trigger = strategy_cycle_trigger
+        self.max_cycles = max_cycles
+        self.max_data_delay = max_data_delay
+
+        # Crash the strategy execution if we get more lag than this.
+        # This is how old the last candle can be.
+        self.max_live_data_lag_tolerance = datetime.timedelta(minutes=30)
+
+        # cycle -> dump mappings
+        self.debug_dump_state = {}
+
+        # Hook in any overrides for strategy cycles
+        self.universe_options = UniverseOptions(
+            candle_time_bucket_override=self.backtest_candle_time_frame_override,
+            stop_loss_time_bucket_override=self.backtest_stop_loss_time_frame_override,
         )
-        valuation_model_factory = uniswap_v2_sell_valuation_factory
-        pricing_model_factory = uniswap_v2_live_pricing_factory
-        return execution_model, sync_method, valuation_model_factory, pricing_model_factory
-    elif execution_type == TradeExecutionType.backtest:
-        logger.info("TODO: Command line backtests are always executed with initial deposit of $10,000")
-        wallet = SimulatedWallet()
-        execution_model = BacktestExecutionModel(wallet, max_slippage=0.01, stop_loss_data_available=True)
-        sync_method = BacktestSyncer(wallet, Decimal(10_000))
-        pricing_model_factory = backtest_pricing_factory
-        valuation_model_factory = backtest_valuation_factory
-        return execution_model, sync_method, valuation_model_factory, pricing_model_factory
-    else:
-        raise NotImplementedError()
-
-
-def create_approval_model(approval_type: ApprovalType) -> ApprovalModel:
-    if approval_type == ApprovalType.unchecked:
-        return UncheckedApprovalModel()
-    elif approval_type == ApprovalType.cli:
-        return CLIApprovalModel()
-    else:
-        raise NotImplementedError()
-
-
-def create_state_store(state_file: Path) -> StateStore:
-    store = JSONFileStore(state_file)
-    return store
 
+    def is_live_trading_unit_test(self) -> bool:
+        """Are we attempting to test live trading functionality in unit tests.
 
-def prepare_cache(executor_id: str, cache_path: Optional[Path]) -> Path:
-    """Fail early if the cache path is not writable.
+        See `test_cli_commands.py`
+        """
+        return self.max_cycles == 0
+
+    def init_state(self) -> State:
+        """Initialize the state for this run.
+
+        - If we are doing live trading, load the last saved state
+
+        - In backtesting the state is always reset.
+          We do not support resumes for crashed backetsting.
+
+        """
+        store: StateStore = self.store
+        if self.reset:
+            logger.info("Resetting the existing state file %s", store)
+            # Create empty state and save it
+            state = store.create(self.name)
+            state.name = self.name
+            store.sync(state)
+        else:
+            if store.is_pristine():
+                logger.info("State is unwritten, creating new one %s", store)
+                # Create empty state and save it
+                state = store.create(self.name)
+                state.name = self.name
+                store.sync(state)
+            else:
+                logger.info("Loading state file %s", store)
+                state = store.load()
+
+        # Check that we did not corrupt the state while writing it to the disk
+        state.perform_integrity_check()
+
+        return state
+
+    def init_execution_model(self):
+        """Initialise the execution.
+
+        Perform preflight checks e.g. to see if our trading accounts look sane.
+        """
+        self.execution_model.initialize()
+        if not self.is_live_trading_unit_test():
+            self.execution_model.preflight_check()
+            logger.info("Preflight checks ok")
+
+    def init_simulation(
+            self,
+            universe_model: UniverseModel,
+            runner: StrategyRunner,
+        ):
+        """Set up running on a simulated blockchain.
+
+        Used with :py:mod:`tradeexecutor.testing.simulated_execution_loop`
+        to allow fine granularity manipulation of in-memory blockchain
+        to simulate trigger conditions in testing.
+        """
+        assert self.execution_context.mode == ExecutionMode.simulated_trading
+        self.init_execution_model()
+        self.universe_model = universe_model
+        self.runner = runner
+
+    def tick(self,
+             unrounded_timestamp: datetime.datetime,
+             cycle_duration: CycleDuration,
+             state: State,
+             cycle: int,
+             live: bool,
+             existing_universe: Optional[StrategyExecutionUniverse]=None,
+             strategy_cycle_timestamp: Optional[datetime.datetime] = None,
+             extra_debug_data: Optional[dict] = None,
+             ) -> StrategyExecutionUniverse:
+        """Run one trade execution tick.
+
+        :param unrounded_timestamp:
+            The approximately time when this ticket was triggered.
+            Alawys after the tick timestamp.
+            Will be rounded to the nearest cycle duration timestamps.
+
+        :param strategy_cycle_timestamp:
+            Precalculated strategy cycle timestamp based on unrounded timestamp
+
+        :param state:
+            The current state of the strategy
+
+        :param cycle:
+            The number of this cycle
+
+        :param cycle_duration:
+            Cycle duration for this cycle. Either from the strategy module,
+            or a backtest override.
+
+        :param existing_universe:
+            If passed, use this universe instead of trying to download
+            and filter new one. This is shortcut for backtesting
+            where the universe does not change between cycles
+            (as opposite to live trading new pairs pop in to the existince).
+
+        :param extra_debug_data:
+            Extra data to be passed to the debug dump used in unit testing.
+        """
+
+        assert isinstance(unrounded_timestamp, datetime.datetime)
+        assert isinstance(state, State)
+        assert isinstance(cycle_duration, CycleDuration)
 
-    Otherwise Docker might spit misleading "Device or resource busy" message.
-    """
+        if strategy_cycle_timestamp:
+            ts = strategy_cycle_timestamp
+        else:
+            ts = snap_to_previous_tick(unrounded_timestamp, cycle_duration)
 
-    assert executor_id
+        # This Python dict collects internal debugging data through this cycle.
+        # Any submodule of strategy execution can add internal information here for
+        # unit testing and manual diagnostics. Any data added must be JSON serializable.
+        debug_details = {
+            "cycle": cycle,
+            "unrounded_timestamp": unrounded_timestamp,
+            "timestamp": ts,
+            "strategy_cycle_trigger": self.strategy_cycle_trigger.value,
+        }
+
+        logger.trade("Performing strategy tick #%d for timestamp %s, cycle length is %s, trigger time was %s, live trading is %s, trading univese is %s",
+                     cycle,
+                     ts,
+                     cycle_duration.value,
+                     unrounded_timestamp,
+                     live,
+                     existing_universe,
+                     )
+
+        if existing_universe is None:
+
+            # We are running backtesting and the universe is not yet loaded.
+            # Unlike live trading, we do not need to reconstruct the universe between
+            # trade cycles.
+
+            # Refresh the trading universe for this cycle
+            if self.strategy_cycle_trigger == StrategyCycleTrigger.cycle_offset:
+                logger.info("Creating new universe from the scratch using create_trading_universe()")
+                universe = self.universe_model.construct_universe(
+                    ts,
+                    self.execution_context.mode,
+                    self.universe_options,
+                )
+
+                # Check if our data is stagnated and we cannot execute the strategy
+                if self.max_data_delay is not None:
+                    self.universe_model.check_data_age(ts, universe, self.max_data_delay)
+            elif self.strategy_cycle_trigger == StrategyCycleTrigger.trading_pair_data_availability:
+                assert existing_universe is not None, "StrategyCycleTrigger.trading_pair_data_availability needs to retain the previous universe"
+            else:
+                raise NotImplementedError()
+        else:
+            # Recycle the universe instance
+            logger.info("Reusing previously loaded universe: %s", existing_universe)
+            universe = existing_universe
+
+        # Run cycle checks
+        self.runner.pretick_check(ts, universe)
+
+        if cycle == 1 and self.backtest_setup is not None:
+            # The hook to set up backtest initial balance
+            logger.info("Performing initial backtest account funding")
+            self.backtest_setup(state, universe, self.sync_model)
+
+        # Execute the strategy tick and trades
+        self.runner.tick(
+            strategy_cycle_timestamp=ts,
+            universe=universe,
+            state=state,
+            debug_details=debug_details,
+            cycle_duration=cycle_duration,
+            cycle=cycle,
+        )
 
-    if not cache_path:
-        cache_path = Path("cache").joinpath(executor_id)
+        state.uptime.record_cycle_complete(cycle)
 
-    logger.info("Dataset cache is %s", cache_path)
+        # Check that state is good before writing it to the disk
+        state.perform_integrity_check()
 
-    os.makedirs(cache_path, exist_ok=True)
+        # Store the current state to disk
+        self.store.sync(state)
 
-    with open(cache_path.joinpath("cache.pid"), "wt") as out:
-        print(os.getpid(), file=out)
+        if extra_debug_data is not None:
+            debug_details.update(extra_debug_data)
 
-    return cache_path
+        # Store debug trace
+        self.debug_dump_state[cycle] = debug_details
 
+        if self.debug_dump_file is not None:
+            # Record and write out the internal debug states after every tick
+            with open(self.debug_dump_file, "wb") as out:
+                pickle.dump(self.debug_dump_state, out)
 
-def create_metadata(name, short_description, long_description, icon_url) -> Metadata:
-    """Create metadata object from the configuration variables."""
-    return Metadata(
-        name,
-        short_description,
-        long_description,
-        icon_url,
-        datetime.datetime.utcnow(),
-    )
+        # Assume universe stays static between cycles
+        # for hourly revaluations
+        return universe
 
+    def update_position_valuations(self, clock: datetime.datetime, state: State, universe: StrategyExecutionUniverse, execution_mode: ExecutionMode):
+        """Revalue positions and update statistics.
 
-def prepare_executor_id(id: Optional[str], strategy_file: Path) -> str:
-    """Autodetect exeuctor id."""
+        A new statistics entry is calculated for portfolio and all of its positions
+        and added to the state.
 
-    if id:
-        # Explicitly passed
-        pass
-    else:
-        # Guess id from the strategy file
-        if strategy_file:
-            id = Path(strategy_file).stem
-            pass
-        else:
-            raise RuntimeError("EXECUTOR_ID or STRATEGY_FILE must be given")
+        :param clock: Real-time or historical clock
+        """
 
-    validate_executor_id(id)
+        # Set up the execution to perform the valuation
 
-    return id
+        if len(state.portfolio.reserves) == 0:
+            logger.info("The strategy has no reserves or deposits yet")
 
+        routing_state, pricing_model, valuation_method = self.runner.setup_routing(universe)
 
-def monkey_patch():
-    """Apply all monkey patches."""
-    patch_dataclasses_json()
-
-
-# Run this during the module loading so that it is
-# applied to all subcommands
-monkey_patch()
-
-
-# Typer documentation https://typer.tiangolo.com/
-@app.command()
-def start(
-
-    # Strategy assets
-    id: str = typer.Option(None, envvar="EXECUTOR_ID", help="Executor id used when programmatically referring to this instance. If not given, take the base of --strategy-file."),
-    log_level: str = typer.Option(None, envvar="LOG_LEVEL", help="The Python default logging level. The defaults are 'info' is live execution, 'warning' if backtesting."),
-    name: Optional[str] = typer.Option(None, envvar="NAME", help="Executor name used in the web interface and notifications"),
-    short_description: Optional[str] = typer.Option(None, envvar="SHORT_DESCRIPTION", help="Short description for metadata"),
-    long_description: Optional[str] = typer.Option(None, envvar="LONG_DESCRIPTION", help="Long description for metadata"),
-    icon_url: Optional[str] = typer.Option(None, envvar="ICON_URL", help="Strategy icon for web rendering and Discord avatar"),
-    strategy_file: Path = typer.Option(..., envvar="STRATEGY_FILE", help="Python strategy file to run"),
-
-    # Live trading or backtest
-    execution_type: TradeExecutionType = typer.Option(..., envvar="EXECUTION_TYPE"),
-    trading_strategy_api_key: str = typer.Option(None, envvar="TRADING_STRATEGY_API_KEY", help="Trading Strategy API key"),
-
-    # Webhook server options
-    http_enabled: bool = typer.Option(False, envvar="HTTP_ENABLED", help="Enable Webhook server"),
-    http_port: int = typer.Option(3456, envvar="HTTP_PORT", help="Which HTTP port to listen. The default is 3456, the default port of Pyramid web server."),
-    http_host: str = typer.Option("0.0.0.0", envvar="HTTP_HOST", help="The IP address to bind for the web server. By default listen to all IP addresses available in the run-time environment."),
-    http_username: str = typer.Option("webhook", envvar="HTTP_USERNAME", help="Username for HTTP Basic Auth protection of webhooks"),
-    http_password: str = typer.Option(None, envvar="HTTP_PASSWORD", help="Password for HTTP Basic Auth protection of webhooks"),
-
-    # Web3 connection options
-    json_rpc_binance: str = typer.Option(None, envvar="JSON_RPC_BINANCE", help="BNB Chain JSON-RPC node URL we connect to"),
-    json_rpc_polygon: str = typer.Option(None, envvar="JSON_RPC_POLYGON", help="Polygon JSON-RPC node URL we connect to"),
-    json_rpc_ethereum: str = typer.Option(None, envvar="JSON_RPC_ETHEREUM", help="Ethereum JSON-RPC node URL we connect to"),
-    json_rpc_avalanche: str = typer.Option(None, envvar="JSON_RPC_AVALANCHE", help="Avalanche C-chain JSON-RPC node URL we connect to"),
-    gas_price_method: Optional[GasPriceMethod] = typer.Option(None, envvar="GAS_PRICE_METHOD", help="How to set the gas price for Ethereum transactions. After the Berlin hardfork Ethereum mainnet introduced base + tip cost gas model. Leave out to autodetect."),
-    confirmation_timeout: int = typer.Option(900, envvar="CONFIRMATION_TIMEOUT", help="How many seconds to wait for transaction batches to confirm"),
-    confirmation_block_count: int = typer.Option(8, envvar="CONFIRMATION_BLOCK_COUNT", help="How many blocks we wait before we consider transaction receipt a final"),
-    private_key: Optional[str] = typer.Option(None, envvar="PRIVATE_KEY", help="Ethereum private key to be used as a hot wallet/broadcast wallet"),
-    minimum_gas_balance: Optional[float] = typer.Option(0.1, envvar="MINUMUM_GAS_BALANCE", help="What is the minimum balance of gas token you need to have in your wallet. If the balance falls below this, abort by crashing and do not attempt to create transactions. Expressed in the native token e.g. ETH."),
-
-    # Logging
-    discord_webhook_url: Optional[str] = typer.Option(None, envvar="DISCORD_WEBHOOK_URL", help="Discord webhook URL for notifications"),
-    logstash_server: Optional[str] = typer.Option(None, envvar="LOGSTASH_SERVER", help="LogStash server hostname where to send logs"),
-
-    # Debugging and unit testing
-    port_mortem_debugging: bool = typer.Option(False, "--post-mortem-debugging", envvar="POST_MORTEM_DEBUGGING", help="Launch ipdb debugger on a main loop crash to debug the exception"),
-    clear_caches: bool = typer.Option(False, "--clear-caches", envvar="CLEAR_CACHES", help="Purge any dataset download caches before starting"),
-    unit_testing: bool = typer.Option(False, "--unit-testing", envvar="UNIT_TESTING", help="The trade executor is called under the unit testing mode. No caches are purged."),
-    reset_state: bool = typer.Option(False, envvar="RESET_STATE"),
-    max_cycles: int = typer.Option(None, envvar="MAX_CYCLES", help="Max main loop cycles run in an automated testing mode"),
-    debug_dump_file: Optional[Path] = typer.Option(None, envvar="DEBUG_DUMP_FILE", help="Write Python Pickle dump of all internal debugging states of the strategy run to this file"),
-
-    # Backtesting
-    backtest_start: Optional[datetime.datetime] = typer.Option(None, envvar="BACKTEST_START", help="Start timestamp of backesting"),
-    backtest_end: Optional[datetime.datetime] = typer.Option(None, envvar="BACKTEST_END", help="End timestamp of backesting"),
-    backtest_candle_time_frame_override: Optional[TimeBucket] = typer.Option(None, envvar="BACKTEST_CANDLE_TIME_FRAME_OVERRIDE", help="Force backtests to use different candle time frame"),
-    backtest_stop_loss_time_frame_override: Optional[TimeBucket] = typer.Option(None, envvar="BACKTEST_STOP_LOSS_TIME_FRAME_OVERRIDE", help="Force backtests to use different candle time frame for stop losses"),
-
-    # Live trading configuration
-    max_slippage: float = typer.Option(0.0025, envvar="MAX_SLIPPAGE", help="Max slippage allowed per trade before failing. The default is 0.0025 is 0.25%."),
-    approval_type: ApprovalType = typer.Option("unchecked", envvar="APPROVAL_TYPE", help="Set a manual approval flow for trades"),
-    stop_loss_check_frequency: Optional[TimeBucket] = typer.Option(None, envvar="STOP_LOSS_CYCLE_DURATION", help="Override live/backtest stop loss check frequency. If not given read from the strategy module."),
-    cycle_offset_minutes: int = typer.Option(8, envvar="CYCLE_OFFSET_MINUTES", help="How many minutes we wait after the tick before executing the tick step"),
-    stats_refresh_minutes: int = typer.Option(60.0, envvar="STATS_REFRESH_MINUTES", help="How often we refresh position statistics. Default to once in an hour."),
-    cycle_duration: CycleDuration = typer.Option(None, envvar="CYCLE_DURATION", help="How long strategy tick cycles use to execute the strategy. While strategy modules offer their own cycle duration value, you can override it here."),
-    position_trigger_check_minutes: int = typer.Option(3.0, envvar="POSITION_TRIGGER_CHECK_MINUTES", help="How often we check for take profit/stop loss triggers. Default to once in 3 minutes. Set 0 to disable."),
-    max_data_delay_minutes: int = typer.Option(3*60, envvar="MAX_DATA_DELAY_MINUTES", help="If our data feed is delayed more than this minutes, abort the execution. Defaukts to 3 hours."),
-    trade_immediately: bool = typer.Option(False, "--trade-immediately", envvar="TRADE_IMMEDIATELY", help="Perform the first rebalance immediately, do not wait for the next trading universe refresh"),
-
-    # Unsorted options
-    state_file: Optional[Path] = typer.Option(None, envvar="STATE_FILE", help="JSON file where we serialise the execution state. If not given defaults to state/{executor-id}.json"),
-    cache_path: Optional[Path] = typer.Option(None, envvar="CACHE_PATH", help="Where to store downloaded datasets. This must be specific to each executor so that there are no write conflicts if multiple executors run on the same server. If not given default to cache/{executor-id}"),
-    ):
-    """Launch Trade Executor instance."""
-    global logger
+        with self.timed_task_context_manager("revalue_portfolio_statistics"):
+            logger.info("Updating position valuations")
+            self.runner.revalue_portfolio(clock, state, valuation_method)
 
-    # Guess id from the strategy file
-    id = prepare_executor_id(id, strategy_file)
+        with self.timed_task_context_manager("update_statistics"):
+            logger.info("Updating position statistics")
+            update_statistics(clock, state.stats, state.portfolio, execution_mode)
 
-    # We always need a name
-    if not name:
-        if strategy_file:
-            name = os.path.basename(strategy_file)
-        else:
-            name = "Unnamed backtest"
+        # Check that state is good before writing it to the disk
+        state.perform_integrity_check()
 
-    if log_level:
-        log_level = log_level.upper()
-    else:
-        if execution_type == TradeExecutionType.backtest:
-            log_level = logging.WARNING
-        else:
-            log_level = logging.INFO
+        # Store the current state to disk
+        self.store.sync(state)
 
-    logger = setup_logging(log_level)
+    def update_summary_statistics(
+            self,
+            state: State,
+    ):
+        """Update the summary card statistics for this strategy."""
 
-    if discord_webhook_url:
-        setup_discord_logging(
-            name,
-            webhook_url=discord_webhook_url,
-            avatar_url=icon_url)
-
-    if logstash_server:
-        setup_logstash_logging(
-            logstash_server,
-            f"executor-{id}",  # Always prefix logged with executor id
-            quiet=False,
-        )
+        if not state.portfolio.is_empty():
+            stats = calculate_summary_statistics(
+                state,
+                self.execution_context.mode,
+            )
+            self.run_state.summary_statistics = stats
 
-    if not state_file:
-        if execution_type != TradeExecutionType.backtest:
-            state_file = f"state/{id}.json"
-
-    cache_path = prepare_cache(id, cache_path)
-
-    confirmation_timeout = datetime.timedelta(seconds=confirmation_timeout)
-
-    if execution_type == TradeExecutionType.uniswap_v2_hot_wallet:
-        web3config = create_web3_config(
-            json_rpc_binance=json_rpc_binance,
-            json_rpc_polygon=json_rpc_polygon,
-            json_rpc_avalanche=json_rpc_avalanche,
-            json_rpc_ethereum=json_rpc_ethereum,
-            gas_price_method=None,
+    def check_position_triggers(self,
+                          ts: datetime.datetime,
+                          state: State,
+                          universe: TradingStrategyUniverse) -> List[TradeExecution]:
+        """Run stop loss price checks.
+
+        Used for live stop loss check; backtesting
+        uses optimised :py:meth:`run_backtest_stop_loss_checks`.
+
+        :param ts:
+            Timestamp of this check cycle
+
+        param universe:
+            Trading universe containing price data for stoploss checks.
+
+        :return:
+            List of generated trigger trades
+        """
+
+        logger.info("Starting stop loss checks at %s", ts)
+
+        if len(state.portfolio.reserves) == 0:
+            logger.info("The strategy has no reserves or deposits yet")
+            return []
+
+        routing_state, pricing_model, valuation_method = self.runner.setup_routing(universe)
+
+        # Do stop loss checks for every time point between now and next strategy cycle
+        trades = self.runner.check_position_triggers(
+            ts,
+            state,
+            universe,
+            pricing_model,
+            routing_state
         )
 
-        if not web3config.has_any_connection():
-            raise RuntimeError("Live trading requires that you pass JSON-RPC connection to one of the networks")
-    else:
-        web3config = None
-
-    # TODO: This strategy file is reloaded again in ExecutionLoop.run()
-    # We do an extra hop here, because we need to know chain_id associated with the strategy,
-    # because there is an inversion of control issue for passing web3 connection around.
-    # Clean this up in the future versions, by changing the order of initialzation.
-    mod = read_strategy_module(strategy_file)
-
-    if web3config is not None:
-
-        if isinstance(mod, StrategyModuleInformation):
-            # This path is not enabled for legacy strategy modules
-            web3config.set_default_chain(mod.chain_id)
-            web3config.check_default_chain_id()
-        else:
-            # Legacy unit testing path.
-            # All chain_ids are 56 (BNB Chain)
-            logger.warning("Legacy strategy module: makes assumption of BNB Chain")
-            web3config.set_default_chain(ChainId.bsc)
-
-    if minimum_gas_balance:
-        minimum_gas_balance = Decimal(minimum_gas_balance)
-
-    execution_model, sync_method, valuation_model_factory, pricing_model_factory = create_trade_execution_model(
-        execution_type,
-        private_key,
-        web3config,
-        confirmation_timeout,
-        confirmation_block_count,
-        max_slippage,
-        minimum_gas_balance,
-    )
-
-    approval_model = create_approval_model(approval_type)
-
-    if state_file:
-        store = create_state_store(Path(state_file))
-    else:
-        # Backtests never have persistent state
-        if execution_type == TradeExecutionType.backtest:
-            logger.info("This backtest run won't create a state file")
-            store = NoneStore(State())
-        else:
-            raise RuntimeError("Does not know how to set up a state file for this run")
+        # Check that state is good before writing it to the disk
+        state.perform_integrity_check()
 
-    metadata = create_metadata(name, short_description, long_description, icon_url)
+        # Store the current state to disk
+        self.store.sync(state)
 
-    # Start the queue that relays info from the web server to the strategy executor
-    command_queue = Queue()
+        return trades
 
-    # Create our webhook server
-    if http_enabled:
-        server = create_webhook_server(http_host, http_port, http_username, http_password, command_queue, store, metadata)
-    else:
-        logger.info("Web server disabled")
-        server = None
-
-    # Create our data client
-    if trading_strategy_api_key:
-        client = Client.create_live_client(trading_strategy_api_key, cache_path=cache_path)
-        if clear_caches:
-            client.clear_caches()
-    else:
-        client = None
-
-    # Currently, all actions require us to have a valid API key
-    # might change in the future
-    if not client:
-        raise RuntimeError("Trading Strategy client instance is not available - needed to run backtests. Make sure trading_strategy_api_key is set.")
-
-    tick_offset = datetime.timedelta(minutes=cycle_offset_minutes)
-
-    if max_data_delay_minutes:
-        max_data_delay = datetime.timedelta(minutes=max_data_delay_minutes)
-    else:
-        max_data_delay = None
-
-    stats_refresh_frequency = datetime.timedelta(minutes=stats_refresh_minutes)
-    position_trigger_check_frequency = datetime.timedelta(minutes=position_trigger_check_minutes)
-
-    logger.info("Loading strategy file %s", strategy_file)
-    strategy_factory = import_strategy_file(strategy_file)
-
-    logger.trade("Trade Executor version %s starting strategy %s", TRADE_EXECUTOR_VERSION, name)
-
-    if backtest_start:
-        # Running as a backtest
-        execution_context = ExecutionContext(
-            mode=ExecutionMode.backtesting,
-            timed_task_context_manager=timed_task,
+    def warm_up_backtest(self):
+        """Load backtesting trading universe.
+
+        Display progress bars for data downloads.
+        """
+        logger.info("Warming up backesting, universe options are %s", self.universe_options)
+        self.universe_model.preload_universe(self.universe_options)
+
+    def warm_up_live_trading(self) -> TradingStrategyUniverse:
+        """Load live trading universe.
+
+        Display progress bars for data downloads.
+        """
+        logger.info("Warming up live trading universe, universe options are %s", self.universe_options)
+        universe = cast(TradingStrategyUniverse, self.universe_model.preload_universe(self.universe_options))
+        logger.info("Warmed up universe %s", universe)
+        return universe
+
+    def run_backtest_trigger_checks(self,
+                                    start_ts: datetime.datetime,
+                                    end_ts: datetime.datetime,
+                                    state: State,
+                                    universe: TradingStrategyUniverse) -> Tuple[int, int]:
+        """Generate stop loss price checks.
+
+        Backtests may use finer grade data for stop loss signals,
+        to be more realistic with actual trading.
+
+        Here we use the finer grade data to check the stop losses
+        on a given time period.
+
+        :param start_ts:
+            When to start testing (exclusive).
+            We test for the next available timestamp.
+
+        :param end_ts:
+            When to stop testing (exclusive).
+
+        :param universe:
+            Trading universe containing price data for stoploss checks.
+
+        :return:
+            Tuple (take profit, stop loss) count triggered
+        """
+
+        assert universe.backtest_stop_loss_candles is not None
+
+        # What is the granularity of our price feed
+        # for stop loss checks.
+        tick_size = universe.backtest_stop_loss_time_bucket
+
+        logger.info("run_backtest_stop_loss_checks with frequency of %s", tick_size.value)
+
+        assert tick_size.to_pandas_timedelta() > pd.Timedelta(0), f"Cannot do stop loss checks, because no stop loss cycle duration was given"
+
+        # Hop to the next tick
+        ts = round_datetime_up(start_ts, tick_size.to_timedelta())
+
+        routing_state, pricing_model, valuation_model = self.runner.setup_routing(universe)
+        assert pricing_model, "Routing did not provide pricing_model"
+
+        assert isinstance(pricing_model, BacktestSimplePricingModel)
+
+        stop_loss_pricing_model = BacktestSimplePricingModel(
+            universe.backtest_stop_loss_candles,
+            self.runner.routing_model,
+            time_bucket=universe.backtest_stop_loss_time_bucket,
+            allow_missing_fees=pricing_model.allow_missing_fees
         )
-    else:
-        if unit_testing:
-            execution_context = ExecutionContext(
-                mode=ExecutionMode.unit_testing_trading,
-                timed_task_context_manager=timed_task,
-            )
-        else:
-            execution_context = ExecutionContext(
-                mode=ExecutionMode.real_trading,
-                timed_task_context_manager=timed_task,
+
+        # Do stop loss checks for every time point between now and next strategy cycle
+        tp = 0
+        sl = 0
+
+        while ts < end_ts:
+            logger.debug("Backtesting take profit/stop loss at %s", ts)
+            trades = self.runner.check_position_triggers(
+                ts,
+                state,
+                universe,
+                stop_loss_pricing_model,
+                routing_state
             )
+            for t in trades:
+                if t.is_stop_loss():
+                    sl += 1
+                elif t.is_take_profit():
+                    tp += 1
+            ts += tick_size.to_timedelta()
 
-    try:
-        loop = ExecutionLoop(
-            name=name,
-            command_queue=command_queue,
-            execution_model=execution_model,
-            execution_context=execution_context,
-            sync_method=sync_method,
-            approval_model=approval_model,
-            pricing_model_factory=pricing_model_factory,
-            valuation_model_factory=valuation_model_factory,
-            store=store,
-            client=client,
-            strategy_factory=strategy_factory,
-            reset=reset_state,
-            max_cycles=max_cycles,
-            debug_dump_file=debug_dump_file,
-            backtest_start=backtest_start,
-            backtest_end=backtest_end,
-            backtest_stop_loss_time_frame_override=backtest_stop_loss_time_frame_override,
-            backtest_candle_time_frame_override=backtest_candle_time_frame_override,
-            stop_loss_check_frequency=stop_loss_check_frequency,
-            cycle_duration=cycle_duration,
-            tick_offset=tick_offset,
-            max_data_delay=max_data_delay,
-            trade_immediately=trade_immediately,
-            stats_refresh_frequency=stats_refresh_frequency,
-            position_trigger_check_frequency=position_trigger_check_frequency,
-        )
-        loop.run()
+        return tp, sl
 
-        # Display summary stats for terminal backtest runs
-        if execution_type == TradeExecutionType.backtest and isinstance(store, NoneStore):
-            display_backtesting_results(store.state)
-
-    except KeyboardInterrupt as e:
-        # CTRL+C shutdown
-        logger.trade("Trade Executor %s shut down by CTRL+C requested: %s", name, e)
-    except Exception as e:
-        # Debug exceptions in production
-        if port_mortem_debugging:
-            import ipdb
-            ipdb.post_mortem()
-        logger.exception(e)
-        raise
-    finally:
-        if server:
-            server.close()
-
-
-@app.command()
-def check_universe(
-    id: str = typer.Option(None, envvar="EXECUTOR_ID", help="Executor id used when programmatically referring to this instance. If not given, take the base of --strategy-file."),
-    strategy_file: Path = typer.Option(..., envvar="STRATEGY_FILE"),
-    trading_strategy_api_key: str = typer.Option(None, envvar="TRADING_STRATEGY_API_KEY", help="Trading Strategy API key"),
-    cache_path: Optional[Path] = typer.Option(None, envvar="CACHE_PATH", help="Where to store downloaded datasets"),
-    max_data_delay_minutes: int = typer.Option(24*60, envvar="MAX_DATA_DELAY_MINUTES", help="How fresh the OHCLV data for our strategy must be before failing"),
-):
-    """Checks that the trading universe is helthy for a given strategy."""
-
-    global logger
-
-    id = prepare_executor_id(id, strategy_file)
-
-    logger = setup_logging()
-
-    logger.info("Loading strategy file %s", strategy_file)
-
-    strategy_factory = import_strategy_file(strategy_file)
-
-    cache_path = prepare_cache(id, cache_path)
-
-    assert trading_strategy_api_key, "TRADING_STRATEGY_API_KEY missing"
-
-    client = Client.create_live_client(trading_strategy_api_key, cache_path=cache_path)
-    client.clear_caches()
-
-    execution_context = ExecutionContext(
-        mode=ExecutionMode.preflight_check,
-        timed_task_context_manager=timed_task
-    )
-
-    max_data_delay = datetime.timedelta(minutes=max_data_delay_minutes)
-
-    run_description: StrategyExecutionDescription = strategy_factory(
-        execution_model=None,
-        execution_context=execution_context,
-        timed_task_context_manager=timed_task,
-        sync_method=None,
-        valuation_model_factory=None,
-        pricing_model_factory=None,
-        approval_model=None,
-        client=client,
-    )
-
-    # Deconstruct strategy input
-    universe_model: TradingStrategyUniverseModel = run_description.universe_model
-
-    ts = datetime.datetime.utcnow()
-    logger.info("Performing universe data check for timestamp %s", ts)
-    universe = universe_model.construct_universe(ts, ExecutionMode.preflight_check, UniverseOptions())
-
-    latest_candle_at = universe_model.check_data_age(ts, universe, max_data_delay)
-    ago = datetime.datetime.utcnow() - latest_candle_at
-    logger.info("Latest OHCLV candle is at: %s, %s ago", latest_candle_at, ago)
-
-
-@app.command()
-def check_wallet(
-    id: str = typer.Option(None, envvar="EXECUTOR_ID", help="Executor id used when programmatically referring to this instance. If not given, take the base of --strategy-file."),
-
-    strategy_file: Path = typer.Option(..., envvar="STRATEGY_FILE"),
-    private_key: str = typer.Option(None, envvar="PRIVATE_KEY"),
-    trading_strategy_api_key: str = typer.Option(None, envvar="TRADING_STRATEGY_API_KEY", help="Trading Strategy API key"),
-    cache_path: Optional[Path] = typer.Option("cache/", envvar="CACHE_PATH", help="Where to store downloaded datasets"),
-
-    # Get minimum gas balance from the env
-    minimum_gas_balance: Optional[float] = typer.Option(0.1, envvar="MINUMUM_GAS_BALANCE", help="What is the minimum balance of gas token you need to have in your wallet. If the balance falls below this, abort by crashing and do not attempt to create transactions. Expressed in the native token e.g. ETH."),
-
-    # Web3 connection options
-    json_rpc_binance: str = typer.Option(None, envvar="JSON_RPC_BINANCE", help="BNB Chain JSON-RPC node URL we connect to"),
-    json_rpc_polygon: str = typer.Option(None, envvar="JSON_RPC_POLYGON", help="Polygon JSON-RPC node URL we connect to"),
-    json_rpc_ethereum: str = typer.Option(None, envvar="JSON_RPC_ETHEREUM", help="Ethereum JSON-RPC node URL we connect to"),
-    json_rpc_avalanche: str = typer.Option(None, envvar="JSON_RPC_AVALANCHE", help="Avalanche C-chain JSON-RPC node URL we connect to"),
-):
-    """Print out the token balances of the hot wallet.
+    def run_backtest(self, state: State) -> dict:
+        """Backtest loop."""
 
-    Check that our hot wallet has cash deposits and gas token deposits.
-    """
+        if self.backtest_end or self.backtest_start:
+            assert self.backtest_start and self.backtest_end, f"If backtesting both start and end must be given, we have {self.backtest_start} - {self.backtest_end}"
 
-    # To run this from command line with .env file you can do
-    # set -o allexport ; source ~/pancake-eth-usd-sma-final.env ; set +o allexport ;  trade-executor check-wallet
+        assert self.backtest_start < self.backtest_end
 
-    global logger
+        ts = self.backtest_start
 
-    id = prepare_executor_id(id, strategy_file)
+        logger.info("Strategy is executed in backtesting mode, starting at %s, cycle duration is %s", ts, self.cycle_duration.value)
 
-    logger = setup_logging()
+        cycle = state.cycle
+        universe = None
 
-    mod = read_strategy_module(strategy_file)
-
-    cache_path = prepare_cache(id, cache_path)
-
-    client = Client.create_live_client(trading_strategy_api_key, cache_path=cache_path)
-
-    execution_context = ExecutionContext(
-        mode=ExecutionMode.preflight_check,
-        timed_task_context_manager=timed_task
-    )
-
-    web3config = create_web3_config(
-        json_rpc_binance,
-        json_rpc_polygon,
-        json_rpc_avalanche,
-        json_rpc_ethereum,
-        GasPriceMethod.london,
-    )
-
-    assert web3config, "No RPC endpoints given. A working JSON-RPC connection is needed for check-wallet"
-
-    # Check that we are connected to the chain strategy assumes
-    web3config.set_default_chain(mod.chain_id)
-    web3config.check_default_chain_id()
-
-    execution_model, sync_method, valuation_model_factory, pricing_model_factory = create_trade_execution_model(
-        execution_type=TradeExecutionType.uniswap_v2_hot_wallet,
-        private_key=private_key,
-        web3config=web3config,
-        confirmation_timeout=60,
-        confirmation_block_count=6,
-        max_slippage=0.01,
-        min_balance_threshold=minimum_gas_balance,
-    )
-
-    hot_wallet = HotWallet.from_private_key(private_key)
-
-    # Set up the strategy engine
-    factory = make_factory_from_strategy_mod(mod)
-    run_description: StrategyExecutionDescription = factory(
-        execution_model=execution_model,
-        execution_context=execution_context,
-        timed_task_context_manager=execution_context.timed_task_context_manager,
-        sync_method=sync_method,
-        valuation_model_factory=valuation_model_factory,
-        pricing_model_factory=pricing_model_factory,
-        approval_model=UncheckedApprovalModel(),
-        client=client,
-    )
-
-    # We construct the trading universe to know what's our reserve asset
-    universe_model: TradingStrategyUniverseModel = run_description.universe_model
-    ts = datetime.datetime.utcnow()
-    universe = universe_model.construct_universe(
-        ts,
-        ExecutionMode.preflight_check,
-        UniverseOptions())
-
-    # Get all tokens from the universe
-    reserve_assets = universe.reserve_assets
-    web3 = web3config.get_default()
-    tokens = [Web3.toChecksumAddress(a.address) for a in reserve_assets]
-
-    logger.info("RPC details")
-
-    # Check the chain is online
-    logger.info(f"  Chain id is {web3.eth.chain_id:,}")
-    logger.info(f"  Latest block is {web3.eth.block_number:,}")
-
-    # Check balances
-    logger.info("Balance details")
-    logger.info("  Hot wallet is %s", hot_wallet.address)
-    gas_balance = web3.eth.get_balance(hot_wallet.address) / 10**18
-    logger.info("  We have %f tokens for gas left", gas_balance)
-    logger.info("  The gas error limit is %f tokens", minimum_gas_balance)
-    balances = fetch_erc20_balances_by_token_list(web3, hot_wallet.address, tokens)
-
-    for asset in reserve_assets:
-        logger.info("Reserve asset: %s", asset.token_symbol)
-
-    for address, balance in balances.items():
-        details = fetch_erc20_details(web3, address)
-        logger.info("  Balance of %s (%s): %s %s", details.name, details.address, details.convert_to_decimals(balance), details.symbol)
-
-    # Check that the routing looks sane
-    # E.g. there is no mismatch between strategy reserve token, wallet and pair universe
-    runner = run_description.runner
-    routing_state, pricing_model, valuation_method = runner.setup_routing(universe)
-    routing_model = runner.routing_model
-
-    logger.info("Execution details")
-    logger.info("  Execution model is %s", get_object_full_name(execution_model))
-    logger.info("  Routing model is %s", get_object_full_name(routing_model))
-    logger.info("  Token pricing model is %s", get_object_full_name(pricing_model))
-    logger.info("  Position valuation model is %s", get_object_full_name(valuation_method))
-
-    # Check we have enough gas
-    execution_model.preflight_check()
-
-    # Check our routes
-    routing_model.perform_preflight_checks_and_logging(routing_state, universe.universe.pairs)
-
-    web3config.close()
-
-
-@app.command()
-def hello():
-    """Check that the application loads without doing anything."""
-    print("Hello blockchain")
-
-
-@app.command()
-def perform_test_trade(
-    id: str = typer.Option(None, envvar="EXECUTOR_ID", help="Executor id used when programmatically referring to this instance. If not given, take the base of --strategy-file."),
-
-    strategy_file: Path = typer.Option(..., envvar="STRATEGY_FILE"),
-    private_key: str = typer.Option(None, envvar="PRIVATE_KEY"),
-    trading_strategy_api_key: str = typer.Option(None, envvar="TRADING_STRATEGY_API_KEY", help="Trading Strategy API key"),
-    state_file: Optional[Path] = typer.Option(None, envvar="STATE_FILE", help="JSON file where we serialise the execution state. If not given defaults to state/{executor-id}.json"),
-    cache_path: Optional[Path] = typer.Option("cache/", envvar="CACHE_PATH", help="Where to store downloaded datasets"),
-
-    # Web3 connection options
-    json_rpc_binance: str = typer.Option(None, envvar="JSON_RPC_BINANCE", help="BNB Chain JSON-RPC node URL we connect to"),
-    json_rpc_polygon: str = typer.Option(None, envvar="JSON_RPC_POLYGON", help="Polygon JSON-RPC node URL we connect to"),
-    json_rpc_ethereum: str = typer.Option(None, envvar="JSON_RPC_ETHEREUM", help="Ethereum JSON-RPC node URL we connect to"),
-    json_rpc_avalanche: str = typer.Option(None, envvar="JSON_RPC_AVALANCHE", help="Avalanche C-chain JSON-RPC node URL we connect to"),
-):
-    """Perform a small test swap.
+        range = self.backtest_end - self.backtest_start
 
-    Tests that the private wallet and the exchange can trade by making 1 USD trade using
-    the routing configuration from the strategy.
+        ts_format = "%Y-%m-%d"
 
-    The trade will be recorded on the state as a position.
-    """
-    global logger
+        friendly_start = self.backtest_start.strftime(ts_format)
+        friendly_end = self.backtest_end.strftime(ts_format)
 
-    id = prepare_executor_id(id, strategy_file)
+        seconds = int(range.total_seconds())
 
-    logger = setup_logging(log_level=logging.INFO)
+        self.warm_up_backtest()
 
-    mod = read_strategy_module(strategy_file)
+        # Allow backtest step to be overwritten from the command line
+        if self.universe_options.candle_time_bucket_override:
+            backtest_step = CycleDuration.from_timebucket(self.universe_options.candle_time_bucket_override)
+        else:
+            backtest_step = self.cycle_duration
 
-    cache_path = prepare_cache(id, cache_path)
-
-    client = Client.create_live_client(trading_strategy_api_key, cache_path=cache_path)
-
-    execution_context = ExecutionContext(
-        mode=ExecutionMode.preflight_check,
-        timed_task_context_manager=timed_task
-    )
-
-    web3config = create_web3_config(
-        json_rpc_binance=json_rpc_binance,
-        json_rpc_polygon=json_rpc_polygon,
-        json_rpc_avalanche=json_rpc_avalanche,
-        json_rpc_ethereum=json_rpc_ethereum,
-        gas_price_method=None,
-    )
-
-    assert web3config, "No RPC endpoints given. A working JSON-RPC connection is needed for check-wallet"
-
-    # Check that we are connected to the chain strategy assumes
-    web3config.set_default_chain(mod.chain_id)
-    web3config.check_default_chain_id()
-
-    execution_model, sync_method, valuation_model_factory, pricing_model_factory = create_trade_execution_model(
-        execution_type=TradeExecutionType.uniswap_v2_hot_wallet,
-        private_key=private_key,
-        web3config=web3config,
-        confirmation_timeout=60,
-        confirmation_block_count=6,
-        max_slippage=2.50,
-        min_balance_threshold=0,
-    )
-
-    if not state_file:
-        state_file = f"state/{id}.json"
-
-    store = create_state_store(Path(state_file))
-
-    if store.is_pristine():
-        state = store.create()
-    else:
-        state = store.load()
-
-    # Set up the strategy engine
-    factory = make_factory_from_strategy_mod(mod)
-    run_description: StrategyExecutionDescription = factory(
-        execution_model=execution_model,
-        execution_context=execution_context,
-        timed_task_context_manager=execution_context.timed_task_context_manager,
-        sync_method=sync_method,
-        valuation_model_factory=valuation_model_factory,
-        pricing_model_factory=pricing_model_factory,
-        approval_model=UncheckedApprovalModel(),
-        client=client,
-    )
-
-    # We construct the trading universe to know what's our reserve asset
-    universe_model: TradingStrategyUniverseModel = run_description.universe_model
-    ts = datetime.datetime.utcnow()
-    universe = universe_model.construct_universe(
-        ts,
-        ExecutionMode.preflight_check,
-        UniverseOptions())
-
-    runner = run_description.runner
-    routing_state, pricing_model, valuation_method = runner.setup_routing(universe)
-
-    make_test_trade(
-        execution_model,
-        pricing_model,
-        sync_method,
-        state,
-        universe,
-        runner.routing_model,
-        routing_state,
-    )
+        cycle_name = backtest_step.value
 
-    # Store the test trade data in the strategy history
-    store.sync(state)
+        assert backtest_step != CycleDuration.cycle_unknown
 
+        # Throttle TQDM updates to 1 per second because
+        # otherwise we crash PyCharm
+        # https://stackoverflow.com/q/43288550/315168
+        last_progress_update = datetime.datetime.utcfromtimestamp(0)
+        progress_update_threshold = datetime.timedelta(seconds=0.1)
+        last_update_ts = None  # The last pushed timestamp to tqdm
+        trigger_checks = 0
+        stop_losses = take_profits = 0
+
+        with tqdm(total=seconds) as progress_bar:
+
+            while True:
+                ts = snap_to_previous_tick(ts, backtest_step)
+                # Bump progress bar forward and update backtest status
+                if datetime.datetime.utcnow() - last_progress_update > progress_update_threshold:
+                    friedly_ts = ts.strftime(ts_format)
+                    trade_count = len(list(state.portfolio.get_all_trades()))
+                    progress_bar.set_description(f"Backtesting {self.name}, {friendly_start} - {friendly_end} at {friedly_ts} ({cycle_name})")
+                    progress_bar.set_postfix({
+                        "trades": trade_count,
+                        "cycles": cycle,
+                        "TPs": take_profits,
+                        "SLs": stop_losses,
+                    })
+                    last_progress_update = datetime.datetime.utcnow()
+                    if last_update_ts:
+                        # Push update for the period
+                        passed_seconds = (ts - last_update_ts).total_seconds()
+                        progress_bar.update(int(passed_seconds))
+                    last_update_ts = ts
+
+                # Decide trades and everything for this cycle
+                universe: TradingStrategyUniverse = self.tick(
+                    ts,
+                    backtest_step,
+                    state,
+                    cycle,
+                    live=False,
+                    strategy_cycle_timestamp=ts,
+                    existing_universe=universe)
+
+                # Revalue our portfolio
+                self.update_position_valuations(ts, state, universe, self.execution_context.mode)
+
+                # Check for termination in integration testing.
+                # TODO: Get rid of this and only support date ranges to run tests
+                if self.max_cycles is not None:
+                    if cycle >= self.max_cycles:
+                        logger.info("Max backtest cycles reached")
+                        break
+
+                # Backtesting
+                next_tick = snap_to_next_tick(ts + datetime.timedelta(seconds=1), backtest_step, self.tick_offset)
+
+                if next_tick >= self.backtest_end:
+                    # Backteting has ended
+                    logger.info("Terminating backtesting. Backtest end %s, current timestamp %s", self.backtest_end, next_tick)
+                    passed_seconds = (ts - last_update_ts).total_seconds()
+                    progress_bar.update(int(passed_seconds))
+                    break
+
+                # If we have stop loss checks enabled on a separate price feed,
+                # run backtest stop loss checks until the next time
+                if universe.backtest_stop_loss_candles is not None:
+                    res = self.run_backtest_trigger_checks(
+                        ts,
+                        next_tick,
+                        state,
+                        universe,
+                    )
+                    take_profits += res[0]
+                    stop_losses += res[1]
+
+                # Add some fuzziness to gacktesting timestamps
+                # TODO: Make this configurable - sub 1h strategies do not work
+                ts = next_tick + datetime.timedelta(minutes=random.randint(0, 4))
+
+                cycle += 1
+
+            # Validate the backtest state at the end.
+            # We want to avoid situation where we have stored
+            # non-serialisable types in the state
+            validate_state_serialisation(state)
+
+            return self.debug_dump_state
+
+    def run_live(self, state: State):
+        """Run live trading cycle.
+
+        :raise LiveSchedulingTaskFailed:
+            If any of live trading concurrent tasks crashes with an exception
+        """
+
+        ts = datetime.datetime.utcnow()
+
+        # Start the watchdog process killer
+        watchdog_registry = create_watchdog_registry(WatchdogMode.thread_based)
+        start_background_watchdog(watchdog_registry)
+        # Create a watchdog thread that checks that the live trading cycle
+        # has completed for every candle + some tolerance minutes.
+        # This will terminate the live trading process if it has hung for a reason or another.
+        live_cycle_max_delay = (self.cycle_duration.to_timedelta() + datetime.timedelta(minutes=15)).total_seconds()
+        register_worker(
+            watchdog_registry,
+            "live_cycle",
+            live_cycle_max_delay)
+
+        # Do not allow starting a strategy that has unclean state
+        state.check_if_clean()
+
+        logger.trade("The execution state was last saved %s", state.last_updated_at)
+
+        if self.is_live_trading_unit_test():
+            # Test app initialisation.
+            # Do not start any background threads.
+            logger.info("Unit test live trading checkup test detected - aborting.")
+            return self.debug_dump_state
+
+        cycle = state.cycle
+        universe: Optional[StrategyExecutionUniverse] = None
+        execution_context = self.execution_context
+        run_state: RunState = self.run_state
+        crash_exception: Optional[Exception] = None
+
+        tick_offset = self.tick_offset
+
+        # We use trading pair data availability endpoint poll
+        # to trigger the cycle.
+        # Start the cycle warmup immediately,
+        # but later wait down in the loop for the data availability.
+        if self.strategy_cycle_trigger == StrategyCycleTrigger.trading_pair_data_availability:
+            tick_offset = datetime.timedelta(0)
+
+        assert execution_context, "ExecutionContext missing"
+
+        universe = self.warm_up_live_trading()
+
+        # Store summary statistics in memory before doing anything else
+        self.update_summary_statistics(state)
+
+        # The first trade will be execute immediately, despite the time offset or tick
+        if self.trade_immediately:
+            ts = datetime.datetime.now()
+            universe = self.tick(ts, self.cycle_duration, state, cycle, live=True)
+
+        def die(exc: Exception):
+            # Shutdown the scheduler and mark an clean exit
+            nonlocal crash_exception
+            logger.exception(exc)
+            scheduler.shutdown(wait=False)
+            crash_exception = exc
+
+        def live_cycle():
+            nonlocal cycle
+            nonlocal universe
+            try:
+
+                extra_debug_data = {}
+
+                # Wall clock time
+                unrounded_timestamp = datetime.datetime.utcnow()
+                strategy_cycle_timestamp = snap_to_previous_tick(unrounded_timestamp, self.cycle_duration)
+
+                logger.info("Executing live strategy cycle %d, now is %s, decision slot is %s",
+                            cycle,
+                            unrounded_timestamp,
+                            strategy_cycle_timestamp
+                            )
+
+                # If we are in trigger mode, poll until we have data available
+                # and then immediately trigger the decision
+                if self.strategy_cycle_trigger == StrategyCycleTrigger.trading_pair_data_availability:
+                    universe_update_result = wait_for_universe_data_availability_jsonl(
+                        strategy_cycle_timestamp,
+                        self.client,
+                        universe,
+                        max_wait=self.max_data_delay,
+                    )
+                    logger.trade("Strategy cycle %d, universe updated result received: %s", cycle, universe_update_result)
+                    universe = universe_update_result.updated_universe
+                    extra_debug_data["universe_update_poll_cycles"] = universe_update_result.poll_cycles
+
+                    # Do a data lag check.
+                    # This is not 100% fool-proof check for multipair strategies,
+                    # as we randomly pick one pair. However it should detect most of market data feed
+                    # stale situtations.
+                    last_candle_timestamp = universe.universe.candles.df.iloc[-1]["timestamp"].to_pydatetime().replace(tzinfo=None)
+                    # We allow 30 minutes + time bucket size lag
+                    if last_candle_timestamp is not None:
+                        max_allowed_lag = self.max_live_data_lag_tolerance + universe.universe.time_bucket.to_timedelta()
+                        lag = strategy_cycle_timestamp - last_candle_timestamp
+                        if lag > max_allowed_lag:
+                            logger.error("Aborting and waiting for manual restart after the data feed is fixed")
+                            raise RuntimeError(f"Strategy market data lag exceeded.\n"
+                                               f"Currently lag to the start of the last candle is {lag}, allowed max lag is {max_allowed_lag}.\n"
+                                               f"Last candle is at {last_candle_timestamp}")
+                else:
+                    # Force universe recreation on every cycle
+                    universe = None
+
+                # Run the main strategy logic
+                universe = self.tick(
+                    unrounded_timestamp,
+                    self.cycle_duration,
+                    state,
+                    cycle=cycle,
+                    strategy_cycle_timestamp=strategy_cycle_timestamp,
+                    existing_universe=universe,
+                    live=True,
+                    extra_debug_data=extra_debug_data,
+                )
+                logger.info("run_live() tick complete, universe is now %s", universe)
+
+                # Post execution, update our statistics
+                try:
+                    self.update_summary_statistics(state)
+                except Exception as e:
+                    # Failing to do the performance statistics is not fatal,
+                    # because this does not contain any state changing events
+                    logger.warning("update_summary_statistics() failed in the live cycle: %s", e)
+                    logger.exception(e)
+                    pass
+
+                # Go to sleep and
+                # and advance to the next cycle
+                cycle += 1
+                state.cycle = cycle
+
+            except Exception as e:
+                die(e)
+
+            # Unit testing mode
+            # Used e.g. test_strategy_cycle_trigger.py
+            if self.max_cycles is not None:
+                if cycle >= self.max_cycles:
+                    logger.info(("Max cycles reached"))
+                    scheduler.shutdown(wait=False)
+
+            run_state.completed_cycle = cycle
+            run_state.cycles += 1
+            run_state.frozen_positions = len(state.portfolio.frozen_positions)
+            run_state.bumb_refreshed()
+
+            # Reset the background watchdog timer
+            mark_alive(watchdog_registry, "live_cycle")
+
+        def live_positions():
+            nonlocal universe
+
+            # We cannot update valuations until we know
+            # trading pair universe, because to know the valuation of the position
+            # we need to know the route how to sell the token of the position
+            if universe is None:
+                logger.info("Universe not yet downloaded")
+                return
+
+            try:
+                ts = datetime.datetime.now()
+
+                self.update_position_valuations(ts, state, universe, execution_context.mode)
+
+                self.update_summary_statistics(state)
+            except Exception as e:
+                die(e)
+
+            run_state.position_revaluations += 1
+            run_state.bumb_refreshed()
+
+        def live_trigger_checks():
+            nonlocal universe
+
+            # We cannot update valuations until we know
+            # trading pair universe, because to know the valuation of the position
+            # we need to know the route how to sell the token of the position
+            if universe is None:
+                logger.info("Universe not yet downloaded")
+                return
+
+            try:
+                ts = datetime.datetime.now()
+                self.check_position_triggers(ts, state, universe)
+            except Exception as e:
+                die(e)
+
+            run_state.position_trigger_checks += 1
+            run_state.bumb_refreshed()
+
+        # Set up live trading tasks using APScheduler
+        executors = {
+            'default': ThreadPoolExecutor(1),
+        }
+        start_time = datetime.datetime(1970, 1, 1)
+
+        # We use a single thread scheduler to run our various tasks.
+        # Any task blocks other tasks - there is no parallerism or multithread support at the moment.
+        # Multithread support would need making the architecture more complex with various locks
+        # that could then be additional source of bugs.
+        scheduler = BlockingScheduler(executors=executors, timezone=datetime.timezone.utc)
+        scheduler.add_job(
+            live_cycle,
+            'interval',
+            seconds=self.cycle_duration.to_timedelta().total_seconds(),
+            start_date=start_time + tick_offset,
+            misfire_grace_time = None,  # Will always run the job no matter how late it is
+        )
 
+        if self.stats_refresh_frequency not in (datetime.timedelta(0), None):
+            scheduler.add_job(
+                live_positions,
+                'interval',
+                seconds=self.stats_refresh_frequency.total_seconds(),
+                start_date=start_time)
+
+        if self.position_trigger_check_frequency not in (datetime.timedelta(0), None):
+            scheduler.add_job(
+                live_trigger_checks,
+                'interval',
+                seconds=self.position_trigger_check_frequency.total_seconds(),
+                start_date=start_time)
+
+        def listen_error(event):
+            if event.exception:
+                logger.info("Scheduled task received exception. event: %s, execption: %s", event, event.exception)
+            else:
+                logger.error("Should not happen")
+
+        scheduler.add_listener(listen_error, EVENT_JOB_ERROR)
+
+        # Display version information on the trade log
+        version_info = self.run_state.version
+        logger.trade(str(version_info))
+
+        try:
+            # https://github.com/agronholm/apscheduler/discussions/683
+            scheduler.start()
+        except KeyboardInterrupt:
+            # https://github.com/agronholm/apscheduler/issues/338
+            scheduler.shutdown(wait=False)
+            raise
+        except Exception as e:
+            logger.error("Scheduler raised an exception %s", e)
+            raise
+
+        logger.info("Scheduler finished - down the live trading loop")
+
+        if crash_exception:
+            raise LiveSchedulingTaskFailed("trade-executor closed because one of the scheduled tasks failed") from crash_exception
+
+        return self.debug_dump_state
+
+    def run(self) -> dict:
+        """The main loop of trade executor.
+
+        Main entry point to the loop.
+
+        - Chooses between live and backtesting execution mode
+
+        - Loads or creates the initial state
+
+        - Sets up strategy runner
+
+        :return:
+            Debug state where each key is the cycle number
+        """
+
+        state = self.init_state()
+        self.init_execution_model()
+
+        run_description: StrategyExecutionDescription = self.strategy_factory(
+            execution_model=self.execution_model,
+            execution_context=self.execution_context,
+            timed_task_context_manager=self.timed_task_context_manager,
+            sync_model=self.sync_model,
+            valuation_model_factory=self.valuation_model_factory,
+            pricing_model_factory=self.pricing_model_factory,
+            approval_model=self.approval_model,
+            client=self.client,
+            routing_model=self.routing_model,
+            run_state=self.run_state,
+        )
 
+        # Expose source code to webhook
+        if self.run_state:
+            self.run_state.source_code = run_description.source_code
+
+        # Deconstruct strategy input
+        self.runner: StrategyRunner = run_description.runner
+        self.universe_model = run_description.universe_model
+
+        # Load cycle_duration from v0.1 strategies,
+        # if not given from the command line to override backtesting data
+        if run_description.cycle_duration and not self.cycle_duration:
+            self.cycle_duration = run_description.cycle_duration
+
+        assert self.cycle_duration is not None, "Did not get strategy cycle duration from constructor or strategy run description"
+
+        if self.backtest_start:
+            # Walk through backtesting range
+            return self.run_backtest(state)
+        else:
+            return self.run_live(state)
```

### Comparing `trade_executor-0.2/tradeexecutor/cli/testtrade.py` & `trade_executor-0.3/tradeexecutor/cli/testtrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Perform a test trade on a universe."""
 import logging
 import datetime
 from decimal import Decimal
 
 from tradingstrategy.universe import Universe
 
-from tradeexecutor.ethereum.hot_wallet_sync import EthereumHotWalletReserveSyncer
+from tradeexecutor.ethereum.hot_wallet_sync_model import EthereumHotWalletReserveSyncer
 from tradeexecutor.state.state import State
 from tradeexecutor.strategy.execution_model import ExecutionModel
 from tradeexecutor.strategy.pandas_trader.position_manager import PositionManager
 from tradeexecutor.strategy.pricing_model import PricingModel
 from tradeexecutor.strategy.routing import RoutingModel, RoutingState
 from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse, translate_trading_pair
 
@@ -28,15 +28,15 @@
 ):
     """Perform a test trade.
 
     Buy and sell 1 token worth for 1 USD to check that
     our trade routing works.
     """
 
-    ts = datetime.datetime.utcnow()\
+    ts = datetime.datetime.utcnow()
 
     # Sync nonce for the hot wallet
     execution_model.initialize()
 
     data_universe: Universe = universe.universe
 
     reserve_asset = universe.get_reserve_asset()
```

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/abi/uniswap/erc20.json` & `trade_executor-0.3/tradeexecutor/ethereum/abi/uniswap/erc20.json`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/abi/uniswap/factory.json` & `trade_executor-0.3/tradeexecutor/ethereum/abi/uniswap/factory.json`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/abi/uniswap/pair.json` & `trade_executor-0.3/tradeexecutor/ethereum/abi/uniswap/pair.json`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/abi/uniswap/uniswap_erc20.json` & `trade_executor-0.3/tradeexecutor/ethereum/abi/uniswap/uniswap_erc20.json`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/uniswap_v2_execution_v0.py` & `trade_executor-0.3/tradeexecutor/testing/ethereumtrader_uniswap_v2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,224 +1,218 @@
-"""Execution model where trade happens directly on Uniswap v2 style exchange.
-
-TODO: Prototype code path. Only preserved for having unit test suite green.
-It has slight API incompatibilities in the later versions.
-"""
+"""Uniswap v2 test trade builder."""
 
 import datetime
 from decimal import Decimal
-from typing import List, Tuple, Optional
-import logging
+from typing import Tuple, List, Optional
+
+from tradeexecutor.ethereum.uniswap_v2.uniswap_v2_live_pricing import UniswapV2LivePricing
+from tradingstrategy.pair import PandasPairUniverse
+from web3 import Web3
 
-from eth_defi.gas import estimate_gas_fees
 from eth_defi.hotwallet import HotWallet
 from eth_defi.uniswap_v2.deployment import UniswapV2Deployment
-from tradeexecutor.ethereum.execution import broadcast_and_resolve
-from tradeexecutor.ethereum.tx import TransactionBuilder
-from tradeexecutor.ethereum.uniswap_v2_routing import UniswapV2RoutingState, UniswapV2SimpleRoutingModel
+from eth_defi.uniswap_v2.fees import estimate_buy_quantity, estimate_sell_price
+
+from tradeexecutor.ethereum.uniswap_v2.uniswap_v2_execution import UniswapV2ExecutionModel
+from tradeexecutor.ethereum.tx import HotWalletTransactionBuilder, TransactionBuilder
+from tradeexecutor.ethereum.uniswap_v2.uniswap_v2_routing import UniswapV2SimpleRoutingModel, UniswapV2RoutingState
 from tradeexecutor.state.freeze import freeze_position_on_failed_trade
-from tradeexecutor.state.state import State
+from tradeexecutor.state.state import State, TradeType
+from tradeexecutor.state.position import TradingPosition
 from tradeexecutor.state.trade import TradeExecution
-from tradeexecutor.strategy.execution_model import ExecutionModel
-from tradeexecutor.strategy.routing import RoutingModel, RoutingState
-from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse
-
-logger = logging.getLogger(__name__)
-
-
-class UniswapV2RoutingInstructions:
-    """Helper class to router Uniswap trades.
-
-    - Define allowed routes to use
-
-    - Define routing for three way trades
-    """
-
-    def __init__(self, routing_table: dict):
-        """
-
-        :param routing_table: Exchange factory address -> router address data
-        """
+from tradeexecutor.state.identifier import TradingPairIdentifier
+from tradeexecutor.ethereum.ethereumtrader import EthereumTrader, get_base_quote_contracts
 
+class UniswapV2TestTrader(EthereumTrader):
+    """Helper class to trade against a locally deployed Uniswap v2 contract.
 
-class UniswapV2ExecutionModelVersion0(ExecutionModel):
-    """Run order execution on a single Uniswap v2 style exchanges.
+    Allows to execute individual trades without need to go through `decide_trades()`
 
-    TODO: This model was used in the first prototype and later discarded.
+    May be used with or without :py:attr:`pricing_model`.
     """
 
     def __init__(self,
                  uniswap: UniswapV2Deployment,
-                 hot_wallet: HotWallet,
-                 min_balance_threshold=Decimal("0.5"),
-                 confirmation_block_count=6,
-                 confirmation_timeout=datetime.timedelta(minutes=5),
-                 max_slippage=0.01,
-                 stop_on_execution_failure=True):
+                 state: State,
+                 pair_universe: PandasPairUniverse,
+                 tx_builder: TransactionBuilder,
+                 pricing_model: Optional[UniswapV2LivePricing] = None,
+                 ):
         """
-        :param state:
+
+        :param web3:
         :param uniswap:
         :param hot_wallet:
-        :param min_balance_threshold: Abort execution if our hot wallet gas fee balance drops below this
-        :param confirmation_block_count: How many blocks to wait for the receipt confirmations to mitigate unstable chain tip issues
-        :param confirmation_timeout: How long we wait transactions to clear
-        :param stop_on_execution_failure: Raise an exception if any of the trades fail top execute
+        :param state:
+        :param pair_universe:
+        :param tx_builder:
+
+        :param pricing_model:
+            Give if you want to get the lp fees estimated
         """
-        self.web3 = uniswap.web3
+
+        assert isinstance(uniswap, UniswapV2Deployment)
+        assert isinstance(tx_builder, TransactionBuilder)
+
+        super().__init__(tx_builder, state, pair_universe)
+
         self.uniswap = uniswap
-        self.hot_wallet = hot_wallet
-        self.stop_on_execution_failure = stop_on_execution_failure
-        self.min_balance_threshold = min_balance_threshold
-        self.confirmation_block_count = confirmation_block_count
-        self.confirmation_timeout = confirmation_timeout
-        self.max_slippage = max_slippage
-
-    @property
-    def chain_id(self) -> int:
-        """Which chain the live execution is connected to."""
-        return self.web3.eth.chain_id
-
-    def is_live_trading(self):
-        return True
-
-    def is_stop_loss_supported(self) -> bool:
-        return False
-
-    def preflight_check(self):
-        """Check that we can connect to the web3 node"""
-
-        # Check JSON-RPC works
-        assert self.web3.eth.block_number > 1
-
-        # Check we have money for gas fees
-        balance = self.hot_wallet.get_native_currency_balance(self.web3)
-        assert balance > self.min_balance_threshold, f"At least {self.min_balance_threshold} native currency need, our wallet {self.hot_wallet.address} has {balance:.8f}"
-
-        # Check Uniswap v2 instance is valid.
-        # Different factories (Sushi, Pancake) share few common public accessors we can call here.
-        try:
-            self.uniswap.factory.functions.allPairsLength().call()
-        except Exception as e:
-            raise AssertionError(f"Uniswap does not function at chain {self.chain_id}, factory address {self.uniswap.factory.address}") from e
-
-    def initialize(self):
-        """Set up the wallet"""
-        logger.info("Initialising Uniswap v2 execution model")
-        self.hot_wallet.sync_nonce(self.web3)
-        balance = self.hot_wallet.get_native_currency_balance(self.web3)
-        logger.info("Our hot wallet is %s with nonce %d and balance %s", self.hot_wallet.address, self.hot_wallet.current_nonce, balance)
-
-    def execute_trades(self,
-                       ts: datetime.datetime,
-                       state: State,
-                       trades: List[TradeExecution],
-                       routing_model: Optional[RoutingModel],
-                       routing_state: Optional[RoutingState],
-                       check_balances=False) -> Tuple[List[TradeExecution], List[TradeExecution]]:
-        """Execute the trades determined by the algo on a designed Uniswap v2 instance.
+        self.execution_model = UniswapV2ExecutionModel(tx_builder)
+        self.pricing_model = pricing_model
 
-        :param routing_model:
-            Ignored.
+    def buy(self,
+            pair: TradingPairIdentifier,
+            amount_in_usd: Decimal,
+            execute=True,
+            slippage_tolerance: Optional[float] = None,
+            ) -> Tuple[TradingPosition, TradeExecution]:
+        """Buy token (trading pair) for a certain value."""
+
+        base_token, quote_token = get_base_quote_contracts(self.web3, pair)
+
+        if self.pricing_model:
+            price_structure = self.pricing_model.get_buy_price(datetime.datetime.utcnow(), pair, amount_in_usd)
+            assumed_price = price_structure.price
+            estimated_lp_fees = price_structure.get_total_lp_fees()
+            assumed_quantity = None
+            reserve = amount_in_usd
+        else:
+            # Shortcut for testing
+            raw_assumed_quantity = estimate_buy_quantity(self.uniswap, base_token, quote_token, amount_in_usd * (10 ** pair.quote.decimals))
+            assumed_quantity = Decimal(raw_assumed_quantity) / Decimal(10**pair.base.decimals)
+            assumed_price = amount_in_usd / assumed_quantity
+            price_structure = estimated_lp_fees = None
+            reserve = None
+
+        position, trade, created = self.state.create_trade(
+            strategy_cycle_at=self.ts,
+            pair=pair,
+            quantity=assumed_quantity,
+            reserve=reserve,
+            assumed_price=float(assumed_price),
+            trade_type=TradeType.rebalance,
+            reserve_currency=pair.quote,
+            reserve_currency_price=1.0,
+            pair_fee=pair.fee,
+            slippage_tolerance=slippage_tolerance,
+            price_structure=price_structure,
+            lp_fees_estimated=estimated_lp_fees,
+        )
 
-        :return: Tuple List of succeeded trades, List of failed trades
-        """
-        assert isinstance(ts, datetime.datetime)
-        assert isinstance(state, State), f"Received {state.__class__}"
-        assert isinstance(routing_model, UniswapV2SimpleRoutingModel), f"Received {routing_state.__class__}"
-        assert isinstance(routing_state, UniswapV2RoutingState), f"Received {routing_state.__class__}"
-
-        fees = estimate_gas_fees(self.web3)
-
-        tx_builder = TransactionBuilder(
-            self.web3,
-            self.hot_wallet,
-            fees,
+        if execute:
+            self.execute_trades_simple([trade])
+
+        return position, trade
+
+    def sell(
+            self,
+            pair: TradingPairIdentifier,
+            quantity: Decimal,
+            execute=True,
+            slippage_tolerance: Optional[float] = None,
+    ) -> Tuple[TradingPosition, TradeExecution]:
+        """Sell tokens on an open position for a certain quantity."""
+
+        assert isinstance(quantity, Decimal)
+
+        base_token, quote_token = get_base_quote_contracts(self.web3, pair)
+
+        if self.pricing_model:
+            price_structure = self.pricing_model.get_sell_price(datetime.datetime.utcnow(), pair, quantity)
+            assumed_price = price_structure.price
+            estimated_lp_fees = price_structure.get_total_lp_fees()
+        else:
+            # Shortcut in test
+            raw_quantity = int(quantity * 10**pair.base.decimals)
+            raw_assumed_quote_token = estimate_sell_price(self.uniswap, base_token, quote_token, raw_quantity)
+            assumed_quota_token = Decimal(raw_assumed_quote_token) / Decimal(10**pair.quote.decimals)
+
+            # assumed_price = quantity / assumed_quota_token
+            assumed_price = assumed_quota_token / quantity
+            price_structure = estimated_lp_fees = None
+
+        position, trade, created = self.state.create_trade(
+            strategy_cycle_at=self.ts,
+            pair=pair,
+            quantity=-quantity,
+            reserve=None,
+            assumed_price=float(assumed_price),
+            trade_type=TradeType.rebalance,
+            reserve_currency=pair.quote,
+            reserve_currency_price=1.0,
+            pair_fee=pair.fee,
+            slippage_tolerance=slippage_tolerance,
+            price_structure=price_structure,
+            lp_fees_estimated=estimated_lp_fees,
         )
 
-        reserve_asset, rate = state.portfolio.get_default_reserve_currency()
+        if execute:
+            self.execute_trades_simple([trade])
+
+        return position, trade
+    
+    def execute_trades_simple(
+        self,
+        trades: List[TradeExecution],
+        stop_on_execution_failure=True,
+        broadcast=True,
+    ) -> Tuple[List[TradeExecution], List[TradeExecution]]:
+        """Execute trades on web3 instance.
+
+        A testing shortcut
+
+        - Create `BlockchainTransaction` instances of each gives `TradeExecution`
+
+        - Execute them on Web3 test connection (EthereumTester / Ganache)
+
+        - Works with single Uniswap test deployment
+
+        :param trades:
+            Trades to be converted to blockchain transactions
+
+        :param stop_on_execution_failure:
+            Raise exception on an error
+
+        :param broadcast:
+            Broadcast trades over web3 connection
+        """
+
+        pair_universe = self.pair_universe   
+        uniswap = self.uniswap
+        state = self.state
+        
+        assert isinstance(pair_universe, PandasPairUniverse)
+
+        reserve_asset, rate = state.portfolio.get_default_reserve()
 
         # We know only about one exchange
         routing_model = UniswapV2SimpleRoutingModel(
             factory_router_map={
-                self.uniswap.factory.address: (self.uniswap.router.address, self.uniswap.init_code_hash),
+                uniswap.factory.address: (uniswap.router.address, uniswap.init_code_hash),
             },
             allowed_intermediary_pairs={},
             reserve_token_address=reserve_asset.address,
+            trading_fee=0.030,
         )
 
         state.start_trades(datetime.datetime.utcnow(), trades)
+        routing_state = UniswapV2RoutingState(pair_universe, self.tx_builder)
+        routing_model.execute_trades_internal(pair_universe, routing_state, trades)
 
-        routing_model.setup_trades(routing_state, trades, check_balances=check_balances)
-        broadcast_and_resolve(self.web3, state, trades, stop_on_execution_failure=self.stop_on_execution_failure)
+        if broadcast:
+            self.broadcast_trades(trades, stop_on_execution_failure)
+
+    def broadcast_trades(self, trades: List[TradeExecution], stop_on_execution_failure=True):
+        """Broadcast prepared trades."""
+
+        state = self.state
+
+        execution_model = UniswapV2ExecutionModel(self.tx_builder)
+        execution_model.broadcast_and_resolve(state, trades, stop_on_execution_failure=stop_on_execution_failure)
 
         # Clean up failed trades
-        freeze_position_on_failed_trade(ts, state, trades)
+        freeze_position_on_failed_trade(datetime.datetime.utcnow(), state, trades)
 
         success = [t for t in trades if t.is_success()]
         failed = [t for t in trades if t.is_failed()]
 
         return success, failed
-
-        # # 2. Capital allocation
-        # # Approvals
-        # approvals = approve_tokens(
-        #     self.web3,
-        #     self.uniswap,
-        #     self.hot_wallet,
-        #     trades
-        # )
-        #
-        # # 2: prepare
-        # # Prepare transactions
-        # prepare_swaps(
-        #     self.web3,
-        #     self.hot_wallet,
-        #     self.uniswap,
-        #     ts,
-        #     state,
-        #     trades,
-        #     underflow_check=False,
-        # )
-        #
-        # #: 3 broadcast
-        #
-        # # Handle approvals separately for now.
-        # # We do not need to wait these to confirm.
-        # confirm_approvals(
-        #     self.web3,
-        #     approvals,
-        #     confirmation_block_count=self.confirmation_block_count,
-        #     max_timeout=self.confirmation_timeout)
-        #
-        # broadcasted = broadcast(
-        #     self.web3,
-        #     ts,
-        #     trades,
-        #     confirmation_block_count=self.confirmation_block_count,
-        # )
-        # #assert trade.get_status() == TradeStatus.broadcasted
-        #
-        # # Resolve
-        # receipts = wait_trades_to_complete(
-        #     self.web3,
-        #     trades,
-        #     confirmation_block_count=self.confirmation_block_count,
-        #     max_timeout=self.confirmation_timeout)
-        #
-        # resolve_trades(
-        #     self.web3,
-        #     self.uniswap,
-        #     ts,
-        #     state,
-        #     broadcasted,
-        #     receipts,
-        #     stop_on_execution_failure=False)
-        #
-        # # Clean up failed trades
-        # return freeze_position_on_failed_trade(ts, state, trades)
-
-    def get_routing_state_details(self) -> object:
-        """Prototype does not know much about routing."""
-        return {
-            "web3": self.web3,
-            "hot_wallet": self.hot_wallet,
-        }
```

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/uniswap_v2_live_pricing.py` & `trade_executor-0.3/tradeexecutor/ethereum/eth_pricing_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,182 +1,201 @@
-"""Uniswap v2 live pricing.
+"""Asset pricing model for Uniswap V2 and V3 like exchanges."""
 
-Directly asks Uniswap v2 asset price from Uniswap pair contract
-and JSON-RPC API.
-"""
-import logging
+import abc
 import datetime
+from dataclasses import dataclass
 from decimal import Decimal, ROUND_DOWN
-from typing import Optional
-
+from typing import Callable, Optional
 from web3 import Web3
 
-from tradeexecutor.ethereum.uniswap_v2_execution import UniswapV2ExecutionModel
-from tradeexecutor.ethereum.uniswap_v2_execution_v0 import UniswapV2ExecutionModelVersion0
-from tradeexecutor.ethereum.uniswap_v2_routing import UniswapV2SimpleRoutingModel, route_tokens, get_uniswap_for_pair
 from tradeexecutor.state.identifier import TradingPairIdentifier
+from tradeexecutor.state.types import USDollarAmount, BPS, USDollarPrice
 from tradeexecutor.strategy.execution_model import ExecutionModel
-
-from eth_defi.uniswap_v2.fees import estimate_buy_price_decimals, estimate_sell_price_decimals, \
-    estimate_buy_received_amount_raw, estimate_sell_received_amount_raw
-from tradeexecutor.state.types import USDollarAmount
+from tradeexecutor.strategy.routing import RoutingModel
+from tradeexecutor.strategy.universe_model import StrategyExecutionUniverse
+from tradeexecutor.strategy.trading_strategy_universe import translate_trading_pair
 from tradeexecutor.strategy.pricing_model import PricingModel
-from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse, translate_trading_pair
+from tradeexecutor.strategy.trade_pricing import TradePricing
+from tradeexecutor.ethereum.routing_model import EthereumRoutingModel
+
+from eth_defi.uniswap_v2.deployment import UniswapV2Deployment
+from eth_defi.uniswap_v3.deployment import UniswapV3Deployment
+
 from tradingstrategy.pair import PandasPairUniverse
 
 
-logger = logging.getLogger(__name__)
+deployment_types = (UniswapV2Deployment | UniswapV3Deployment)
 
 
-class UniswapV2LivePricing(PricingModel):
-    """Always pull the latest dollar price for an asset from Uniswap v2 deployment.
+class EthereumPricingModel(PricingModel):
+    """Get a price for the asset.
 
-    Supports
+    Needed for various aspects
 
-    - Two-way BUSD -> Cake
+    - Revaluate portfolio positiosn
 
-    - Three-way trades BUSD -> BNB -> Cake
+    - Estimate buy/sell price for the live trading so we can calculate slippage
 
-    ... within a single exchange.
+    - Get the historical price in backtesting
 
-    .. note ::
+    Timestamp is passed to the pricing method. However we expect it only be honoured during
+    the backtesting - live execution may always use the latest price.
 
-        If a trade quantity/currency amount is not given uses
-        a "default small value" that is 0.1. Depending on the token,
-        this value might be too much/too little, as Uniswap
-        fixed point math starts to break for very small amounts.
-        For example, for USDC trade 10 cents is already quite low.
+    .. note ::
 
-    More information
+        For example, in futures markets there could be different fees
+        on buy/sell transctions.
 
-    - `About ask and bid <https://www.investopedia.com/terms/b/bid-and-ask.asp>`_:
+    Used by UniswapV2LivePricing and UniswapV3LivePricing
     """
 
     def __init__(self,
                  web3: Web3,
                  pair_universe: PandasPairUniverse,
-                 routing_model: UniswapV2SimpleRoutingModel,
-                 very_small_amount=Decimal("0.10")):
+                 routing_model: EthereumRoutingModel,
+                 very_small_amount: Decimal):
 
         assert isinstance(web3, Web3)
-        assert isinstance(routing_model, UniswapV2SimpleRoutingModel)
         assert isinstance(pair_universe, PandasPairUniverse)
 
         self.web3 = web3
         self.pair_universe = pair_universe
         self.very_small_amount = very_small_amount
         self.routing_model = routing_model
 
+        assert isinstance(self.very_small_amount, Decimal)
+    
     def get_pair_for_id(self, internal_id: int) -> Optional[TradingPairIdentifier]:
         """Look up a trading pair.
 
         Useful if a strategy is only dealing with pair integer ids.
 
         :return:
             None if the price data is not available
         """
         pair = self.pair_universe.get_pair_by_id(internal_id)
-        if not pair:
-            return None
-        return translate_trading_pair(pair)
-
+        return translate_trading_pair(pair) if pair else None
+    
     def check_supported_quote_token(self, pair: TradingPairIdentifier):
         assert pair.quote.address == self.routing_model.reserve_token_address, f"Quote token {self.routing_model.reserve_token_address} not supported for pair {pair}, pair tokens are {pair.base.address} - {pair.quote.address}"
+        
+    def get_mid_price(self,
+                      ts: datetime.datetime,
+                      pair: TradingPairIdentifier) -> USDollarAmount:
+        """Get the mid price from Uniswap pool.
+
+        Gets tricky, because we calculate dollar mid-price, not
+        quote token midprice.
+        
+        Mid price is an non-trddeable price between the best ask
+        and the best pid.
 
-    def get_sell_price(self,
-                       ts: datetime.datetime,
-                       pair: TradingPairIdentifier,
-                       quantity: Optional[Decimal],
-                       ) -> USDollarAmount:
-        """Get live price on Uniswap."""
-
-        if quantity is None:
-            quantity = Decimal(self.very_small_amount)
+        :param ts:
+            Timestamp. Ignored for live pricing models.
 
-        target_pair, intermediate_pair = self.routing_model.route_pair(self.pair_universe, pair)
+        :param pair:
+            Which trading pair price we query.
 
-        base_addr, quote_addr, intermediate_addr = route_tokens(target_pair, intermediate_pair)
+        :return:
+            The mid price for the pair at a timestamp.
+        """
 
-        uniswap = get_uniswap_for_pair(self.web3, self.routing_model.factory_router_map, target_pair)
+        # TODO: Use native Uniswap router functions to get the mid price
+        # Here we are using a hack)
+        bp = self.get_buy_price(ts, pair, self.very_small_amount)
+        sp = self.get_sell_price(ts, pair, self.very_small_amount)
+        return (bp.price + sp.price) / 2
 
-        # In three token trades, be careful to use the correct reserve token
-        quantity_raw = target_pair.base.convert_to_raw_amount(quantity)
+    def quantize_base_quantity(self, pair: TradingPairIdentifier, quantity: Decimal, rounding=ROUND_DOWN) -> Decimal:
+        """Convert any base token quantity to the native token units by its ERC-20 decimals."""
+        assert isinstance(pair, TradingPairIdentifier)
+        decimals = pair.base.decimals
+        return Decimal(quantity).quantize((Decimal(10) ** Decimal(-decimals)), rounding=rounding)
+    
+    def get_pair_fee(self,
+                     ts: datetime.datetime,
+                     pair: TradingPairIdentifier,
+                     ) -> Optional[float]:
+        """Estimate the trading/LP fees for a trading pair.
+
+        This information can come either from the exchange itself (Uni v2 compatibles),
+        or from the trading pair (Uni v3).
+
+        The return value is used to fill the
+        fee values for any newly opened trades.
+
+        :param ts:
+            Timestamp of the trade. Note that currently
+            fees do not vary over time, but might
+            do so in the future.
 
-        received_raw = estimate_sell_received_amount_raw(
-            uniswap,
-            base_addr,
-            quote_addr,
-            quantity_raw,
-            intermediate_token_address=intermediate_addr
-        )
+        :param pair:
+            Trading pair for which we want to have the fee.
 
-        if intermediate_pair is not None:
-            received = intermediate_pair.quote.convert_to_decimal(received_raw)
-        else:
-            received = target_pair.quote.convert_to_decimal(received_raw)
+            Can be left empty if the underlying exchange is always
+            offering the same fee.
 
-        return float(received / quantity)
+        :return:
+            The estimated trading fee, expressed as %.
 
-    def get_buy_price(self,
+            Returns None if the fee information is not available.
+            This can be different from zero fees.
+        """
+        return pair.fee
+    
+    @abc.abstractmethod
+    def get_uniswap(self, target_pair: TradingPairIdentifier) -> deployment_types:
+        """Helper function to speed up Uniswap v2 or v3 deployment resolution."""
+    
+    @abc.abstractmethod
+    def get_sell_price(self,
                        ts: datetime.datetime,
                        pair: TradingPairIdentifier,
-                       reserve: Optional[Decimal],
-                       ) -> USDollarAmount:
-        """Get live price on Uniswap.
+                       quantity: Optional[Decimal]) -> TradePricing:
+        """Get the sell price for an asset.
 
-        :param reserve:
-            The buy size in quote token e.g. in dollars
+        :param ts:
+            When to get the price.
+            Used in backtesting.
+            Live models may ignore.
 
-        :return: Price for one reserve unit e.g. a dollar
+        :param pair:
+            Trading pair we are intereted in
+
+        :param quantity:
+            If the sel quantity is known, get the price with price impact.
+
+        :return:
+            Price structure for the trade.
         """
 
-        if reserve is None:
-            reserve = Decimal(self.very_small_amount)
-        else:
-            assert isinstance(reserve, Decimal), f"Reserve must be decimal, got {reserve.__class__}: {reserve}"
-
-        target_pair, intermediate_pair = self.routing_model.route_pair(self.pair_universe, pair)
-
-        base_addr, quote_addr, intermediate_addr = route_tokens(target_pair, intermediate_pair)
-
-        uniswap = get_uniswap_for_pair(self.web3, self.routing_model.factory_router_map, target_pair)
-
-        # In three token trades, be careful to use the correct reserve token
-        if intermediate_pair is not None:
-            reserve_raw = intermediate_pair.quote.convert_to_raw_amount(reserve)
-            self.check_supported_quote_token(intermediate_pair)
-        else:
-            reserve_raw = target_pair.quote.convert_to_raw_amount(reserve)
-            self.check_supported_quote_token(pair)
-
-        token_raw_received = estimate_buy_received_amount_raw(
-            uniswap,
-            base_addr,
-            quote_addr,
-            reserve_raw,
-            intermediate_token_address=intermediate_addr
-        )
-        token_received = target_pair.base.convert_to_decimal(token_raw_received)
-        return float(reserve / token_received)
+    @abc.abstractmethod
+    def get_buy_price(self,
+                      ts: datetime.datetime,
+                      pair: TradingPairIdentifier,
+                      reserve: Optional[Decimal]
+                      ) -> TradePricing:
+        """Get the sell price for an asset.
+
+        :param ts:
+            When to get the price.
+            Used in backtesting.
+            Live models may ignore.
 
-    def quantize_base_quantity(self, pair: TradingPairIdentifier, quantity: Decimal, rounding=ROUND_DOWN) -> Decimal:
-        """Convert any base token quantity to the native token units by its ERC-20 decimals."""
-        assert isinstance(pair, TradingPairIdentifier)
-        decimals = pair.base.decimals
-        return Decimal(quantity).quantize((Decimal(10) ** Decimal(-decimals)), rounding=ROUND_DOWN)
+        :param pair:
+            Trading pair we are intereted in
 
+        :param reserve:
+            If the buy token quantity quantity is known,
+            get the buy price with price impact.
+
+        :return:
+            Price structure for the trade.
+        """
+        
 
-def uniswap_v2_live_pricing_factory(
-        execution_model: ExecutionModel,
-        universe: TradingStrategyUniverse,
-        routing_model: UniswapV2SimpleRoutingModel) -> UniswapV2LivePricing:
-
-    assert isinstance(universe, TradingStrategyUniverse)
-    assert isinstance(execution_model, (UniswapV2ExecutionModelVersion0, UniswapV2ExecutionModel)), f"Execution model not compatible with this execution model. Received {execution_model}"
-    assert isinstance(routing_model, UniswapV2SimpleRoutingModel), f"This pricing method only works with Uniswap routing model, we received {routing_model}"
-
-    web3 = execution_model.web3
-    return UniswapV2LivePricing(
-        web3,
-        universe.universe.pairs,
-        routing_model)
+#: This factory creates a new pricing model for each trade cycle.
+#: Pricing model depends on the trading universe that may change for each strategy tick,
+#: as new trading pairs appear.
+#: Thus, we need to reconstruct pricing model as the start of the each tick.
+PricingModelFactory = Callable[[ExecutionModel, StrategyExecutionUniverse, RoutingModel], PricingModel]
```

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/uniswap_v2_routing.py` & `trade_executor-0.3/tradeexecutor/ethereum/routing_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,365 +1,168 @@
-"""Route trades to different Uniswap v2 like exchanges."""
-
 import logging
-from collections import defaultdict
-from decimal import Decimal
-from typing import Dict, Set, List, Optional, Tuple
-
-from eth_typing import HexAddress, ChecksumAddress
-from web3 import Web3
-from web3.contract import Contract
+from typing import Type
+
+from eth_defi.tx import AssetDelta
+from tradeexecutor.strategy.routing import RoutingModel
+from typing import Dict, List, Optional, Tuple
+
+from tradingstrategy.chain import ChainId
 
-from eth_defi.abi import get_deployed_contract
 from eth_defi.gas import estimate_gas_fees
-from eth_defi.token import fetch_erc20_details
-from eth_defi.uniswap_v2.deployment import UniswapV2Deployment, fetch_deployment
-from eth_defi.uniswap_v2.swap import swap_with_slippage_protection
-from tradeexecutor.ethereum.execution import get_token_for_asset
-from tradeexecutor.ethereum.tx import TransactionBuilder
+
+from tradeexecutor.ethereum.tx import HotWalletTransactionBuilder
 from tradeexecutor.state.blockhain_transaction import BlockchainTransaction
 from tradeexecutor.state.identifier import TradingPairIdentifier, AssetIdentifier
 from tradeexecutor.state.trade import TradeExecution
-from tradeexecutor.strategy.routing import RoutingModel, RoutingState, CannotRouteTrade
+from tradeexecutor.strategy.routing import RoutingModel, CannotRouteTrade
 from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse, translate_trading_pair, \
     translate_token
 from tradingstrategy.pair import PandasPairUniverse
 
 from tradeexecutor.strategy.universe_model import StrategyExecutionUniverse
-
+from tradeexecutor.ethereum.routing_state import EthereumRoutingState
 
 logger = logging.getLogger(__name__)
 
-
-class OutOfBalance(Exception):
-    """Did not have enough tokens"""
-
-
-class UniswapV2RoutingState(RoutingState):
-    """Manage transaction building for multiple Uniswap trades.
-
-    - Lifespan is one rebalance - remembers already made approvals
-
-    - Web3 connection and hot wallet
-
-    - Approval tx creation
-
-    - Swap tx creation
-
-    Manage the state of already given approvals here,
-    so that we do not do duplicates.
-
-    The approvals are not persistent in the executor state,
-    but are specific for each cycle.
-    """
-
-    def __init__(self,
-                 pair_universe: PandasPairUniverse,
-                 tx_builder: TransactionBuilder,
-                 swap_gas_limit=2_000_000):
-        self.pair_universe = pair_universe
-        self.tx_builder = tx_builder
-        self.hot_wallet = tx_builder.hot_wallet
-        self.web3 = self.tx_builder.web3
-        # router -> erc-20 mappings
-        self.approved_routes = defaultdict(set)
-        self.swap_gas_limit = swap_gas_limit
-
-    def is_route_approved(self, router_address: str):
-        return router_address in self.approved_routes
-
-    def mark_router_approved(self, token_address, router_address):
-        self.approved_routes[router_address].add(token_address)
-
-    def is_approved_on_chain(self, token_address: str, router_address: str) -> bool:
-        erc_20 = get_deployed_contract(self.web3, "ERC20MockDecimals.json", token_address)
-        # Assume allowance is always infinity
-        return erc_20.functions.allowance.call(self.hot_wallet.address, router_address) > 0
-
-    def get_uniswap_for_pair(self, factory_router_map: dict, target_pair: TradingPairIdentifier) -> UniswapV2Deployment:
-        """Get a router for a trading pair."""
-        return get_uniswap_for_pair(self.web3, factory_router_map, target_pair)
-
-    def check_has_enough_tokens(
-            self,
-            erc_20: Contract,
-            amount: int,
-    ):
-        """Check we have enough buy side tokens to do a trade.
-
-        This might not be the case if we are preparing transactions ahead of time and
-        sell might have not happened yet.
-        """
-        balance = erc_20.functions.balanceOf(self.hot_wallet.address).call()
-        if balance < amount:
-            token_details = fetch_erc20_details(
-                erc_20.web3,
-                erc_20.address,
-            )
-            d_balance = token_details.convert_to_decimals(balance)
-            d_amount = token_details.convert_to_decimals(amount)
-            raise OutOfBalance(f"Address {self.hot_wallet.address} does not have enough {token_details} tokens to trade. Need {d_amount}, has {d_balance}")
-
-    def ensure_token_approved(self,
-                              token_address: str,
-                              router_address: str) -> List[BlockchainTransaction]:
-        """Make sure we have ERC-20 approve() for the trade
-
-        - Infinite approval on-chain
-
-        - ...or previous approval in this state,
-
-        :param token_address:
-        :param router_address:
-
-        :return: Create 0 or 1 transactions if needs to be approved
-        """
-
-        if token_address in self.approved_routes[router_address]:
-            # Already approved for this cycle in previous trade
-            return []
-
-        erc_20 = get_deployed_contract(self.web3, "ERC20MockDecimals.json", Web3.toChecksumAddress(token_address))
-
-        # Set internal state we are approved
-        self.mark_router_approved(token_address, router_address)
-
-        hot_wallet = self.tx_builder.hot_wallet
-
-        if erc_20.functions.allowance(hot_wallet.address, router_address).call() > 0:
-            # already approved in previous execution cycle
-            return []
-        else:
-            # Create infinite approval
-            tx = self.tx_builder.create_transaction(
-                erc_20,
-                "approve",
-                (router_address, 2**256-1),
-                100_000,  # For approve, assume it cannot take more than 100k gas
-            )
-
-            return [tx]
-
-    def trade_on_router_two_way(self,
-            uniswap: UniswapV2Deployment,
-            target_pair: TradingPairIdentifier,
-            reserve_asset: AssetIdentifier,
-            reserve_amount: int,
-            max_slippage: float,
-            check_balances: False):
-        """Prepare the actual swap.
-
-        :param check_balances:
-            Check on-chain balances that the account has enough tokens
-            and raise exception if not.
-        """
-
-        web3 = self.web3
-        hot_wallet = self.tx_builder.hot_wallet
-
-        if reserve_asset == target_pair.quote:
-            # Buy with e.g. BUSD
-            base_token = get_token_for_asset(web3, target_pair.base)
-            quote_token = get_token_for_asset(web3, target_pair.quote)
-        elif reserve_asset == target_pair.base:
-            # Sell, flip the direction
-            base_token = get_token_for_asset(web3, target_pair.quote)
-            quote_token = get_token_for_asset(web3, target_pair.base)
-        else:
-            raise RuntimeError(f"Cannot trade {target_pair}")
-
-        if check_balances:
-            self.check_has_enough_tokens(quote_token, reserve_amount)
-
-        bound_swap_func = swap_with_slippage_protection(
-            uniswap,
-            recipient_address=hot_wallet.address,
-            base_token=base_token,
-            quote_token=quote_token,
-            amount_in=reserve_amount,
-            max_slippage=max_slippage * 100,  # In BPS
-        )
-        tx = self.tx_builder.sign_transaction(bound_swap_func, self.swap_gas_limit)
-        return [tx]
-
-    def trade_on_router_three_way(self,
-            uniswap: UniswapV2Deployment,
-            target_pair: TradingPairIdentifier,
-            intermediary_pair: TradingPairIdentifier,
-            reserve_asset: AssetIdentifier,
-            reserve_amount: int,
-            max_slippage: float,
-            check_balances: False):
-        """Prepare the actual swap for three way trade.
-
-        :param check_balances:
-            Check on-chain balances that the account has enough tokens
-            and raise exception if not.
-        """
-
-        web3 = self.web3
-        hot_wallet = self.tx_builder.hot_wallet
-
-        # Check we can chain two pairs
-        assert intermediary_pair.base == target_pair.quote, f"Could not hop from intermediary {intermediary_pair} -> destination {target_pair}"
-
-        assert target_pair.exchange_address, f"Target pair {target_pair} missing exchange information"
-        assert intermediary_pair.exchange_address, f"Intermediary pair {intermediary_pair} missing exchange information"
-
-        # Check routing happens on the same exchange
-        assert intermediary_pair.exchange_address.lower() == target_pair.exchange_address.lower()
-
-        if reserve_asset == intermediary_pair.quote:
-            # Buy BUSD -> BNB -> Cake
-            base_token = get_token_for_asset(web3, target_pair.base)
-            quote_token = get_token_for_asset(web3, intermediary_pair.quote)
-            intermediary_token = get_token_for_asset(web3, intermediary_pair.base)
-        elif reserve_asset == target_pair.base:
-            # Sell, Cake -> BNB -> BUSD
-            base_token = get_token_for_asset(web3, intermediary_pair.quote)  # BUSD
-            quote_token = get_token_for_asset(web3, target_pair.base)  # Cake
-            intermediary_token = get_token_for_asset(web3, intermediary_pair.base)  # BNB
-        else:
-            raise RuntimeError(f"Cannot trade {target_pair} through {intermediary_pair}")
-
-        if check_balances:
-            self.check_has_enough_tokens(quote_token, reserve_amount)
-
-        bound_swap_func = swap_with_slippage_protection(
-            uniswap,
-            recipient_address=hot_wallet.address,
-            base_token=base_token,
-            quote_token=quote_token,
-            amount_in=reserve_amount,
-            max_slippage=max_slippage * 100,  # In BPS,
-            intermediate_token=intermediary_token,
-        )
-
-        tx = self.tx_builder.sign_transaction(bound_swap_func, self.swap_gas_limit)
-        return [tx]
-
-
-class UniswapV2SimpleRoutingModel(RoutingModel):
-    """A simple router that does not optimise the trade execution cost.
+class EthereumRoutingModel(RoutingModel):
+    """A simple router that does not optimise the trade execution cost. Designed for uniswap-v2 forks.
 
     - Able to trade on multiple exchanges
 
     - Able to three-way trades through predefined intermediary hops,
       either on the exchange itself or some outside exchange
     """
-
+    
     def __init__(self,
-                 factory_router_map: Dict[str, Tuple[str, Optional[str]]],
                  allowed_intermediary_pairs: Dict[str, str],
                  reserve_token_address: str,
+                 chain_id: Optional[ChainId] = None,
                  ):
         """
-        :param factory_router_map:
+        
+        
+        :param addresses:
             Defines router smart contracts to be used with each DEX.
-            Each Uniswap v2 is uniquely identified by its factory contract.
-            Addresses always lowercase.
+            
+            Each Uniswap v2 is uniquely identified by its factory contract. Addresses always lowercase. Factory Router map
+            
+            For Uniswap V3, addresses is a dict of factory, router, position_manager,
+            and quoter addresses
 
         :param allowed_intermediary_pairs:
 
             Quote token address -> pair smart contract address mapping.
 
             Because we hold our reserves only in one currecy e.g. BUSD
             and we want to trade e.g. Cake/BNB pairs, we need to whitelist
             BNB as an allowed intermediary token.
             This makes it possible to do BUSD -> BNB -> Cake trade.
             This set is the list of pair smart contract addresses that
             are allowed to be used as a hop.
 
+        :param chain_id:
+            Store the chain id for which these routes were generated for.
+
         :param reserve_token_address:
             Token address of our reserve currency.
             Relevent for buy/sell routing.
             Lowercase.
         """
 
-        assert type(factory_router_map) == dict
-        assert type(allowed_intermediary_pairs) == dict
-        assert type(reserve_token_address) == str
-
-        assert reserve_token_address.lower() == reserve_token_address
-
-        # Convert all key addresses to lowercase to
-        # avoid mix up with Ethereum address checksums
-        self.factory_router_map = {k.lower(): v for k, v in factory_router_map.items()}
-        self.allowed_intermediary_pairs = {k.lower(): v.lower() for k, v in allowed_intermediary_pairs.items()}
-        self.reserve_token_address = reserve_token_address
-
-    def get_reserve_asset(self, pair_universe: PandasPairUniverse) -> AssetIdentifier:
-        """Translate our reserve token address tok an asset description."""
-        assert pair_universe is not None, "Pair universe missing"
-        reserve_token = pair_universe.get_token(self.reserve_token_address)
-        assert reserve_token, f"Pair universe does not contain our reserve asset {self.reserve_token_address}"
-        return translate_token(reserve_token)
+        super().__init__(allowed_intermediary_pairs, reserve_token_address)
+        
+        self.chain_id = chain_id
 
     def make_direct_trade(self,
-                          routing_state: UniswapV2RoutingState,
+                          routing_state: EthereumRoutingState,
                           target_pair: TradingPairIdentifier,
                           reserve_asset: AssetIdentifier,
                           reserve_amount: int,
                           max_slippage: float,
+                          address_map: Dict,
                           check_balances=False,
+                          asset_deltas: Optional[List[AssetDelta]] = None,
                           ) -> List[BlockchainTransaction]:
         """Prepare a trade where target pair has out reserve asset as a quote token.
 
         :return:
             List of approval transactions (if any needed)
         """
-        uniswap = routing_state.get_uniswap_for_pair(self.factory_router_map, target_pair)
+        uniswap = routing_state.get_uniswap_for_pair(address_map, target_pair)
         token_address = reserve_asset.address
-        txs = routing_state.ensure_token_approved(token_address, uniswap.router.address)
+        
+        # TODO find better way of doing this. Use inheritance?
+        if hasattr(uniswap, "router"):
+            txs = routing_state.ensure_token_approved(token_address, uniswap.router.address)
+        elif hasattr(uniswap, "swap_router"):
+            txs = routing_state.ensure_token_approved(token_address, uniswap.swap_router.address)
+        else:
+            raise TypeError("Incorrect Uniswap Instance provided. Can't get router.")
+            
         txs += routing_state.trade_on_router_two_way(
             uniswap,
             target_pair,
             reserve_asset,
             reserve_amount,
             max_slippage,
             check_balances,
+            asset_deltas=asset_deltas,
             )
         return txs
 
     def make_multihop_trade(self,
-                          routing_state: UniswapV2RoutingState,
+                          routing_state: EthereumRoutingState, # doesn't get full typing
+                              # EthereumRoutingState throws error
+                              # due to circular import
                           target_pair: TradingPairIdentifier,
                           intermediary_pair: TradingPairIdentifier,
                           reserve_asset: AssetIdentifier,
                           reserve_amount: int,
                           max_slippage: float,
+                          address_map: Dict,
                           check_balances=False,
+                          asset_deltas: Optional[List[AssetDelta]] = None,
                           ) -> List[BlockchainTransaction]:
         """Prepare a trade where target pair has out reserve asset as a quote token.
 
         :return:
             List of approval transactions (if any needed)
         """
-        uniswap = routing_state.get_uniswap_for_pair(self.factory_router_map, target_pair)
+        uniswap = routing_state.get_uniswap_for_pair(address_map, target_pair)
         token_address = reserve_asset.address
-        txs = routing_state.ensure_token_approved(token_address, uniswap.router.address)
+        
+        # TODO find better way of doing this. Use inheritance?
+        if hasattr(uniswap, "router"):
+            txs = routing_state.ensure_token_approved(token_address, uniswap.router.address)
+        elif hasattr(uniswap, "swap_router"):
+            txs = routing_state.ensure_token_approved(token_address, uniswap.swap_router.address)
+        else:
+            raise TypeError("Incorrect Uniswap Instance provided. Can't get router.")
+        
         txs += routing_state.trade_on_router_three_way(
             uniswap,
             target_pair,
             intermediary_pair,
             reserve_asset,
             reserve_amount,
             max_slippage,
             check_balances,
+            asset_deltas=asset_deltas,
             )
         return txs
 
     def trade(self,
-              routing_state: UniswapV2RoutingState,
+              routing_state: EthereumRoutingState,
               target_pair: TradingPairIdentifier,
               reserve_asset: AssetIdentifier,
               reserve_asset_amount: int,  # Raw amount of the reserve asset
               max_slippage: float=0.01,
               check_balances=False,
               intermediary_pair: Optional[TradingPairIdentifier] = None,
+              asset_deltas: Optional[List[AssetDelta]] = None,
               ) -> List[BlockchainTransaction]:
         """
 
         :param routing_state:
         :param target_pair:
         :param reserve_asset:
         :param reserve_asset_amount:
@@ -373,96 +176,48 @@
             BUSD -> BNB -> Cake.
         :return:
             List of prepared transactions to make this trade.
             These transactions, like approve() may relate to the earlier
             transactions in the `routing_state`.
         """
 
-        assert type(reserve_asset_amount) == int
-        assert max_slippage is not None, "Max slippage must be given"
-        assert type(max_slippage) == float
-        assert reserve_asset_amount > 0, f"For sells, switch reserve_asset to different token. Got target_pair: {target_pair}, reserve_asset: {reserve_asset}, amount: {reserve_asset_amount}"
+        self.pre_trade_assertions(reserve_asset_amount, max_slippage, target_pair, reserve_asset)
 
         # Our reserves match directly the asset on trading pair
         # -> we can do one leg trade
         if not intermediary_pair:
             if target_pair.quote == reserve_asset or target_pair.base == reserve_asset:
                 return self.make_direct_trade(
                     routing_state,
                     target_pair,
                     reserve_asset,
                     reserve_asset_amount,
                     max_slippage=max_slippage,
                     check_balances=check_balances,
+                    asset_deltas=asset_deltas,
                 )
             raise RuntimeError(f"Do not how to trade reserve {reserve_asset} with {target_pair}")
         else:
 
-            assert intermediary_pair.pool_address.lower() in self.allowed_intermediary_pairs.values(), f"Does not how to trade a pair. Got intermediary pair {intermediary_pair} that is not allowed, allowed intermediary pairs are {self.allowed_intermediary_pairs}"
+            self.intermediary_pair_assertion(intermediary_pair)
 
             return self.make_multihop_trade(
                 routing_state,
                 target_pair,
                 intermediary_pair,
                 reserve_asset,
                 reserve_asset_amount,
                 max_slippage=max_slippage,
                 check_balances=check_balances,
+                asset_deltas=asset_deltas,
             )
-
-    def route_pair(self, pair_universe: PandasPairUniverse, trading_pair: TradingPairIdentifier) \
-            -> Tuple[TradingPairIdentifier, Optional[TradingPairIdentifier]]:
-        """Return Uniswap routing information (path components) for a trading pair.
-
-        For three-way pairs, figure out the intermedia step.
-
-        :return:
-            (router address, target pair, intermediate pair) tuple
-        """
-
-        assert isinstance(trading_pair, TradingPairIdentifier)
-
-        reserve_asset = self.get_reserve_asset(pair_universe)
-
-        # We can directly do a two-way trade
-        if trading_pair.quote == reserve_asset:
-            return trading_pair, None
-
-        # Only issue for legacy code
-        assert pair_universe, "PairUniverse must be given so that we know how to route three way trades"
-
-        # Try to find a mid-hop pool for the trade
-        intermediate_pair_contract_address = self.allowed_intermediary_pairs.get(trading_pair.quote.address.lower())
-
-        if not intermediate_pair_contract_address:
-            raise CannotRouteTrade(f"Does not know how to trade pair {trading_pair} - supported intermediate tokens are {list(self.allowed_intermediary_pairs.keys())}")
-
-        dex_pair = pair_universe.get_pair_by_smart_contract(intermediate_pair_contract_address)
-        assert dex_pair is not None, f"Pair universe did not contain pair for a pair contract address {intermediate_pair_contract_address}, quote token is {trading_pair.quote}"
-
-        intermediate_pair = translate_trading_pair(dex_pair)
-        if not intermediate_pair:
-            raise CannotRouteTrade(f"Universe does not have a trading pair with smart contract address {intermediate_pair_contract_address}")
-
-        return trading_pair, intermediate_pair
-
-    def route_trade(self, pair_universe: PandasPairUniverse, trade: TradeExecution) -> Tuple[TradingPairIdentifier, Optional[TradingPairIdentifier]]:
-        """Figure out how to map an abstract trade to smart contracts.
-
-        Decide if we can do a direct trade in the pair pool.
-        or if we need to hop through another pool to buy the token we want to buy.
-
-        :return:
-            target pair, intermediary pair tuple
-        """
-        return self.route_pair(pair_universe, trade.pair)
-
+    
     def execute_trades_internal(self,
                        pair_universe: PandasPairUniverse,
-                       routing_state: UniswapV2RoutingState,
+                       routing_state: EthereumRoutingState,
                        trades: List[TradeExecution],
                        check_balances=False):
         """Split for testability.
 
         :param check_balances:
             Check that the wallet has enough reserves to perform the trades
             before executing them. Because we are selling before buying.
@@ -478,64 +233,73 @@
         txs: List[BlockchainTransaction] = []
 
         reserve_asset = self.get_reserve_asset(pair_universe)
 
         for t in trades:
             assert len(t.blockchain_transactions) == 0, f"Trade {t} had already blockchain transactions associated with it"
 
+            # TODO: Add support for accurate multihop asset deltas
+            if t.slippage_tolerance is not None:
+                asset_deltas = t.calculate_asset_deltas()
+            else:
+                # Old path that does not slippage tolerances for trades
+                asset_deltas = None
+
             target_pair, intermediary_pair = self.route_trade(pair_universe, t)
 
             if intermediary_pair is None:
                 # Two way trade
-                # Decide betwen buying and selling
-                if t.is_buy():
-                   trade_txs = self.trade(
+                # Decide between buying and selling
+                trade_txs = (
+                    self.trade(
                         routing_state,
                         target_pair=target_pair,
                         reserve_asset=reserve_asset,
                         reserve_asset_amount=t.get_raw_planned_reserve(),
                         check_balances=check_balances,
+                        asset_deltas=asset_deltas,
                     )
-                else:
-                    trade_txs = self.trade(
+                    if t.is_buy()
+                    else self.trade(
                         routing_state,
                         target_pair=target_pair,
                         reserve_asset=target_pair.base,
                         reserve_asset_amount=-t.get_raw_planned_quantity(),
                         check_balances=check_balances,
+                        asset_deltas=asset_deltas,
                     )
+                )
+            elif t.is_buy():
+                trade_txs = self.trade(
+                    routing_state,
+                    target_pair=target_pair,
+                    reserve_asset=reserve_asset,
+                    reserve_asset_amount=t.get_raw_planned_reserve(),
+                    check_balances=check_balances,
+                    intermediary_pair=intermediary_pair,
+                )
             else:
-                # Three-way trade!
-                if t.is_buy():
-                    trade_txs = self.trade(
-                        routing_state,
-                        target_pair=target_pair,
-                        reserve_asset=reserve_asset,
-                        reserve_asset_amount=t.get_raw_planned_reserve(),
-                        check_balances=check_balances,
-                        intermediary_pair=intermediary_pair,
-                    )
-                else:
-                    trade_txs = self.trade(
-                        routing_state,
-                        target_pair=target_pair,
-                        reserve_asset=target_pair.base,
-                        reserve_asset_amount=-t.get_raw_planned_quantity(),
-                        check_balances=check_balances,
-                        intermediary_pair=intermediary_pair,
-                    )
+                trade_txs = self.trade(
+                    routing_state,
+                    target_pair=target_pair,
+                    reserve_asset=target_pair.base,
+                    reserve_asset_amount=-t.get_raw_planned_quantity(),
+                    check_balances=check_balances,
+                    intermediary_pair=intermediary_pair,
+                    asset_deltas=asset_deltas,
+                )
 
             t.set_blockchain_transactions(trade_txs)
             txs += trade_txs
 
         # Now all trades have transactions associated with them.
         # We can start to execute transactions.
 
     def setup_trades(self,
-                     routing_state: UniswapV2RoutingState,
+                     routing_state: EthereumRoutingState,
                      trades: List[TradeExecution],
                      check_balances=False):
         """Strategy and live execution connection.
 
         Turns abstract strategy trades to real blockchain transactions.
 
         - Modifies TradeExecution objects in place and associates a blockchain transaction for each
@@ -549,78 +313,81 @@
 
 
         :param max_slippage:
             Max slippaeg tolerated per trade. 0.01 is 1%.
 
         """
         return self.execute_trades_internal(routing_state.pair_universe, routing_state, trades, check_balances)
-
+    
     def create_routing_state(self,
                              universe: StrategyExecutionUniverse,
-                             execution_details: dict) -> RoutingState:
+                             execution_details: dict,
+                             Routing_State: Type[EthereumRoutingState] 
+                             # Doesn't get full typing
+                             # Type[UniswapV2RoutingState] | Type[UniswapV3RoutingState]
+                             # throws error due to circular import
+                             ) -> EthereumRoutingState:
         """Create a new routing state for this cycle.
 
         - Connect routing to web3 and hot wallet
 
         - Read on-chain data on what gas fee we are going to use
 
         - Setup transaction builder based on this information
         """
 
         assert isinstance(universe, TradingStrategyUniverse)
         assert universe is not None, "Universe is required"
         assert universe.universe.pairs is not None, "Pairs are required"
 
-        web3 = execution_details["web3"]
-        hot_wallet = execution_details["hot_wallet"]
 
-        fees = estimate_gas_fees(web3)
-        logger.info("Estimated gas fees for chain %d: %s", web3.eth.chain_id, fees)
-        tx_builder = TransactionBuilder(web3, hot_wallet, fees)
-        routing_state = UniswapV2RoutingState(universe.universe.pairs, tx_builder)
-        return routing_state
+        tx_builder = execution_details.get("tx_builder")
+        if tx_builder is not None:
+            # Modern code path
+            routing_state = Routing_State(universe.universe.pairs, tx_builder=tx_builder)
+        else:
+            # Legacy code path - do not use
 
-    def perform_preflight_checks_and_logging(self,
-        routing_state: UniswapV2RoutingState,
-        pair_universe: PandasPairUniverse):
-        """"Checks the integrity of the routing.
+            web3 = execution_details["web3"]
 
-        - Called from check-wallet to see our routing and balances are good
-        """
+            # Hot wallet is not present in dummy execution model
+            hot_wallet = execution_details.get("hot_wallet")
 
-        logger.info("Routing details")
-        for factory, router in self.factory_router_map.items():
-            logger.info("  Factory %s uses router %s", factory, router[0])
+            fees = estimate_gas_fees(web3)
 
-        reserve = self.get_reserve_asset(pair_universe)
-        logger.info("  Routed reserve asset is %s", reserve)
+            logger.info("Gas fee estimations for chain %d: %s", web3.eth.chain_id, fees)
 
+            logger.info("Estimated gas fees for chain %d: %s", web3.eth.chain_id, fees)
+            if hot_wallet is not None:
+                tx_builder = HotWalletTransactionBuilder(web3, hot_wallet)
+                routing_state = Routing_State(universe.universe.pairs, tx_builder)
+            else:
+                routing_state = Routing_State(universe.universe.pairs,
+                                              tx_builder=None,
+                                              web3=web3)
 
-def route_tokens(
-        trading_pair: TradingPairIdentifier,
-        intermediate_pair: Optional[TradingPairIdentifier],
-)-> Tuple[ChecksumAddress, ChecksumAddress, Optional[ChecksumAddress]]:
-    """Convert trading pair route to physical token addresses.
-    """
+        return routing_state
+    
+    def route_trade(self, pair_universe: PandasPairUniverse, trade: TradeExecution) -> Tuple[TradingPairIdentifier, Optional[TradingPairIdentifier]]:
+        """Figure out how to map an abstract trade to smart contracts.
 
-    if intermediate_pair is None:
-        return (Web3.toChecksumAddress(trading_pair.base.address),
-            Web3.toChecksumAddress(trading_pair.quote.address),
-            None)
-
-    return (Web3.toChecksumAddress(trading_pair.base.address),
-        Web3.toChecksumAddress(intermediate_pair.quote.address),
-        Web3.toChecksumAddress(trading_pair.quote.address))
-
-
-def get_uniswap_for_pair(web3: Web3, factory_router_map: dict, target_pair: TradingPairIdentifier) -> UniswapV2Deployment:
-    """Get a router for a trading pair."""
-    assert target_pair.exchange_address, f"Exchange address missing for {target_pair}"
-    factory_address = Web3.toChecksumAddress(target_pair.exchange_address)
-    router_address, init_code_hash = factory_router_map[factory_address.lower()]
-
-    return fetch_deployment(
-        web3,
-        factory_address,
-        Web3.toChecksumAddress(router_address),
-        init_code_hash=init_code_hash,
-    )
+        Decide if we can do a direct trade in the pair pool.
+        or if we need to hop through another pool to buy the token we want to buy.
+
+        :return:
+            target pair, intermediary pair tuple
+        """
+        return self.route_pair(pair_universe, trade.pair)
+    
+    def intermediary_pair_assertion(self, intermediary_pair: TradingPairIdentifier):
+        assert intermediary_pair.pool_address.lower() in self.allowed_intermediary_pairs.values(), f"Does not how to trade a pair. Got intermediary pair {intermediary_pair} that is not allowed, allowed intermediary pairs are {self.allowed_intermediary_pairs}"
+    
+    def reserve_asset_logging(self, pair_universe: PandasPairUniverse) -> None:
+        reserve = self.get_reserve_asset(pair_universe)
+        logger.info("  Routed reserve asset is %s", reserve)
+    
+    @staticmethod
+    def route_pair_assertions(trading_pair, pair_universe):
+        assert isinstance(trading_pair, TradingPairIdentifier)
+
+        # Only issue for legacy code
+        assert pair_universe, "PairUniverse must be given so that we know how to route three way trades"
```

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/uniswap_v2_valuation.py` & `trade_executor-0.3/tradeexecutor/ethereum/uniswap_v2/uniswap_v2_valuation.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,50 +2,42 @@
 
 Value positions based on their "dump" price on Uniswap,
 assuming we get the worst possible single trade execution.
 """
 import datetime
 from typing import Tuple
 
-from tradeexecutor.ethereum.uniswap_v2_live_pricing import UniswapV2LivePricing
+from tradeexecutor.ethereum.uniswap_v2.uniswap_v2_live_pricing import UniswapV2LivePricing
 from tradeexecutor.state.position import TradingPosition
 from tradeexecutor.state.types import USDollarAmount
-from tradeexecutor.strategy.valuation import ValuationModel
+from tradeexecutor.ethereum.eth_valuation import EthereumPoolRevaluator
 
 
-class UniswapV2PoolRevaluator(ValuationModel):
+class UniswapV2PoolRevaluator(EthereumPoolRevaluator):
     """Re-value assets based on their on-chain price.
 
     Does directly JSON-RPC call to get the latest price in the Uniswap pools.
 
     Only uses direct route - mostly useful for testing, may not give a realistic price in real
     world with multiple order routing options.
 
     .. warning ::
 
         This valuation metohd always uses the latest price. It
         cannot be used for backtesting.
     """
 
     def __init__(self, pricing_model: UniswapV2LivePricing):
-        self.pricing_model = pricing_model
+        
+        super().__init__(pricing_model)
+        
+        assert isinstance(pricing_model, UniswapV2LivePricing)
 
     def __call__(self,
                  ts: datetime.datetime,
                  position: TradingPosition) -> Tuple[datetime.datetime, USDollarAmount]:
-        assert isinstance(ts, datetime.datetime)
-        pair = position.pair
 
-        assert position.is_long(), "Short not supported"
-
-        quantity = position.get_quantity()
-        # Cannot do pricing for zero quantity
-        if quantity == 0:
-            return ts, 0.0
-
-        price = self.pricing_model.get_sell_price(ts, pair, quantity)
-
-        return ts, price
+        return super().__call__(ts, position)
 
 
 def uniswap_v2_sell_valuation_factory(pricing_model):
     return UniswapV2PoolRevaluator(pricing_model)
```

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/uniswap_v2_valuation_v0.py` & `trade_executor-0.3/tradeexecutor/ethereum/uniswap_v2/uniswap_v2_valuation_v0.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 """
 
 import datetime
 from typing import Tuple
 
 from eth_defi.uniswap_v2.deployment import UniswapV2Deployment
 from eth_defi.uniswap_v2.fees import estimate_sell_received_amount_raw
-from tradeexecutor.ethereum.uniswap_v2_live_pricing import UniswapV2LivePricing
 from tradeexecutor.state.position import TradingPosition
 from tradeexecutor.state.types import USDollarAmount
 from tradeexecutor.strategy.valuation import ValuationModel
 
 
 class UniswapV2PoolValuationMethodV0(ValuationModel):
     """Legacy valuation methdd.
```

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/universe.py` & `trade_executor-0.3/tradeexecutor/ethereum/universe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 """Reverse engineering Trading Strategy trading universe from the local EVM tester Uniswap v2 deployment."""
-from typing import List
+from typing import List, Optional
 
 import pandas as pd
 from web3 import Web3
 
 from eth_defi.uniswap_v2.deployment import UniswapV2Deployment
 from tradeexecutor.state.identifier import TradingPairIdentifier
 from tradingstrategy.chain import ChainId
 from tradingstrategy.exchange import ExchangeUniverse, Exchange, ExchangeType
 from tradingstrategy.pair import DEXPair, PandasPairUniverse
 
 
-def create_pair_universe(web3: Web3, exchange: Exchange, pairs: List[TradingPairIdentifier]) -> PandasPairUniverse:
-    """Creates a PairUniverse from Trade Executor test data.
+def create_pair_universe(web3: Web3, exchange: Optional[Exchange], pairs: List[TradingPairIdentifier]) -> PandasPairUniverse:
+    """Creates a PairUniverse from on-chain test data.
 
-    PairUniverse is used by QSTrader based tests, so we need to support it.
+    A test trading universe.
+
+    :param web3:
+        Web3 connection to the test backend
+
+    :param exchange:
+        Exchange under which pairs are assigned
+
+    :param pairs:
+        Trading pairs that will form this pair universe
     """
 
     chain_id = ChainId(web3.eth.chain_id)
 
     data = []
     for p in pairs:
         assert p.exchange_address
         assert p.base.decimals
         assert p.quote.decimals
         assert p.base.address != p.quote.address
+        assert p.fee is not None, f"Pair missing fee {p}"
         dex_pair = DEXPair(
             pair_id=int(p.get_identifier(), 16),
             chain_id=chain_id,
             exchange_id=exchange.exchange_id if exchange else 1,
             exchange_address=p.exchange_address if exchange else None,
             address=p.pool_address,
             dex_type=ExchangeType.uniswap_v2,
@@ -36,14 +46,15 @@
             quote_token_symbol=p.quote.token_symbol,
             token0_symbol=p.base.token_symbol,
             token1_symbol=p.quote.token_symbol,
             token0_address=p.base.address,
             token1_address=p.quote.address,
             token0_decimals=p.base.decimals,
             token1_decimals=p.quote.decimals,
+            fee=int(p.fee * 10000),
         )
         data.append(dex_pair.to_dict())
     df = pd.DataFrame(data)
     return PandasPairUniverse(df)
 
 
 def create_exchange_universe(web3: Web3, uniswaps: List[UniswapV2Deployment]) -> ExchangeUniverse:
```

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/wallet.py` & `trade_executor-0.3/tradeexecutor/ethereum/wallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         current_reserves: List[ReservePosition],
         supported_reserve_currencies: List[AssetIdentifier]) -> List[ReserveUpdateEvent]:
     """Check the address for any incoming stablecoin transfers to see how much cash we have."""
 
     our_chain_id = web3.eth.chain_id
 
     # Get raw ERC-20 holdings of the address
-    balances = update_wallet_balances(web3, wallet_address, [web3.toChecksumAddress(a.address) for a in supported_reserve_currencies])
+    balances = update_wallet_balances(web3, wallet_address, [web3.to_checksum_address(a.address) for a in supported_reserve_currencies])
 
     reserves_per_token = {r.asset.address: r for r in current_reserves}
 
     events: ReserveUpdateEvent = []
 
     for currency in supported_reserve_currencies:
 
@@ -60,15 +60,15 @@
 
         if currency.address in reserves_per_token:
             # We have an existing record of having this reserve
             current_value = reserves_per_token[address].quantity
         else:
             current_value = Decimal(0)
 
-        decimal_holding = balances.get(Web3.toChecksumAddress(address))
+        decimal_holding = balances.get(Web3.to_checksum_address(address))
 
         # We get decimals = None if Ganache is acting
         assert decimal_holding.decimals, f"Token did not have decimals: token:{currency} holding:{decimal_holding}"
 
         if (decimal_holding is not None) and (decimal_holding.value != current_value):
             evt = ReserveUpdateEvent(
                 asset=currency,
```

### Comparing `trade_executor-0.2/tradeexecutor/ethereum/web3config.py` & `trade_executor-0.3/tradeexecutor/ethereum/web3config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Web3 connection configuration."""
 
 import logging
 from dataclasses import field, dataclass
 from typing import Dict, Optional
 
 from eth_defi.gas import GasPriceMethod, node_default_gas_price_strategy
+from eth_defi.middleware import http_retry_request_with_sleep_middleware
 from tradingstrategy.chain import ChainId
 from web3 import Web3, HTTPProvider
 from web3.middleware import geth_poa_middleware
+from web3.providers.eth_tester.middleware import default_transaction_fields_middleware, ethereum_tester_middleware
 
 from tradeexecutor.utils.url import get_url_domain
 
 #: List of currently supportd EVM blockchains
 SUPPORTED_CHAINS = [
     ChainId.ethereum,
     ChainId.avalanche,
     ChainId.polygon,
     ChainId.bsc,
+    ChainId.arbitrum,
+    ChainId.anvil
 ]
 
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -47,22 +51,34 @@
             JSON-RPC node URL
 
         :param gas_price_method:
             How do we estimate gas for a transaction
             If not given autodetect the method.
         """
 
-        web3 = Web3(HTTPProvider(url))
+        provider = HTTPProvider(url)
+
+        # Web3 6.0 fixes
+        provider.middlewares = (
+            #    attrdict_middleware,
+            # default_transaction_fields_middleware,
+            #ethereum_tester_middleware,
+        )
+
+        web3 = Web3(provider)
+
+        web3.middleware_onion.clear()
 
         # Read numeric chain id from JSON-RPC
         chain_id = web3.eth.chain_id
 
         if gas_price_method is None:
-            if chain_id == ChainId.ethereum.value:
-                # Ethereum supports maxBaseFee method
+            if chain_id in (ChainId.ethereum.value, ChainId.ganache.value, ChainId.avalanche.value, ChainId.polygon.value, ChainId.anvil.value):
+                # Ethereum supports maxBaseFee method (London hard fork)
+                # Same for Avalanche C-chain https://twitter.com/avalancheavax/status/1389763933448323073
 
                 gas_price_method = GasPriceMethod.london
             else:
                 # Other nodes have the legacy method
                 #
                 #   File "/Users/moo/Library/Caches/pypoetry/virtualenvs/trade-executor-8Oz1GdY1-py3.10/lib/python3.10/site-packages/web3/contract.py", line 1672, in build_transaction_for_function
                 #     prepared_transaction = fill_transaction_defaults(web3, prepared_transaction)
@@ -75,40 +91,58 @@
                 #     return self.__dict__[key]  # type: ignore
                 # KeyError: 'baseFeePerGas'
 
                 gas_price_method = GasPriceMethod.legacy
 
         assert isinstance(gas_price_method, GasPriceMethod)
 
-        logger.info("Connected to chain id: %d, using gas price method %s", chain_id, gas_price_method.name)
+        chain_id_obj = ChainId(chain_id)
+
+        logger.trade("Connected to chain: %s, node provider: %s, gas pricing method: %s",
+                     chain_id_obj.name,
+                     get_url_domain(url),
+                     gas_price_method.name)
 
         # London is the default method
         if gas_price_method == GasPriceMethod.legacy:
             logger.info("Setting up gas price middleware for Web3")
             web3.eth.set_gas_price_strategy(node_default_gas_price_strategy)
 
         # Set POA middleware if needed
-        if chain_id in (ChainId.bsc.value, ChainId.polygon.value):
-            logger.info("Using proof-of-authority web3 middleware")
+        if chain_id in (ChainId.bsc.value, ChainId.polygon.value, ChainId.avalanche.value):
+            logger.info("Using proof-of-authority web3 middleware for chain %d", chain_id)
             web3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
+        # Set up automatic rqeuest replays in the case of network issues
+        web3.middleware_onion.inject(http_retry_request_with_sleep_middleware, layer=0)
+
         return web3
 
     def close(self):
         """Close all connections."""
         # Web3.py does not offer close
         pass
 
+    def choose_single_chain(self):
+        """Set the default chain we are connected to.
+
+        Ensure we have exactly 1 JSON-RPC endpoint configured.
+        """
+        assert len(self.connections) == 1, f"Expected a single web3 connection, got JSON-RPC for chains {list(self.connections.keys())}"
+        default_chain_id = next(iter(self.connections.keys()))
+        self.set_default_chain(default_chain_id)
+        self.check_default_chain_id()
+
     def set_default_chain(self, chain_id: ChainId):
         """Set the default chain our strategy runs on.
 
         Most strategies are single chain strategies.
         Set the chain id we expect these strategies to run on.
         """
-        assert isinstance(chain_id, ChainId), f"Got {chain_id}"
+        assert isinstance(chain_id, ChainId), f"Attempt to set null chain as the default: {chain_id}"
         self.default_chain_id = chain_id
 
     def get_connection(self, chain_id: ChainId) -> Optional[Web3]:
         """Get a connection to a specific network."""
         return self.connections[chain_id]
 
     def get_default(self) -> Web3:
@@ -116,15 +150,15 @@
 
         Assumes exactly 1 node connection available.
         """
         assert self.default_chain_id
         try:
             return self.connections[self.default_chain_id]
         except KeyError:
-            raise RuntimeError(f"We haev {self.default_chain_id.name} configured as the default blockchain, but we do not have a connection for it in the connection pool. Did you pass right RPC configuration?")
+            raise RuntimeError(f"We have {self.default_chain_id.name} configured as the default blockchain, but we do not have a connection for it in the connection pool. Did you pass right RPC configuration?")
 
     def check_default_chain_id(self):
         """Check that we are connected to the correct chain.
 
         The JSON-RPC node chain id should be the same as in the strategy module.
         """
```

### Comparing `trade_executor-0.2/tradeexecutor/monkeypatch/dataclasses_json.py` & `trade_executor-0.3/tradeexecutor/monkeypatch/dataclasses_json.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,85 @@
-"""Fix dataclasses_json to always serialised and deserialise dates in the timezone-naive format."""
-from datetime import datetime
-from datetime import timezone
+"""Fix dataclasses_json to support us.
+
+ - Always serialised and deserialise dates in the timezone-naive format
+
+ - Add support for timedelta objects
+
+ """
+
+import json
+from datetime import datetime, timedelta
 from decimal import Decimal
+from enum import Enum
+from typing import Collection, Mapping
 from uuid import UUID
 
 from dataclasses_json import core
 
+from tradeexecutor.utils.timestamp import convert_and_validate_timestamp_as_float
+
+
+# Mankeypatched _ExtendedEncoder.default()
+def _patched_default(self, o) -> core.Json:
+    result: core.Json
+    if core._isinstance_safe(o, Collection):
+        if core._isinstance_safe(o, Mapping):
+            result = dict(o)
+        else:
+            result = list(o)
+    elif core._isinstance_safe(o, datetime):
+        #assert o.tzinfo == None, "Received a datetime with attached tz info: {o}"
+        result = convert_and_validate_timestamp_as_float(o)
+    #
+    # Patch timedelta support
+    #
+    elif core._isinstance_safe(o, timedelta):
+        result = o.total_seconds()
+    elif core._isinstance_safe(o, UUID):
+        result = str(o)
+    elif core._isinstance_safe(o, Enum):
+        result = o.value
+    elif core._isinstance_safe(o, Decimal):
+        result = str(o)
+    else:
+        result = json.JSONEncoder.default(self, o)
+    return result
+
 
 def _patched_support_extended_types(field_type, field_value):
     if core._issubclass_safe(field_type, datetime):
         if isinstance(field_value, datetime):
             res = field_value
         else:
             # Fixed here
             # tz = datetime.now(timezone.utc).astimezone().tzinfo
-            res = datetime.fromtimestamp(field_value, tz=None)
+            res = datetime.utcfromtimestamp(field_value)
+    #
+    # Add timedelta support
+    #
+    elif core._issubclass_safe(field_type, timedelta):
+        if isinstance(field_value, timedelta):
+            res = field_value
+        else:
+            # Fixed here
+            # tz = datetime.now(timezone.utc).astimezone().tzinfo
+            res = timedelta(seconds=field_value)
     elif core._issubclass_safe(field_type, Decimal):
         res = (field_value
                if isinstance(field_value, Decimal)
                else Decimal(field_value))
     elif core._issubclass_safe(field_type, UUID):
         res = (field_value
                if isinstance(field_value, UUID)
                else UUID(field_value))
     else:
         res = field_value
     return res
 
 
 def patch_dataclasses_json():
+    """Add monkey patched fixes to dataclasses_json package"""
     if core._support_extended_types != _patched_support_extended_types:
         core._support_extended_types = _patched_support_extended_types
 
+    core._ExtendedEncoder.default = _patched_default
+
```

### Comparing `trade_executor-0.2/tradeexecutor/state/__init__.py` & `trade_executor-0.3/tradeexecutor/state/__init__.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/state/freeze.py` & `trade_executor-0.3/tradeexecutor/state/freeze.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             assert position is not None, f"Could not find the position for trade {t}"
 
             assert position.is_open(), "Cannot freeze position that is not open"
             portfolio.frozen_positions[position.position_id] = position
             position.frozen_at = ts
             del portfolio.open_positions[position.position_id]
 
+            # Mark assets automatically blacklisted so no future trades
             state.blacklist_asset(position.pair.base)
 
             failed.append(t)
         else:
             succeeded.append(t)
 
     return succeeded, failed
```

### Comparing `trade_executor-0.2/tradeexecutor/state/store.py` & `trade_executor-0.3/tradeexecutor/state/store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """State serialisation to disk and JavaScript clients."""
 import abc
+import datetime
 import enum
 import json
 import os
 import shutil
 import tempfile
 from pathlib import Path
 import logging
@@ -38,16 +39,23 @@
         """Load the state from the storage."""
 
     @abc.abstractmethod
     def sync(self, state: State):
         """Save the state to the storage."""
 
     @abc.abstractmethod
-    def create(self) -> State:
-        """Create a new state storage."""
+    def create(self, name: str) -> State:
+        """Create a new state storage.
+
+        :param name:
+            Name of the strategy this State belongs to
+        """
+        state = State()
+        state.name = name
+        return state
 
 
 class JSONFileStore(StateStore):
     """Store the state of the executor as a JSON file.
 
     - Read by strategy on a startup
 
@@ -56,28 +64,34 @@
 
     def __init__(self, path: Union[Path, str]):
         assert path
         if not isinstance(path, Path):
             path = Path(path)
         self.path = path
 
+    def __repr__(self):
+        path = os.path.abspath(self.path)
+        return f"<JSON file at {path}>"
+
     def is_pristine(self) -> bool:
         return not self.path.exists()
 
     def load(self) -> State:
         logger.info("Loaded state from %s", self.path)
         with open(self.path, "rt") as inp:
             return State.from_json(inp.read())
 
     def sync(self, state: State):
         """Write new JSON state dump using Linux atomic file replacement."""
         dirname, basename = os.path.split(self.path)
         temp = tempfile.NamedTemporaryFile(mode='wt', delete=False, dir=dirname)
         with open(temp.name, "wt") as out:
 
+            state.last_updated_at = datetime.datetime.utcnow()
+
             # Insert special validation logic here to have
             # friendly error messages for the JSON serialisation errors
             data = state.to_dict(encode_json=False)
             validate_nested_state_dict(data)
 
             try:
                 txt = json.dumps(data, cls=_ExtendedEncoder)
@@ -90,17 +104,17 @@
                 raise
 
             out.write(txt)
             logger.info("Saved state to %s, total %d chars", self.path, len(txt))
         temp.close()
         shutil.move(temp.name, self.path)
 
-    def create(self) -> State:
+    def create(self, name: str) -> State:
         logger.info("Created new state for %s", self.path)
-        return State()
+        return super().create(name)
 
 
 class NoneStore(StateStore):
     """Store that is not persistent.
 
     Used in unit tests. Seed with initial state.
     """
@@ -117,13 +131,13 @@
         return False
 
     def load(self) -> State:
         return self.state
 
     def sync(self, state: State):
         """Do not persist anything."""
-        pass
+        state.last_updated_at = datetime.datetime.utcnow()
 
     def create(self) -> State:
         raise NotImplementedError("This should not be called for NoneStore.\n"
                                   "Backtest have explicit state set for them at the start that should not be cleared.")
```

### Comparing `trade_executor-0.2/tradeexecutor/state/validator.py` & `trade_executor-0.3/tradeexecutor/state/validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 Any error message contains tree presentation of the state,
 so you can easily locate any values that are bad, unlike with :py:mod:`json`.
 """
 import datetime
 from decimal import Decimal
 from enum import Enum
+from json.encoder import INFINITY
 from types import NoneType
 
 import pandas as pd
 import numpy as np
 
 from tradeexecutor.state.state import State
 
@@ -28,30 +29,58 @@
     float,
     int,
     str,
     NoneType,
     Enum,  # Supported by dadtaclasses_json
     datetime.datetime,  # Supported by dadtaclasses_json
     Decimal,  # Supported by dadtaclasses_json
+    datetime.timedelta,
 )
 
 #: We especially do not want to see these in serialisation.
 #: We need to do negative test, because Pandas types to some base class
 #: magic.
 BAD_VALUE_TYPES = (
     np.float32,
     np.float64,
     pd.Timedelta,
     pd.Timestamp,
 )
 
+_inf=INFINITY
+
+_neginf=-INFINITY
+
+# https://www.tutorialspoint.com/what-is-javascript-s-highest-integer-value-that-a-number-can-go-to-without-losing-precision
+JS_MAX_INT = 9007199254740991
+
 
 def validate_state_value(name: str | int, val: object):
     """Check the state value against our whitelist and blacklist."""
 
+    if type(val) in (int, float):
+        # JavaScript number compatibility check
+
+        o = val
+        if o != o:
+            text = 'NaN'
+        elif o == _inf:
+            text = 'Infinity'
+        elif o == _neginf:
+            text = '-Infinity'
+        else:
+            text = None
+
+        if text:
+            raise BadStateData(f"{name}: {val} ({type(val)} - not a number: {text}")
+
+    if type(val) == int:
+        if val > JS_MAX_INT:
+            raise BadStateData(f"{name}: {val} ({type(val)} - larger than JavaScript max int")
+
     if isinstance(val, BAD_VALUE_TYPES):
         raise BadStateData(f"{name}: {val} ({type(val)} - blacklisted value type")
 
     if not isinstance(val, ALLOWED_VALUE_TYPES):
         raise BadStateData(f"{name}: {val} ({type(val)} - value type is not in supported serialisable types")
```

### Comparing `trade_executor-0.2/tradeexecutor/statistics/core.py` & `trade_executor-0.3/tradeexecutor/statistics/core.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/strategy/approval.py` & `trade_executor-0.3/tradeexecutor/strategy/approval.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/strategy/bootstrap.py` & `trade_executor-0.3/tradeexecutor/strategy/bootstrap.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,26 +6,29 @@
 
 See :py:mod:`strategy_module` instead.
 
 """
 import logging
 from contextlib import AbstractContextManager
 from pathlib import Path
+from typing import Optional
 
+from tradeexecutor.strategy.routing import RoutingModel
 from tradingstrategy.client import Client
 
-from tradeexecutor.ethereum.default_routes import get_routing_model
-from tradeexecutor.state.sync import SyncMethod
+from tradeexecutor.ethereum.routing_data import get_routing_model
+from tradeexecutor.strategy.sync_model import SyncMethodV0, SyncModel
 from tradeexecutor.strategy.approval import ApprovalModel
 from tradeexecutor.strategy.description import StrategyExecutionDescription
 from tradeexecutor.strategy.execution_context import ExecutionContext
 from tradeexecutor.strategy.execution_model import ExecutionModel
 from tradeexecutor.strategy.factory import StrategyFactory
 from tradeexecutor.strategy.pandas_trader.runner import PandasTraderRunner
 from tradeexecutor.strategy.pricing_model import PricingModelFactory
+from tradeexecutor.strategy.run_state import RunState
 from tradeexecutor.strategy.strategy_module import read_strategy_module, StrategyModuleInformation
 from tradeexecutor.strategy.strategy_type import StrategyType
 from tradeexecutor.strategy.trading_strategy_universe import DefaultTradingStrategyUniverseModel
 from tradeexecutor.strategy.valuation import ValuationModelFactory
 
 logger = logging.getLogger(__name__)
 
@@ -88,51 +91,67 @@
 
     assert mod_info, "chain_id blockchain information missing from the strategy module"
 
     def default_strategy_factory(
             *ignore,
             execution_model: ExecutionModel,
             execution_context: ExecutionContext,
-            sync_method: SyncMethod,
+            sync_model: SyncModel,
             pricing_model_factory: PricingModelFactory,
             valuation_model_factory: ValuationModelFactory,
             client: Client,
             timed_task_context_manager: AbstractContextManager,
             approval_model: ApprovalModel,
+            run_state: RunState,
+            routing_model: Optional[RoutingModel]=None,
             **kwargs) -> StrategyExecutionDescription:
 
+        # Migration assert
+        assert run_state, "run_state needs to be passed for new strategies"
+
         if ignore:
             # https://www.python.org/dev/peps/pep-3102/
             raise TypeError("Only keyword arguments accepted")
 
+        if sync_model is not None:
+            assert isinstance(sync_model, SyncModel), f"SyncModel not good: {sync_model}"
+
         universe_model = DefaultTradingStrategyUniverseModel(
             client,
             execution_context,
             mod_info.create_trading_universe)
 
-        routing_model = get_routing_model(
-            execution_context,
-            mod_info.trade_routing,
-            mod_info.reserve_currency)
+        # Routing model can come with hardcoded Python tables of addresses (see default_routes.py)
+        # or it is dynamically generated for any local dev chain.
+        # If it is not dynamically generated, here set up one of the default routing models from
+        # strategy module's trade_routing var.
+        if routing_model is None:
+            routing_model = get_routing_model(
+                execution_context,
+                mod_info.trade_routing,
+                mod_info.reserve_currency)
 
         runner = PandasTraderRunner(
             timed_task_context_manager=timed_task_context_manager,
             execution_model=execution_model,
             approval_model=approval_model,
             valuation_model_factory=valuation_model_factory,
-            sync_method=sync_method,
+            sync_model=sync_model,
             pricing_model_factory=pricing_model_factory,
             routing_model=routing_model,
             decide_trades=mod_info.decide_trades,
+            execution_context=execution_context,
+            run_state=run_state,
         )
 
         return StrategyExecutionDescription(
             universe_model=universe_model,
             runner=runner,
             trading_strategy_engine_version=mod_info.trading_strategy_engine_version,
             cycle_duration=mod_info.trading_strategy_cycle,
             chain_id=mod_info.chain_id,
+            source_code=mod_info.source_code,
         )
 
     return default_strategy_factory
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/cycle.py` & `trade_executor-0.3/tradeexecutor/strategy/cycle.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,38 +20,66 @@
 
     All cycles are aligned to the wall clock time.
     E.g. 24h cycle is always run at 00:00.
 
     See :ref:`strategy cycle` for more information.
     """
 
+    #: Run `decide_trades()` one second
+    #:
+    #: Only used in unit testing.
+    #: See `strategies/test_only_/enzymy_end_to_end.py`.
+    #:
+    cycle_1s = "1s"
+
     #: Run `decide_trades()` every minute
     cycle_1m = "1m"
 
     #: Run `decide_trades()` every 5 minutes
     cycle_5m = "5m"
 
     #: Run `decide_trades()` every 15 minutes
     cycle_15m = "15m"
 
+    #: Run `decide_trades()` every 30 minutes
+    cycle_30m = "30m"
+
     #: Run `decide_trades()` every hour
     cycle_1h = "1h"
 
+    #: Run `decide_trades()` every 2 hours
+    cycle_2h = "2h"
+
     #: Run `decide_trades()` every 4 hours
     cycle_4h = "4h"
 
+    #: Run `decide_trades()` every 6 hours
+    cycle_6h = "6h"
+
     #: Run `decide_trades()` for every 8 hours
     cycle_8h = "8h"
 
+    #: Run `decide_trades()` for every 10 hours
+    cycle_10h = "10h"
+
+    #: Run `decide_trades()` for every 12 hours
+    cycle_12h = "12h"
+
     #: Run `decide_trades()` for every 16 hours
     cycle_16h = "16h"
 
     #: Run `decide_trades()` for every 24h hours
     cycle_1d = "1d"
 
+    #: Run `decide_trades()` for every 4 days
+    cycle_4d = "4d"
+
+    #: Run `decide_trades()` for every week
+    cycle_7d = "7d"
+
     #: Don't really know or care about the trade cycle duration.
     #:
     #: Used when doing a simulated execution loop
     #: with `set_up_simulated_execution_loop`
     #: and where the time is ticked through manually by producing
     #: new blocks with EthereumTester chain.
     cycle_unknown = "unknown"
@@ -158,19 +186,27 @@
         return ts
 
     delta = tick_size.to_timedelta()
     return round_datetime_down(ts, delta, offset)
 
 
 _TICK_DURATIONS = {
+    CycleDuration.cycle_1s: datetime.timedelta(seconds=1),
     CycleDuration.cycle_1m: datetime.timedelta(minutes=1),
     CycleDuration.cycle_5m: datetime.timedelta(minutes=5),
     CycleDuration.cycle_15m: datetime.timedelta(minutes=15),
+    CycleDuration.cycle_30m: datetime.timedelta(minutes=30),
     CycleDuration.cycle_1h: datetime.timedelta(hours=1),
+    CycleDuration.cycle_2h: datetime.timedelta(hours=2),
     CycleDuration.cycle_4h: datetime.timedelta(hours=4),
+    CycleDuration.cycle_6h: datetime.timedelta(hours=6),
     CycleDuration.cycle_8h: datetime.timedelta(hours=8),
+    CycleDuration.cycle_10h: datetime.timedelta(hours=10),
+    CycleDuration.cycle_12h: datetime.timedelta(hours=12),
     CycleDuration.cycle_16h: datetime.timedelta(hours=16),
     CycleDuration.cycle_1d: datetime.timedelta(hours=24),
+    CycleDuration.cycle_4d: datetime.timedelta(days=4),
+    CycleDuration.cycle_7d: datetime.timedelta(days=7),
     CycleDuration.cycle_unknown: datetime.timedelta(days=0),
 }
 
 assert len(_TICK_DURATIONS) == len(CycleDuration)  # sanity check
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/description.py` & `trade_executor-0.3/tradeexecutor/strategy/description.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,7 +43,14 @@
     #: Blockchain id for this strategy.
     #:
     #: Necessary for single chain strategies to know
     #: on which chain we operate.
     #:
     chain_id: Optional[ChainId] = None
 
+    #: Source code of the strategy.
+    #:
+    #: Only applicable for strategies that were read as a strategy module,
+    #: not applicable to backtesting notebooks.
+    source_code: Optional[str] = None
+
+
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/execution_context.py` & `trade_executor-0.3/tradeexecutor/strategy/execution_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,25 +53,35 @@
 
     #: Prefilight checks
     #:
     #: In this execution mode, we are invoked from the command line
     #: to check that all of our files and connections are intact.
     preflight_check = "preflight_check"
 
+    #: One off diagnostic and scripts
+    #:
+    #: Used in the interactive :ref:`console.
+    #: and debugging scripts.
+    one_off = "one_off"
+
     def is_live_trading(self) -> bool:
         """Are we trading  real time?"""
         return self in (self.real_trading, self.paper_trading, self.unit_testing_trading, self.simulated_trading)
 
     def is_fresh_data_always_needed(self):
         """Should we purge caches for each trade cycle.
 
         This will force the redownload of data on each cycle.
         """
         return self in (self.real_trading, self.paper_trading, self.simulated_trading)
 
+    def is_unit_testing(self) -> bool:
+        """Are we executing unit tests."""
+        return self in (self.unit_testing_trading,)
+
 
 @dataclass
 class ExecutionContext:
     """Information about the strategy execution environment.
 
     This is passed to `create_trading_universe` and couple of other
     functions and they can determine and take action based
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/execution_model.py` & `trade_executor-0.3/tradeexecutor/strategy/execution_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,33 +5,63 @@
 - Backtesting via :py:mod:`tradeexecutor.backtest.backtest_execution`
 
 - Live execution against Uniswap v2 via :py:mod:`tradeexecutor.ethereum.uniswap_v2_execution`
 """
 import abc
 import datetime
 import enum
-from typing import List
+from typing import List, Dict, Tuple, TypedDict, Optional
+from web3 import Web3
+from hexbytes import HexBytes
 
+from eth_defi.hotwallet import HotWallet
+from tradeexecutor.ethereum.tx import TransactionBuilder
 from tradeexecutor.state.state import State
 from tradeexecutor.state.trade import TradeExecution
 from tradeexecutor.strategy.routing import RoutingModel, RoutingState
+from tradeexecutor.state.blockhain_transaction import BlockchainTransaction
 
 
 class AutoClosingOrderUnsupported(Exception):
     """Raised when trade execution does not support stop loss/take profit.
 
     Stop loss handling requires special support from the trade execution engine.
     See :py:meth:`ExecutionModel.is_stop_loss_supported` for more details.
     """
 
 
+class RoutingStateDetails(TypedDict):
+    """Detailts a trade router needs from the execeution mode to set its internal state.
+
+    The content may differ if we are doing backtesting (no live execution objects needed),
+    live trading or running some very legacy code.
+
+    TODO: API unfinished. Needs to be cleaned up.
+
+    TODO: Mark everything `NotRequired` if Python 3.11 migrated
+    """
+
+    tx_builder: TransactionBuilder
+
+    #: TODO: Legacy - moved to Txbuilder
+    web3: Web3
+
+    #: TODO: Legacy - moved to Txbuilder
+    wallet: HotWallet
+
+    #: TODO: Legacy - moved to Txbuilder
+    hot_wallet: HotWallet
+
+
 class ExecutionModel(abc.ABC):
     """Define how trades are executed.
 
     See also :py:class:`tradeexecutor.strategy.mode.ExecutionMode`.
+    
+    Used directly by BacktestExecutionModel, and indirectly (through EthereumExecutionModel) by UniswapV2ExecutionModel and UniswapV3ExecutionModel
     """
 
     @abc.abstractmethod
     def preflight_check(self):
         """Check that we can start the trade executor
 
         :raise: AssertionError if something is a miss
@@ -43,18 +73,16 @@
 
         Read any on-chain, etc., data to get synced.
 
         - Read EVM nonce for the hot wallet from the chain
         """
 
     @abc.abstractmethod
-    def get_routing_state_details(self) -> object:
+    def get_routing_state_details(self) -> RoutingStateDetails:
         """Get needed details to establish a routing state.
-
-        TODO: API Unfinished
         """
 
     @abc.abstractmethod
     def is_stop_loss_supported(self) -> bool:
         """Do we support stop-loss/take profit functionality with this execution model?
 
         - For backtesting we need to have data stream for candles used to calculate stop loss
@@ -98,32 +126,45 @@
             Max slippage % allowed on trades before trade execution fails.
 
         :param check_balances:
             Check that on-chain accounts have enough balance before creating transaction objects.
             Useful during unit tests to spot issues in trade routing.
         """
 
+    @abc.abstractmethod
+    def repair_unconfirmed_trades(self, state: State) -> List[TradeExecution]:
+        """Repair unconfirmed trades.
+
+        Repair trades that failed to properly broadcast or confirm due to
+        blockchain node issues.
+
+        :return:
+            List of fixed trades
+        """
+
 
-class TradeExecutionType(enum.Enum):
+class AssetManagementMode(enum.Enum):
     """Default execution options.
 
     What kind of trade instruction execution model the strategy does.
 
     Give options for command line parameters and such.
 
     TODO: Clean up unused options.
     """
 
     #: Does not make any trades, just captures and logs them
     dummy = "dummy"
 
     #: Server-side normal Ethereum private eky account
-    uniswap_v2_hot_wallet = "uniswap_v2_hot_wallet"
+    hot_wallet = "hot_wallet"
 
     #: Trading using Enzyme Protocol pool, single oracle mode
-    single_oracle_pooled = "single_oracle_pooled"
-
-    #: Trading using oracle network, oracles form a consensus using a judge smart contract
-    multi_oracle_judged = "multi_oracle_judged"
+    enzyme = "enzyme"
 
     #: Simulate execution using backtest data
-    backtest = "backtest"
+    #:
+    #: - Does not make any real trades
+    #:
+    #: - Does not connect to any network or blockchain
+    #:
+    backtest = "backtest"
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/factory.py` & `trade_executor-0.3/tradeexecutor/strategy/factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from typing import Protocol, Optional
 
 from contextlib import AbstractContextManager
 
 from tradingstrategy.client import Client
 
-from tradeexecutor.state.sync import SyncMethod
+from tradeexecutor.strategy.sync_model import SyncMethodV0, SyncModel
 from tradeexecutor.strategy.approval import ApprovalModel
 from tradeexecutor.strategy.description import StrategyExecutionDescription
 from tradeexecutor.strategy.execution_model import ExecutionModel
 from tradeexecutor.strategy.pricing_model import PricingModelFactory
 from tradeexecutor.strategy.routing import RoutingModel
 from tradeexecutor.strategy.valuation import ValuationModelFactory
 
@@ -22,15 +22,15 @@
 class StrategyFactory(Protocol):
     """A callable that creates a new strategy when loaded from an external script."""
 
     # Only accept kwargs as per https://www.python.org/dev/peps/pep-3102/
     def __call__(
         *ignore,
         execution_model: ExecutionModel,
-        sync_method: SyncMethod,
+        sync_model: SyncModel,
         pricing_model_factory: PricingModelFactory,
         valuation_model_factory: ValuationModelFactory,
         client: Optional[Client],
         timed_task_context_manager: AbstractContextManager,
         approval_model: ApprovalModel,
         routing_model: Optional[RoutingModel] = None,
         **kwargs) -> StrategyExecutionDescription:
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/output.py` & `trade_executor-0.3/tradeexecutor/strategy/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     symbol = up_symbol if position.get_total_profit_percent() >= 0 else down_symbol
     if position.pair.info_url:
         link = position.pair.info_url
     else:
         link = ""
 
     lines =[
-        f"{symbol} #{position.position_id} {position.pair.get_human_description()} size:${position.get_value():,.2f}, profit:{position.get_total_profit_usd():.2f}% ({position.get_total_profit_usd():,.4f} USD)"
+        f"{symbol} #{position.position_id} {position.pair.get_human_description()} size:${position.get_value():,.2f}, profit:{position.get_total_profit_percent():.2f}% ({position.get_total_profit_usd():,.4f} USD)"
     ]
 
     if position.has_executed_trades():
         price_diff = position.get_current_price() - position.get_opening_price()
         lines.append(f"   current price:${position.get_current_price():,.8f}, open price:${position.get_opening_price():,.8f}, diff:{price_diff:,.8f} USD")
         lines.append(f"   last tx:${position.get_last_tx_hash()}")
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/pandas_trader/rebalance.py` & `trade_executor-0.3/tradeexecutor/strategy/pandas_trader/rebalance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,25 @@
 """Alpha model rebalancing.
 
 Based on the new alpha model weights, rebalance the existing portfolio.
 """
 import logging
+from _decimal import Decimal
 from typing import List, Dict
 
 from tradeexecutor.state.portfolio import Portfolio
 from tradeexecutor.state.trade import TradeExecution
+from tradeexecutor.state.types import USDollarAmount
+from tradeexecutor.strategy.alpha_model import AlphaModel
 from tradeexecutor.strategy.pandas_trader.position_manager import PositionManager
-
+from tradeexecutor.strategy.weighting import check_normalised_weights
 
 logger = logging.getLogger(__name__)
 
 
-class BadWeightsException(Exception):
-    """Sum of weights not 1."""
-
-
-
-def check_normalised_weights(weights: Dict[int, float], epsilon=0.0001):
-    """Check that the sum of weights is good."""
-
-    total = sum(weights.values())
-    if abs(total - 1) > epsilon:
-        raise BadWeightsException(f"Total sum of normalised portfolio weights was not 1."
-                                  f"Sum: {total}")
-
-
-def clip_to_normalised(weights: Dict[int, float]) -> Dict[int, float]:
-    """If the sum of the weights are not exactly 1, then decrease the largest member to make the same sum 1 precise.
-
-    """
-    total = sum(weights.values())
-    diff = total - 1
-    largest = max(weights.items(), key=lambda x: x[1])
-
-    clipped = largest[1] - diff
-
-    fixed = weights.copy()
-    fixed[largest[0]] = clipped
-
-    total = sum(fixed.values())
-    assert total == 1
-    return fixed
-
-
 def get_existing_portfolio_weights(portfolio: Portfolio) -> Dict[int, float]:
     """Calculate the existing portfolio weights.
 
     Cash is not included in the weighting.
     """
 
     total = portfolio.get_open_position_equity()
@@ -81,22 +52,26 @@
         if id not in diffs:
             # Sell all
             diffs[id] = -old_weight
 
     return diffs
 
 
-def rebalance_portfolio(
+def rebalance_portfolio_old(
         position_manager: PositionManager,
         new_weights: Dict[int, float],
-        portfolio_total_value: float,
-        min_trade_threshold=10.0,
+        portfolio_total_value: USDollarAmount,
+        min_trade_threshold: USDollarAmount = 10.0,
 ) -> List[TradeExecution]:
     """Rebalance a portfolio based on alpha model weights.
 
+    .. warning ::
+
+        This is old deprecated method. Do not use anymore.
+
     This will generate
 
     - Sells for the existing assets
 
     - Buys for new assetes or assets where we want to increase our position
 
     :param portfolio:
@@ -133,25 +108,34 @@
     trades: List[TradeExecution] = []
 
     for pair_id, value in dollar_values.items():
         pair = position_manager.get_trading_pair(pair_id)
         weight = new_weights.get(pair.internal_id, 0)
         dollar_diff = value
 
-        logger.info("Rebalancing %s, old weight: %f, new weight: %f, diff: %f USD",
+        if dollar_diff < 0:
+            # Calculate token amount
+            quantity_diff = Decimal(position_manager.estimate_asset_quantity(pair, dollar_diff))
+        else:
+            quantity_diff = None
+
+        logger.info("Rebalancing %s, old weight: %f, new weight: %f, diff: %f USD %f %s",
                     pair,
                     existing_weights.get(pair_id, 0),
                     weight,
-                    dollar_diff)
+                    dollar_diff,
+                    quantity_diff,
+                    pair.base.token_symbol,
+                    )
 
         if abs(dollar_diff) < min_trade_threshold:
             logger.info("Not doing anything, value %f below trade threshold %f", value, min_trade_threshold)
         else:
-            position_rebalance_trades = position_manager.adjust_position(pair, dollar_diff, weight)
-            assert len(position_rebalance_trades) == 1, "Assuming always on trade for rebalacne"
+            position_rebalance_trades = position_manager.adjust_position(pair, dollar_diff, quantity_diff, weight)
+            assert len(position_rebalance_trades) == 1, "Assuming always on trade for rebalance"
             logger.info("Adjusting holdings for %s: %s", pair, position_rebalance_trades[0])
             trades += position_rebalance_trades
 
     trades.sort(key=lambda t: t.get_execution_sort_position())
 
     # Return all rebalance trades
-    return trades
+    return trades
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/pandas_trader/trade_decision.py` & `trade_executor-0.3/tradeexecutor/strategy/pandas_trader/trade_decision.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/strategy/pricing_model.py` & `trade_executor-0.3/tradeexecutor/strategy/dummy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,99 @@
-"""Asset pricing model."""
-
-import abc
+"""A testing executoin model without actual execution."""
 import datetime
-from decimal import Decimal, ROUND_DOWN
-from typing import Callable, Optional
+from typing import List
+
+from web3 import Web3
 
-from tradeexecutor.state.identifier import TradingPairIdentifier
-from tradeexecutor.state.types import USDollarAmount
+from tradeexecutor.state.state import State
+from tradeexecutor.state.trade import TradeExecution
 from tradeexecutor.strategy.execution_model import ExecutionModel
-from tradeexecutor.strategy.routing import RoutingModel
-from tradeexecutor.strategy.universe_model import StrategyExecutionUniverse
+from tradeexecutor.strategy.routing import RoutingModel, RoutingState
 
 
-class PricingModel(abc.ABC):
-    """Get a price for the asset.
+class DummyExecutionModel(ExecutionModel):
+    """Trade executor that does not connect to anything.
 
-    Needed for various aspects
+    Used in testing.
+    """
 
-    - Revaluate portfolio positiosn
+    def __init__(self, web3: Web3):
+        self.web3 = web3
 
-    - Estimate buy/sell price for the live trading so we can calculate slippage
+    def preflight_check(self):
+        """Check that we can start the trade executor
 
-    - Get the historical price in backtesting
+        :raise: AssertionError if something is a miss
+        """
 
-    Timestamp is passed to the pricing method. However we expect it only be honoured during
-    the backtesting - live execution may always use the latest price.
+    def initialize(self):
+        """Set up the execution model ready to make trades.
 
-    .. note ::
+        Read any on-chain, etc., data to get synced.
 
-        For example, in futures markets there could be different fees
-        on buy/sell transctions.
+        - Read EVM nonce for the hot wallet from the chain
+        """
 
-    """
+    def get_routing_state_details(self) -> object:
+        """Get needed details to establish a routing state.
 
-    @abc.abstractmethod
-    def get_sell_price(self,
-                       ts: datetime.datetime,
-                       pair: TradingPairIdentifier,
-                       quantity: Optional[Decimal]) -> USDollarAmount:
-        """Get the sell price for an asset.
+        """
+        return {
+            "web3": self.web3,
+        }
 
-        :param ts:
-            When to get the price.
-            Used in backtesting.
-            Live models may ignore.
+    def is_stop_loss_supported(self) -> bool:
+        """Do we support stop-loss/take profit functionality with this execution model?
 
-        :param pair:
-            Trading pair we are intereted in
+        - For backtesting we need to have data stream for candles used to calculate stop loss
 
-        :param quantity:
-            If the sel quantity is known, get the price with price impact.
+        - For production execution, we need to have special oracle data streams
+          for checking real-time stop loss
         """
 
-    @abc.abstractmethod
-    def get_buy_price(self,
-                      ts: datetime.datetime,
-                      pair: TradingPairIdentifier,
-                      reserve: Optional[Decimal]
-                      ) -> USDollarAmount:
-        """Get the sell price for an asset.
+    def execute_trades(self,
+                       ts: datetime.datetime,
+                       state: State,
+                       trades: List[TradeExecution],
+                       routing_model: RoutingModel,
+                       routing_state: RoutingState,
+                       max_slippage=0.005,
+                       check_balances=False,
+                       ):
+        """Execute the trades determined by the algo on a designed Uniswap v2 instance.
 
         :param ts:
-            When to get the price.
-            Used in backtesting.
-            Live models may ignore.
-
-        :param pair:
-            Trading pair we are intereted in
-
-        :param reserve:
-            If the buy token quantity quantity is known,
-            get the buy price with price impact.
-        """
+            Timestamp of the trade cycle.
+
+        :param universe:
+            Current trading universe for this cycle.
+
+        :param state:
+            State of the trade executor.
+
+        :param trades:
+            List of trades decided by the strategy.
+            Will be executed and modified in place.
 
-    @abc.abstractmethod
-    def quantize_base_quantity(self, pair: TradingPairIdentifier, quantity: Decimal, rounding=ROUND_DOWN) -> Decimal:
-        """Convert any base token quantity to the native token units by its ERC-20 decimals."""
+        :param routing_model:
+            Routing model how to execute the trades
+
+        :param routing_state:
+            State of already made on-chain transactions and such on this cycle
+
+        :param max_slippage:
+            Max slippage % allowed on trades before trade execution fails.
+
+        :param check_balances:
+            Check that on-chain accounts have enough balance before creating transaction objects.
+            Useful during unit tests to spot issues in trade routing.
+        """
 
+    def repair_unconfirmed_trades(self, state: State) -> List[TradeExecution]:
+        """Repair unconfirmed trades.
 
-#: This factory creates a new pricing model for each trade cycle.
-#: Pricing model depends on the trading universe that may change for each strategy tick,
-#: as new trading pairs appear.
-#: Thus, we need to reconstruct pricing model as the start of the each tick.
-PricingModelFactory = Callable[[ExecutionModel, StrategyExecutionUniverse, RoutingModel], PricingModel]
+        Repair trades that failed to properly broadcast or confirm due to
+        blockchain node issues.
 
+        :return:
+            List of fixed trades
+        """
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/qstrader/alpha_model.py` & `trade_executor-0.3/tradeexecutor/strategy/qstrader/alpha_model.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/strategy/qstrader/order_sizer.py` & `trade_executor-0.3/tradeexecutor/strategy/qstrader/order_sizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,16 @@
             after_cost_dollar_weight = pre_cost_dollar_weight - est_costs
 
             asset_quantity = 0
 
             if weight > 0:
 
                 trading_pair = self.pricing_model.get_pair_for_id(asset)
-                asset_price = self.pricing_model.get_buy_price(dt, trading_pair, Decimal(after_cost_dollar_weight))
+                price_structure = self.pricing_model.get_buy_price(dt, trading_pair, Decimal(after_cost_dollar_weight))
+                asset_price = price_structure.price
 
                 if asset_price is not None:
 
                     if after_cost_dollar_weight > 0:
                         if np.isnan(asset_price):
                             raise ValueError(
                                 'Asset price for "%s" at timestamp "%s" is Not-a-Number (NaN). '
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/qstrader/portfolio_construction_model.py` & `trade_executor-0.3/tradeexecutor/strategy/qstrader/portfolio_construction_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                 # to disappear as well.
                 price = target_prices.get(asset)
                 if price is None:
                     logger.warning(f"Price missing for asset {asset} - prices are {target_prices}")
                     continue
 
                 if isinstance(dt, pd.Timestamp):
-                    dt = dt.to_pydatetime()
+                    dt = dt.to_pydatetime().replace(tzinfo=None)
 
                 position, trade, created = self.state.create_trade(
                     dt,
                     executor_pair,
                     quantity,
                     None,
                     price,
@@ -278,15 +278,16 @@
         # Obtain current Broker account portfolio
         current_portfolio = self._obtain_current_portfolio()
 
         # Get prices for existing assets so we have some idea how much they sell for
         for asset_id, asset_data in current_portfolio.items():
             pair = self.pricing_model.get_pair_for_id(asset_id)
             if pair:
-                target_prices[asset_id] = self.pricing_model.get_buy_price(dt, pair, None)
+                price_structure = self.pricing_model.get_buy_price(dt, pair, None)
+                target_prices[asset_id] = price_structure.price
 
         # Expose internal states to unit tests
         debug_details["positions_at_start_of_construction"] = current_portfolio.copy()  # current_portfolio is mutated later
 
         # Create rebalance trade Orders
         rebalance_trades = self._generate_rebalance_trades(
             dt, target_portfolio, current_portfolio, target_prices, debug_details
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/qstrader/runner.py` & `trade_executor-0.3/tradeexecutor/strategy/qstrader/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,75 +43,75 @@
         self.alpha_model = alpha_model
         self.max_data_age = max_data_age
         # TODO: Make starter configuration
         self.cash_buffer = cash_buffer
 
         assert kwargs.get("routing_model"), "Routing model missing"
 
-    def report_strategy_thinking(self, clock: datetime.datetime, universe: TradingStrategyUniverse, state: State, trades: List[TradeExecution], debug_details: dict):
-        """Report alpha model status."""
-        buf = StringIO()
-        universe = universe.universe
-
-        # TODO: move report_strategy_thinking() to a separate reporter class
-
-        data_start, data_end = universe.candles.get_timestamp_range()
-        liquidity_start, liquidity_end = universe.liquidity.get_timestamp_range()
-
-        print("Strategy thinking", file=buf)
-        print("", file=buf)
-        print("Dataset status:", file=buf)
-        print("", file=buf)
-        print(f"   Cash buffer: {self.cash_buffer * 100:.2f}%", file=buf)
-        print(f"   Candle dataset: {data_start} - {data_end}", file=buf)
-        print(f"   Liquidity dataset: {liquidity_start} - {liquidity_end}", file=buf)
-        print("", file=buf)
-
-        # Alpha model weights does not contain zero weight entries
-        alpha_model_weights = debug_details["alpha_model_weights"]
-
-        # Normalised weights do contain zero weight entries
-        normalised_weights = debug_details.get("normalised_weights", {})
-
-        if alpha_model_weights:
-            print("Alpha model weights:", file=buf)
-            print("", file=buf)
-
-            for pair_id, weight in alpha_model_weights.items():
-                norm_weight = normalised_weights.get(pair_id, weight)
-                pair = universe.pairs.get_pair_by_id(pair_id)
-                tp = translate_trading_pair(pair)
-                link = tp.info_url or ""
-                if "extra_debug_data" in debug_details:
-                    momentum = debug_details["extra_debug_data"][pair_id]["momentum"]
-                    print(f"    {tp.get_human_description()} weight:{norm_weight*100:.2f}%, momentum:{momentum*100:.2f}%", file=buf)
-                    if link:
-                        print(f"    link: {link}", file=buf)
-                    print("", file=buf)
-        else:
-            print("Error: Could not calculate any momentum! Data missing?", file=buf)
-
-        good_candle_count = debug_details.get("good_candle_count")
-        problem_candle_count = debug_details.get("problem_candle_count")
-        low_liquidity_count = debug_details.get("low_liquidity_count")
-        bad_momentum_count = debug_details.get("bad_momentum_count")
-        funny_price_count = debug_details.get("funny_price_count")
-        candle_range_start = debug_details.get("candle_range_start")
-        candle_range_end = debug_details.get("candle_range_end")
-        print("", file=buf)
-        print("Alpha model data quality:", file=buf)
-        print("", file=buf)
-        print(f"   Evaluated momentum range: {candle_range_start} - {candle_range_end}", file=buf)
-        print(f"   Pairs with good candles data: {good_candle_count}", file=buf)
-        print(f"   Pairs with bad price value: {funny_price_count}", file=buf)
-        print(f"   Pairs with negative momentum result: {bad_momentum_count}", file=buf)
-        print(f"   Pairs with problems in candles data: {problem_candle_count}", file=buf)
-        print(f"   Pairs with low liquidity: {low_liquidity_count}", file=buf)
-
-        logger.trade(buf.getvalue())
+    # def report_strategy_thinking(self, clock: datetime.datetime, universe: TradingStrategyUniverse, state: State, trades: List[TradeExecution], debug_details: dict):
+    #     """Report alpha model status."""
+    #     buf = StringIO()
+    #     universe = universe.universe
+    #
+    #     # TODO: move report_strategy_thinking() to a separate reporter class
+    #
+    #     data_start, data_end = universe.candles.get_timestamp_range()
+    #     liquidity_start, liquidity_end = universe.liquidity.get_timestamp_range()
+    #
+    #     print("Strategy thinking", file=buf)
+    #     print("", file=buf)
+    #     print("Dataset status:", file=buf)
+    #     print("", file=buf)
+    #     print(f"   Cash buffer: {self.cash_buffer * 100:.2f}%", file=buf)
+    #     print(f"   Candle dataset: {data_start} - {data_end}", file=buf)
+    #     print(f"   Liquidity dataset: {liquidity_start} - {liquidity_end}", file=buf)
+    #     print("", file=buf)
+    #
+    #     # Alpha model weights does not contain zero weight entries
+    #     alpha_model_weights = debug_details["alpha_model_weights"]
+    #
+    #     # Normalised weights do contain zero weight entries
+    #     normalised_weights = debug_details.get("normalised_weights", {})
+    #
+    #     if alpha_model_weights:
+    #         print("Alpha model weights:", file=buf)
+    #         print("", file=buf)
+    #
+    #         for pair_id, weight in alpha_model_weights.items():
+    #             norm_weight = normalised_weights.get(pair_id, weight)
+    #             pair = universe.pairs.get_pair_by_id(pair_id)
+    #             tp = translate_trading_pair(pair)
+    #             link = tp.info_url or ""
+    #             if "extra_debug_data" in debug_details:
+    #                 momentum = debug_details["extra_debug_data"][pair_id]["momentum"]
+    #                 print(f"    {tp.get_human_description()} weight:{norm_weight*100:.2f}%, momentum:{momentum*100:.2f}%", file=buf)
+    #                 if link:
+    #                     print(f"    link: {link}", file=buf)
+    #                 print("", file=buf)
+    #     else:
+    #         print("Error: Could not calculate any momentum! Data missing?", file=buf)
+    #
+    #     good_candle_count = debug_details.get("good_candle_count")
+    #     problem_candle_count = debug_details.get("problem_candle_count")
+    #     low_liquidity_count = debug_details.get("low_liquidity_count")
+    #     bad_momentum_count = debug_details.get("bad_momentum_count")
+    #     funny_price_count = debug_details.get("funny_price_count")
+    #     candle_range_start = debug_details.get("candle_range_start")
+    #     candle_range_end = debug_details.get("candle_range_end")
+    #     print("", file=buf)
+    #     print("Alpha model data quality:", file=buf)
+    #     print("", file=buf)
+    #     print(f"   Evaluated momentum range: {candle_range_start} - {candle_range_end}", file=buf)
+    #     print(f"   Pairs with good candles data: {good_candle_count}", file=buf)
+    #     print(f"   Pairs with bad price value: {funny_price_count}", file=buf)
+    #     print(f"   Pairs with negative momentum result: {bad_momentum_count}", file=buf)
+    #     print(f"   Pairs with problems in candles data: {problem_candle_count}", file=buf)
+    #     print(f"   Pairs with low liquidity: {low_liquidity_count}", file=buf)
+    #
+    #     logger.trade(buf.getvalue())
 
     def on_data_signal(self):
         pass
 
     def on_clock(self,
                  clock: datetime.datetime,
                  executor_universe: TradingStrategyUniverse,
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/runner.py` & `trade_executor-0.3/tradeexecutor/strategy/runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 import logging
 from io import StringIO
 
 from typing import List, Optional, Tuple
 
 from tradeexecutor.strategy.approval import ApprovalModel
 from tradeexecutor.strategy.cycle import CycleDuration
+from tradeexecutor.strategy.execution_context import ExecutionContext
 from tradeexecutor.strategy.execution_model import ExecutionModel
-from tradeexecutor.state.sync import SyncMethod
+from tradeexecutor.strategy.sync_model import SyncMethodV0, SyncModel
+from tradeexecutor.strategy.run_state import RunState
 from tradeexecutor.strategy.output import output_positions, DISCORD_BREAK_CHAR, output_trades
 from tradeexecutor.strategy.pandas_trader.position_manager import PositionManager
 from tradeexecutor.strategy.pricing_model import PricingModelFactory, PricingModel
 from tradeexecutor.strategy.routing import RoutingModel, RoutingState
-from tradeexecutor.strategy.stoploss import check_position_triggers
+from tradeexecutor.strategy.stop_loss import check_position_triggers
 from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse
 from tradeexecutor.strategy.universe_model import StrategyExecutionUniverse
 
 from tradeexecutor.state.state import State
 from tradeexecutor.state.position import TradingPosition
 from tradeexecutor.state.trade import TradeExecution
 from tradeexecutor.state.reserve import ReservePosition
@@ -51,24 +53,35 @@
     """
 
     def __init__(self,
                  timed_task_context_manager: AbstractContextManager,
                  execution_model: ExecutionModel,
                  approval_model: ApprovalModel,
                  valuation_model_factory: ValuationModelFactory,
-                 sync_method: SyncMethod,
+                 sync_model: Optional[SyncModel],
                  pricing_model_factory: PricingModelFactory,
-                 routing_model: Optional[RoutingModel]=None):
+                 execution_context: ExecutionContext,
+                 routing_model: Optional[RoutingModel] = None,
+                 run_state: Optional[RunState] = None,
+                 ):
+
+        assert isinstance(execution_context, ExecutionContext)
+
+        if sync_model is not None:
+            assert isinstance(sync_model, SyncModel)
+
         self.timed_task_context_manager = timed_task_context_manager
         self.execution_model = execution_model
         self.approval_model = approval_model
         self.valuation_model_factory = valuation_model_factory
-        self.sync_method = sync_method
+        self.sync_model = sync_model
         self.pricing_model_factory = pricing_model_factory
         self.routing_model = routing_model
+        self.run_state = run_state
+        self.execution_context = execution_context
 
     @abc.abstractmethod
     def pretick_check(self, ts: datetime.datetime, universe: StrategyExecutionUniverse):
         """Called when the trade executor instance is started.
 
         :param client: Trading Strategy client to check server versions etc.
 
@@ -76,31 +89,50 @@
 
         :param ts: Real-time clock signal or past clock timestamp in the case of unit testing
 
         :raise PreflightCheckFailed: In the case we cannot go live
         """
         pass
 
-    def sync_portfolio(self, ts: datetime.datetime, universe: StrategyExecutionUniverse, state: State, debug_details: dict):
+    def is_progress_report_needed(self) -> bool:
+        """Do we log the strategy steps to logger?
+
+        - Disabled for backtesting to speed up
+
+        - Can be enabled by hacking this function if backtesting needs debugging
+        """
+        return self.execution_context.mode.is_live_trading() or self.execution_context.mode.is_unit_testing()
+
+    def sync_portfolio(self, strategy_cycle_ts: datetime.datetime, universe: StrategyExecutionUniverse, state: State, debug_details: dict):
         """Adjust portfolio balances based on the external events.
 
         External events include
+
         - Deposits
+
         - Withdrawals
+
         - Interest accrued
+
         - Token rebases
         """
         assert isinstance(universe, StrategyExecutionUniverse), f"Universe was {universe}"
-        reserve_assets = universe.reserve_assets
+        reserve_assets = list(universe.reserve_assets)
         assert len(reserve_assets) > 0, "No reserve assets available"
         assert len(reserve_assets) == 1, f"We only support strategies with a single reserve asset, got {self.reserve_assets}"
         token = reserve_assets[0]
         assert token.decimals and token.decimals > 0, f"Reserve asset lacked decimals"
-        reserve_update_events = self.sync_method(state.portfolio, ts, reserve_assets)
+        reserve_update_events = self.sync_model.sync_treasury(
+            strategy_cycle_ts,
+            state,
+            supported_reserves=reserve_assets,
+        )
         assert type(reserve_update_events) == list
+
+        # Update the debug data for tests with our events
         debug_details["reserve_update_events"] = reserve_update_events
         debug_details["total_equity_at_start"] = state.portfolio.get_total_equity()
         debug_details["total_cash_at_start"] = state.portfolio.get_current_cash()
 
     def revalue_portfolio(self, ts: datetime.datetime, state: State, valuation_method: ValuationModel):
         """Revalue portfolio based on the data."""
         state.revalue_positions(ts, valuation_method)
@@ -137,78 +169,120 @@
         tick = debug_details.get("cycle", 1)
         print(f"Portfolio status (before rebalance), tick #{tick}", file=buf)
         print("", file=buf)
         print(f"Total equity: ${portfolio.get_total_equity():,.2f}, in cash: ${portfolio.get_current_cash():,.2f}", file=buf)
         print(f"Life-time positions: {portfolio.next_position_id - 1}, trades: {portfolio.next_trade_id - 1}", file=buf)
         print(DISCORD_BREAK_CHAR, file=buf)
 
-        print(f"Currently open positions:", file=buf)
-        print("", file=buf)
-        output_positions(portfolio.open_positions.values(), buf)
-
-        print(DISCORD_BREAK_CHAR, file=buf)
-
-        print(f"Frozen positions (${portfolio.get_frozen_position_equity():,.2f}):", file=buf)
-        print("", file=buf)
-        output_positions(portfolio.frozen_positions.values(), buf)
-
-        print(DISCORD_BREAK_CHAR, file=buf)
+        if len(portfolio.open_positions) > 0:
+            print(f"Currently open positions:", file=buf)
+            print("", file=buf)
+            output_positions(portfolio.open_positions.values(), buf)
+
+            print(DISCORD_BREAK_CHAR, file=buf)
+        else:
+            logger.info("No open positions")
+
+        if portfolio.get_frozen_position_equity() > 0:
+            print(f"Frozen positions (${portfolio.get_frozen_position_equity():,.2f}):", file=buf)
+            print("", file=buf)
+            output_positions(portfolio.frozen_positions.values(), buf)
+
+            print(DISCORD_BREAK_CHAR, file=buf)
+        else:
+            logger.info("No frozen positions")
 
         print("Reserves:", file=buf)
         print("", file=buf)
         reserve: ReservePosition
         for reserve in state.portfolio.reserves.values():
             print(f"    {reserve.quantity:,.2f} {reserve.asset.token_symbol}", file=buf)
 
         logger.trade(buf.getvalue())
 
     def report_before_execution(self, clock: datetime.datetime, universe: StrategyExecutionUniverse, state: State, trades: List[TradeExecution], debug_details: dict):
         buf = StringIO()
-        print("New trades to be executed", file=buf)
-        print("", file=buf)
-        position: TradingPosition
-        portfolio = state.portfolio
-        output_trades(trades, portfolio, buf)
+
+        if len(trades) > 0:
+            print("New trades to be executed", file=buf)
+            print("", file=buf)
+            position: TradingPosition
+            portfolio = state.portfolio
+            output_trades(trades, portfolio, buf)
+        else:
+            print("No new trades", file=buf)
         logger.trade(buf.getvalue())
 
     def report_after_execution(self, clock: datetime.datetime, universe: StrategyExecutionUniverse, state: State, debug_details: dict):
         buf = StringIO()
         portfolio = state.portfolio
         
         print("Portfolio status (after rebalance)", file=buf)
         print("", file=buf)
         print(f"Total equity: ${portfolio.get_total_equity():,.2f}, Cash: ${portfolio.get_current_cash():,.2f}", file=buf)
 
         print(DISCORD_BREAK_CHAR, file=buf)
 
-        print(f"Opened/open positions:", file=buf)
-        print("", file=buf)
-        output_positions(portfolio.open_positions.values(), buf)
+        if len(portfolio.open_positions) > 0:
+            print(f"Opened/open positions:", file=buf)
+            print("", file=buf)
+            output_positions(portfolio.open_positions.values(), buf)
+
+            print(DISCORD_BREAK_CHAR, file=buf)
+        else:
+            logger.info("No positions opened")
 
-        print(DISCORD_BREAK_CHAR, file=buf)
 
         closed_positions = list(portfolio.get_positions_closed_at(clock))
-        print(f"Closed positions:", file=buf)
-        output_positions(closed_positions, buf)
-
-        print(DISCORD_BREAK_CHAR, file=buf)
+        if len(closed_positions) > 0:
+            print(f"Closed positions:", file=buf)
+            output_positions(closed_positions, buf)
+
+            print(DISCORD_BREAK_CHAR, file=buf)
+        else:
+            logger.info("No closed positions")
 
         print("Reserves:", file=buf)
         print("", file=buf)
         reserve: ReservePosition
         for reserve in state.portfolio.reserves.values():
             print(f"    {reserve.quantity:,.2f} {reserve.asset.token_symbol}", file=buf)
         logger.trade(buf.getvalue())
 
-    def report_strategy_thinking(self, clock: datetime.datetime, universe: StrategyExecutionUniverse, state: State, trades: List[TradeExecution], debug_details: dict):
-        """Strategy runner subclass can fill in.
+    def report_strategy_thinking(self,
+                                 strategy_cycle_timestamp: datetime.datetime,
+                                 cycle: int,
+                                 universe: TradingStrategyUniverse,
+                                 state: State,
+                                 trades: List[TradeExecution],
+                                 debug_details: dict):
+        """Strategy admin helpers to understand a live running strategy.
+
+        - Post latest variables
+
+        - Draw the single pair strategy visualisation.
 
-        By default, no-op. Override in the subclass.
+        :param strategy_cycle_timestamp:
+            real time lock
+
+        :param cycle:
+            Cycle number
+
+        :param universe:
+            Currnet trading universe
+
+        :param trades:
+            Trades executed on this cycle
+
+        :param state:
+            Current execution state
+
+        :param debug_details:
+            Dict of random debug stuff
         """
-        pass
 
     def setup_routing(self, universe: StrategyExecutionUniverse) -> Tuple[RoutingState, PricingModel, ValuationModel]:
         """Setups routing state for this cycle.
 
         :param universe:
             The currently tradeable universe
 
@@ -218,37 +292,49 @@
 
         assert self.routing_model, "Routing model not set"
 
         # Get web3 connection, hot wallet
         routing_state_details = self.execution_model.get_routing_state_details()
 
         # Initialise the current routing state with execution details
+        logger.info("Setting up routing. Routing model is %s, details are %s, universe is %s",
+                    self.routing_model,
+                    routing_state_details,
+                    universe,
+                    )
         routing_state = self.routing_model.create_routing_state(universe, routing_state_details)
 
         # Create a pricing model for assets
         pricing_model = self.pricing_model_factory(self.execution_model, universe, self.routing_model)
 
         assert pricing_model, "pricing_model_factory did not return a value"
 
         # Create a valuation model for positions
         valuation_model = self.valuation_model_factory(pricing_model)
 
+        logger.debug("setup_routing(): routing_state: %s, pricing_model: %s, valuation_model: %s",
+                     routing_state,
+                     pricing_model,
+                     valuation_model
+                     )
+
         return routing_state, pricing_model, valuation_model
 
     def tick(self,
-             clock: datetime.datetime,
+             strategy_cycle_timestamp: datetime.datetime,
              universe: StrategyExecutionUniverse,
              state: State,
              debug_details: dict,
-             cycle_duration: Optional[CycleDuration]=None,
-        ) -> dict:
+             cycle_duration: Optional[CycleDuration] = None,
+             cycle: Optional[int] = None,
+             ) -> dict:
         """Execute the core functions of a strategy.
 
-        :param clock:
-            Current timestamp of the execution cycle
+        :param strategy_cycle_timestamp:
+            Current timestamp of the execution cycle.
 
         :param universe:
             Loaded trading data
 
         :param state:
             The current state of the strategy (open position, past trades, visualisation)
 
@@ -256,73 +342,107 @@
             Internal bunch of data used in unit testing
 
         :param cycle_duration:
             The currenct cycle duration (time between ticks).
             This may be specific in a strategy module, but also overridden for testing.
             This is used only for logging purposes.
 
+        :param cycle:
+            Strategy cycle number
+
+        :param execution_context:
+            Live or backtesting
+
         :return: Debug details dictionary where different subsystems can write their diagnostics information what is happening during the dict.
             Mostly useful for integration testing.
         """
 
         assert isinstance(universe, StrategyExecutionUniverse)
 
+        assert isinstance(strategy_cycle_timestamp, datetime.datetime)
+
+        if cycle_duration not in (CycleDuration.cycle_unknown, CycleDuration.cycle_1s, None):
+            assert strategy_cycle_timestamp.second == 0, f"Cycle duration {cycle_duration}: Does not look like a cycle timestamp: {strategy_cycle_timestamp}, should be even minutes"
+
         friendly_cycle_duration = cycle_duration.value if cycle_duration else "-"
-        with self.timed_task_context_manager("strategy_tick", clock=clock, cycle_duration=friendly_cycle_duration):
+        with self.timed_task_context_manager("strategy_tick", clock=strategy_cycle_timestamp, cycle_duration=friendly_cycle_duration):
 
             routing_state, pricing_model, valuation_model = self.setup_routing(universe)
             assert pricing_model, "Routing did not provide pricing_model"
 
             # Watch incoming deposits
             with self.timed_task_context_manager("sync_portfolio"):
-                self.sync_portfolio(clock, universe, state, debug_details)
+                self.sync_portfolio(strategy_cycle_timestamp, universe, state, debug_details)
 
             # Assing a new value for every existing position
             with self.timed_task_context_manager("revalue_portfolio"):
-                self.revalue_portfolio(clock, state, valuation_model)
+                self.revalue_portfolio(strategy_cycle_timestamp, state, valuation_model)
 
             # Log output
-            self.report_after_sync_and_revaluation(clock, universe, state, debug_details)
+            if self.is_progress_report_needed():
+                self.report_after_sync_and_revaluation(strategy_cycle_timestamp, universe, state, debug_details)
 
             # Run the strategy cycle
             with self.timed_task_context_manager("decide_trades"):
-                rebalance_trades = self.on_clock(clock, universe, pricing_model, state, debug_details)
+                rebalance_trades = self.on_clock(strategy_cycle_timestamp, universe, pricing_model, state, debug_details)
                 assert type(rebalance_trades) == list
                 debug_details["rebalance_trades"] = rebalance_trades
-                logger.info("We have %d trades", len(rebalance_trades))
 
-            # Log output
-            self.report_strategy_thinking(clock, universe, state, rebalance_trades, debug_details)
+                # Make some useful diagnostics output for log files to troubleshoot if something
+                # when wrong internally
+                _, last_point_at = state.visualisation.get_timestamp_range()
+                logger.info("We have %d new trades, %d total visualisation points, last visualisation point at %s",
+                            len(rebalance_trades),
+                            state.visualisation.get_total_points(),
+                            last_point_at
+                            )
+
+            # Log what our strategy decided
+            if self.is_progress_report_needed():
+                self.report_strategy_thinking(
+                    strategy_cycle_timestamp=strategy_cycle_timestamp,
+                    cycle=cycle,
+                    universe=universe,
+                    state=state,
+                    trades=rebalance_trades,
+                    debug_details=debug_details)
+
+            # Shortcut quit here if no trades are needed
+            if len(rebalance_trades) == 0:
+                logger.trade("No action taken: strategy decided not to open or close any positions")
+                return debug_details
 
             # Ask user confirmation for any trades
             with self.timed_task_context_manager("confirm_trades"):
                 approved_trades = self.approval_model.confirm_trades(state, rebalance_trades)
                 assert type(approved_trades) == list
                 logger.info("After approval we have %d trades left", len(approved_trades))
                 debug_details["approved_trades"] = approved_trades
 
             # Log output
-            self.report_before_execution(clock, universe, state, approved_trades, debug_details)
+            if self.is_progress_report_needed():
+                self.report_before_execution(strategy_cycle_timestamp, universe, state, approved_trades, debug_details)
 
             # Physically execute the trades
             with self.timed_task_context_manager("execute_trades", trade_count=len(approved_trades)):
 
                 # Unit tests can turn this flag to make it easier to see why trades fail
                 check_balances = debug_details.get("check_balances", False)
 
                 self.execution_model.execute_trades(
-                    clock,
+                    strategy_cycle_timestamp,
                     state,
                     approved_trades,
                     self.routing_model,
                     routing_state,
                     check_balances=check_balances)
 
             # Log output
-            self.report_after_execution(clock, universe, state, debug_details)
+            if self.is_progress_report_needed():
+                self.report_after_execution(strategy_cycle_timestamp, universe, state, debug_details)
 
         return debug_details
 
     def check_position_triggers(self,
         clock: datetime.datetime,
         state: State,
         universe: StrategyExecutionUniverse,
@@ -342,37 +462,58 @@
         - check_position_triggers() is much more lightweight and can be called much more frequently,
           even once per minute
 
         :return:
             List of generated stop loss trades
         """
 
+        if routing_state is None:
+            # Dummy executoin model
+            return
+
         assert isinstance(routing_state, RoutingState)
         assert isinstance(stop_loss_pricing_model, PricingModel)
 
         with self.timed_task_context_manager("check_position_triggers"):
 
             # We use PositionManager.close_position()
             # to generate trades to close stop loss positions
             position_manager = PositionManager(
                 clock,
-                universe,
+                universe.universe,
                 state,
                 stop_loss_pricing_model,
             )
 
-            stop_loss_trades = check_position_triggers(position_manager)
+            triggered_trades = check_position_triggers(position_manager)
 
-            approved_trades = self.approval_model.confirm_trades(state, stop_loss_trades)
+            approved_trades = self.approval_model.confirm_trades(state, triggered_trades)
 
             if approved_trades:
                 logger.info("Executing %d stop loss/take profit trades at %s", len(approved_trades), clock)
                 self.execution_model.execute_trades(
                     clock,
                     state,
                     approved_trades,
                     self.routing_model,
                     routing_state,
                     check_balances=False)
 
             return approved_trades
 
+
+    def repair_state(self, state: State) -> List[TradeExecution]:
+        """Repair unclean state issues.
+
+        Currently supports
+
+        - Fixing unfinished trades
+
+        :return:
+            List of fixed trades
+        """
+
+        logger.info("Reparing the state")
+
+        repaired = []
+        repaired += self.execution_model.repair_unconfirmed_trades(state)
+        return repaired
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/strategy_module.py` & `trade_executor-0.3/tradeexecutor/strategy/strategy_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -262,14 +262,21 @@
     """Describe elements that we need to have in a strategy module.
 
     The class variables are the same name as found in the Python strategy module.
     They can be uppercase or lowercase - all strategy module variables
     are exported as lowercase.
 
     """
+
+    #: The source code of the strategy
+    #:
+    #: Can be set `None` for strategies that are not public.
+    #:
+    source_code: Optional[str]
+
     trading_strategy_engine_version: str
     trading_strategy_type: StrategyType
     trading_strategy_cycle: CycleDuration
     trade_routing: TradeRouting
     reserve_currency: ReserveCurrency
     decide_trades: DecideTradesProtocol
 
@@ -324,22 +331,23 @@
         if self.trade_routing is None:
             raise StrategyModuleNotValid(f"trade_routing missing on the strategy")
 
         if self.chain_id:
             assert isinstance(self.chain_id, ChainId), f"Strategy module chain_in varaible expected ChainId instance, got {self.chain_id}"
 
 
-def parse_strategy_module(python_module_exports: dict) -> StrategyModuleInformation:
+def parse_strategy_module(python_module_exports: dict, source_code: Optional[str]=None) -> StrategyModuleInformation:
     """Parse a loaded .py module that describes a trading strategy.
 
     :param python_module_exports:
         Python module
 
     """
     return StrategyModuleInformation(
+        source_code,
         python_module_exports.get("trading_strategy_engine_version"),
         python_module_exports.get("trading_strategy_type"),
         python_module_exports.get("trading_strategy_cycle"),
         python_module_exports.get("trade_routing"),
         python_module_exports.get("reserve_currency"),
         python_module_exports.get("decide_trades"),
         python_module_exports.get("create_trading_universe"),
@@ -361,14 +369,17 @@
     """
     logger.info("Reading strategy %s", path)
 
     assert isinstance(path, Path)
 
     strategy_exports = runpy.run_path(path.as_posix())
 
+    with open(path.as_posix(), "rt") as inp:
+        source_code = inp.read()
+
     # For user convenience, make everything case-insentitive,
     # assume lowercase from no on
     strategy_exports = {k.lower(): v for k, v in strategy_exports.items()}
 
     version = strategy_exports.get("trading_strategy_engine_version")
 
     if version is None:
@@ -379,11 +390,11 @@
         if strategy_runner is None:
             raise StrategyModuleNotValid(f"{path} Python module does not declare trading_strategy_engine_version or strategy_factory variables")
 
         return strategy_runner
 
     logger.info("Strategy module %s, engine version %s", path, version)
 
-    mod_info = parse_strategy_module(strategy_exports)
+    mod_info = parse_strategy_module(strategy_exports, source_code)
     mod_info.validate()
 
     return mod_info
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/strategy_type.py` & `trade_executor-0.3/tradeexecutor/strategy/strategy_type.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/strategy/trading_strategy_universe.py` & `trade_executor-0.3/tradeexecutor/strategy/trading_strategy_universe.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 
 import contextlib
 import datetime
 import textwrap
 from abc import abstractmethod
 from dataclasses import dataclass
 import logging
-from typing import List, Optional, Callable, Tuple, Set, Dict, Iterable
+from math import isnan
+from typing import List, Optional, Callable, Tuple, Set, Dict, Iterable, Collection
 
 import pandas as pd
 
-from tradeexecutor.backtest.data_preload import preload_data
 from tradeexecutor.strategy.execution_context import ExecutionMode, ExecutionContext
 from tradingstrategy.token import Token
 
 from tradeexecutor.state.identifier import AssetIdentifier, TradingPairIdentifier
 from tradeexecutor.strategy.universe_model import StrategyExecutionUniverse, UniverseModel, DataTooOld, UniverseOptions
 from tradingstrategy.candle import GroupedCandleUniverse
 from tradingstrategy.chain import ChainId
-from tradingstrategy.client import Client
+from tradingstrategy.client import Client, BaseClient
 from tradingstrategy.exchange import ExchangeUniverse, Exchange, ExchangeType
-from tradingstrategy.liquidity import GroupedLiquidityUniverse
+from tradingstrategy.liquidity import GroupedLiquidityUniverse, ResampledLiquidityUniverse
 from tradingstrategy.pair import DEXPair, PandasPairUniverse, resolve_pairs_based_on_ticker, \
-    filter_for_exchanges, filter_for_quote_tokens, StablecoinFilteringMode, filter_for_stablecoins
+    filter_for_exchanges, filter_for_quote_tokens, StablecoinFilteringMode, filter_for_stablecoins, \
+    HumanReadableTradingPairDescription
 from tradingstrategy.timebucket import TimeBucket
 from tradingstrategy.universe import Universe
 from tradingstrategy.utils.groupeduniverse import filter_for_pairs
 
 
 logger = logging.getLogger(__name__)
 
@@ -56,14 +57,17 @@
 
     #: Candle data for all pairs
     candles: Optional[pd.DataFrame] = None
 
     #: All liquidity samples
     liquidity: Optional[pd.DataFrame] = None
 
+    #: Liquidity data granularity
+    liquidity_time_bucket: Optional[TimeBucket] = None
+
     #: Granularity of backtesting OHLCV data
     backtest_stop_loss_time_bucket: Optional[TimeBucket] = None
 
     #: All candles in stop loss time bucket
     backtest_stop_loss_candles: Optional[pd.DataFrame] = None
 
     def __post_init__(self):
@@ -75,23 +79,105 @@
         liquidity = self.liquidity
         if liquidity is not None:
             assert isinstance(liquidity, pd.DataFrame), f"Expected DataFrame, got {liquidity.__class__}"
 
 
 @dataclass
 class TradingStrategyUniverse(StrategyExecutionUniverse):
-    """A trading executor trading universe that using data from TradingStrategy.ai data feeds."""
+    """A trading executor trading universe that using data from TradingStrategy.ai data feeds.
+
+    - Supports generic trading universe definitions
+
+    - Adds special support for reserve currency handling and
+      take profit/stop loss backtesting
+    """
 
-    #: Trading universe datasets
+    #: Trading universe datasets.
+    #:
+    #: This encapsulates more generic `Universe` class from `tradingstrategy` package.
     universe: Optional[Universe] = None
 
+    #: Are we using special take profit/stop loss trigger data.
+    #:
+    #: If we are, what is the time granularity of this data.
     backtest_stop_loss_time_bucket: Optional[TimeBucket] = None
 
+    #: Special Pandas data feed for candles used only during the backtesting.
+    #:
+    #: This allows us to simulate take profit and stop loss trigger orders
+    #: that would be based on real-time market data in a live execution environment.
     backtest_stop_loss_candles: Optional[GroupedCandleUniverse] = None
 
+    #: How much historic data is needed by the strategy to make its decision.
+    #:
+    #: This is the explicit time frame in days or hours for the historical
+    #: data before today for the strategy to make a decision.
+    #:
+    #: This will limit the amount of data downloaded from the oracle
+    #: and greatly optimise the strategy decision execution.
+    #:
+    #: E.g. for 90 days you can use `datetime.timedelta(days=90)`
+    required_history_period: Optional[datetime.timedelta] = None
+
+    def __repr__(self):
+        pair_count = self.universe.pairs.get_count()
+        if pair_count <= 3:
+            pair_tickers = [f"{p.base_token_symbol}-{p.quote_token_symbol}" for p in self.universe.pairs.iterate_pairs()]
+            return f"<TradingStrategyUniverse for {', '.join(pair_tickers)}>"
+        else:
+            return f"<TradingStrategyUniverse for {self.universe.pairs.get_count()} pairs>"
+
+    def clone(self) -> "TradingStrategyUniverse":
+        """Create a copy of this universe.
+
+        Any dataframes are now copied,
+        but set by reference.
+        """
+        u = self.universe
+        new_universe = Universe(
+            time_bucket=u.time_bucket,
+            chains=u.chains,
+            exchanges=u.exchanges,
+            pairs=u.pairs,
+            candles=u.candles,
+            liquidity=u.liquidity,
+        )
+        return TradingStrategyUniverse(
+            universe=new_universe,
+            backtest_stop_loss_time_bucket=self.backtest_stop_loss_time_bucket,
+            backtest_stop_loss_candles=self.backtest_stop_loss_candles,
+            reserve_assets=self.reserve_assets,
+            required_history_period=self.required_history_period,
+        )
+
+    def get_pair_count(self) -> int:
+        return self.universe.pairs.get_count()
+
+    def is_empty(self) -> bool:
+        """This is an empty universe
+
+        - without trading pairs
+
+        - ...or without candles
+        """
+        candles = self.universe.candles.df if self.universe.candles else []
+        return self.universe.pairs.get_count() == 0 or len(candles) == 0
+
+    def is_single_pair_universe(self) -> bool:
+        """Is this trading universe made for a single pair trading.
+
+        Note that even a single pair universe may contain two trading pairs,
+        if we need intermediate routing pairs. E.g. AAVE -> BNB -> BUSD/
+        """
+
+        # TODO: Make a stupid assumption here
+        # as our strategies currently have 1 or 2 pairs for single pair trading.
+        # Convert this to a proper flag later.
+        return self.universe.pairs.get_count() <= 2
+
     def has_stop_loss_data(self) -> bool:
         """Do we have data available to determine trade stop losses.
 
         Note that this applies for backtesting only - when
         doing production trade execution, stop loss data is not part of the universe
         but real time pricing comes directly from the exchange using real-time
         side channels.
@@ -108,48 +194,96 @@
         if len(self.reserve_assets) != 1:
             raise TradingUniverseIssue(f"Only single reserve asset strategies supported for now, got {self.reserve_assets}")
 
         for a in self.reserve_assets:
             if a.decimals == 0:
                 raise TradingUniverseIssue(f"Reserve asset lacks decimals {a}")
 
-    @staticmethod
+    def get_pair_by_human_description(self, desc: HumanReadableTradingPairDescription) -> TradingPairIdentifier:
+        """Get pair by its human-readable description.
+
+        See :py:meth:`tradingstrategy.pair.PandasPairUniverse.get_pair_by_human_description`
+
+        The trading pair must be loaded in the exchange universe.
+
+        :return:
+            The trading pair on the exchange.
+
+            Highest volume trading pair if multiple matches.
+
+        :raise NoPairFound:
+            In the case input data cannot be resolved.
+
+        """
+        assert self.universe.exchange_universe, "You must set universe.exchange_universe to be able to use this method"
+        pair = self.universe.pairs.get_pair_by_human_description(self.universe.exchange_universe, desc)
+        return translate_trading_pair(pair)
+
     def create_single_pair_universe(
         dataset: Dataset,
-        chain_id: ChainId,
-        exchange_slug: str,
-        base_token: str,
-        quote_token: str,
+        chain_id: Optional[ChainId] = None,
+        exchange_slug: Optional[str] = None,
+        base_token: Optional[str] = None,
+        quote_token: Optional[str] = None,
+        pair: Optional[HumanReadableTradingPairDescription] = None
     ) -> "TradingStrategyUniverse":
         """Filters down the dataset for a single trading pair.
 
         This is ideal for strategies that only want to trade a single pair.
 
-        :param reserve_currency:
-            If set use this as a reserve currency,
-            otherwise use quote_token.
+        :param pair:
+            Give the pair we create the universe for
+
+        :param exchange_slug:
+            Legacy.
+
+            This or `pair`.
+
+        :param chain_id:
+            Legacy.
+
+            This or `pair`.
+
+        :param base_token:
+            Legacy.
+
+            This or `pair`.
+
+        :param quote_token:
+            Legacy.
+
+            This or `pair`.
         """
 
+        if pair:
+            chain_id, exchange_slug, base_token, quote_token, *fees = pair
+
+            if len(fees) > 0:
+                raise NotImplementedError("This method still lacks fee filtering")
+
         # We only trade on Pancakeswap v2
         exchange_universe = dataset.exchanges
         exchange = exchange_universe.get_by_chain_and_slug(chain_id, exchange_slug)
         assert exchange, f"No exchange {exchange_slug} found on chain {chain_id.name}"
 
         # Create trading pair database
         pair_universe = PandasPairUniverse.create_single_pair_universe(
             dataset.pairs,
             exchange,
             base_token,
             quote_token,
         )
 
         # Get daily candles as Pandas DataFrame
-        all_candles = dataset.candles
-        filtered_candles = filter_for_pairs(all_candles, pair_universe.df)
-        candle_universe = GroupedCandleUniverse(filtered_candles)
+        if dataset.candles is not None:
+            all_candles = dataset.candles
+            filtered_candles = filter_for_pairs(all_candles, pair_universe.df)
+            candle_universe = GroupedCandleUniverse(filtered_candles)
+        else:
+            candle_universe = None
 
         # Get liquidity candles as Pandas Dataframe
         if dataset.liquidity is not None and not dataset.liquidity.empty:
             all_liquidity = dataset.liquidity
             filtered_liquidity = filter_for_pairs(all_liquidity, pair_universe.df)
             liquidity_universe = GroupedLiquidityUniverse(filtered_liquidity)
         else:
@@ -301,14 +435,15 @@
     def create_multipair_universe(
         dataset: Dataset,
         chain_ids: Iterable[ChainId],
         exchange_slugs: Iterable[str],
         quote_tokens: Iterable[str],
         reserve_token: str,
         factory_router_map: Dict[str, tuple],
+        liquidity_resample_frequency: Optional[str] = None,
     ) -> "TradingStrategyUniverse":
         """Create a trading universe where pairs match a filter conditions.
 
         These universe may contain thousands of trading pairs.
         This is for strategies that trade across multiple pairs,
         like momentum strategies.
 
@@ -327,78 +462,204 @@
         :param reserve_token:
             The token addresses that are used as reserve assets.
 
         :param factory_router_map:
             Ensure we have a router address for every exchange we are going to use.
             TODO: In the future this information is not needed.
 
+        :param liquidity_resample_frequency:
+            Create a resampled liquidity universe instead of accurate one.
+
+            If given, this will set `Universe.resampled_liquidity` attribute.
+
+            Using :py:class:`ResampledLiquidityUniverse` will greatly
+            speed up backtests that estimate trading pair liquidity,
+            by trading off sample accuracy for code execution speed.
+
+            Must be a Pandas frequency string value, like `1d`.
+
+            Note that resamping itself takes a lot of time upfront,
+            so you want to use this only if the backtest takes lont time.
         """
 
         assert type(chain_ids) == list or type(chain_ids) == set
         assert type(exchange_slugs) == list or type(exchange_slugs) == set
         assert type(quote_tokens) == list or type(quote_tokens) == set
         assert type(reserve_token) == str
         assert reserve_token.startswith("0x")
 
         for t in quote_tokens:
             assert t.startswith("0x")
 
+        time_bucket = dataset.time_bucket
+
         # Normalise input parameters
         chain_ids = set(chain_ids)
         exchange_slugs = set(exchange_slugs)
         quote_tokens = set(q.lower() for q in quote_tokens)
         factory_router_map = {k.lower(): v for k, v in factory_router_map.items()}
 
         x: Exchange
         avail_exchanges = dataset.exchanges.exchanges
         our_exchanges = {x for x in avail_exchanges.values() if (x.chain_id in chain_ids) and (x.exchange_slug in exchange_slugs)}
+        exchange_universe = ExchangeUniverse.from_collection(our_exchanges)
 
         # Check we got all exchanges in the dataset
         for x in our_exchanges:
             assert x.address.lower() in factory_router_map, f"Could not find router for a exchange {x.exchange_slug}, factory {x.address}, router map is: {factory_router_map}"
 
         # Choose all trading pairs that are on our supported exchanges and
         # with our supported quote tokens
         pairs_df = filter_for_exchanges(dataset.pairs, list(our_exchanges))
         pairs_df = filter_for_quote_tokens(pairs_df, quote_tokens)
 
         # Remove stablecoin -> stablecoin pairs, because
         # trading between stable does not make sense for our strategies
         pairs_df = filter_for_stablecoins(pairs_df, StablecoinFilteringMode.only_volatile_pairs)
 
-        # Create trading pair database
-        pairs = PandasPairUniverse(pairs_df)
+        # Create the trading pair data for this specific strategy
+        pairs = PandasPairUniverse(
+            pairs_df,
+            exchange_universe=exchange_universe,
+        )
 
         # We do a bit detour here as we need to address the assets by their trading pairs first
         reserve_token_info = pairs.get_token(reserve_token)
         assert reserve_token_info, f"Reserve token {reserve_token} missing the trading pairset"
         reserve_assets = [
             translate_token(reserve_token_info)
         ]
 
         # Get daily candles as Pandas DataFrame
         all_candles = dataset.candles
         filtered_candles = filter_for_pairs(all_candles, pairs_df)
-        candle_universe = GroupedCandleUniverse(filtered_candles)
+        candle_universe = GroupedCandleUniverse(filtered_candles, time_bucket=time_bucket)
 
         # Get liquidity candles as Pandas Dataframe
         all_liquidity = dataset.liquidity
         filtered_liquidity = filter_for_pairs(all_liquidity, pairs_df)
-        liquidity_universe = GroupedLiquidityUniverse(filtered_liquidity)
+
+        if liquidity_resample_frequency is None:
+            liquidity_universe = GroupedLiquidityUniverse(filtered_liquidity, time_bucket=dataset.liquidity_time_bucket)
+            resampled_liquidity = None
+        else:
+            liquidity_universe = None
+            # Do just a print notification now, consider beta
+            # Optimally we want to resample, then store on a local disk cache,
+            # so that we do not need to run resample at the start of each backtest
+            print(f"Resamping liquidity data to {liquidity_resample_frequency}, this may take a long time")
+            resampled_liquidity = ResampledLiquidityUniverse(filtered_liquidity, resample_period=liquidity_resample_frequency)
+
+        if dataset.backtest_stop_loss_candles is not None:
+            backtest_stop_loss_time_bucket = dataset.backtest_stop_loss_time_bucket
+            filtered_candles = filter_for_pairs(dataset.backtest_stop_loss_candles, pairs_df)
+            backtest_stop_loss_candles = GroupedCandleUniverse(filtered_candles, time_bucket=dataset.backtest_stop_loss_time_bucket)
+        else:
+            backtest_stop_loss_time_bucket = None
+            backtest_stop_loss_candles = None
 
         universe = Universe(
             time_bucket=dataset.time_bucket,
             chains=chain_ids,
             pairs=pairs,
             exchanges=our_exchanges,
             candles=candle_universe,
             liquidity=liquidity_universe,
+            resampled_liquidity=resampled_liquidity,
+            exchange_universe=exchange_universe,
+        )
+
+        return TradingStrategyUniverse(
+            universe=universe,
+            reserve_assets=reserve_assets,
+            backtest_stop_loss_time_bucket=backtest_stop_loss_time_bucket,
+            backtest_stop_loss_candles=backtest_stop_loss_candles,
+        )
+
+    @staticmethod
+    def create_multichain_universe_by_pair_descriptions(
+        dataset: Dataset,
+        pairs: Collection[HumanReadableTradingPairDescription],
+        reserve_token_symbol: str,
+    ) -> "TradingStrategyUniverse":
+        """Create a trading universe based on list of (exchange, pair tuples)
+
+        This is designed for backtesting multipe pairs across different chains.
+        The created universe do not have any routing options and thus
+        cannot make any trades.
+
+        :param dataset:
+            Datasets downloaded from the oracle
+
+        :param pairs:
+            List of trading pairs to filter down.
+
+            The pair set is desigend to be small, couple of dozens of pairs max.
+
+            See :py:data:`HumanReadableTradingPairDescription`.
+
+        :param reserve_token_symbol:
+            The token symbol of the reverse asset.
+
+            Because we do not support routing, we just pick the first matching token.
+        """
+
+        time_bucket = dataset.time_bucket
+
+        # Create trading pair database
+        pair_universe = PandasPairUniverse(dataset.pairs)
+
+        # Filter pairs first and then rest by the resolved pairs
+        our_pairs = {pair_universe.get_pair_by_human_description(dataset.exchanges, d) for d in pairs}
+        chain_ids = {d[0] for d in pairs}
+        pair_ids = {p.pair_id for p in our_pairs}
+        exchange_ids = {p.exchange_id for p in our_pairs}
+        our_exchanges = {dataset.exchanges.get_by_id(id) for id in exchange_ids}
+        filtered_pairs_df = dataset.pairs.loc[dataset.pairs["pair_id"].isin(pair_ids)]
+
+        # Recreate universe again, now with limited pairs
+        pair_universe = PandasPairUniverse(filtered_pairs_df)
+
+        # We do a bit detour here as we need to address the assets by their trading pairs first
+        reserve_token = None
+        for p in pair_universe.iterate_pairs():
+            if p.quote_token_symbol == reserve_token_symbol:
+                translated_pair = translate_trading_pair(p)
+                reserve_token = translated_pair.quote
+
+        assert reserve_token, f"Reserve token {reserve_token_symbol} missing the pair quote tokens"
+        reserve_assets = [
+            reserve_token
+        ]
+
+        # Get daily candles as Pandas DataFrame
+        all_candles = dataset.candles
+        filtered_candles = filter_for_pairs(all_candles, filtered_pairs_df)
+        candle_universe = GroupedCandleUniverse(filtered_candles, time_bucket=time_bucket)
+
+        universe = Universe(
+            time_bucket=dataset.time_bucket,
+            chains=chain_ids,
+            pairs=pair_universe,
+            exchanges=our_exchanges,
+            candles=candle_universe,
+            exchange_universe=ExchangeUniverse.from_collection(our_exchanges),
         )
 
-        return TradingStrategyUniverse(universe=universe, reserve_assets=reserve_assets)
+        if dataset.backtest_stop_loss_candles is not None:
+            stop_loss_candle_universe = GroupedCandleUniverse(dataset.backtest_stop_loss_candles)
+        else:
+            stop_loss_candle_universe = None
+
+        return TradingStrategyUniverse(
+            universe=universe,
+            reserve_assets=reserve_assets,
+            backtest_stop_loss_time_bucket=dataset.backtest_stop_loss_time_bucket,
+            backtest_stop_loss_candles=stop_loss_candle_universe,
+        )
 
 
 class TradingStrategyUniverseModel(UniverseModel):
     """A universe constructor that builds the trading universe data using Trading Strategy client.
 
     On a live exeuction, trade universe is reconstructor for the every tick,
     by refreshing the trading data from the server.
@@ -574,44 +835,46 @@
     - At the start of the backtests or at each cycle of live trading, call
       the `create_trading_universe` callback of the strategy
 
     - Validate the output of the function
     """
 
     def __init__(self,
-                 client: Optional[Client],
+                 client: Optional[BaseClient],
                  execution_context: ExecutionContext,
                  create_trading_universe: Callable):
         """
 
         :param candle_time_frame_override:
             Use this candle time bucket instead one given in the strategy file.
             Allows to "speedrun" strategies.
 
         :param stop_loss_time_frame_override:
             Use this stop loss frequency instead one given in the strategy file.
             Allows to "speedrun" strategies.
 
         """
-        assert isinstance(client, Client) or client is None
+        assert isinstance(client, BaseClient) or client is None
         assert isinstance(execution_context, ExecutionContext), f"Got {execution_context}"
         assert isinstance(create_trading_universe, Callable), f"Got {create_trading_universe}"
         self.client = client
         self.execution_context = execution_context
         self.create_trading_universe = create_trading_universe
 
     def preload_universe(self, universe_options: UniverseOptions):
         """Triggered before backtesting execution.
 
         - Load all datasets with progress bar display.
 
         - Not triggered in live trading, as universe changes between cycles
         """
+        # TODO: Circular imports
+        from tradeexecutor.backtest.data_preload import preload_data
         with self.execution_context.timed_task_context_manager(task_name="preload_universe"):
-            preload_data(
+            return preload_data(
                 self.client,
                 self.create_trading_universe,
                 universe_options=universe_options)
 
     def construct_universe(self,
                            ts: datetime.datetime,
                            mode: ExecutionMode,
@@ -685,21 +948,47 @@
     quote = AssetIdentifier(
         chain_id=pair.chain_id.value,
         address=pair.quote_token_address,
         token_symbol=pair.quote_token_symbol,
         decimals=pair.quote_token_decimals,
     )
 
+    if pair.fee and isnan(pair.fee):
+        # Repair some broken data
+        fee = None
+    else:
+        # Convert DEXPair.fee BPS to %
+        # So, after this, fee can either be multiplier or None
+        if pair.fee is not None:
+            # If BPS fee is set it must be more than 1 BPS.
+            # Allow explicit fee = 0 in testing.
+            # if pair.fee != 0:
+            #     assert pair.fee > 1, f"DEXPair fee must be in BPS, got {pair.fee}"
+            
+            # can receive fee in bps or multiplier, but not raw form
+            if pair.fee > 1:
+                fee = pair.fee/10_000
+                
+            else:
+                fee = pair.fee
+            
+            # highest fee tier is currently 1% and lowest in 0.01%
+            if fee != 0:
+                assert 0.0001 <= fee <= 0.01, "bug in converting fee to multiplier, make sure bps"
+        else:
+            fee = None
+
     return TradingPairIdentifier(
         base=base,
         quote=quote,
         pool_address=pair.address,
         internal_id=pair.pair_id,
         info_url=pair.get_trading_pair_page_url(),
         exchange_address=pair.exchange_address,
+        fee=fee,
     )
 
 
 def create_pair_universe_from_code(chain_id: ChainId, pairs: List[TradingPairIdentifier]) -> "PandasPairUniverse":
     """Create the trading universe from handcrafted data.
 
     Used in unit testing.
@@ -721,43 +1010,68 @@
             quote_token_symbol=p.quote.token_symbol,
             token0_symbol=p.base.token_symbol,
             token1_symbol=p.quote.token_symbol,
             token0_address=p.base.address,
             token1_address=p.quote.address,
             token0_decimals=p.base.decimals,
             token1_decimals=p.quote.decimals,
+            fee=int(p.fee * 10_000) if p.fee else None,  # Convert to bps according to the documentation
         )
         data.append(dex_pair.to_dict())
     df = pd.DataFrame(data)
     return PandasPairUniverse(df)
 
 
 def load_all_data(
-        client: Client,
+        client: BaseClient,
         time_frame: TimeBucket,
         execution_context: ExecutionContext,
         universe_options: UniverseOptions,
+        with_liquidity=True,
+        liquidity_time_frame: Optional[TimeBucket] = None,
+        stop_loss_time_frame: Optional[TimeBucket] = None,
 ) -> Dataset:
     """Load all pair, candle and liquidity data for a given time bucket.
 
     - Backtest data is never reloaded
 
     - Live trading purges old data fields and reloads data
 
     :param client:
         Trading Strategy client instance
 
     :param time_frame:
-        Candle time bucket to load
+        Candle time bucket of which granularity to data to load.
+
+        Set to `TimeBucket.not_applicable` to downlaod only exchange and pair data,
+        as used in unit testing.
 
     :param execution_context:
         Defines if we are live or backtesting
+
+    :param with_liquidity:
+        Load liquidity data.
+
+        Note that all pairs may not have liquidity data available.
+
+    :param stop_loss_time_frame:
+        Load more granular candle data for take profit /tstop loss backtesting.
+
+    :param liquidity_time_frame:
+        Enable downloading different granularity of liquidity data.
+
+        If not given default to `time_frame`.
+
+    :return:
+        Dataset that covers all historical data.
+
+        This dataset is big and you need to filter it down for backtests.
     """
 
-    assert isinstance(client, Client)
+    assert isinstance(client, BaseClient)
     assert isinstance(time_frame, TimeBucket)
     assert isinstance(execution_context, ExecutionContext)
 
     # Apply overrides
     time_frame = universe_options.candle_time_bucket_override or time_frame
 
     assert universe_options.stop_loss_time_bucket_override is None, "Not supported yet"
@@ -769,35 +1083,52 @@
             logger.info("Purging trading data caches")
             client.clear_caches()
         else:
             logger.info("Using cached data if available")
 
         exchanges = client.fetch_exchange_universe()
         pairs = client.fetch_pair_universe().to_pandas()
-        candles = client.fetch_all_candles(time_frame).to_pandas()
-        liquidity = client.fetch_all_liquidity_samples(time_frame).to_pandas()
+
+        candles = liquidity = stop_loss_candles = None
+
+        if time_frame != TimeBucket.not_applicable:
+            candles = client.fetch_all_candles(time_frame).to_pandas()
+
+            if with_liquidity:
+                if not liquidity_time_frame:
+                    liquidity_time_frame = time_frame
+                liquidity = client.fetch_all_liquidity_samples(liquidity_time_frame).to_pandas()
+
+            if stop_loss_time_frame:
+                stop_loss_candles = client.fetch_all_candles(stop_loss_time_frame).to_pandas()
+
+
         return Dataset(
             time_bucket=time_frame,
+            liquidity_time_bucket=liquidity_time_frame,
             exchanges=exchanges,
             pairs=pairs,
             candles=candles,
             liquidity=liquidity,
+            backtest_stop_loss_time_bucket=stop_loss_time_frame,
+            backtest_stop_loss_candles=stop_loss_candles,
         )
 
 
 def load_pair_data_for_single_exchange(
-        client: Client,
+        client: BaseClient,
         execution_context: ExecutionContext,
         time_bucket: TimeBucket,
-        chain_id: ChainId,
-        exchange_slug: str,
-        pair_tickers: Set[Tuple[str, str]],
-        universe_options: UniverseOptions,
+        chain_id: Optional[ChainId] = None,
+        exchange_slug: Optional[str] = None,
+        pair_tickers: Set[Tuple[str, str]] | Collection[HumanReadableTradingPairDescription] | None = None,
+        universe_options: UniverseOptions = None,
         liquidity=False,
-        stop_loss_time_bucket: Optional[TimeBucket]=None,
+        stop_loss_time_bucket: Optional[TimeBucket] = None,
+        required_history_period: Optional[datetime.timedelta] = None,
 ) -> Dataset:
     """Load pair data for a single decentralised exchange.
 
     If you are not trading the full trading universe,
     this function does a much smaller dataset download than
     :py:func:`load_all_data`.
 
@@ -808,14 +1139,27 @@
       Furthermore, the data is stored in :py:class:`Client`
       disk cache for the subsequent notebook and backtest runs.
 
     - Live trading purges old data fields and reloads data
 
     Example:
 
+    ... code-block:: python
+
+        TRADING_PAIR = (ChainId.avalanche, "trader-joe", "WAVAX", "USDC")
+
+        dataset = load_pair_data_for_single_exchange(
+            client,
+            pair=TRADING_PAIR,
+            execution_context=execution_context,
+            universe_options=universe_options,
+        )
+
+    Example (old):
+
     .. code-block:: python
 
         # Time bucket for our candles
         candle_time_bucket = TimeBucket.d1
 
         # Which chain we are trading
         chain_id = ChainId.bsc
@@ -842,22 +1186,28 @@
     :param client:
         Trading Strategy client instance
 
     :param time_bucket:
         The candle time frame
 
     :param chain_id:
-        Which blockchain hosts our exchange
+        Which blockchain hosts our exchange.
+
+        Legacy. Give this or `pair`.
 
     :param exchange_slug:
         Which exchange hosts our trading pairs
 
+        Legacy. Give this or `pair`.
+
     :param exchange_slug:
         Which exchange hosts our trading pairs
 
+        Legacy. Give this or `pair`.
+
     :param pair_tickers:
         List of trading pair tickers as base token quote token tuples.
         E.g. `[('WBNB', 'BUSD'), ('Cake', 'BUSD')]`.
 
     :param liquidity:
         Set true to load liquidity data as well
 
@@ -868,21 +1218,29 @@
     :param execution_context:
         Defines if we are live or backtesting
 
     :param universe_options:
         Override values given the strategy file.
         Used in testing the framework.
 
+    :param required_history_period:
+        How much historical data we need to load.
+
+        Depends on the strategy. Defaults to load all data.
     """
 
     assert isinstance(client, Client)
     assert isinstance(time_bucket, TimeBucket)
     assert isinstance(execution_context, ExecutionContext)
-    assert isinstance(chain_id, ChainId)
-    assert isinstance(exchange_slug, str)
+    if chain_id is not None:
+        assert isinstance(chain_id, ChainId)
+
+    if exchange_slug is not None:
+        assert isinstance(exchange_slug, str)
+
     assert isinstance(universe_options, UniverseOptions)
 
     # Apply overrides
     stop_loss_time_bucket = universe_options.stop_loss_time_bucket_override or stop_loss_time_bucket
     time_bucket = universe_options.candle_time_bucket_override or time_bucket
 
     live = execution_context.live_trading
@@ -899,41 +1257,48 @@
 
         # Resolve full pd.Series for each pair
         # we are interested in
         our_pairs = resolve_pairs_based_on_ticker(
             pairs_df,
             chain_id,
             exchange_slug,
-            pair_tickers
+            pair_tickers,
         )
 
         assert len(our_pairs) > 0, f"Pair data not found {chain_id.name}, {exchange_slug}, {pair_tickers}"
 
         assert len(our_pairs) == len(pair_tickers), f"Pair resolution failed. Wanted to have {len(pair_tickers)} pairs, but after pair id resolution ended up with {len(our_pairs)} pairs"
 
         our_pair_ids = set(our_pairs["pair_id"])
 
         if len(our_pair_ids) > 1:
             desc = f"Loading OHLCV data for {exchange_slug}"
         else:
             pair = pair_tickers[0]
             desc = f"Loading OHLCV data for {pair[0]}-{pair[1]}"
 
+        if required_history_period is not None:
+            start_time = datetime.datetime.utcnow() - required_history_period
+        else:
+            start_time = None
+
         candles = client.fetch_candles_by_pair_ids(
             our_pair_ids,
             time_bucket,
             progress_bar_description=desc,
+            start_time=start_time,
         )
 
         if stop_loss_time_bucket:
             stop_loss_desc = f"Loading granular price data for stop loss/take profit for {exchange_slug}"
             stop_loss_candles = client.fetch_candles_by_pair_ids(
                 our_pair_ids,
                 stop_loss_time_bucket,
                 progress_bar_description=stop_loss_desc,
+                start_time=start_time,
             )
         else:
             stop_loss_candles = None
 
         if liquidity:
             raise NotImplemented("Partial liquidity data loading is not yet supported")
 
@@ -942,7 +1307,146 @@
             exchanges=exchanges,
             pairs=our_pairs,
             candles=candles,
             liquidity=None,
             backtest_stop_loss_time_bucket=stop_loss_time_bucket,
             backtest_stop_loss_candles=stop_loss_candles,
         )
+
+
+
+def load_partial_data(
+        client: BaseClient,
+        execution_context: ExecutionContext,
+        time_bucket: TimeBucket,
+        pairs: Collection[HumanReadableTradingPairDescription],
+        universe_options: UniverseOptions,
+        liquidity=False,
+        stop_loss_time_bucket: Optional[TimeBucket]=None,
+        required_history_period: Optional[datetime.timedelta] = None,
+        start_at: Optional[datetime.datetime] = None,
+        end_at: Optional[datetime.datetime] = None,
+        name: Optional[str] = None,
+) -> Dataset:
+    """Load pair data for named trading pairs.a
+
+    A loading function designed to load data for 2-20 pairs.
+    Instead of loading all pair data over Parquet datasets,
+    load only specific pair data from their corresponding JSONL endpoints.
+
+    :param client:
+        Trading Strategy client instance
+
+    :param time_bucket:
+        The candle time frame
+
+    :param chain_id:
+        Which blockchain hosts our exchange
+
+    :param exchange_slug:
+        Which exchange hosts our trading pairs
+
+    :param exchange_slug:
+        Which exchange hosts our trading pairs
+
+    :param pair_tickers:
+        List of trading pair tickers as base token quote token tuples.
+        E.g. `[('WBNB', 'BUSD'), ('Cake', 'BUSD')]`.
+
+    :param liquidity:
+        Set true to load liquidity data as well
+
+    :param stop_loss_time_bucket:
+        If set load stop loss trigger
+        data using this candle granularity.
+
+    :param execution_context:
+        Defines if we are live or backtesting
+
+    :param universe_options:
+        Override values given the strategy file.
+        Used in testing the framework.
+
+    :param required_history_period:
+        How much historical data we need to load.
+
+        Depends on the strategy. Defaults to load all data.
+
+    :param start_at:
+        Load data for a specific backtesting data range.
+
+    :param end_at:
+        Load data for a specific backtesting data range.
+
+    :param name:
+        The loading operation name used in progress bars
+
+    :return:
+        Datataset containing the requested data
+
+    """
+
+    assert isinstance(client, Client)
+    assert isinstance(time_bucket, TimeBucket)
+    assert isinstance(execution_context, ExecutionContext)
+    assert isinstance(universe_options, UniverseOptions)
+
+    # Apply overrides
+    stop_loss_time_bucket = universe_options.stop_loss_time_bucket_override or stop_loss_time_bucket
+    time_bucket = universe_options.candle_time_bucket_override or time_bucket
+
+    assert start_at and end_at, "Current implementatation is designed for backtest use only and needs both start_at and end_at timestamps"
+
+    with execution_context.timed_task_context_manager("load_partial_pair_data", time_bucket=time_bucket.value):
+
+        exchange_universe = client.fetch_exchange_universe()
+
+        pairs_df = client.fetch_pair_universe().to_pandas()
+        pair_universe = PandasPairUniverse(pairs_df)
+
+        # Filter pairs first and then rest by the resolved pairs
+        our_pairs = {pair_universe.get_pair_by_human_description(exchange_universe, d) for d in pairs}
+        our_pair_ids = {p.pair_id for p in our_pairs}
+        exchange_ids = {p.exchange_id for p in our_pairs}
+        our_exchanges = {exchange_universe.get_by_id(id) for id in exchange_ids}
+        our_exchange_universe = ExchangeUniverse.from_collection(our_exchanges)
+
+        # Eliminate the pairs we are not interested in from the database
+        filtered_pairs_df = pairs_df.loc[pairs_df["pair_id"].isin(our_pair_ids)]
+
+        # Autogenerate names by the pair count
+        if not name:
+            name = f"{len(filtered_pairs_df)} pairs"
+
+        progress_bar_desc = f"Loading OHLCV data for {name}"
+        candles = client.fetch_candles_by_pair_ids(
+            our_pair_ids,
+            time_bucket,
+            progress_bar_description=progress_bar_desc,
+            start_time=start_at,
+            end_time=end_at,
+        )
+
+        if stop_loss_time_bucket:
+            stop_loss_desc = f"Loading stop loss/take granular data for {name}"
+            stop_loss_candles = client.fetch_candles_by_pair_ids(
+                our_pair_ids,
+                stop_loss_time_bucket,
+                progress_bar_description=stop_loss_desc,
+                start_time=start_at,
+                end_time=end_at,
+            )
+        else:
+            stop_loss_candles = None
+
+        if liquidity:
+            raise NotImplemented("Partial liquidity data loading is not yet supported")
+
+        return Dataset(
+            time_bucket=time_bucket,
+            exchanges=our_exchange_universe,
+            pairs=filtered_pairs_df,
+            candles=candles,
+            liquidity=None,
+            backtest_stop_loss_time_bucket=stop_loss_time_bucket,
+            backtest_stop_loss_candles=stop_loss_candles,
+        )
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/universe_model.py` & `trade_executor-0.3/tradeexecutor/strategy/universe_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Construct the trading universe for the strategy."""
 import abc
 import datetime
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import List, Optional, Collection
 
 from tradingstrategy.timebucket import TimeBucket
 
 from tradeexecutor.state.identifier import AssetIdentifier
 from tradeexecutor.strategy.execution_context import ExecutionMode
 
 
@@ -23,15 +23,17 @@
 
     #: The list of reserve assets used in this strategy.
     #:
     #: Currently we support only one reserve asset per strategy, though in the
     #: future there can be several.
     #:
     #: Usually return the list of a BUSD/USDC/similar stablecoin.
-    reserve_assets: List[AssetIdentifier]
+    #:
+    #: TODO: Migrate to Set[] in all the code
+    reserve_assets: Collection[AssetIdentifier]
 
     def __post_init__(self):
         # Check that reserve assets look good
         for asset in self.reserve_assets:
             assert asset.token_symbol, f"Missing token symbol {asset}"
             assert asset.decimals, f"Missing token decimals {asset}"
 
@@ -73,15 +75,15 @@
 class UniverseModel(abc.ABC):
     """Create and manage trade universe.
 
     On a live execution, the trade universe is reconstructor for the every tick,
     by refreshing the trading data from the server.
     """
 
-    def preload_universe(self, universe_options: UniverseOptions):
+    def preload_universe(self, universe_options: UniverseOptions) -> StrategyExecutionUniverse:
         """Triggered before backtesting execution.
 
         - Load all datasets with progress bar display
 
         - Data is saved in FS cache
 
         - Not triggered in live trading, as universe changes between cycles
```

### Comparing `trade_executor-0.2/tradeexecutor/strategy/valuation.py` & `trade_executor-0.3/tradeexecutor/strategy/valuation.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 
 
 class ValuationModel(Protocol):
     """Revalue a current position.
 
     TODO: See if this should be moved inside state module, as it is referred by state.revalue_positions.
+    
+    Used by EthereumPoolRevaluator model (which, in turn, is used by UniswapV2PoolRevaluator and UniswapV3PoolRevaluator)
     """
 
     def __call__(self,
                  ts: datetime.datetime,
                  position: TradingPosition) -> Tuple[datetime.datetime, USDollarAmount]:
         """
 
@@ -48,17 +50,17 @@
         assert position.is_long(), "Short not supported"
 
         quantity = position.get_quantity()
         # Cannot do pricing for zero quantity
         if quantity == 0:
             return ts, 0.0
 
-        price = self.pricing_model.get_sell_price(ts, pair, position)
+        price_structure = self.pricing_model.get_sell_price(ts, pair, position)
 
-        return ts, price
+        return ts, price_structure.price
 
 
 class ValuationModelFactory(Protocol):
     """Creates a valuation method.
 
     - Valuation method is recreated for each cycle
```

### Comparing `trade_executor-0.2/tradeexecutor/testing/backtest_trader.py` & `trade_executor-0.3/tradeexecutor/testing/backtest_trader.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from tradeexecutor.backtest.backtest_execution import BacktestExecutionModel
 from tradeexecutor.backtest.backtest_pricing import BacktestSimplePricingModel
 from tradeexecutor.backtest.backtest_routing import BacktestRoutingModel, BacktestRoutingState
 from tradeexecutor.state.state import State, TradeType
 from tradeexecutor.state.position import TradingPosition
 from tradeexecutor.state.trade import TradeExecution
 from tradeexecutor.state.identifier import TradingPairIdentifier
+from tradeexecutor.state.types import USDollarAmount, BPS, USDollarPrice
+from tradeexecutor.strategy.trade_pricing import TradePricing
 from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse
 
 
 class BacktestTrader:
     """Helper class to generate trades for backtesting.
 
     Directly generate trades without going through a strategy.
@@ -43,69 +45,105 @@
         execution_details = execution_model.get_routing_state_details()
         self.routing_state: BacktestRoutingState = self.routing_model.create_routing_state(universe, execution_details)
 
     def time_travel(self, timestamp: datetime.datetime):
         """Set the timestamp for the next executions."""
         self.ts = timestamp
 
-    def get_buy_price(self, pair: TradingPairIdentifier, reserve: Decimal) -> float:
+    def get_buy_price(self, pair: TradingPairIdentifier, reserve: Decimal) -> TradePricing:
         """Get the historical price for our current backtest time."""
-        price = self.pricing_model.get_buy_price(self.ts, pair, reserve)
-        return float(price)  # Convert from numpy.float32
+        return self.pricing_model.get_buy_price(self.ts, pair, reserve)
 
-    def get_sell_price(self, pair: TradingPairIdentifier, quantity: Decimal) -> float:
+    def get_sell_price(self, pair: TradingPairIdentifier, quantity: Decimal) -> TradePricing:
         """Get the historical price for our current backtest time."""
-        price = self.pricing_model.get_sell_price(self.ts, pair, quantity)
-        return float(price)  # Convert from numpy.float32
+        return self.pricing_model.get_sell_price(self.ts, pair, quantity)
 
-    def create(self, pair: TradingPairIdentifier, quantity: Optional[Decimal], reserve: Optional[Decimal], price: float) -> Tuple[TradingPosition, TradeExecution]:
+    def create(self,
+               pair: TradingPairIdentifier,
+               quantity: Optional[Decimal],
+               reserve: Optional[Decimal],
+               price: float,
+               planned_mid_price: Optional[USDollarPrice] = None,
+               ) -> Tuple[TradingPosition, TradeExecution]:
         """Open a new trade."""
 
         assert len(self.universe.reserve_assets) == 1
 
         # 1. Plan
         position, trade, created = self.state.create_trade(
-            ts=self.ts,
+            strategy_cycle_at=self.ts,
             pair=pair,
             quantity=quantity,
             reserve=reserve,
             assumed_price=price,
             trade_type=TradeType.rebalance,
             reserve_currency=self.universe.reserve_assets[0],
-            reserve_currency_price=1.0)
+            reserve_currency_price=1.0,
+            planned_mid_price=planned_mid_price,
+        )
 
         return position, trade
 
-    def create_and_execute(self, pair: TradingPairIdentifier, quantity: Optional[Decimal], reserve: Optional[Decimal], price: float) -> Tuple[TradingPosition, TradeExecution]:
+    def create_and_execute(self,
+                           pair: TradingPairIdentifier,
+                           quantity: Optional[Decimal],
+                           reserve: Optional[Decimal],
+                           price: float,
+                           lp_fee: Optional[BPS] = None,
+                           lp_fees_estimated: Optional[USDollarAmount] = None,
+                           planned_mid_price: Optional[USDollarPrice] = None,
+                           ) -> Tuple[TradingPosition, TradeExecution]:
 
         assert price > 0
         assert type(price) == float
 
         assert not(quantity and reserve), "Give only quantity (sell) or reserve (buy)"
 
         # 1. Plan
         position, trade = self.create(
             pair=pair,
             quantity=quantity,
             reserve=reserve,
-            price=price)
+            price=price,
+            planned_mid_price=planned_mid_price,
+        )
+
+        trade.fee_tier = lp_fee
+        trade.lp_fees_estimated = lp_fees_estimated
 
         # Run trade start, simulated broadcast, simulated execution using
         # backtest execution model
         self.execution_model.execute_trades(
             self.ts,
             self.state,
             [trade],
             self.routing_model,
             self.routing_state,
             check_balances=True)
 
         return position, trade
 
     def buy(self, pair, reserve) -> Tuple[TradingPosition, TradeExecution]:
-        assumed_price = self.get_buy_price(pair, reserve)
-        return self.create_and_execute(pair, quantity=None, reserve=reserve, price=assumed_price)
+        price_structure = self.get_buy_price(pair, reserve)
+        return self.create_and_execute(
+            pair,
+            quantity=None,
+            reserve=reserve,
+            price=price_structure.price,
+            lp_fee=price_structure.get_fee_percentage(),
+            lp_fees_estimated=price_structure.get_total_lp_fees(),
+            planned_mid_price=price_structure.mid_price,
+        )
 
     def sell(self, pair, quantity) -> Tuple[TradingPosition, TradeExecution]:
-        assumed_price = self.get_sell_price(pair, quantity)
-        return self.create_and_execute(pair, quantity=-quantity, reserve=None, price=assumed_price)
+        price_structure = self.get_sell_price(pair, quantity)
+        return self.create_and_execute(
+            pair,
+            quantity=-quantity,
+            reserve=None,
+            price=price_structure.price,
+            lp_fee=price_structure.get_fee_percentage(),
+            lp_fees_estimated=price_structure.get_total_lp_fees(),
+            planned_mid_price=price_structure.mid_price)
+
+
```

### Comparing `trade_executor-0.2/tradeexecutor/testing/dummy_trader.py` & `trade_executor-0.3/tradeexecutor/testing/dummy_trader.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,23 +29,27 @@
 
     def time_travel(self, timestamp: datetime.datetime):
         self.ts = timestamp
 
     def create(self, pair: TradingPairIdentifier, quantity: Decimal, price: float) -> Tuple[TradingPosition, TradeExecution]:
         """Open a new trade."""
         # 1. Plan
+        
         position, trade, created = self.state.create_trade(
-            ts=self.ts,
+            strategy_cycle_at=self.ts,
             pair=pair,
             quantity=quantity,
             reserve=None,
             assumed_price=price,
             trade_type=TradeType.rebalance,
             reserve_currency=pair.quote,
-            reserve_currency_price=1.0)
+            reserve_currency_price=1.0,
+            planned_mid_price=price,
+            pair_fee=pair.fee
+        )
 
         self.ts += datetime.timedelta(seconds=1)
         return position, trade
 
     def create_and_execute(self, pair: TradingPairIdentifier, quantity: Decimal, price: float) -> Tuple[TradingPosition, TradeExecution]:
 
         assert price > 0
```

### Comparing `trade_executor-0.2/tradeexecutor/testing/ethereumtrader.py` & `trade_executor-0.3/tradeexecutor/testing/ethereumtrader_uniswap_v3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,158 +1,175 @@
-"""Ethereum test trading."""
+"""Ethereum test trading for uniswap v3."""
 
 import datetime
 from decimal import Decimal
-from typing import Tuple, List
+from typing import Tuple, List, Optional
 
 from tradingstrategy.pair import PandasPairUniverse
 from web3 import Web3
 
 from eth_defi.abi import get_deployed_contract
 from eth_defi.gas import estimate_gas_fees
 from eth_defi.hotwallet import HotWallet
-from eth_defi.uniswap_v2.deployment import UniswapV2Deployment
-from eth_defi.uniswap_v2.fees import estimate_buy_quantity, estimate_sell_price
-from tradeexecutor.ethereum.execution import broadcast_and_resolve
-from tradeexecutor.ethereum.tx import TransactionBuilder
-from tradeexecutor.ethereum.uniswap_v2_routing import UniswapV2SimpleRoutingModel, UniswapV2RoutingState
+from eth_defi.uniswap_v3.deployment import UniswapV3Deployment
+from eth_defi.uniswap_v3.price import UniswapV3PriceHelper
+
+from tradeexecutor.ethereum.tx import HotWalletTransactionBuilder, TransactionBuilder
+from tradeexecutor.ethereum.uniswap_v3.uniswap_v3_routing import UniswapV3SimpleRoutingModel, UniswapV3RoutingState
+from tradeexecutor.ethereum.uniswap_v3.uniswap_v3_execution import UniswapV3ExecutionModel
 from tradeexecutor.state.freeze import freeze_position_on_failed_trade
 from tradeexecutor.state.state import State, TradeType
 from tradeexecutor.state.position import TradingPosition
-from tradeexecutor.state.trade import TradeExecution, TradeStatus
+from tradeexecutor.state.trade import TradeExecution
 from tradeexecutor.state.identifier import TradingPairIdentifier
-from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse
+from tradeexecutor.ethereum.ethereumtrader import EthereumTrader
 
 
-class EthereumTestTrader:
+class UniswapV3TestTrader(EthereumTrader):
     """Helper class to trade against EthereumTester unit testing network."""
 
-    def __init__(self, web3: Web3, uniswap: UniswapV2Deployment, hot_wallet: HotWallet, state: State, pair_universe: PandasPairUniverse):
-        self.web3 = web3
+    def __init__(self,
+                 uniswap: UniswapV3Deployment,
+                 state: State,
+                 pair_universe: PandasPairUniverse,
+                 tx_builder: Optional[TransactionBuilder] = None,
+                 ):
+
+        super().__init__(tx_builder, state, pair_universe)
         self.uniswap = uniswap
-        self.state = state
-        self.hot_wallet = hot_wallet
-        self.pair_universe = pair_universe
-
-        self.ts = datetime.datetime(2022, 1, 1, tzinfo=None)
-        self.lp_fees = 2.50  # $2.5
-        self.gas_units_consumed = 150_000  # 150k gas units per swap
-        self.gas_price = 15 * 10**9  # 15 Gwei/gas unit
-
-        self.native_token_price = 1
-        self.confirmation_block_count = 0
-
-    def execute(self, trades: List[TradeExecution]):
-        execute_trades_simple(
-            self.state,
-            self.pair_universe,
-            trades,
-            self.web3,
-            self.hot_wallet,
-            self.uniswap,
-        )
+
+        self.execution_model = UniswapV3ExecutionModel(tx_builder)
+        self.price_helper = UniswapV3PriceHelper(uniswap)
+        self.tx_builder = tx_builder
 
     def buy(self, pair: TradingPairIdentifier, amount_in_usd: Decimal, execute=True) -> Tuple[TradingPosition, TradeExecution]:
         """Buy token (trading pair) for a certain value."""
         # Estimate buy price
-        base_token = get_deployed_contract(self.web3, "ERC20MockDecimals.json", Web3.toChecksumAddress(pair.base.address))
-        quote_token = get_deployed_contract(self.web3, "ERC20MockDecimals.json", Web3.toChecksumAddress(pair.quote.address))
-        raw_assumed_quantity = estimate_buy_quantity(self.uniswap, base_token, quote_token, amount_in_usd * (10 ** pair.quote.decimals))
+        base_token = get_deployed_contract(self.web3, "ERC20MockDecimals.json", Web3.to_checksum_address(pair.base.address))
+        quote_token = get_deployed_contract(self.web3, "ERC20MockDecimals.json", Web3.to_checksum_address(pair.quote.address))
+        
+        amount_in = int(amount_in_usd * (10 ** pair.quote.decimals))
+        
+        raw_fee = int(pair.fee * 1_000_000)
+        
+        # TODO see estimate_buy_quantity in eth_defi/uniswap_v2/fees
+        raw_assumed_quantity = self.price_helper.get_amount_out(
+            amount_in,
+            [quote_token.address, base_token.address],
+            [raw_fee]
+        )
+        
         assumed_quantity = Decimal(raw_assumed_quantity) / Decimal(10**pair.base.decimals)
         assumed_price = amount_in_usd / assumed_quantity
 
         position, trade, created= self.state.create_trade(
-            ts=self.ts,
+            strategy_cycle_at=self.ts,
             pair=pair,
             quantity=assumed_quantity,
             reserve=None,
             assumed_price=float(assumed_price),
             trade_type=TradeType.rebalance,
             reserve_currency=pair.quote,
-            reserve_currency_price=1.0)
+            reserve_currency_price=1.0,
+            pair_fee=pair.fee
+        )
 
         if execute:
-            self.execute([trade])
+            self.execute_trades_simple([trade])
         return position, trade
 
     def sell(self, pair: TradingPairIdentifier, quantity: Decimal, execute=True) -> Tuple[TradingPosition, TradeExecution]:
         """Sell token token (trading pair) for a certain quantity."""
 
         assert isinstance(quantity, Decimal)
-
-        base_token = get_deployed_contract(self.web3, "ERC20MockDecimals.json", Web3.toChecksumAddress(pair.base.address))
-        quote_token = get_deployed_contract(self.web3, "ERC20MockDecimals.json", Web3.toChecksumAddress(pair.quote.address))
+        
+        base_token = get_deployed_contract(self.web3, "ERC20MockDecimals.json", Web3.to_checksum_address(pair.base.address))
+        quote_token = get_deployed_contract(self.web3, "ERC20MockDecimals.json", Web3.to_checksum_address(pair.quote.address))
 
         raw_quantity = int(quantity * 10**pair.base.decimals)
-        raw_assumed_quote_token = estimate_sell_price(self.uniswap, base_token, quote_token, raw_quantity)
+        
+        raw_fee = int(pair.fee * 1_000_000)
+        
+        # TODO see estimate_sell_price() in eth_defi/uniswap_v2/fees.py
+        raw_assumed_quote_token = self.price_helper.get_amount_out(
+            raw_quantity,
+            [base_token.address, quote_token.address],
+            [raw_fee]
+        )
+        
         assumed_quota_token = Decimal(raw_assumed_quote_token) / Decimal(10**pair.quote.decimals)
 
         # assumed_price = quantity / assumed_quota_token
         assumed_price = assumed_quota_token / quantity
 
         position, trade, created = self.state.create_trade(
-            ts=self.ts,
+            strategy_cycle_at=self.ts,
             pair=pair,
             quantity=-quantity,
             reserve=None,
             assumed_price=float(assumed_price),
             trade_type=TradeType.rebalance,
             reserve_currency=pair.quote,
-            reserve_currency_price=1.0)
+            reserve_currency_price=1.0,
+            pair_fee=pair.fee
+        )
 
         if execute:
-            self.execute([trade])
+            self.execute_trades_simple([trade])
         return position, trade
 
+    def execute_trades_simple(
+            self,
+            trades: List[TradeExecution],
+            max_slippage=0.01, 
+            stop_on_execution_failure=True
+    ) -> Tuple[List[TradeExecution], List[TradeExecution]]:
+        """Execute trades on web3 instance.
+
+        A testing shortcut
+
+        - Create `BlockchainTransaction` instances
+
+        - Execute them on Web3 test connection (EthereumTester / Ganache)
+
+        - Works with single Uniswap test deployment
+        """
+
+        pair_universe = self.pair_universe   
+        web3 = self.web3
+        uniswap = self.uniswap
+        state = self.state   
+        
+        assert isinstance(pair_universe, PandasPairUniverse)
+
+        fees = estimate_gas_fees(web3)
+
+        tx_builder = self.tx_builder
+
+        reserve_asset, rate = state.portfolio.get_default_reserve()
+
+        # We know only about one exchange
+        routing_model = UniswapV3SimpleRoutingModel(
+            address_map={
+                "factory": uniswap.factory.address,
+                "router": uniswap.swap_router.address,
+                "position_manager": uniswap.position_manager.address,
+                "quoter": uniswap.quoter.address
+            },
+            allowed_intermediary_pairs={},
+            reserve_token_address=reserve_asset.address,
+        )
 
-def execute_trades_simple(
-        state: State,
-        pair_universe: PandasPairUniverse,
-        trades: List[TradeExecution],
-        web3: Web3,
-        hot_wallet: HotWallet,
-        uniswap: UniswapV2Deployment,
-        max_slippage=0.01, stop_on_execution_failure=True) -> Tuple[List[TradeExecution], List[TradeExecution]]:
-    """Execute trades on web3 instance.
-
-    A testing shortcut
-
-    - Create `BlockchainTransaction` instances
-
-    - Execute them on Web3 test connection (EthereumTester / Ganache)
-
-    - Works with single Uniswap test deployment
-    """
-
-    assert isinstance(pair_universe, PandasPairUniverse)
-
-    fees = estimate_gas_fees(web3)
-
-    tx_builder = TransactionBuilder(
-        web3,
-        hot_wallet,
-        fees,
-    )
-
-    reserve_asset, rate = state.portfolio.get_default_reserve_currency()
-
-    # We know only about one exchange
-    routing_model = UniswapV2SimpleRoutingModel(
-        factory_router_map={
-            uniswap.factory.address: (uniswap.router.address, uniswap.init_code_hash),
-        },
-        allowed_intermediary_pairs={},
-        reserve_token_address=reserve_asset.address,
-    )
-
-    state.start_trades(datetime.datetime.utcnow(), trades)
-    routing_state = UniswapV2RoutingState(pair_universe, tx_builder)
-    routing_model.execute_trades_internal(pair_universe, routing_state, trades)
-    broadcast_and_resolve(web3, state, trades, stop_on_execution_failure=stop_on_execution_failure)
+        state.start_trades(datetime.datetime.utcnow(), trades)
+        routing_state = UniswapV3RoutingState(pair_universe, tx_builder)
+        routing_model.execute_trades_internal(pair_universe, routing_state, trades)
+        
+        execution_model = UniswapV3ExecutionModel(self.tx_builder)
+        execution_model.broadcast_and_resolve(state, trades, stop_on_execution_failure=stop_on_execution_failure)
 
-    # Clean up failed trades
-    freeze_position_on_failed_trade(datetime.datetime.utcnow(), state, trades)
+        # Clean up failed trades
+        freeze_position_on_failed_trade(datetime.datetime.utcnow(), state, trades)
 
-    success = [t for t in trades if t.is_success()]
-    failed = [t for t in trades if t.is_failed()]
+        success = [t for t in trades if t.is_success()]
+        failed = [t for t in trades if t.is_failed()]
 
-    return success, failed
+        return success, failed
```

### Comparing `trade_executor-0.2/tradeexecutor/testing/pairuniversetrader.py` & `trade_executor-0.3/tradeexecutor/testing/pairuniversetrader.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,37 +17,41 @@
     def __init__(self, state: State):
         self.state = state
         self.nonce = 1
 
     def buy(self, pair: TradingPairIdentifier, amount_in_usd: Decimal) -> TradeExecution:
         """Buy token (trading pair) for a certain value."""
 
-        reserve_currency, exchange_rate = self.state.portfolio.get_default_reserve_currency()
+        reserve_currency, exchange_rate = self.state.portfolio.get_default_reserve()
 
         position, trade, created = self.state.create_trade(
-            ts=datetime.datetime.utcnow(),
+            strategy_cycle_at=datetime.datetime.utcnow(),
             pair=pair,
             assumed_price=1.0,
             quantity=None,
             reserve=amount_in_usd,
             trade_type=TradeType.rebalance,
             reserve_currency=reserve_currency,
-            reserve_currency_price=1.0)
+            reserve_currency_price=1.0,
+            pair_fee=pair.fee,
+        )
 
         return trade
 
     def sell(self, pair: TradingPairIdentifier, quantity: Decimal) -> TradeExecution:
         """Sell token token (trading pair) for a certain quantity."""
 
-        reserve_currency, exchange_rate = self.state.portfolio.get_default_reserve_currency()
+        reserve_currency, exchange_rate = self.state.portfolio.get_default_reserve()
 
         position, trade, created = self.state.create_trade(
-            ts=datetime.datetime.utcnow(),
+            strategy_cycle_at=datetime.datetime.utcnow(),
             pair=pair,
             assumed_price=1.0,
             quantity=-quantity,
             reserve=None,
             trade_type=TradeType.rebalance,
             reserve_currency=reserve_currency,
-            reserve_currency_price=1.0)
+            reserve_currency_price=1.0,
+            pair_fee=pair.fee,
+        )
 
         return trade
```

### Comparing `trade_executor-0.2/tradeexecutor/testing/simulated_execution_loop.py` & `trade_executor-0.3/tradeexecutor/testing/simulated_execution_loop.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,29 +5,36 @@
 import queue
 
 from eth_account.signers.local import LocalAccount
 from eth_defi.hotwallet import HotWallet
 from web3 import Web3
 
 from tradeexecutor.cli.loop import ExecutionLoop
-from tradeexecutor.ethereum.hot_wallet_sync import EthereumHotWalletReserveSyncer
-from tradeexecutor.ethereum.uniswap_v2_execution import UniswapV2ExecutionModel
-from tradeexecutor.ethereum.uniswap_v2_live_pricing import UniswapV2LivePricing
-from tradeexecutor.ethereum.uniswap_v2_routing import UniswapV2SimpleRoutingModel
-from tradeexecutor.ethereum.uniswap_v2_valuation import UniswapV2PoolRevaluator
+from tradeexecutor.ethereum.hot_wallet_sync_model import EthereumHotWalletReserveSyncer, HotWalletSyncModel
+from tradeexecutor.ethereum.tx import HotWalletTransactionBuilder
 from tradeexecutor.state.state import State
 from tradeexecutor.state.store import NoneStore
 from tradeexecutor.strategy.approval import UncheckedApprovalModel
 from tradeexecutor.strategy.cycle import CycleDuration
 from tradeexecutor.strategy.execution_context import ExecutionContext, ExecutionMode
 from tradeexecutor.strategy.pandas_trader.runner import PandasTraderRunner
 from tradeexecutor.strategy.strategy_module import DecideTradesProtocol
 from tradeexecutor.strategy.universe_model import StaticUniverseModel, StrategyExecutionUniverse
 from tradeexecutor.utils.timer import timed_task
 
+from tradeexecutor.ethereum.uniswap_v2.uniswap_v2_execution import UniswapV2ExecutionModel
+from tradeexecutor.ethereum.uniswap_v2.uniswap_v2_live_pricing import UniswapV2LivePricing
+from tradeexecutor.ethereum.uniswap_v2.uniswap_v2_routing import UniswapV2SimpleRoutingModel
+from tradeexecutor.ethereum.uniswap_v2.uniswap_v2_valuation import UniswapV2PoolRevaluator
+
+from tradeexecutor.ethereum.uniswap_v3.uniswap_v3_execution import UniswapV3ExecutionModel
+from tradeexecutor.ethereum.uniswap_v3.uniswap_v3_live_pricing import UniswapV3LivePricing
+from tradeexecutor.ethereum.uniswap_v3.uniswap_v3_routing import UniswapV3SimpleRoutingModel
+from tradeexecutor.ethereum.uniswap_v3.uniswap_v3_valuation import UniswapV3PoolRevaluator
+
 
 def set_up_simulated_execution_loop_uniswap_v2(
         *ignore,
         web3: Web3,
         decide_trades: DecideTradesProtocol,
         universe: StrategyExecutionUniverse,
         routing_model: UniswapV2SimpleRoutingModel,
@@ -37,18 +44,19 @@
     """Set up a simulated execution loop.
 
     Create a strategy execution that connects to in-memory blockchain simulation.
 
     This allows us to step through trades block by block and have
     strategies to respodn to price action (e.g. stop loss)
 
-    Currently hardcoded for Uniswap v2 exchanges only.
-
     See `test_uniswap_live_stop_loss.py` for an example.
 
+    :param wallet_account:
+        A trader account with some deployed money
+
     :return:
         Execution loop you can manually poke forward tick by tick,
         block by block.
     """
 
     if ignore:
         # https://www.python.org/dev/peps/pep-3102/
@@ -62,24 +70,28 @@
     )
 
     # Create empty state for this backtest
     store = NoneStore(state)
 
     hot_wallet = HotWallet(wallet_account)
 
-    hot_wallet_sync = EthereumHotWalletReserveSyncer(web3, wallet_account.address)
+    # hot_wallet_sync = EthereumHotWalletReserveSyncer(web3, wallet_account.address)
+    sync_model = HotWalletSyncModel(web3, hot_wallet)
+    sync_model.setup_all(state, list(universe.reserve_assets))
 
     cycle_duration = CycleDuration.cycle_unknown
 
     universe_model = StaticUniverseModel(universe)
 
+    tx_builder = HotWalletTransactionBuilder(web3, hot_wallet)
+
     execution_model = UniswapV2ExecutionModel(
-        web3,
-        hot_wallet,
+        tx_builder,
         max_slippage=1.00,
+        confirmation_block_count=0,  # Must be zero for the test chain
     )
 
     # Pricing model factory for single Uni v2 exchange
     def pricing_model_factory(execution_model, universe, routing_model):
         return UniswapV2LivePricing(
             web3,
             universe.universe.pairs,
@@ -90,26 +102,129 @@
         return UniswapV2PoolRevaluator(pricing_model)
 
     runner = PandasTraderRunner(
         timed_task_context_manager=timed_task,
         execution_model=execution_model,
         approval_model=UncheckedApprovalModel(),
         valuation_model_factory=valuation_model_factory,
-        sync_method=hot_wallet_sync,
+        sync_model=sync_model,
+        pricing_model_factory=pricing_model_factory,
+        routing_model=routing_model,
+        decide_trades=decide_trades,
+        execution_context=execution_context,
+    )
+
+    loop = ExecutionLoop(
+        name="simulated_execution",
+        command_queue=queue.Queue(),
+        execution_context=execution_context,
+        execution_model=execution_model,
+        sync_model=sync_model,
+        pricing_model_factory=pricing_model_factory,
+        valuation_model_factory=valuation_model_factory,
+        strategy_factory=None,
+        store=store,
+        cycle_duration=cycle_duration,
+        client=None,
+        approval_model=UncheckedApprovalModel(),
+        stats_refresh_frequency=datetime.timedelta(0),
+        position_trigger_check_frequency=datetime.timedelta(0),
+    )
+
+    loop.init_simulation(
+        universe_model,
+        runner,
+    )
+
+    return loop
+
+
+def set_up_simulated_execution_loop_uniswap_v3(
+        *ignore,
+        web3: Web3,
+        decide_trades: DecideTradesProtocol,
+        universe: StrategyExecutionUniverse,
+        routing_model: UniswapV3SimpleRoutingModel,
+        state: State,
+        wallet_account: LocalAccount,
+) -> ExecutionLoop:
+    """Set up a simulated execution loop for Uniswap V3.
+
+    Create a strategy execution that connects to in-memory blockchain simulation.
+
+    This allows us to step through trades block by block and have
+    strategies to respodn to price action (e.g. stop loss)
+
+    See `test_uniswap_live_stop_loss_uniswap_v3.py` for an example.
+
+    :return:
+        Execution loop you can manually poke forward tick by tick,
+        block by block.
+    """
+
+    if ignore:
+        # https://www.python.org/dev/peps/pep-3102/
+        raise TypeError("Only keyword arguments accepted")
+
+    assert isinstance(wallet_account, LocalAccount)
+    assert isinstance(routing_model, UniswapV3SimpleRoutingModel)
+
+    execution_context = ExecutionContext(
+        mode=ExecutionMode.simulated_trading,
+    )
+
+    # Create empty state for this backtest
+    store = NoneStore(state)
+
+    hot_wallet = HotWallet(wallet_account)
+
+    # hot_wallet_sync = EthereumHotWalletReserveSyncer(web3, wallet_account.address)
+    sync_model = HotWalletSyncModel(web3, hot_wallet)
+
+    cycle_duration = CycleDuration.cycle_unknown
+
+    universe_model = StaticUniverseModel(universe)
+
+    tx_builder = HotWalletTransactionBuilder(web3, hot_wallet)
+
+    execution_model = UniswapV3ExecutionModel(
+        tx_builder,
+        max_slippage=1.00,
+        confirmation_block_count=0,  # Must be zero for the test chain
+    )
+
+    # Pricing model factory for single Uni v2 exchange
+    def pricing_model_factory(execution_model, universe, routing_model):
+        return UniswapV3LivePricing(
+            web3,
+            universe.universe.pairs,
+            routing_model)
+
+    # Valuation model factory for single Uni v2 exchange
+    def valuation_model_factory(pricing_model):
+        return UniswapV3PoolRevaluator(pricing_model)
+
+    runner = PandasTraderRunner(
+        timed_task_context_manager=timed_task,
+        execution_model=execution_model,
+        approval_model=UncheckedApprovalModel(),
+        valuation_model_factory=valuation_model_factory,
+        sync_model=sync_model,
         pricing_model_factory=pricing_model_factory,
         routing_model=routing_model,
         decide_trades=decide_trades,
+        execution_context=execution_context,
     )
 
     loop = ExecutionLoop(
         name="simulated_execution",
         command_queue=queue.Queue(),
         execution_context=execution_context,
         execution_model=execution_model,
-        sync_method=hot_wallet_sync,
+        sync_model=sync_model,
         pricing_model_factory=pricing_model_factory,
         valuation_model_factory=valuation_model_factory,
         strategy_factory=None,
         store=store,
         cycle_duration=cycle_duration,
         client=None,
         approval_model=UncheckedApprovalModel(),
```

### Comparing `trade_executor-0.2/tradeexecutor/testing/simulated_trader.py` & `trade_executor-0.3/tradeexecutor/testing/simulated_trader.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,44 +22,49 @@
 
     def buy(self,
             ts: datetime.datetime,
             pair: TradingPairIdentifier,
             amount_in_usd: Decimal) -> TradeExecution:
         """Buy token (trading pair) for a certain value."""
 
-        price = self.pricing_model.get_buy_price(ts, pair, amount_in_usd)
+        price_structure = self.pricing_model.get_buy_price(ts, pair, amount_in_usd)
+        price = price_structure.price
 
-        reserve_currency, exchange_rate = self.state.portfolio.get_default_reserve_currency()
+        reserve_currency, exchange_rate = self.state.portfolio.get_default_reserve()
 
         position, trade, created = self.state.create_trade(
-            ts=datetime.datetime.utcnow(),
+            strategy_cycle_at=datetime.datetime.utcnow(),
             pair=pair,
             assumed_price=price,
             quantity=None,
             reserve=amount_in_usd,
             trade_type=TradeType.rebalance,
             reserve_currency=reserve_currency,
-            reserve_currency_price=1.0)
+            reserve_currency_price=1.0,
+            pair_fee=pair.fee
+        )
 
         return trade
 
     def sell(self, pair: TradingPairIdentifier, quantity: Decimal) -> TradeExecution:
         """Sell token token (trading pair) for a certain quantity."""
 
-        reserve_currency, exchange_rate = self.state.portfolio.get_default_reserve_currency()
+        reserve_currency, exchange_rate = self.state.portfolio.get_default_reserve()
 
         position, trade, created = self.state.create_trade(
-            ts=datetime.datetime.utcnow(),
+            strategy_cycle_at=datetime.datetime.utcnow(),
             pair=pair,
             assumed_price=1.0,
             quantity=-quantity,
             reserve=None,
             trade_type=TradeType.rebalance,
             reserve_currency=reserve_currency,
-            reserve_currency_price=1.0)
+            reserve_currency_price=1.0,
+            pair_fee=pair.fee
+        )
 
         return trade
 
     def simulate_execution(self, state: State, trade: TradeExecution, price_impact=1):
         ts = trade.opened_at
         price = trade.planned_price
         quantity = trade.planned_quantity
```

### Comparing `trade_executor-0.2/tradeexecutor/testing/synthetic_exchange_data.py` & `trade_executor-0.3/tradeexecutor/testing/synthetic_exchange_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Generate synthetic exchange."""
+from typing import Optional
+
 from tradeexecutor.backtest.backtest_routing import BacktestRoutingModel
+from tradeexecutor.state.types import BPS
 from tradeexecutor.strategy.trading_strategy_universe import TradingStrategyUniverse
 from tradeexecutor.testing.synthetic_ethereum_data import generate_random_ethereum_address
 from tradingstrategy.chain import ChainId
 from tradingstrategy.exchange import Exchange, ExchangeType
 from tradingstrategy.pair import DEXPair
 
 
@@ -16,15 +19,15 @@
         address=address,
         exchange_type=ExchangeType.uniswap_v2,
         pair_count=0,
     )
     return exchange
 
 
-def generate_simple_routing_model(universe: TradingStrategyUniverse) -> BacktestRoutingModel:
+def generate_simple_routing_model(universe: TradingStrategyUniverse, trading_fee: Optional[BPS] = None) -> BacktestRoutingModel:
     """Creates a routing model for data generated synthetically.
 
     - Assumes there is only one exchange in the trading universe
 
     - Assumes all pairs in the trading universe have the same quote token and its stablecoin
     """
 
@@ -50,8 +53,9 @@
     allowed_intermediary_pairs = {
     }
 
     return BacktestRoutingModel(
         factory_router_map,
         allowed_intermediary_pairs,
         reserve_token_address=reserve_asset.address,
+        trading_fee=trading_fee,
     )
```

### Comparing `trade_executor-0.2/tradeexecutor/testing/synthetic_price_data.py` & `trade_executor-0.3/tradeexecutor/testing/synthetic_price_data.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/utils/blockchain.py` & `trade_executor-0.3/tradeexecutor/utils/blockchain.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/utils/timer.py` & `trade_executor-0.3/tradeexecutor/utils/timer.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/utils/timestamp.py` & `trade_executor-0.3/tradeexecutor/utils/timestamp.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,22 +27,41 @@
     return timestamp
 
 
 def convert_and_validate_timestamp_as_int(timestamp: Union[pd.Timestamp, datetime.datetime]) -> int:
     """Serialise timestamp as UNIX epoch seconds UTC.
 
     Needed when we need to have time based keys in our state,
-    as the current JSON encoder cannot directly encode datetime.datetime keys/
+    as the current JSON encoder cannot directly encode datetime.datetime keys.
+
+    :return:
+        UNIX UTC timestamp
     """
     timestamp = convert_and_validate_timestamp(timestamp)
 
     # https://stackoverflow.com/a/5499906/315168
     return int(calendar.timegm(timestamp.utctimetuple()))
 
 
+def convert_and_validate_timestamp_as_float(timestamp: Union[pd.Timestamp, datetime.datetime]) -> float:
+    """Serialise timestamp as UNIX epoch seconds UTC.
+
+    Needed when we need to have time based keys in our state,
+    as the current JSON encoder cannot directly encode datetime.datetime keys.
+
+    :return:
+        UNIX UTC timestamp
+    """
+    timestamp = convert_and_validate_timestamp(timestamp)
+
+    # https://stackoverflow.com/a/5499906/315168
+    return calendar.timegm(timestamp.utctimetuple())
+
+
+
 def json_encode_timedelta(val: datetime.timedelta) -> float:
     """Encode timestamp objects as number of seconds passed"""
     return val.total_seconds()
 
 
 def json_decode_timedelta(val: float) -> datetime.timedelta:
     """Decode timestamp objects as number of seconds passed"""
```

### Comparing `trade_executor-0.2/tradeexecutor/utils/url.py` & `trade_executor-0.3/tradeexecutor/utils/url.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/webhook/app.py` & `trade_executor-0.3/tradeexecutor/webhook/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pyramid.authorization import ALL_PERMISSIONS
 from pyramid.view import forbidden_view_config
 
 from . import api
 from .error import exception_view
 from ..state.metadata import Metadata
 from ..state.store import JSONFileStore
+from ..strategy.run_state import RunState
 
 logger = logging.getLogger(__name__)
 
 
 @forbidden_view_config()
 def forbidden_view(request):
     if request.authenticated_userid is None:
@@ -67,15 +68,22 @@
 
     config.pyramid_openapi3_register_routes()
 
     config.scan(package='tradeexecutor.webhook.api')
     config.scan(package='tradeexecutor.webhook.events')
 
 
-def create_pyramid_app(username, password, command_queue: Queue, store: JSONFileStore, metadata: Metadata, production=False) -> Router:
+def create_pyramid_app(
+        username,
+        password,
+        command_queue: Queue,
+        store: JSONFileStore,
+        metadata: Metadata,
+        run_state: RunState,
+        production=False) -> Router:
     """Create WSGI app for Trading Strategy backend."""
 
     settings = {
         'production': production,
         'command_queue': command_queue,
     }
 
@@ -104,16 +112,18 @@
             config.set_root_factory(lambda request: Root())
         else:
             logger.info("Authentication policy disabled")
 
         init_web_api(config)
 
         # Expose the state store to the webhook
+        # by sharing the global objects across threads
         config.registry["store"] = store
         config.registry["metadata"] = metadata
+        config.registry["run_state"] = run_state
 
         config.add_exception_view(exception_view)
 
         if production:
             # Because datadog import modifies the global process and messes up things,
             # do not touch it if not absoluteneeded
             # https://docs.datadoghq.com/tracing/setup_overview/setup/python/?tab=containers
```

### Comparing `trade_executor-0.2/tradeexecutor/webhook/error.py` & `trade_executor-0.3/tradeexecutor/webhook/error.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/webhook/events.py` & `trade_executor-0.3/tradeexecutor/webhook/events.py`

 * *Files identical despite different names*

### Comparing `trade_executor-0.2/tradeexecutor/webhook/server.py` & `trade_executor-0.3/tradeexecutor/webhook/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from eth_defi.utils import is_localhost_port_listening
 from webtest.http import StopableWSGIServer
 
 from .app import create_pyramid_app
 from ..state.metadata import Metadata
 from ..state.store import JSONFileStore
+from ..strategy.run_state import RunState
 
 logger =  logging.getLogger(__name__)
 
 
 class WebhookServer(StopableWSGIServer):
     """Create a Waitress server that we can gracefully shut down.
 
@@ -44,25 +45,21 @@
 def create_webhook_server(
         host: str,
         port: int,
         username: str,
         password: str,
         queue: Queue,
         store: JSONFileStore,
-        metadata: Metadata) -> WebhookServer:
+        metadata: Metadata,
+        execution_state: RunState,
+) -> WebhookServer:
     """Starts the webhook web  server in a separate thread.
 
     :param queue: The command queue for commands posted in the webhook that offers async execution.
     """
 
-    #assert username, "Username must be given"
-    #assert password, "Password must be given"
-
-    if (not username) and (not password):
-        logger.warning("Web server started without username and password")
-
-    app = create_pyramid_app(username, password, queue, store, metadata, production=False)
+    app = create_pyramid_app(username, password, queue, store, metadata, execution_state, production=False)
     server = WebhookServer.create(app, host=host, port=port, clear_untrusted_proxy_headers=True)
     logger.info("Webhook server will spawn at %s:%d, using username %s", host, port, username)
     # Wait until the server has started
     server.wait()
     return server
```

### Comparing `trade_executor-0.2/setup.py` & `trade_executor-0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from setuptools import setup
 
 packages = \
 ['tradeexecutor',
  'tradeexecutor.analysis',
  'tradeexecutor.backtest',
  'tradeexecutor.cli',
+ 'tradeexecutor.cli.commands',
  'tradeexecutor.ethereum',
+ 'tradeexecutor.ethereum.enzyme',
+ 'tradeexecutor.ethereum.uniswap_v2',
+ 'tradeexecutor.ethereum.uniswap_v3',
  'tradeexecutor.monkeypatch',
  'tradeexecutor.state',
  'tradeexecutor.statistics',
  'tradeexecutor.strategy',
  'tradeexecutor.strategy.pandas_trader',
  'tradeexecutor.strategy.qstrader',
  'tradeexecutor.testing',
@@ -23,47 +27,50 @@
 
 install_requires = \
 ['ipywidgets>=7.0,<8.0',
  'jupyterlab>=3.5.0,<4.0.0',
  'matplotlib>=3.6.0,<4.0.0',
  'pandas-ta>=0.3.14-beta.0,<0.4.0',
  'requests>=2.27.1,<3.0.0',
- 'tqdm-loggable>=0.1.1,<0.2.0',
+ 'tblib>=1.7.0,<2.0.0',
+ 'tqdm-loggable==0.1.3',
  'tqdm>=4.64.1,<5.0.0',
- 'trading-strategy==0.8.5',
- 'web3-ethereum-defi>=0.11.1,<0.12.0',
- 'web3>=5.26.0,<6.0.0']
+ 'trading-strategy==0.14']
 
 extras_require = \
-{'execution': ['typer>=0.4.0,<0.5.0',
+{':extra == "data"': ['web3-ethereum-defi==0.18.3'],
+ ':extra == "execution"': ['python-logstash-tradingstrategy==0.5.1'],
+ 'execution': ['typer>=0.4.0,<0.5.0',
                'colorama>=0.4.4,<0.5.0',
                'coloredlogs>=15.0.1,<16.0.0',
                'prompt-toolkit>=3.0.31,<4.0.0',
                'APScheduler>=3.9.1,<4.0.0',
-               'python-logstash-tradingstrategy>=0.5.0,<0.6.0',
                'python-logging-discord-handler>=0.1.3,<0.2.0',
-               'python-dotenv>=0.21.0,<0.22.0'],
+               'python-dotenv>=0.21.0,<0.22.0',
+               'kaleido==0.2.1'],
  'qstrader': ['trading-strategy-qstrader>=0.5,<0.6'],
+ 'quantstats': ['quantstats>=0.0.59,<0.0.60'],
  'web-server': ['pyramid>=2.0,<3.0',
-                'pyramid-openapi3>=0.13,<0.14',
+                'pyramid-openapi3>=0.16.0,<0.17.0',
                 'waitress>=2.0.0,<3.0.0',
-                'WebTest>=3.0.0,<4.0.0']}
+                'WebTest>=3.0.0,<4.0.0',
+                'openapi-core<0.17']}
 
 entry_points = \
 {'console_scripts': ['get-latest-release = '
                      'tradeexecutor.cli.latest_release:main',
                      'prepare-docker-env = '
                      'tradeexecutor.cli.prepare_docker_env:main',
                      'trade-executor = tradeexecutor.cli.main:app']}
 
 setup_kwargs = {
     'name': 'trade-executor',
-    'version': '0.2',
-    'description': 'Trading strategy execution and backtesting',
-    'long_description': '[![.github/workflows/tests.yml](https://github.com/tradingstrategy-ai/trade-executor/actions/workflows/tests.yml/badge.svg)](https://github.com/tradingstrategy-ai/trade-executor/actions/workflows/tests.yml)\n\n# Trade Executor\n\nTrade Executor is a Python framework for executing algorithmic trading strategies on decentralised exchanges. \n\n**Note**: This is early alpha software. Please pop in to the Discord for any questions. \n\n## Features\n\n- [High quality documentation](https://tradingstrategy.ai/docs/)\n- Support [decentralised markets like Uniswap, PancakeSwap](https://tradingstrategy.ai/docs/overview/supported-markets.html) \n- [Live trading](https://tradingstrategy.ai/docs/running/live-trading.html) and [backtesting](https://tradingstrategy.ai/docs/running/backtesting.html)  \n- [Webhook web serverPlain](https://tradingstrategy.ai/docs/running/webhook.html) for web and JavaScript integration\n- Run the strategy execution as [Python application or Docker container](https://tradingstrategy.ai/docs/running/cli.html)\n\n## More information\n\n- [Read documentation on running and backtesting strategies](https://tradingstrategy.ai/docs/running/index.html)\n- Visit [Trading Strategy website to learn about algorithmic trading on decentralised exchanges](https://tradingstrategy.ai)\n- [Join the Discord for any questions](https://tradingstrategy.ai/community)\n\n## Installation\n\n```shell\ngit clone git@github.com:tradingstrategy-ai/trade-executor.git\ncd trade-executor\ngit submodule update --init --recursive\npoetry install -E web-server -E execution\n```\n\n## Architecture overview\n\n![Archiecture overview](docs/deployment-overview.drawio.svg)\n\n## Development\n\nSee [docs](./docs).\n\n## Community\n\n* [Trading Strategy website](https://tradingstrategy.ai)\n\n* [Blog](https://tradingstrategy.ai/blog)\n\n* [Twitter](https://twitter.com/TradingProtocol)\n\n* [Discord](https://tradingstrategy.ai/community#discord) \n\n* [Telegram channel](https://t.me/trading_protocol)\n\n## License \n\n- AGPL\n',
+    'version': '0.3',
+    'description': 'Algorithmic trading backtesting and execution engine for decentralised finance',
+    'long_description': '[![Automated test suite and Docker image build](https://github.com/tradingstrategy-ai/trade-executor/actions/workflows/test-and-build-image.yml/badge.svg)](https://github.com/tradingstrategy-ai/trade-executor/actions/workflows/test-and-build-image.yml)\n\n# Trade Executor: Algorithmic Trading Engine for DeFi \n\n`trade-executor` is a Python framework for backtesting and live execution of algorithmic trading strategies on decentralised exchanges. \n\n**Note**: This is early beta software. [Please pop in to the Discord for any questions](https://tradingstrategy.ai/community). \n\n## Features\n\n- Only trading framework that has been built grounds up for [decentralised finance](https://tradingstrategy.ai/glossary/decentralised-finance)\n- [High quality documentation](https://tradingstrategy.ai/docs/)\n- Support [decentralised markets like Uniswap, PancakeSwap](https://tradingstrategy.ai/docs/overview/supported-markets.html)\n- [Backtesting enginer](https://tradingstrategy.ai/docs/running/backtesting.html)\n- [Live trading](https://tradingstrategy.ai/docs/running/live-trading.html)   \n- [Webhook web server](https://tradingstrategy.ai/docs/running/webhook.html) for JavaScript frontend and monitoring system integration\n- Deploy as [Docker container](https://tradingstrategy.ai/docs/running/cli.html)\n\n## Prerequisites\n\nYou need to know\n\n- Basics of Python \n- Basics of trading\n- [We have collected learning material for developers new to algorithmic trading](https://tradingstrategy.ai/docs/learn/index.html)\n\n## Getting started\n\nFirst study the example code\n\n- [Code examples](https://tradingstrategy.ai/docs/programming/code-examples/running.html)\n- [Trading strategy examples](https://tradingstrategy.ai/docs/programming/code-examples/running.html)\n- [See TradingView PineScript porting example](https://tradingstrategy.ai/blog/avalanche-summit-ii-workshop)\n\n## More information\n\n- [Read documentation on running and backtesting strategies](https://tradingstrategy.ai/docs/running/index.html)\n- Visit [Trading Strategy website to learn about algorithmic trading on decentralised exchanges](https://tradingstrategy.ai)\n- [Join the Discord for any questions](https://tradingstrategy.ai/community)\n\n## Installation\n\n**Note**: The project is under active development. We recommend any developers to use Github master branch\nfor installations.\n\n```shell\ngit clone git@github.com:tradingstrategy-ai/trade-executor.git\ncd trade-executor\ngit submodule update --init --recursive\n\n# Extra dependencies\n# - execution: infrastructure to run live strategies\n# - web-server: support webhook server of live strategy executors\n# - qstrader: still needed to run legacy unit tests\npoetry install -E web-server -E execution -E qstrader -E quantstats\n``` \n\nOr with pip:\n\n```shell\npip install -e ".[web-server,execution,qstrader,quantstats]" \n```\n\n## Architecture overview\n\nHere is an example of a live trading deployment of a `trade-executor` package.\n\n![Architecture overview](docs/deployment-overview.drawio.svg)\n\n## Running tests\n\nSee [internal development documentation](https://tradingstrategy.ai/docs/programming/development.html). \n\n## Community\n\n- [Trading Strategy website](https://tradingstrategy.ai)\n- [Community Discord server](https://tradingstrategy.ai/community#discord)\n- [Blog](https://tradingstrategy.ai/blog)\n- [Twitter](https://twitter.com/TradingProtocol)\n- [Telegram channel](https://t.me/trading_protocol)\n- [Newsletter](https://tradingstrategy.ai/newsletter)\n\n## License \n\n- AGPL\n- [Contact for the commercial dual licensing](https://tradingstrategy.ai/about)\n',
     'author': 'Mikko Ohtamaa',
     'author_email': 'mikko@tradingstrategy.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://tradingstrategy.ai',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `trade_executor-0.2/PKG-INFO` & `trade_executor-0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,134 @@
 Metadata-Version: 2.1
 Name: trade-executor
-Version: 0.2
-Summary: Trading strategy execution and backtesting
+Version: 0.3
+Summary: Algorithmic trading backtesting and execution engine for decentralised finance
 Home-page: https://tradingstrategy.ai
 License: APGL
-Keywords: algorithmic trading,ethereum,cryptocurrency,uniswap,quantitative finance,binance,blockchain,pancakeswap,polygon,web3
+Keywords: algorithmic trading,ethereum,cryptocurrency,uniswap,quantitative finance,binance,coinbase,pancakeswap
 Author: Mikko Ohtamaa
 Author-email: mikko@tradingstrategy.ai
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: data
 Provides-Extra: execution
 Provides-Extra: qstrader
+Provides-Extra: quantstats
 Provides-Extra: web-server
-Requires-Dist: APScheduler (>=3.9.1,<4.0.0); extra == "execution"
-Requires-Dist: WebTest (>=3.0.0,<4.0.0); extra == "web-server"
-Requires-Dist: colorama (>=0.4.4,<0.5.0); extra == "execution"
-Requires-Dist: coloredlogs (>=15.0.1,<16.0.0); extra == "execution"
+Requires-Dist: APScheduler (>=3.9.1,<4.0.0) ; extra == "execution"
+Requires-Dist: WebTest (>=3.0.0,<4.0.0) ; extra == "web-server"
+Requires-Dist: colorama (>=0.4.4,<0.5.0) ; extra == "execution"
+Requires-Dist: coloredlogs (>=15.0.1,<16.0.0) ; extra == "execution"
 Requires-Dist: ipywidgets (>=7.0,<8.0)
 Requires-Dist: jupyterlab (>=3.5.0,<4.0.0)
+Requires-Dist: kaleido (==0.2.1) ; extra == "execution"
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
+Requires-Dist: openapi-core (<0.17) ; extra == "web-server"
 Requires-Dist: pandas-ta (>=0.3.14-beta.0,<0.4.0)
-Requires-Dist: prompt-toolkit (>=3.0.31,<4.0.0); extra == "execution"
-Requires-Dist: pyramid (>=2.0,<3.0); extra == "web-server"
-Requires-Dist: pyramid-openapi3 (>=0.13,<0.14); extra == "web-server"
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0); extra == "execution"
-Requires-Dist: python-logging-discord-handler (>=0.1.3,<0.2.0); extra == "execution"
-Requires-Dist: python-logstash-tradingstrategy (>=0.5.0,<0.6.0); extra == "execution"
+Requires-Dist: prompt-toolkit (>=3.0.31,<4.0.0) ; extra == "execution"
+Requires-Dist: pyramid (>=2.0,<3.0) ; extra == "web-server"
+Requires-Dist: pyramid-openapi3 (>=0.16.0,<0.17.0) ; extra == "web-server"
+Requires-Dist: python-dotenv (>=0.21.0,<0.22.0) ; extra == "execution"
+Requires-Dist: python-logging-discord-handler (>=0.1.3,<0.2.0) ; extra == "execution"
+Requires-Dist: python-logstash-tradingstrategy (==0.5.1) ; extra == "execution"
+Requires-Dist: quantstats (>=0.0.59,<0.0.60) ; extra == "quantstats"
 Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: tblib (>=1.7.0,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: tqdm-loggable (>=0.1.1,<0.2.0)
-Requires-Dist: trading-strategy (==0.8.5)
-Requires-Dist: trading-strategy-qstrader (>=0.5,<0.6); extra == "qstrader"
-Requires-Dist: typer (>=0.4.0,<0.5.0); extra == "execution"
-Requires-Dist: waitress (>=2.0.0,<3.0.0); extra == "web-server"
-Requires-Dist: web3 (>=5.26.0,<6.0.0)
-Requires-Dist: web3-ethereum-defi (>=0.11.1,<0.12.0)
+Requires-Dist: tqdm-loggable (==0.1.3)
+Requires-Dist: trading-strategy (==0.14)
+Requires-Dist: trading-strategy-qstrader (>=0.5,<0.6) ; extra == "qstrader"
+Requires-Dist: typer (>=0.4.0,<0.5.0) ; extra == "execution"
+Requires-Dist: waitress (>=2.0.0,<3.0.0) ; extra == "web-server"
+Requires-Dist: web3-ethereum-defi (==0.18.3) ; extra == "data"
 Project-URL: Repository, https://github.com/tradingstrategy-ai/trade-executor
 Description-Content-Type: text/markdown
 
-[![.github/workflows/tests.yml](https://github.com/tradingstrategy-ai/trade-executor/actions/workflows/tests.yml/badge.svg)](https://github.com/tradingstrategy-ai/trade-executor/actions/workflows/tests.yml)
+[![Automated test suite and Docker image build](https://github.com/tradingstrategy-ai/trade-executor/actions/workflows/test-and-build-image.yml/badge.svg)](https://github.com/tradingstrategy-ai/trade-executor/actions/workflows/test-and-build-image.yml)
 
-# Trade Executor
+# Trade Executor: Algorithmic Trading Engine for DeFi 
 
-Trade Executor is a Python framework for executing algorithmic trading strategies on decentralised exchanges. 
+`trade-executor` is a Python framework for backtesting and live execution of algorithmic trading strategies on decentralised exchanges. 
 
-**Note**: This is early alpha software. Please pop in to the Discord for any questions. 
+**Note**: This is early beta software. [Please pop in to the Discord for any questions](https://tradingstrategy.ai/community). 
 
 ## Features
 
+- Only trading framework that has been built grounds up for [decentralised finance](https://tradingstrategy.ai/glossary/decentralised-finance)
 - [High quality documentation](https://tradingstrategy.ai/docs/)
-- Support [decentralised markets like Uniswap, PancakeSwap](https://tradingstrategy.ai/docs/overview/supported-markets.html) 
-- [Live trading](https://tradingstrategy.ai/docs/running/live-trading.html) and [backtesting](https://tradingstrategy.ai/docs/running/backtesting.html)  
-- [Webhook web serverPlain](https://tradingstrategy.ai/docs/running/webhook.html) for web and JavaScript integration
-- Run the strategy execution as [Python application or Docker container](https://tradingstrategy.ai/docs/running/cli.html)
+- Support [decentralised markets like Uniswap, PancakeSwap](https://tradingstrategy.ai/docs/overview/supported-markets.html)
+- [Backtesting enginer](https://tradingstrategy.ai/docs/running/backtesting.html)
+- [Live trading](https://tradingstrategy.ai/docs/running/live-trading.html)   
+- [Webhook web server](https://tradingstrategy.ai/docs/running/webhook.html) for JavaScript frontend and monitoring system integration
+- Deploy as [Docker container](https://tradingstrategy.ai/docs/running/cli.html)
+
+## Prerequisites
+
+You need to know
+
+- Basics of Python 
+- Basics of trading
+- [We have collected learning material for developers new to algorithmic trading](https://tradingstrategy.ai/docs/learn/index.html)
+
+## Getting started
+
+First study the example code
+
+- [Code examples](https://tradingstrategy.ai/docs/programming/code-examples/running.html)
+- [Trading strategy examples](https://tradingstrategy.ai/docs/programming/code-examples/running.html)
+- [See TradingView PineScript porting example](https://tradingstrategy.ai/blog/avalanche-summit-ii-workshop)
 
 ## More information
 
 - [Read documentation on running and backtesting strategies](https://tradingstrategy.ai/docs/running/index.html)
 - Visit [Trading Strategy website to learn about algorithmic trading on decentralised exchanges](https://tradingstrategy.ai)
 - [Join the Discord for any questions](https://tradingstrategy.ai/community)
 
 ## Installation
 
+**Note**: The project is under active development. We recommend any developers to use Github master branch
+for installations.
+
 ```shell
 git clone git@github.com:tradingstrategy-ai/trade-executor.git
 cd trade-executor
 git submodule update --init --recursive
-poetry install -E web-server -E execution
-```
 
-## Architecture overview
+# Extra dependencies
+# - execution: infrastructure to run live strategies
+# - web-server: support webhook server of live strategy executors
+# - qstrader: still needed to run legacy unit tests
+poetry install -E web-server -E execution -E qstrader -E quantstats
+``` 
 
-![Archiecture overview](docs/deployment-overview.drawio.svg)
+Or with pip:
 
-## Development
+```shell
+pip install -e ".[web-server,execution,qstrader,quantstats]" 
+```
 
-See [docs](./docs).
+## Architecture overview
 
-## Community
+Here is an example of a live trading deployment of a `trade-executor` package.
 
-* [Trading Strategy website](https://tradingstrategy.ai)
+![Architecture overview](docs/deployment-overview.drawio.svg)
 
-* [Blog](https://tradingstrategy.ai/blog)
+## Running tests
 
-* [Twitter](https://twitter.com/TradingProtocol)
+See [internal development documentation](https://tradingstrategy.ai/docs/programming/development.html). 
 
-* [Discord](https://tradingstrategy.ai/community#discord) 
+## Community
 
-* [Telegram channel](https://t.me/trading_protocol)
+- [Trading Strategy website](https://tradingstrategy.ai)
+- [Community Discord server](https://tradingstrategy.ai/community#discord)
+- [Blog](https://tradingstrategy.ai/blog)
+- [Twitter](https://twitter.com/TradingProtocol)
+- [Telegram channel](https://t.me/trading_protocol)
+- [Newsletter](https://tradingstrategy.ai/newsletter)
 
 ## License 
 
 - AGPL
+- [Contact for the commercial dual licensing](https://tradingstrategy.ai/about)
```

