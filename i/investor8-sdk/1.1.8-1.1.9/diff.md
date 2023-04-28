# Comparing `tmp/investor8-sdk-1.1.8.tar.gz` & `tmp/investor8-sdk-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investor8-sdk-1.1.8.tar", last modified: Mon Apr 11 12:06:10 2022, max compression
+gzip compressed data, was "investor8-sdk-1.1.9.tar", last modified: Tue Apr 12 14:29:22 2022, max compression
```

## Comparing `investor8-sdk-1.1.8.tar` & `investor8-sdk-1.1.9.tar`

### file list

```diff
@@ -1,460 +1,460 @@
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.764888 investor8-sdk-1.1.8/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      310 2022-04-11 12:06:10.764888 investor8-sdk-1.1.8/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    24117 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/README.md
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.080848 investor8-sdk-1.1.8/investor8-sdk/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6683 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/__init__.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.112849 investor8-sdk-1.1.8/investor8-sdk/api/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      657 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22037 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/earnings_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7158 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/email_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    36089 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/financials_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    53494 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/metrics_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    76825 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/news_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17866 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/price_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22457 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/screener_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4743 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/search_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    54811 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/stock_info_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11081 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/tags_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)   100956 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api/user_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    25068 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/api_client.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8232 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/configuration.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.268859 investor8-sdk-1.1.8/investor8-sdk/models/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5963 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/models/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6055 2021-11-17 08:35:43.000000 investor8-sdk-1.1.8/investor8-sdk/models/authentication_request.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4710 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/change_password_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8286 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/company_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8388 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/create_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/create_update_news.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10917 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/create_user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4406 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/create_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17887 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/current_momentum_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6642 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/daily_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11962 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/detailed_latest_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22102 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/earning_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/email_type.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6266 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/financial_report_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8957 2021-11-17 08:35:44.000000 investor8-sdk-1.1.8/investor8-sdk/models/financial_tag.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4315 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/financials_growth.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4469 2021-11-13 23:15:07.000000 investor8-sdk-1.1.8/investor8-sdk/models/get_user_plots_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3940 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/get_watchlists_by_user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5332 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/historical_financial_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10232 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/historical_return.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5642 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/historical_returns_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6638 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/historical_value_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2530 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/history_length.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4970 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/latest_financial_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4975 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/latest_financials_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4670 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/latest_financials_with_growth_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9514 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/latest_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3860 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/list_exchange_sector_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3696 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/login_user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/market_highlight.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10054 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/market_highlight_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2573 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/market_highlight_status.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5518 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6273 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/momentum_metric_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4515 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/monthly_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3805 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/monthly_returns.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4170 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/news_categories_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2516 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/news_source.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/period_metric_value.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3701 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/period_return.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10369 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/plot_detail_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9401 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3612 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/plot_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3956 2021-11-17 08:35:45.000000 investor8-sdk-1.1.8/investor8-sdk/models/previous_close_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2520 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/profile_name.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16040 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/recent_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2491 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/req_type.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3843 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/reset_password_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4455 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/result_field.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7235 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/return_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    20453 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/sa_attributes_prices.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5272 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/sa_sector_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3749 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/sector_returns_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5404 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/send_email_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11218 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/standardized_financial.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19697 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    12742 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_financial.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5160 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_financial_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7640 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    15887 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_info_master_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16447 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_ipo.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17047 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_news.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19789 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_news_details.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2562 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_news_status.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10948 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_popularity_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4335 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_popularity_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7156 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_price.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11115 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11172 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_rating_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19866 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/stock_summary_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/string_message_result.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8600 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/tag_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5855 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/tag_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17494 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/upcoming_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5570 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/update_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4929 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/update_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10305 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/user.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11161 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3883 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/validate_watchlist_name_request_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2021-11-17 08:35:46.000000 investor8-sdk-1.1.8/investor8-sdk/models/validate_watchlist_name_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5022 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/models/value_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3070 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/models/view_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5511 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/models/watchlist.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4947 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/models/watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    13024 2021-11-17 08:35:47.000000 investor8-sdk-1.1.8/investor8-sdk/rest.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.272859 investor8-sdk-1.1.8/investor8_sdk/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6915 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/investor8_sdk/__init__.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.280859 investor8-sdk-1.1.8/investor8_sdk/api/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      663 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/investor8_sdk/api/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21875 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/api/earnings_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7158 2022-01-02 07:37:24.000000 investor8-sdk-1.1.8/investor8_sdk/api/email_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    37142 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/api/financials_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    84567 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/api/metrics_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    55688 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/api/news_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21594 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/api/price_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    22295 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/api/screener_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4716 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/api/search_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10867 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/investor8_sdk/api/settings_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    60641 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/investor8_sdk/api/stock_info_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11000 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/investor8_sdk/api/tags_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    41760 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/investor8_sdk/api/user_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    25068 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/investor8_sdk/api_client.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8501 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/investor8_sdk/configuration.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.348863 investor8-sdk-1.1.8/investor8_sdk/models/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6189 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/investor8_sdk/models/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3684 2022-04-11 12:06:04.000000 investor8-sdk-1.1.8/investor8_sdk/models/active_company_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3861 2022-04-11 12:06:04.000000 investor8-sdk-1.1.8/investor8_sdk/models/add_to_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6927 2022-04-11 12:06:04.000000 investor8-sdk-1.1.8/investor8_sdk/models/authentication_request.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2543 2022-04-11 12:06:04.000000 investor8-sdk-1.1.8/investor8_sdk/models/authentication_source.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3992 2022-01-02 07:37:21.000000 investor8-sdk-1.1.8/investor8_sdk/models/authorize_account_request_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3398 2022-01-02 07:37:21.000000 investor8-sdk-1.1.8/investor8_sdk/models/authorize_account_response_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4982 2022-01-02 07:37:21.000000 investor8-sdk-1.1.8/investor8_sdk/models/change_password_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8286 2022-04-11 12:06:04.000000 investor8-sdk-1.1.8/investor8_sdk/models/company_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3755 2022-04-11 12:06:04.000000 investor8-sdk-1.1.8/investor8_sdk/models/create_auth_req_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9680 2022-04-11 12:06:04.000000 investor8-sdk-1.1.8/investor8_sdk/models/create_plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2022-01-02 07:37:21.000000 investor8-sdk-1.1.8/investor8_sdk/models/create_update_news.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12576 2022-01-02 07:37:21.000000 investor8-sdk-1.1.8/investor8_sdk/models/create_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11840 2022-01-02 07:37:21.000000 investor8-sdk-1.1.8/investor8_sdk/models/create_user_res_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4661 2022-04-11 12:06:04.000000 investor8-sdk-1.1.8/investor8_sdk/models/create_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4359 2022-04-11 12:06:04.000000 investor8-sdk-1.1.8/investor8_sdk/models/current_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17707 2022-04-11 12:06:04.000000 investor8-sdk-1.1.8/investor8_sdk/models/current_momentum_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6642 2022-04-11 12:06:04.000000 investor8-sdk-1.1.8/investor8_sdk/models/daily_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11962 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/detailed_latest_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    22102 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/earning_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2022-01-02 07:37:22.000000 investor8-sdk-1.1.8/investor8_sdk/models/email_type.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12479 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/financial_metric_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6266 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/financial_report_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12079 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/financial_tag.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4315 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/financials_growth.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3940 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/get_watchlists_by_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7999 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/historical_daily_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5332 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/historical_financial_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3975 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/historical_indicator_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10232 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/historical_return.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5642 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/historical_returns_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6638 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/historical_value_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2530 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/history_length.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5140 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/i8_terminal_check_version_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4153 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/i8_terminal_version.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4189 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/i8_terminal_version_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4970 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/latest_financial_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4975 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/latest_financials_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4670 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/latest_financials_with_growth_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9514 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/latest_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3860 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/list_exchange_sector_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7200 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/log_terminal_usage.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3867 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/login_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3942 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/login_with_code_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2022-01-02 07:37:22.000000 investor8-sdk-1.1.8/investor8_sdk/models/market_highlight.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10225 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/market_highlight_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2573 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/market_highlight_status.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6171 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/metadata_properties_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11975 2022-04-10 12:05:22.000000 investor8-sdk-1.1.8/investor8_sdk/models/metric_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5518 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/investor8_sdk/models/metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8808 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/metrics_metadata.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6273 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/momentum_metric_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4515 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/monthly_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3805 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/monthly_returns.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4170 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/news_categories_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2516 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/news_source.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/period_metric_value.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3701 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/period_return.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11050 2022-01-02 07:37:22.000000 investor8-sdk-1.1.8/investor8_sdk/models/plot_detail_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10058 2022-01-02 07:37:22.000000 investor8-sdk-1.1.8/investor8_sdk/models/plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3612 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/plot_response_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3956 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/previous_close_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2520 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/profile_name.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16040 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/recent_earning_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3882 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/remove_from_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3792 2022-01-02 07:37:23.000000 investor8-sdk-1.1.8/investor8_sdk/models/rename_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2504 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/req_type.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4019 2022-01-02 07:37:23.000000 investor8-sdk-1.1.8/investor8_sdk/models/reset_password_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4455 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/result_field.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7235 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/return_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    20453 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/sa_attributes_prices.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5272 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/sa_sector_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3749 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/sector_returns_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5585 2022-01-02 07:37:23.000000 investor8-sdk-1.1.8/investor8_sdk/models/send_email_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11218 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/standardized_financial.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19697 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_earning_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12742 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_financial.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5160 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_financial_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7640 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15887 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_info_master_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16447 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_ipo.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17047 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_news.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19789 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_news_details.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2562 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_news_status.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10948 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_popularity_details_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4335 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_popularity_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7156 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_price.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11115 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11172 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_rating_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19866 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/models/stock_summary_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2022-01-02 07:37:23.000000 investor8-sdk-1.1.8/investor8_sdk/models/string_message_result.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8600 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/models/tag_details_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5855 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/models/tag_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6930 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/models/trading_calendar_details_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17494 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/models/upcoming_earning_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5651 2022-01-02 07:37:23.000000 investor8-sdk-1.1.8/investor8_sdk/models/update_plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11673 2022-01-02 07:37:23.000000 investor8-sdk-1.1.8/investor8_sdk/models/user.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16668 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/models/user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4052 2022-01-02 07:37:23.000000 investor8-sdk-1.1.8/investor8_sdk/models/validate_watchlist_name_request_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2022-01-02 07:37:23.000000 investor8-sdk-1.1.8/investor8_sdk/models/validate_watchlist_name_response_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5022 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/models/value_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3156 2022-01-02 07:37:24.000000 investor8-sdk-1.1.8/investor8_sdk/models/view_plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5511 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/models/watchlist.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4947 2022-04-11 12:06:07.000000 investor8-sdk-1.1.8/investor8_sdk/models/watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    13024 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/investor8_sdk/rest.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.272859 investor8-sdk-1.1.8/investor8_sdk.egg-info/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      310 2022-04-11 12:06:09.000000 investor8-sdk-1.1.8/investor8_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17185 2022-04-11 12:06:09.000000 investor8-sdk-1.1.8/investor8_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        1 2022-04-11 12:06:09.000000 investor8-sdk-1.1.8/investor8_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       48 2022-04-11 12:06:09.000000 investor8-sdk-1.1.8/investor8_sdk.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       48 2022-04-11 12:06:09.000000 investor8-sdk-1.1.8/investor8_sdk.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       38 2022-04-11 12:06:10.764888 investor8-sdk-1.1.8/setup.cfg
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      995 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/setup.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.356864 investor8-sdk-1.1.8/swagger_client/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6783 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/__init__.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.388866 investor8-sdk-1.1.8/swagger_client/api/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      668 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    21759 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/earnings_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7123 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/email_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    35928 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/financials_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    53243 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/metrics_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    76448 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/news_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17777 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/price_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22350 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/screener_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4726 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/search_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    54542 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/stock_info_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11028 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/tags_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)   100424 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api/user_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    25072 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/api_client.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8233 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/configuration.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.540875 investor8-sdk-1.1.8/swagger_client/models/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6050 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/models/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6055 2021-11-09 17:29:55.000000 investor8-sdk-1.1.8/swagger_client/models/authentication_request.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4710 2021-11-09 17:29:55.000000 investor8-sdk-1.1.8/swagger_client/models/change_password_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8286 2021-11-09 17:29:55.000000 investor8-sdk-1.1.8/swagger_client/models/company_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8388 2021-11-09 17:29:55.000000 investor8-sdk-1.1.8/swagger_client/models/create_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2021-11-09 17:29:55.000000 investor8-sdk-1.1.8/swagger_client/models/create_update_news.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10917 2021-11-09 17:29:55.000000 investor8-sdk-1.1.8/swagger_client/models/create_user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4406 2021-11-09 17:29:55.000000 investor8-sdk-1.1.8/swagger_client/models/create_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17887 2021-11-09 17:29:55.000000 investor8-sdk-1.1.8/swagger_client/models/current_momentum_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6642 2021-11-09 17:29:55.000000 investor8-sdk-1.1.8/swagger_client/models/daily_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11962 2021-11-09 17:29:55.000000 investor8-sdk-1.1.8/swagger_client/models/detailed_latest_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22102 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/earning_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/email_type.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6266 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/financial_report_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7482 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/financial_tag.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4315 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/financials_growth.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4469 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/get_user_plots_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3940 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/get_watchlists_by_user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5332 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/historical_financial_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10232 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/historical_return.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5642 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/historical_returns_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6638 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/historical_value_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2530 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/history_length.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4970 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/latest_financial_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4975 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/latest_financials_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4670 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/latest_financials_with_growth_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9514 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/latest_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3860 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/list_exchange_sector_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3696 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/login_user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/market_highlight.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10054 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/market_highlight_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2573 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/market_highlight_status.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5518 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6273 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/momentum_metric_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4515 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/monthly_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3805 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/monthly_returns.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4170 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/news_categories_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2516 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/news_source.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/period_metric_value.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3701 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/period_return.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10057 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3612 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/plot_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3956 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/previous_close_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2520 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/profile_name.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16040 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/recent_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2491 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/req_type.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3843 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/reset_password_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4455 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/result_field.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7235 2021-11-09 17:29:56.000000 investor8-sdk-1.1.8/swagger_client/models/return_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    20453 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/sa_attributes_prices.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5272 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/sa_sector_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3749 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/sector_returns_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5404 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/send_email_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11218 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/standardized_financial.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19697 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    12742 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_financial.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5160 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_financial_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7640 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    15887 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_info_master_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16447 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_ipo.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17047 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_news.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19789 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_news_details.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2562 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_news_status.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10948 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_popularity_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4335 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_popularity_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7156 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_price.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11115 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11172 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_rating_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19866 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/stock_summary_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/string_message_result.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8600 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/tag_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5855 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/tag_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17494 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/upcoming_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5570 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/update_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4929 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/update_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10305 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/user.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10584 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3883 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/validate_watchlist_name_request_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/validate_watchlist_name_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5022 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/value_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3070 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/view_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5511 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/watchlist.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4947 2021-11-09 17:29:57.000000 investor8-sdk-1.1.8/swagger_client/models/watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    13024 2021-11-09 17:29:58.000000 investor8-sdk-1.1.8/swagger_client/rest.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:10.760887 investor8-sdk-1.1.8/test/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-11 12:06:08.000000 investor8-sdk-1.1.8/test/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-02-07 12:25:08.000000 investor8-sdk-1.1.8/test/test_active_company_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      959 2021-11-22 21:48:03.000000 investor8-sdk-1.1.8/test/test_add_to_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:00.000000 investor8-sdk-1.1.8/test/test_authentication_request.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-12-22 22:21:41.000000 investor8-sdk-1.1.8/test/test_authentication_source.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2021-12-14 09:16:29.000000 investor8-sdk-1.1.8/test/test_authorize_account_request_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1039 2021-12-14 09:16:29.000000 investor8-sdk-1.1.8/test/test_authorize_account_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:00.000000 investor8-sdk-1.1.8/test/test_change_password_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_company_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-12 18:39:44.000000 investor8-sdk-1.1.8/test/test_create_auth_req_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:03.000000 investor8-sdk-1.1.8/test/test_create_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_create_update_news.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_create_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-24 20:49:06.000000 investor8-sdk-1.1.8/test/test_create_user_res_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:40.000000 investor8-sdk-1.1.8/test/test_create_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-02-21 08:35:39.000000 investor8-sdk-1.1.8/test/test_current_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_current_momentum_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_daily_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_detailed_latest_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_earning_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1386 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_earnings_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_email_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_email_type.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/test/test_financial_metric_metadata_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_financial_report_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_financial_tag.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1900 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_financials_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_financials_growth.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      943 2021-10-29 23:03:04.000000 investor8-sdk-1.1.8/test/test_get_user_plots_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1001 2021-10-20 06:52:41.000000 investor8-sdk-1.1.8/test/test_get_watchlists_by_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-28 01:16:15.000000 investor8-sdk-1.1.8/test/test_historical_daily_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1027 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_historical_financial_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2022-01-04 11:42:54.000000 investor8-sdk-1.1.8/test/test_historical_indicator_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_historical_return.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_historical_returns_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      995 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_historical_value_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_history_length.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1025 2022-03-12 13:22:27.000000 investor8-sdk-1.1.8/test/test_i8_terminal_check_version_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-03-09 08:58:36.000000 investor8-sdk-1.1.8/test/test_i8_terminal_version.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      983 2022-03-09 08:58:36.000000 investor8-sdk-1.1.8/test/test_i8_terminal_version_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_latest_financial_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:01.000000 investor8-sdk-1.1.8/test/test_latest_financials_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1055 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_latest_financials_with_growth_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_latest_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_list_exchange_sector_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-04-10 12:05:22.000000 investor8-sdk-1.1.8/test/test_log_terminal_usage.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_login_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-13 18:18:13.000000 investor8-sdk-1.1.8/test/test_login_with_code_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      937 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_market_highlight.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_market_highlight_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_market_highlight_status.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2022-04-11 12:06:05.000000 investor8-sdk-1.1.8/test/test_metadata_properties_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2021-12-05 23:31:58.000000 investor8-sdk-1.1.8/test/test_metric_metadata_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      871 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2455 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_metrics_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2022-04-11 12:06:06.000000 investor8-sdk-1.1.8/test/test_metrics_metadata.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_momentum_metric_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_monthly_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_monthly_returns.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2988 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_news_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_news_categories_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_news_source.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_period_metric_value.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_period_return.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      849 2021-10-29 23:03:05.000000 investor8-sdk-1.1.8/test/test_plot.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-11-10 20:39:48.000000 investor8-sdk-1.1.8/test/test_plot_detail_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      875 2021-10-29 23:03:05.000000 investor8-sdk-1.1.8/test/test_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      941 2021-11-01 09:44:52.000000 investor8-sdk-1.1.8/test/test_plot_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_previous_close_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1267 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_price_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_profile_name.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_recent_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      999 2021-11-24 17:08:48.000000 investor8-sdk-1.1.8/test/test_remove_from_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-11-24 17:08:48.000000 investor8-sdk-1.1.8/test/test_rename_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_req_type.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_reset_password_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_result_field.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_return_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_sa_attributes_prices.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_sa_sector_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1374 2021-10-01 15:22:04.000000 investor8-sdk-1.1.8/test/test_screener_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      790 2021-10-01 15:22:04.000000 investor8-sdk-1.1.8/test/test_search_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_sector_returns_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_send_email_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      910 2022-03-09 08:58:38.000000 investor8-sdk-1.1.8/test/test_settings_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_standardized_financial.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_stock_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_stock_financial.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_stock_financial_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2416 2021-10-01 15:22:04.000000 investor8-sdk-1.1.8/test/test_stock_info_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_stock_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_stock_info_master_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:02.000000 investor8-sdk-1.1.8/test/test_stock_ipo.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_stock_news.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_stock_news_details.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_stock_news_status.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_stock_popularity_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_stock_popularity_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_stock_price.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-13 20:41:56.000000 investor8-sdk-1.1.8/test/test_stock_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_stock_rating_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_stock_summary_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_string_message_result.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_tag_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      899 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_tag_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1004 2021-10-01 15:22:04.000000 investor8-sdk-1.1.8/test/test_tags_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-01 22:19:51.000000 investor8-sdk-1.1.8/test/test_trading_calendar_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_upcoming_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:06.000000 investor8-sdk-1.1.8/test/test_update_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:42.000000 investor8-sdk-1.1.8/test/test_update_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      847 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_user.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2280 2021-10-01 15:22:04.000000 investor8-sdk-1.1.8/test/test_user_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1073 2021-10-31 21:17:37.000000 investor8-sdk-1.1.8/test/test_validate_watchlist_name_request_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1081 2021-10-31 21:17:37.000000 investor8-sdk-1.1.8/test/test_validate_watchlist_name_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.8/test/test_value_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      909 2021-10-29 23:03:06.000000 investor8-sdk-1.1.8/test/test_view_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-20 06:52:42.000000 investor8-sdk-1.1.8/test/test_watchlist.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-20 06:52:42.000000 investor8-sdk-1.1.8/test/test_watchlist_dto.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.580092 investor8-sdk-1.1.9/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      310 2022-04-12 14:29:22.580092 investor8-sdk-1.1.9/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    24117 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/README.md
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:21.976057 investor8-sdk-1.1.9/investor8-sdk/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6683 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/__init__.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.008058 investor8-sdk-1.1.9/investor8-sdk/api/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      657 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22037 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/earnings_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7158 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/email_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    36089 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/financials_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    53494 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/metrics_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    76825 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/news_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17866 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/price_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22457 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/screener_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4743 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/search_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    54811 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/stock_info_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11081 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/tags_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)   100956 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api/user_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    25068 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/api_client.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8232 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/configuration.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.160067 investor8-sdk-1.1.9/investor8-sdk/models/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5963 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/models/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6055 2021-11-17 08:35:43.000000 investor8-sdk-1.1.9/investor8-sdk/models/authentication_request.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4710 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/change_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8286 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/company_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8388 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/create_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/create_update_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10917 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/create_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4406 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/create_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17887 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/current_momentum_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6642 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/daily_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11962 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/detailed_latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22102 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/earning_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/email_type.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6266 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/financial_report_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8957 2021-11-17 08:35:44.000000 investor8-sdk-1.1.9/investor8-sdk/models/financial_tag.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4315 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/financials_growth.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4469 2021-11-13 23:15:07.000000 investor8-sdk-1.1.9/investor8-sdk/models/get_user_plots_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3940 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/get_watchlists_by_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5332 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/historical_financial_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10232 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/historical_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5642 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/historical_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6638 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/historical_value_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2530 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/history_length.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4970 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/latest_financial_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4975 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/latest_financials_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4670 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/latest_financials_with_growth_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9514 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3860 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/list_exchange_sector_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3696 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/login_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/market_highlight.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10054 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/market_highlight_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2573 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/market_highlight_status.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5518 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6273 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/momentum_metric_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4515 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/monthly_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3805 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/monthly_returns.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4170 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/news_categories_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2516 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/news_source.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/period_metric_value.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3701 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/period_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10369 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/plot_detail_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9401 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3612 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/plot_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3956 2021-11-17 08:35:45.000000 investor8-sdk-1.1.9/investor8-sdk/models/previous_close_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2520 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/profile_name.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16040 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/recent_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2491 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/req_type.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3843 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/reset_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4455 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/result_field.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7235 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/return_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    20453 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/sa_attributes_prices.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5272 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/sa_sector_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3749 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/sector_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5404 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/send_email_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11218 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/standardized_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19697 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    12742 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5160 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_financial_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7640 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    15887 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_info_master_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16447 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_ipo.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17047 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19789 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_news_details.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2562 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_news_status.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10948 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_popularity_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4335 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_popularity_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7156 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_price.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11115 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11172 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_rating_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19866 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/stock_summary_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/string_message_result.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8600 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/tag_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5855 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/tag_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17494 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/upcoming_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5570 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/update_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4929 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/update_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10305 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/user.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11161 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3883 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/validate_watchlist_name_request_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2021-11-17 08:35:46.000000 investor8-sdk-1.1.9/investor8-sdk/models/validate_watchlist_name_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5022 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/models/value_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3070 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/models/view_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5511 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/models/watchlist.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4947 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/models/watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    13024 2021-11-17 08:35:47.000000 investor8-sdk-1.1.9/investor8-sdk/rest.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.164068 investor8-sdk-1.1.9/investor8_sdk/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6915 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/__init__.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.172068 investor8-sdk-1.1.9/investor8_sdk/api/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      663 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21875 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/api/earnings_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7158 2022-01-02 07:37:24.000000 investor8-sdk-1.1.9/investor8_sdk/api/email_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    37142 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/api/financials_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    84567 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/api/metrics_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    55688 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/api/news_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21594 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/api/price_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    22295 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/screener_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4716 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/search_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10867 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/settings_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    60641 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/stock_info_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11000 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/tags_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    41760 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api/user_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    25068 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/api_client.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8501 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/configuration.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.236072 investor8-sdk-1.1.9/investor8_sdk/models/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6189 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/models/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3684 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/active_company_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3861 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/add_to_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6927 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/authentication_request.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2543 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/authentication_source.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3992 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/authorize_account_request_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3398 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/authorize_account_response_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4982 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/change_password_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8286 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/company_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3755 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_auth_req_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9680 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_update_news.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12576 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11840 2022-01-02 07:37:21.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_user_res_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4661 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/create_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4359 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/current_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17707 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/current_momentum_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6642 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/daily_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11962 2022-04-12 14:29:16.000000 investor8-sdk-1.1.9/investor8_sdk/models/detailed_latest_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    22102 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/earning_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2022-01-02 07:37:22.000000 investor8-sdk-1.1.9/investor8_sdk/models/email_type.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12479 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/financial_metric_metadata_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6266 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/financial_report_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12079 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/financial_tag.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4315 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/financials_growth.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3940 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/get_watchlists_by_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7999 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_daily_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5332 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_financial_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3975 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_indicator_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10232 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_return.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5642 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_returns_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6638 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/historical_value_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2530 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/history_length.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5140 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_check_version_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4153 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_version.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4189 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_version_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4970 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/latest_financial_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4975 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/latest_financials_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4670 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/latest_financials_with_growth_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9514 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/latest_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3860 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/list_exchange_sector_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7200 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/log_terminal_usage.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3867 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/login_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3942 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/login_with_code_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2022-01-02 07:37:22.000000 investor8-sdk-1.1.9/investor8_sdk/models/market_highlight.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10225 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/market_highlight_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2573 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/market_highlight_status.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6171 2022-04-12 14:29:17.000000 investor8-sdk-1.1.9/investor8_sdk/models/metadata_properties_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11975 2022-04-10 12:05:22.000000 investor8-sdk-1.1.9/investor8_sdk/models/metric_metadata_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5518 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8808 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/metrics_metadata.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6273 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/momentum_metric_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4515 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/monthly_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3805 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/monthly_returns.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4170 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/news_categories_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2516 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/news_source.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/period_metric_value.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3701 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/period_return.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11050 2022-01-02 07:37:22.000000 investor8-sdk-1.1.9/investor8_sdk/models/plot_detail_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10058 2022-01-02 07:37:22.000000 investor8-sdk-1.1.9/investor8_sdk/models/plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3612 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/plot_response_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3956 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/previous_close_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2520 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/profile_name.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16040 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/recent_earning_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3882 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/remove_from_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3792 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/rename_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2504 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/req_type.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4019 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/reset_password_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4455 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/result_field.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7235 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/return_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    20453 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/sa_attributes_prices.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5272 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/sa_sector_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3749 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/sector_returns_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5585 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/send_email_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11218 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/standardized_financial.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19697 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_earning_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12742 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_financial.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5160 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_financial_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7640 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15887 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_info_master_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16447 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_ipo.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17047 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_news.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19789 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_news_details.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2562 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_news_status.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10948 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_popularity_details_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4335 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_popularity_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7156 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_price.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11115 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11172 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_rating_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19866 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/stock_summary_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/string_message_result.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8600 2022-04-12 14:29:18.000000 investor8-sdk-1.1.9/investor8_sdk/models/tag_details_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5855 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/tag_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6930 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/trading_calendar_details_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17494 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/upcoming_earning_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5651 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/update_plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11673 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/user.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17586 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4052 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/validate_watchlist_name_request_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2022-01-02 07:37:23.000000 investor8-sdk-1.1.9/investor8_sdk/models/validate_watchlist_name_response_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5022 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/value_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3156 2022-01-02 07:37:24.000000 investor8-sdk-1.1.9/investor8_sdk/models/view_plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5511 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/watchlist.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4947 2022-04-12 14:29:19.000000 investor8-sdk-1.1.9/investor8_sdk/models/watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    13024 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/investor8_sdk/rest.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.164068 investor8-sdk-1.1.9/investor8_sdk.egg-info/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      310 2022-04-12 14:29:21.000000 investor8-sdk-1.1.9/investor8_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17185 2022-04-12 14:29:21.000000 investor8-sdk-1.1.9/investor8_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        1 2022-04-12 14:29:21.000000 investor8-sdk-1.1.9/investor8_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       48 2022-04-12 14:29:21.000000 investor8-sdk-1.1.9/investor8_sdk.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       48 2022-04-12 14:29:21.000000 investor8-sdk-1.1.9/investor8_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       38 2022-04-12 14:29:22.580092 investor8-sdk-1.1.9/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      995 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/setup.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.240072 investor8-sdk-1.1.9/swagger_client/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6783 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/__init__.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.268074 investor8-sdk-1.1.9/swagger_client/api/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      668 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    21759 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/earnings_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7123 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/email_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    35928 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/financials_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    53243 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/metrics_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    76448 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/news_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17777 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/price_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22350 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/screener_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4726 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/search_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    54542 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/stock_info_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11028 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/tags_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)   100424 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api/user_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    25072 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/api_client.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8233 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/configuration.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.412082 investor8-sdk-1.1.9/swagger_client/models/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6050 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/models/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6055 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/authentication_request.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4710 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/change_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8286 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/company_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8388 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/create_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/create_update_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10917 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/create_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4406 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/create_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17887 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/current_momentum_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6642 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/daily_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11962 2021-11-09 17:29:55.000000 investor8-sdk-1.1.9/swagger_client/models/detailed_latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    22102 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/earning_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/email_type.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6266 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/financial_report_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7482 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/financial_tag.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4315 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/financials_growth.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4469 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/get_user_plots_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3940 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/get_watchlists_by_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5332 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/historical_financial_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10232 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/historical_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5642 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/historical_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6638 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/historical_value_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2530 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/history_length.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4970 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/latest_financial_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4975 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/latest_financials_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4670 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/latest_financials_with_growth_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9514 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3860 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/list_exchange_sector_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3696 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/login_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/market_highlight.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10054 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/market_highlight_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2573 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/market_highlight_status.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5518 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     6273 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/momentum_metric_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4515 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/monthly_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3805 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/monthly_returns.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4170 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/news_categories_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2516 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/news_source.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/period_metric_value.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3701 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/period_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10057 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3612 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/plot_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3956 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/previous_close_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2520 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/profile_name.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16040 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/recent_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2491 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/req_type.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3843 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/reset_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4455 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/result_field.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7235 2021-11-09 17:29:56.000000 investor8-sdk-1.1.9/swagger_client/models/return_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    20453 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/sa_attributes_prices.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5272 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/sa_sector_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3749 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/sector_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5404 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/send_email_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11218 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/standardized_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19697 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    12742 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5160 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_financial_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7640 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    15887 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_info_master_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    16447 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_ipo.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17047 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19789 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_news_details.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2562 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_news_status.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10948 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_popularity_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4335 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_popularity_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     7156 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_price.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11115 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11172 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_rating_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    19866 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/stock_summary_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/string_message_result.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     8600 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/tag_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5855 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/tag_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    17494 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/upcoming_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5570 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/update_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4929 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/update_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10305 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/user.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    10584 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3883 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/validate_watchlist_name_request_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/validate_watchlist_name_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5022 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/value_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     3070 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/view_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     5511 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/watchlist.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     4947 2021-11-09 17:29:57.000000 investor8-sdk-1.1.9/swagger_client/models/watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    13024 2021-11-09 17:29:58.000000 investor8-sdk-1.1.9/swagger_client/rest.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:22.576092 investor8-sdk-1.1.9/test/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-04-12 14:29:20.000000 investor8-sdk-1.1.9/test/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-02-07 12:25:08.000000 investor8-sdk-1.1.9/test/test_active_company_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      959 2021-11-22 21:48:03.000000 investor8-sdk-1.1.9/test/test_add_to_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:00.000000 investor8-sdk-1.1.9/test/test_authentication_request.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-12-22 22:21:41.000000 investor8-sdk-1.1.9/test/test_authentication_source.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2021-12-14 09:16:29.000000 investor8-sdk-1.1.9/test/test_authorize_account_request_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1039 2021-12-14 09:16:29.000000 investor8-sdk-1.1.9/test/test_authorize_account_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:00.000000 investor8-sdk-1.1.9/test/test_change_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_company_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-12 18:39:44.000000 investor8-sdk-1.1.9/test/test_create_auth_req_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:03.000000 investor8-sdk-1.1.9/test/test_create_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_create_update_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_create_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-24 20:49:06.000000 investor8-sdk-1.1.9/test/test_create_user_res_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:40.000000 investor8-sdk-1.1.9/test/test_create_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-02-21 08:35:39.000000 investor8-sdk-1.1.9/test/test_current_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_current_momentum_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_daily_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_detailed_latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_earning_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1386 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_earnings_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_email_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_email_type.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2022-04-11 12:06:05.000000 investor8-sdk-1.1.9/test/test_financial_metric_metadata_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_financial_report_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_financial_tag.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1900 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_financials_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_financials_growth.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      943 2021-10-29 23:03:04.000000 investor8-sdk-1.1.9/test/test_get_user_plots_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1001 2021-10-20 06:52:41.000000 investor8-sdk-1.1.9/test/test_get_watchlists_by_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-28 01:16:15.000000 investor8-sdk-1.1.9/test/test_historical_daily_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1027 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_historical_financial_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2022-01-04 11:42:54.000000 investor8-sdk-1.1.9/test/test_historical_indicator_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_historical_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_historical_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      995 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_historical_value_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_history_length.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1025 2022-03-12 13:22:27.000000 investor8-sdk-1.1.9/test/test_i8_terminal_check_version_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-03-09 08:58:36.000000 investor8-sdk-1.1.9/test/test_i8_terminal_version.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      983 2022-03-09 08:58:36.000000 investor8-sdk-1.1.9/test/test_i8_terminal_version_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_latest_financial_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:01.000000 investor8-sdk-1.1.9/test/test_latest_financials_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1055 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_latest_financials_with_growth_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_list_exchange_sector_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-04-10 12:05:22.000000 investor8-sdk-1.1.9/test/test_log_terminal_usage.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_login_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-13 18:18:13.000000 investor8-sdk-1.1.9/test/test_login_with_code_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      937 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_market_highlight.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_market_highlight_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_market_highlight_status.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2022-04-11 12:06:05.000000 investor8-sdk-1.1.9/test/test_metadata_properties_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2021-12-05 23:31:58.000000 investor8-sdk-1.1.9/test/test_metric_metadata_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      871 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2455 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_metrics_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2022-04-11 12:06:06.000000 investor8-sdk-1.1.9/test/test_metrics_metadata.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_momentum_metric_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_monthly_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_monthly_returns.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2988 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_news_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_news_categories_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_news_source.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_period_metric_value.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_period_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      849 2021-10-29 23:03:05.000000 investor8-sdk-1.1.9/test/test_plot.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-11-10 20:39:48.000000 investor8-sdk-1.1.9/test/test_plot_detail_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      875 2021-10-29 23:03:05.000000 investor8-sdk-1.1.9/test/test_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      941 2021-11-01 09:44:52.000000 investor8-sdk-1.1.9/test/test_plot_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_previous_close_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1267 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_price_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_profile_name.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_recent_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      999 2021-11-24 17:08:48.000000 investor8-sdk-1.1.9/test/test_remove_from_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-11-24 17:08:48.000000 investor8-sdk-1.1.9/test/test_rename_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_req_type.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_reset_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_result_field.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_return_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_sa_attributes_prices.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_sa_sector_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1374 2021-10-01 15:22:04.000000 investor8-sdk-1.1.9/test/test_screener_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      790 2021-10-01 15:22:04.000000 investor8-sdk-1.1.9/test/test_search_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_sector_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_send_email_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      910 2022-03-09 08:58:38.000000 investor8-sdk-1.1.9/test/test_settings_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_standardized_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_financial_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2416 2021-10-01 15:22:04.000000 investor8-sdk-1.1.9/test/test_stock_info_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_info_master_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:02.000000 investor8-sdk-1.1.9/test/test_stock_ipo.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_news_details.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_news_status.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_popularity_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_popularity_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_price.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-13 20:41:56.000000 investor8-sdk-1.1.9/test/test_stock_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_rating_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_stock_summary_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_string_message_result.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_tag_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      899 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_tag_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1004 2021-10-01 15:22:04.000000 investor8-sdk-1.1.9/test/test_tags_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-01 22:19:51.000000 investor8-sdk-1.1.9/test/test_trading_calendar_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_upcoming_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:06.000000 investor8-sdk-1.1.9/test/test_update_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:42.000000 investor8-sdk-1.1.9/test/test_update_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      847 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_user.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2280 2021-10-01 15:22:04.000000 investor8-sdk-1.1.9/test/test_user_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1073 2021-10-31 21:17:37.000000 investor8-sdk-1.1.9/test/test_validate_watchlist_name_request_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1081 2021-10-31 21:17:37.000000 investor8-sdk-1.1.9/test/test_validate_watchlist_name_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.9/test/test_value_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      909 2021-10-29 23:03:06.000000 investor8-sdk-1.1.9/test/test_view_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-20 06:52:42.000000 investor8-sdk-1.1.9/test/test_watchlist.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-20 06:52:42.000000 investor8-sdk-1.1.9/test/test_watchlist_dto.py
```

### Comparing `investor8-sdk-1.1.8/README.md` & `investor8-sdk-1.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # investor8-sdk
 No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.1
-- Package version: 1.1.8
+- Package version: 1.1.9
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `investor8-sdk-1.1.8/investor8-sdk/__init__.py` & `investor8-sdk-1.1.9/investor8-sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/__init__.py` & `investor8-sdk-1.1.9/investor8-sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/earnings_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/earnings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/email_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/email_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/financials_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/financials_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/metrics_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/news_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/news_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/price_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/price_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/screener_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/screener_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/search_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/search_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/stock_info_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/stock_info_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/tags_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api/user_api.py` & `investor8-sdk-1.1.9/investor8-sdk/api/user_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/api_client.py` & `investor8-sdk-1.1.9/investor8-sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/configuration.py` & `investor8-sdk-1.1.9/investor8-sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/__init__.py` & `investor8-sdk-1.1.9/investor8-sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/authentication_request.py` & `investor8-sdk-1.1.9/investor8-sdk/models/authentication_request.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/change_password_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/change_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/company_info_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/company_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/create_plot_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/create_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/create_update_news.py` & `investor8-sdk-1.1.9/investor8-sdk/models/create_update_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/create_user_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/create_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/create_watchlist_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/create_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/current_momentum_metrics_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/current_momentum_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/daily_metrics_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/detailed_latest_price_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/detailed_latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/earning_metrics_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/earning_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/email_type.py` & `investor8-sdk-1.1.9/investor8-sdk/models/email_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/financial_report_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/financial_report_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/financial_tag.py` & `investor8-sdk-1.1.9/investor8-sdk/models/financial_tag.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/financials_growth.py` & `investor8-sdk-1.1.9/investor8-sdk/models/financials_growth.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/get_user_plots_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/get_user_plots_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/get_watchlists_by_user_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/get_watchlists_by_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/historical_financial_metrics.py` & `investor8-sdk-1.1.9/investor8-sdk/models/historical_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/historical_return.py` & `investor8-sdk-1.1.9/investor8-sdk/models/historical_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/historical_returns_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/historical_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/historical_value_metrics.py` & `investor8-sdk-1.1.9/investor8-sdk/models/historical_value_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/history_length.py` & `investor8-sdk-1.1.9/investor8-sdk/models/history_length.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/latest_financial_metrics_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/latest_financial_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/latest_financials_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/latest_financials_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/latest_financials_with_growth_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/latest_financials_with_growth_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/latest_price_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/list_exchange_sector_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/list_exchange_sector_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/login_user_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/login_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/market_highlight.py` & `investor8-sdk-1.1.9/investor8-sdk/models/market_highlight.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/market_highlight_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/market_highlight_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/market_highlight_status.py` & `investor8-sdk-1.1.9/investor8-sdk/models/market_highlight_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/metrics.py` & `investor8-sdk-1.1.9/investor8-sdk/models/metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/momentum_metric_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/momentum_metric_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/monthly_metrics.py` & `investor8-sdk-1.1.9/investor8-sdk/models/monthly_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/monthly_returns.py` & `investor8-sdk-1.1.9/investor8-sdk/models/monthly_returns.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/news_categories_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/news_categories_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/news_source.py` & `investor8-sdk-1.1.9/investor8-sdk/models/news_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/period_metric_value.py` & `investor8-sdk-1.1.9/investor8-sdk/models/period_metric_value.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/period_return.py` & `investor8-sdk-1.1.9/investor8-sdk/models/period_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/plot_detail_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/plot_detail_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/plot_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/plot_response_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/plot_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/previous_close_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/previous_close_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/profile_name.py` & `investor8-sdk-1.1.9/investor8-sdk/models/profile_name.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/recent_earning_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/recent_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/req_type.py` & `investor8-sdk-1.1.9/investor8-sdk/models/req_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/reset_password_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/reset_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/result_field.py` & `investor8-sdk-1.1.9/investor8-sdk/models/result_field.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/return_metrics.py` & `investor8-sdk-1.1.9/investor8-sdk/models/return_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/sa_attributes_prices.py` & `investor8-sdk-1.1.9/investor8-sdk/models/sa_attributes_prices.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/sa_sector_price_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/sa_sector_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/sector_returns_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/sector_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/send_email_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/send_email_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/standardized_financial.py` & `investor8-sdk-1.1.9/investor8-sdk/models/standardized_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_earning_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_financial.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_financial_metrics.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_info_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_info_master_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_info_master_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_ipo.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_ipo.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_news.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_news_details.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_news_details.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_news_status.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_news_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_popularity_details_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_popularity_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_popularity_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_popularity_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_price.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_price.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_price_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_rating_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_rating_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/stock_summary_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/stock_summary_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/string_message_result.py` & `investor8-sdk-1.1.9/investor8-sdk/models/string_message_result.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/tag_details_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/tag_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/tag_info_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/tag_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/upcoming_earning_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/upcoming_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/update_plot_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/update_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/update_watchlist_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/update_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/user.py` & `investor8-sdk-1.1.9/investor8-sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/user_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/validate_watchlist_name_request_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/validate_watchlist_name_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/validate_watchlist_name_response_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/validate_watchlist_name_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/value_metrics_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/value_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/view_plot_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/view_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/watchlist.py` & `investor8-sdk-1.1.9/investor8-sdk/models/watchlist.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/models/watchlist_dto.py` & `investor8-sdk-1.1.9/investor8-sdk/models/watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8-sdk/rest.py` & `investor8-sdk-1.1.9/investor8-sdk/rest.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/__init__.py` & `investor8-sdk-1.1.9/investor8_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/__init__.py` & `investor8-sdk-1.1.9/investor8_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/earnings_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/earnings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/email_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/email_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/financials_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/financials_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/metrics_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/news_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/news_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/price_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/price_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/screener_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/screener_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/search_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/search_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/settings_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/settings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/stock_info_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/stock_info_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/tags_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api/user_api.py` & `investor8-sdk-1.1.9/investor8_sdk/api/user_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/api_client.py` & `investor8-sdk-1.1.9/investor8_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.1.8/python'
+        self.user_agent = 'Swagger-Codegen/1.1.9/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `investor8-sdk-1.1.8/investor8_sdk/configuration.py` & `investor8-sdk-1.1.9/investor8_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,9 +250,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.1\n"\
-               "SDK Package Version: 1.1.8".\
+               "SDK Package Version: 1.1.9".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/__init__.py` & `investor8-sdk-1.1.9/investor8_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/active_company_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/active_company_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/add_to_watchlist_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/add_to_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/authentication_request.py` & `investor8-sdk-1.1.9/investor8_sdk/models/authentication_request.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/authentication_source.py` & `investor8-sdk-1.1.9/investor8_sdk/models/authentication_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/authorize_account_request_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/authorize_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/authorize_account_response_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/authorize_account_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/change_password_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/change_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/company_info_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/company_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/create_auth_req_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/create_auth_req_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/create_plot_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/create_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/create_update_news.py` & `investor8-sdk-1.1.9/investor8_sdk/models/create_update_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/create_user_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/create_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/create_user_res_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/create_user_res_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/create_watchlist_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/create_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/current_metrics_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/current_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/current_momentum_metrics_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/current_momentum_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/daily_metrics_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/detailed_latest_price_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/detailed_latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/earning_metrics_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/earning_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/email_type.py` & `investor8-sdk-1.1.9/investor8_sdk/models/email_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/financial_metric_metadata_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/financial_metric_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/financial_report_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/financial_report_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/financial_tag.py` & `investor8-sdk-1.1.9/investor8_sdk/models/financial_tag.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/financials_growth.py` & `investor8-sdk-1.1.9/investor8_sdk/models/financials_growth.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/get_watchlists_by_user_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/get_watchlists_by_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/historical_daily_metrics_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/historical_daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/historical_financial_metrics.py` & `investor8-sdk-1.1.9/investor8_sdk/models/historical_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/historical_indicator_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/historical_indicator_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/historical_return.py` & `investor8-sdk-1.1.9/investor8_sdk/models/historical_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/historical_returns_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/historical_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/historical_value_metrics.py` & `investor8-sdk-1.1.9/investor8_sdk/models/historical_value_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/history_length.py` & `investor8-sdk-1.1.9/investor8_sdk/models/history_length.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/i8_terminal_check_version_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_check_version_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/i8_terminal_version.py` & `investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_version.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/i8_terminal_version_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/i8_terminal_version_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/latest_financial_metrics_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/latest_financial_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/latest_financials_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/latest_financials_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/latest_financials_with_growth_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/latest_financials_with_growth_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/latest_price_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/list_exchange_sector_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/list_exchange_sector_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/log_terminal_usage.py` & `investor8-sdk-1.1.9/investor8_sdk/models/log_terminal_usage.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/login_user_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/login_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/login_with_code_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/login_with_code_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/market_highlight.py` & `investor8-sdk-1.1.9/investor8_sdk/models/market_highlight.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/market_highlight_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/market_highlight_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/market_highlight_status.py` & `investor8-sdk-1.1.9/investor8_sdk/models/market_highlight_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/metadata_properties_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/metadata_properties_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/metric_metadata_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/metric_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/metrics.py` & `investor8-sdk-1.1.9/investor8_sdk/models/metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/metrics_metadata.py` & `investor8-sdk-1.1.9/investor8_sdk/models/metrics_metadata.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/momentum_metric_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/momentum_metric_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/monthly_metrics.py` & `investor8-sdk-1.1.9/investor8_sdk/models/monthly_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/monthly_returns.py` & `investor8-sdk-1.1.9/investor8_sdk/models/monthly_returns.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/news_categories_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/news_categories_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/news_source.py` & `investor8-sdk-1.1.9/investor8_sdk/models/news_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/period_metric_value.py` & `investor8-sdk-1.1.9/investor8_sdk/models/period_metric_value.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/period_return.py` & `investor8-sdk-1.1.9/investor8_sdk/models/period_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/plot_detail_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/plot_detail_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/plot_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/plot_response_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/plot_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/previous_close_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/previous_close_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/profile_name.py` & `investor8-sdk-1.1.9/investor8_sdk/models/profile_name.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/recent_earning_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/recent_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/remove_from_watchlist_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/remove_from_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/rename_watchlist_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/rename_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/req_type.py` & `investor8-sdk-1.1.9/investor8_sdk/models/req_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/reset_password_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/reset_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/result_field.py` & `investor8-sdk-1.1.9/investor8_sdk/models/result_field.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/return_metrics.py` & `investor8-sdk-1.1.9/investor8_sdk/models/return_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/sa_attributes_prices.py` & `investor8-sdk-1.1.9/investor8_sdk/models/sa_attributes_prices.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/sa_sector_price_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/sa_sector_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/sector_returns_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/sector_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/send_email_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/send_email_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/standardized_financial.py` & `investor8-sdk-1.1.9/investor8_sdk/models/standardized_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_earning_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_financial.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_financial_metrics.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_info_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_info_master_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_info_master_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_ipo.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_ipo.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_news.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_news_details.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_news_details.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_news_status.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_news_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_popularity_details_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_popularity_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_popularity_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_popularity_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_price.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_price.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_price_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_rating_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_rating_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/stock_summary_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/stock_summary_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/string_message_result.py` & `investor8-sdk-1.1.9/investor8_sdk/models/string_message_result.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/tag_details_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/tag_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/tag_info_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/tag_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/trading_calendar_details_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/trading_calendar_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/upcoming_earning_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/upcoming_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/update_plot_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/update_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/user.py` & `investor8-sdk-1.1.9/investor8_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/user_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/user_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,16 @@
         'token': 'str',
         'premium_start_date': 'datetime',
         'charging_start_date': 'datetime',
         'charging_next_date': 'datetime',
         'cancel_date': 'datetime',
         'auth_source': 'AuthenticationSource',
         'subscription_id': 'str',
-        'referer': 'str'
+        'referer': 'str',
+        'allow_terminal_logging': 'bool'
     }
 
     attribute_map = {
         'user_id': 'UserId',
         'first_name': 'FirstName',
         'last_name': 'LastName',
         'email': 'Email',
@@ -66,18 +67,19 @@
         'token': 'Token',
         'premium_start_date': 'PremiumStartDate',
         'charging_start_date': 'ChargingStartDate',
         'charging_next_date': 'ChargingNextDate',
         'cancel_date': 'CancelDate',
         'auth_source': 'AuthSource',
         'subscription_id': 'SubscriptionId',
-        'referer': 'Referer'
+        'referer': 'Referer',
+        'allow_terminal_logging': 'AllowTerminalLogging'
     }
 
-    def __init__(self, user_id=None, first_name=None, last_name=None, email=None, roles=None, opt_for_newsletter=None, country=None, email_confirmed=None, created_time=None, last_modified=None, profile_name=None, api_key=None, token=None, premium_start_date=None, charging_start_date=None, charging_next_date=None, cancel_date=None, auth_source=None, subscription_id=None, referer=None):  # noqa: E501
+    def __init__(self, user_id=None, first_name=None, last_name=None, email=None, roles=None, opt_for_newsletter=None, country=None, email_confirmed=None, created_time=None, last_modified=None, profile_name=None, api_key=None, token=None, premium_start_date=None, charging_start_date=None, charging_next_date=None, cancel_date=None, auth_source=None, subscription_id=None, referer=None, allow_terminal_logging=None):  # noqa: E501
         """UserDto - a model defined in Swagger"""  # noqa: E501
         self._user_id = None
         self._first_name = None
         self._last_name = None
         self._email = None
         self._roles = None
         self._opt_for_newsletter = None
@@ -91,14 +93,15 @@
         self._premium_start_date = None
         self._charging_start_date = None
         self._charging_next_date = None
         self._cancel_date = None
         self._auth_source = None
         self._subscription_id = None
         self._referer = None
+        self._allow_terminal_logging = None
         self.discriminator = None
         self.user_id = user_id
         if first_name is not None:
             self.first_name = first_name
         if last_name is not None:
             self.last_name = last_name
         if email is not None:
@@ -131,14 +134,16 @@
             self.cancel_date = cancel_date
         if auth_source is not None:
             self.auth_source = auth_source
         if subscription_id is not None:
             self.subscription_id = subscription_id
         if referer is not None:
             self.referer = referer
+        if allow_terminal_logging is not None:
+            self.allow_terminal_logging = allow_terminal_logging
 
     @property
     def user_id(self):
         """Gets the user_id of this UserDto.  # noqa: E501
 
 
         :return: The user_id of this UserDto.  # noqa: E501
@@ -554,14 +559,35 @@
 
         :param referer: The referer of this UserDto.  # noqa: E501
         :type: str
         """
 
         self._referer = referer
 
+    @property
+    def allow_terminal_logging(self):
+        """Gets the allow_terminal_logging of this UserDto.  # noqa: E501
+
+
+        :return: The allow_terminal_logging of this UserDto.  # noqa: E501
+        :rtype: bool
+        """
+        return self._allow_terminal_logging
+
+    @allow_terminal_logging.setter
+    def allow_terminal_logging(self, allow_terminal_logging):
+        """Sets the allow_terminal_logging of this UserDto.
+
+
+        :param allow_terminal_logging: The allow_terminal_logging of this UserDto.  # noqa: E501
+        :type: bool
+        """
+
+        self._allow_terminal_logging = allow_terminal_logging
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/validate_watchlist_name_request_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/validate_watchlist_name_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/validate_watchlist_name_response_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/validate_watchlist_name_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/value_metrics_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/value_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/view_plot_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/view_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/watchlist.py` & `investor8-sdk-1.1.9/investor8_sdk/models/watchlist.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/models/watchlist_dto.py` & `investor8-sdk-1.1.9/investor8_sdk/models/watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk/rest.py` & `investor8-sdk-1.1.9/investor8_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/investor8_sdk.egg-info/SOURCES.txt` & `investor8-sdk-1.1.9/investor8_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/setup.py` & `investor8-sdk-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "investor8-sdk"
-VERSION = "1.1.8"
+VERSION = "1.1.9"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `investor8-sdk-1.1.8/swagger_client/__init__.py` & `investor8-sdk-1.1.9/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/__init__.py` & `investor8-sdk-1.1.9/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/earnings_api.py` & `investor8-sdk-1.1.9/swagger_client/api/earnings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/email_api.py` & `investor8-sdk-1.1.9/swagger_client/api/email_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/financials_api.py` & `investor8-sdk-1.1.9/swagger_client/api/financials_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/metrics_api.py` & `investor8-sdk-1.1.9/swagger_client/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/news_api.py` & `investor8-sdk-1.1.9/swagger_client/api/news_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/price_api.py` & `investor8-sdk-1.1.9/swagger_client/api/price_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/screener_api.py` & `investor8-sdk-1.1.9/swagger_client/api/screener_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/search_api.py` & `investor8-sdk-1.1.9/swagger_client/api/search_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/stock_info_api.py` & `investor8-sdk-1.1.9/swagger_client/api/stock_info_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/tags_api.py` & `investor8-sdk-1.1.9/swagger_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api/user_api.py` & `investor8-sdk-1.1.9/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/api_client.py` & `investor8-sdk-1.1.9/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/configuration.py` & `investor8-sdk-1.1.9/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/__init__.py` & `investor8-sdk-1.1.9/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/authentication_request.py` & `investor8-sdk-1.1.9/swagger_client/models/authentication_request.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/change_password_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/change_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/company_info_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/company_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/create_plot_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/create_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/create_update_news.py` & `investor8-sdk-1.1.9/swagger_client/models/create_update_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/create_user_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/create_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/create_watchlist_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/create_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/current_momentum_metrics_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/current_momentum_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/daily_metrics_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/detailed_latest_price_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/detailed_latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/earning_metrics_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/earning_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/email_type.py` & `investor8-sdk-1.1.9/swagger_client/models/email_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/financial_report_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/financial_report_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/financial_tag.py` & `investor8-sdk-1.1.9/swagger_client/models/financial_tag.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/financials_growth.py` & `investor8-sdk-1.1.9/swagger_client/models/financials_growth.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/get_user_plots_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/get_user_plots_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/get_watchlists_by_user_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/get_watchlists_by_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/historical_financial_metrics.py` & `investor8-sdk-1.1.9/swagger_client/models/historical_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/historical_return.py` & `investor8-sdk-1.1.9/swagger_client/models/historical_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/historical_returns_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/historical_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/historical_value_metrics.py` & `investor8-sdk-1.1.9/swagger_client/models/historical_value_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/history_length.py` & `investor8-sdk-1.1.9/swagger_client/models/history_length.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/latest_financial_metrics_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/latest_financial_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/latest_financials_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/latest_financials_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/latest_financials_with_growth_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/latest_financials_with_growth_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/latest_price_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/list_exchange_sector_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/list_exchange_sector_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/login_user_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/login_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/market_highlight.py` & `investor8-sdk-1.1.9/swagger_client/models/market_highlight.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/market_highlight_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/market_highlight_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/market_highlight_status.py` & `investor8-sdk-1.1.9/swagger_client/models/market_highlight_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/metrics.py` & `investor8-sdk-1.1.9/swagger_client/models/metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/momentum_metric_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/momentum_metric_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/monthly_metrics.py` & `investor8-sdk-1.1.9/swagger_client/models/monthly_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/monthly_returns.py` & `investor8-sdk-1.1.9/swagger_client/models/monthly_returns.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/news_categories_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/news_categories_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/news_source.py` & `investor8-sdk-1.1.9/swagger_client/models/news_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/period_metric_value.py` & `investor8-sdk-1.1.9/swagger_client/models/period_metric_value.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/period_return.py` & `investor8-sdk-1.1.9/swagger_client/models/period_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/plot_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/plot_response_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/plot_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/previous_close_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/previous_close_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/profile_name.py` & `investor8-sdk-1.1.9/swagger_client/models/profile_name.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/recent_earning_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/recent_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/req_type.py` & `investor8-sdk-1.1.9/swagger_client/models/req_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/reset_password_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/reset_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/result_field.py` & `investor8-sdk-1.1.9/swagger_client/models/result_field.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/return_metrics.py` & `investor8-sdk-1.1.9/swagger_client/models/return_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/sa_attributes_prices.py` & `investor8-sdk-1.1.9/swagger_client/models/sa_attributes_prices.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/sa_sector_price_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/sa_sector_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/sector_returns_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/sector_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/send_email_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/send_email_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/standardized_financial.py` & `investor8-sdk-1.1.9/swagger_client/models/standardized_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_earning_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_financial.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_financial_metrics.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_info_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_info_master_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_info_master_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_ipo.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_ipo.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_news.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_news_details.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_news_details.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_news_status.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_news_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_popularity_details_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_popularity_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_popularity_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_popularity_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_price.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_price.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_price_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_rating_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_rating_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/stock_summary_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/stock_summary_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/string_message_result.py` & `investor8-sdk-1.1.9/swagger_client/models/string_message_result.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/tag_details_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/tag_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/tag_info_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/tag_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/upcoming_earning_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/upcoming_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/update_plot_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/update_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/update_watchlist_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/update_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/user.py` & `investor8-sdk-1.1.9/swagger_client/models/user.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/user_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/validate_watchlist_name_request_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/validate_watchlist_name_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/validate_watchlist_name_response_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/validate_watchlist_name_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/value_metrics_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/value_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/view_plot_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/view_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/watchlist.py` & `investor8-sdk-1.1.9/swagger_client/models/watchlist.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/models/watchlist_dto.py` & `investor8-sdk-1.1.9/swagger_client/models/watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/swagger_client/rest.py` & `investor8-sdk-1.1.9/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_active_company_dto.py` & `investor8-sdk-1.1.9/test/test_active_company_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_add_to_watchlist_dto.py` & `investor8-sdk-1.1.9/test/test_add_to_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_authentication_request.py` & `investor8-sdk-1.1.9/test/test_authentication_request.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_authentication_source.py` & `investor8-sdk-1.1.9/test/test_authentication_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_authorize_account_request_dto.py` & `investor8-sdk-1.1.9/test/test_authorize_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_authorize_account_response_dto.py` & `investor8-sdk-1.1.9/test/test_authorize_account_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_change_password_dto.py` & `investor8-sdk-1.1.9/test/test_change_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_company_info_dto.py` & `investor8-sdk-1.1.9/test/test_company_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_create_auth_req_dto.py` & `investor8-sdk-1.1.9/test/test_create_auth_req_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_create_plot_dto.py` & `investor8-sdk-1.1.9/test/test_create_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_create_update_news.py` & `investor8-sdk-1.1.9/test/test_create_update_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_create_user_dto.py` & `investor8-sdk-1.1.9/test/test_create_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_create_user_res_dto.py` & `investor8-sdk-1.1.9/test/test_create_user_res_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_create_watchlist_dto.py` & `investor8-sdk-1.1.9/test/test_create_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_current_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_current_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_current_momentum_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_current_momentum_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_daily_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_detailed_latest_price_dto.py` & `investor8-sdk-1.1.9/test/test_detailed_latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_earning_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_earning_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_earnings_api.py` & `investor8-sdk-1.1.9/test/test_earnings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_email_api.py` & `investor8-sdk-1.1.9/test/test_email_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_email_type.py` & `investor8-sdk-1.1.9/test/test_email_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_financial_metric_metadata_dto.py` & `investor8-sdk-1.1.9/test/test_financial_metric_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_financial_report_dto.py` & `investor8-sdk-1.1.9/test/test_financial_report_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_financial_tag.py` & `investor8-sdk-1.1.9/test/test_financial_tag.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_financials_api.py` & `investor8-sdk-1.1.9/test/test_financials_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_financials_growth.py` & `investor8-sdk-1.1.9/test/test_financials_growth.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_get_user_plots_dto.py` & `investor8-sdk-1.1.9/test/test_get_user_plots_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_get_watchlists_by_user_dto.py` & `investor8-sdk-1.1.9/test/test_get_watchlists_by_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_historical_daily_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_historical_daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_historical_financial_metrics.py` & `investor8-sdk-1.1.9/test/test_historical_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_historical_indicator_dto.py` & `investor8-sdk-1.1.9/test/test_historical_indicator_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_historical_return.py` & `investor8-sdk-1.1.9/test/test_historical_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_historical_returns_dto.py` & `investor8-sdk-1.1.9/test/test_historical_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_historical_value_metrics.py` & `investor8-sdk-1.1.9/test/test_historical_value_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_history_length.py` & `investor8-sdk-1.1.9/test/test_history_length.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_i8_terminal_check_version_dto.py` & `investor8-sdk-1.1.9/test/test_i8_terminal_check_version_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_i8_terminal_version.py` & `investor8-sdk-1.1.9/test/test_i8_terminal_version.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_i8_terminal_version_dto.py` & `investor8-sdk-1.1.9/test/test_i8_terminal_version_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_latest_financial_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_latest_financial_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_latest_financials_dto.py` & `investor8-sdk-1.1.9/test/test_latest_financials_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_latest_financials_with_growth_dto.py` & `investor8-sdk-1.1.9/test/test_latest_financials_with_growth_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_latest_price_dto.py` & `investor8-sdk-1.1.9/test/test_latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_list_exchange_sector_dto.py` & `investor8-sdk-1.1.9/test/test_list_exchange_sector_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_log_terminal_usage.py` & `investor8-sdk-1.1.9/test/test_log_terminal_usage.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_login_user_dto.py` & `investor8-sdk-1.1.9/test/test_login_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_login_with_code_dto.py` & `investor8-sdk-1.1.9/test/test_login_with_code_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_market_highlight.py` & `investor8-sdk-1.1.9/test/test_market_highlight.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_market_highlight_dto.py` & `investor8-sdk-1.1.9/test/test_market_highlight_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_market_highlight_status.py` & `investor8-sdk-1.1.9/test/test_market_highlight_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_metadata_properties_dto.py` & `investor8-sdk-1.1.9/test/test_metadata_properties_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_metric_metadata_dto.py` & `investor8-sdk-1.1.9/test/test_metric_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_metrics.py` & `investor8-sdk-1.1.9/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_metrics_api.py` & `investor8-sdk-1.1.9/test/test_metrics_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_metrics_metadata.py` & `investor8-sdk-1.1.9/test/test_metrics_metadata.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_momentum_metric_dto.py` & `investor8-sdk-1.1.9/test/test_momentum_metric_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_monthly_metrics.py` & `investor8-sdk-1.1.9/test/test_monthly_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_monthly_returns.py` & `investor8-sdk-1.1.9/test/test_monthly_returns.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_news_api.py` & `investor8-sdk-1.1.9/test/test_news_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_news_categories_dto.py` & `investor8-sdk-1.1.9/test/test_news_categories_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_news_source.py` & `investor8-sdk-1.1.9/test/test_news_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_period_metric_value.py` & `investor8-sdk-1.1.9/test/test_period_metric_value.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_period_return.py` & `investor8-sdk-1.1.9/test/test_period_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_plot.py` & `investor8-sdk-1.1.9/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_plot_detail_dto.py` & `investor8-sdk-1.1.9/test/test_plot_detail_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_plot_dto.py` & `investor8-sdk-1.1.9/test/test_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_plot_response_dto.py` & `investor8-sdk-1.1.9/test/test_plot_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_previous_close_dto.py` & `investor8-sdk-1.1.9/test/test_previous_close_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_price_api.py` & `investor8-sdk-1.1.9/test/test_price_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_profile_name.py` & `investor8-sdk-1.1.9/test/test_profile_name.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_recent_earning_dto.py` & `investor8-sdk-1.1.9/test/test_recent_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_remove_from_watchlist_dto.py` & `investor8-sdk-1.1.9/test/test_remove_from_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_rename_watchlist_dto.py` & `investor8-sdk-1.1.9/test/test_rename_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_req_type.py` & `investor8-sdk-1.1.9/test/test_req_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_reset_password_dto.py` & `investor8-sdk-1.1.9/test/test_reset_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_result_field.py` & `investor8-sdk-1.1.9/test/test_result_field.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_return_metrics.py` & `investor8-sdk-1.1.9/test/test_return_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_sa_attributes_prices.py` & `investor8-sdk-1.1.9/test/test_sa_attributes_prices.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_sa_sector_price_dto.py` & `investor8-sdk-1.1.9/test/test_sa_sector_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_screener_api.py` & `investor8-sdk-1.1.9/test/test_screener_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_search_api.py` & `investor8-sdk-1.1.9/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_sector_returns_dto.py` & `investor8-sdk-1.1.9/test/test_sector_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_send_email_dto.py` & `investor8-sdk-1.1.9/test/test_send_email_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_settings_api.py` & `investor8-sdk-1.1.9/test/test_settings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_standardized_financial.py` & `investor8-sdk-1.1.9/test/test_standardized_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_earning_dto.py` & `investor8-sdk-1.1.9/test/test_stock_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_financial.py` & `investor8-sdk-1.1.9/test/test_stock_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_financial_metrics.py` & `investor8-sdk-1.1.9/test/test_stock_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_info_api.py` & `investor8-sdk-1.1.9/test/test_stock_info_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_info_dto.py` & `investor8-sdk-1.1.9/test/test_stock_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_info_master_dto.py` & `investor8-sdk-1.1.9/test/test_stock_info_master_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_ipo.py` & `investor8-sdk-1.1.9/test/test_stock_ipo.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_news.py` & `investor8-sdk-1.1.9/test/test_stock_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_news_details.py` & `investor8-sdk-1.1.9/test/test_stock_news_details.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_news_status.py` & `investor8-sdk-1.1.9/test/test_stock_news_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_popularity_details_dto.py` & `investor8-sdk-1.1.9/test/test_stock_popularity_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_popularity_dto.py` & `investor8-sdk-1.1.9/test/test_stock_popularity_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_price.py` & `investor8-sdk-1.1.9/test/test_stock_price.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_price_dto.py` & `investor8-sdk-1.1.9/test/test_stock_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_rating_dto.py` & `investor8-sdk-1.1.9/test/test_stock_rating_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_stock_summary_dto.py` & `investor8-sdk-1.1.9/test/test_stock_summary_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_string_message_result.py` & `investor8-sdk-1.1.9/test/test_string_message_result.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_tag_details_dto.py` & `investor8-sdk-1.1.9/test/test_tag_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_tag_info_dto.py` & `investor8-sdk-1.1.9/test/test_tag_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_tags_api.py` & `investor8-sdk-1.1.9/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_trading_calendar_details_dto.py` & `investor8-sdk-1.1.9/test/test_trading_calendar_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_upcoming_earning_dto.py` & `investor8-sdk-1.1.9/test/test_upcoming_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_update_plot_dto.py` & `investor8-sdk-1.1.9/test/test_update_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_update_watchlist_dto.py` & `investor8-sdk-1.1.9/test/test_update_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_user.py` & `investor8-sdk-1.1.9/test/test_user.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_user_api.py` & `investor8-sdk-1.1.9/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_user_dto.py` & `investor8-sdk-1.1.9/test/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_validate_watchlist_name_request_dto.py` & `investor8-sdk-1.1.9/test/test_validate_watchlist_name_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_validate_watchlist_name_response_dto.py` & `investor8-sdk-1.1.9/test/test_validate_watchlist_name_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_value_metrics_dto.py` & `investor8-sdk-1.1.9/test/test_value_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_view_plot_dto.py` & `investor8-sdk-1.1.9/test/test_view_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_watchlist.py` & `investor8-sdk-1.1.9/test/test_watchlist.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.8/test/test_watchlist_dto.py` & `investor8-sdk-1.1.9/test/test_watchlist_dto.py`

 * *Files identical despite different names*

