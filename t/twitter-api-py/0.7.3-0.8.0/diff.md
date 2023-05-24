# Comparing `tmp/twitter_api_py-0.7.3.tar.gz` & `tmp/twitter_api_py-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter_api_py-0.7.3.tar", max compression
+gzip compressed data, was "twitter_api_py-0.8.0.tar", max compression
```

## Comparing `twitter_api_py-0.7.3.tar` & `twitter_api_py-0.8.0.tar`

### file list

```diff
@@ -1,275 +1,275 @@
--rw-r--r--   0        0        0     1497 2023-05-22 12:26:38.951757 twitter_api_py-0.7.3/LICENSE
--rw-r--r--   0        0        0     2126 2023-05-22 12:26:38.951757 twitter_api_py-0.7.3/README.md
--rw-r--r--   0        0        0     1672 2023-05-22 12:26:38.979758 twitter_api_py-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      480 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/__init__.py
--rw-r--r--   0        0        0     1041 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
--rw-r--r--   0        0        0      311 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
--rw-r--r--   0        0        0      311 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_real_client.py
--rw-r--r--   0        0        0     1388 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
--rw-r--r--   0        0        0      306 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
--rw-r--r--   0        0        0      808 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
--rw-r--r--   0        0        0      315 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
--rw-r--r--   0        0        0      315 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_real_client.py
--rw-r--r--   0        0        0     1211 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
--rw-r--r--   0        0        0      311 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
--rw-r--r--   0        0        0      311 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_real_client.py
--rw-r--r--   0        0        0      831 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
--rw-r--r--   0        0        0      306 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
--rw-r--r--   0        0        0      306 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_real_client.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/__init__.py
--rw-r--r--   0        0        0      365 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
--rw-r--r--   0        0        0     1140 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
--rw-r--r--   0        0        0      462 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
--rw-r--r--   0        0        0      793 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
--rw-r--r--   0        0        0      444 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
--rw-r--r--   0        0        0      722 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
--rw-r--r--   0        0        0      392 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
--rw-r--r--   0        0        0      798 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
--rw-r--r--   0        0        0      501 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
--rw-r--r--   0        0        0      751 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
--rw-r--r--   0        0        0      648 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/session_resources.py
--rw-r--r--   0        0        0      357 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
--rw-r--r--   0        0        0     1596 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
--rw-r--r--   0        0        0     1875 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
--rw-r--r--   0        0        0     4005 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
--rw-r--r--   0        0        0     1103 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth1_session.py
--rw-r--r--   0        0        0     1716 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
--rw-r--r--   0        0        0     3466 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
--rw-r--r--   0        0        0      823 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth2_session.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/request/__init__.py
--rw-r--r--   0        0        0     1375 2023-05-22 12:26:38.995759 twitter_api_py-0.7.3/twitter_api/client/request/request_async_client.py
--rw-r--r--   0        0        0      460 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/client/request/request_async_mock_client.py
--rw-r--r--   0        0        0     5306 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/client/request/request_async_real_client.py
--rw-r--r--   0        0        0     1786 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/client/request/request_client.py
--rw-r--r--   0        0        0     3832 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/client/request/request_mock_client.py
--rw-r--r--   0        0        0     7358 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/client/request/request_real_client.py
--rw-r--r--   0        0        0    32384 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/client/twitter_api_async_client.py
--rw-r--r--   0        0        0    15048 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/client/twitter_api_async_mock_client.py
--rw-r--r--   0        0        0    14661 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/client/twitter_api_async_real_client.py
--rw-r--r--   0        0        0    32143 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/client/twitter_api_client.py
--rw-r--r--   0        0        0    27423 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/client/twitter_api_mock_client.py
--rw-r--r--   0        0        0    13652 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/client/twitter_api_real_client.py
--rw-r--r--   0        0        0    11214 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/error.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/__init__.py
--rw-r--r--   0        0        0      603 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/manager/__init__.py
--rw-r--r--   0        0        0      677 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
--rw-r--r--   0        0        0     1301 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/manager/mixins/__init__.py
--rw-r--r--   0        0        0     2251 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/manager/mixins/dict_rate_limit_checker_mixin.py
--rw-r--r--   0        0        0      672 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/manager/mixins/raise_rate_limit_handler_mixin.py
--rw-r--r--   0        0        0     3287 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/manager/mixins/sleep_rate_limit_handler_mixin.py
--rw-r--r--   0        0        0      908 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
--rw-r--r--   0        0        0     1358 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/manager/rate_limit_manager.py
--rw-r--r--   0        0        0     3751 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/rate_limit.py
--rw-r--r--   0        0        0      291 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/rate_limit_info.py
--rw-r--r--   0        0        0      102 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/rate_limit/rate_limit_target.py
--rw-r--r--   0        0        0      281 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/api_resources.py
--rw-r--r--   0        0        0      437 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/oauth2_invalidate_token/__init__.py
--rw-r--r--   0        0        0     2331 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
--rw-r--r--   0        0        0      332 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/oauth2_token/__init__.py
--rw-r--r--   0        0        0     2223 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/oauth2_token/post_oauth2_token.py
--rw-r--r--   0        0        0      522 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversation_messages/__init__.py
--rw-r--r--   0        0        0     2370 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
--rw-r--r--   0        0        0      422 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversations/__init__.py
--rw-r--r--   0        0        0     2199 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py
--rw-r--r--   0        0        0      654 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
--rw-r--r--   0        0        0     8948 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
--rw-r--r--   0        0        0      657 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py
--rw-r--r--   0        0        0     2444 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
--rw-r--r--   0        0        0      429 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweet/__init__.py
--rw-r--r--   0        0        0     1492 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweet/delete_v2_tweet.py
--rw-r--r--   0        0        0     3142 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweet/get_v2_tweet.py
--rw-r--r--   0        0        0      439 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweet_retweeted_by/__init__.py
--rw-r--r--   0        0        0     6602 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
--rw-r--r--   0        0        0      428 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets/__init__.py
--rw-r--r--   0        0        0     3007 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets/get_v2_tweets.py
--rw-r--r--   0        0        0     2956 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets/post_v2_tweets.py
--rw-r--r--   0        0        0      419 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_all/__init__.py
--rw-r--r--   0        0        0     6019 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
--rw-r--r--   0        0        0      452 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_recent/__init__.py
--rw-r--r--   0        0        0     6118 2023-05-22 12:26:38.999759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
--rw-r--r--   0        0        0      452 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_stream/__init__.py
--rw-r--r--   0        0        0     3669 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
--rw-r--r--   0        0        0      751 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py
--rw-r--r--   0        0        0     2164 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0     3149 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0      286 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user/__init__.py
--rw-r--r--   0        0        0     2833 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user/get_v2_user.py
--rw-r--r--   0        0        0      382 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user_followers/__init__.py
--rw-r--r--   0        0        0     6551 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user_followers/get_v2_user_followers.py
--rw-r--r--   0        0        0      387 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user_following/__init__.py
--rw-r--r--   0        0        0     1944 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user_following/post_v2_user_following.py
--rw-r--r--   0        0        0      402 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user_liked_tweets/__init__.py
--rw-r--r--   0        0        0     7972 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
--rw-r--r--   0        0        0      378 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user_retweets/__init__.py
--rw-r--r--   0        0        0     1946 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py
--rw-r--r--   0        0        0      342 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user_tweets/__init__.py
--rw-r--r--   0        0        0     8381 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py
--rw-r--r--   0        0        0      290 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_users/__init__.py
--rw-r--r--   0        0        0     2733 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_users/get_v2_users.py
--rw-r--r--   0        0        0      310 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_users_by/__init__.py
--rw-r--r--   0        0        0     2808 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_users_by/get_v2_users_by.py
--rw-r--r--   0        0        0      407 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_users_by_username/__init__.py
--rw-r--r--   0        0        0     3078 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/__init__.py
--rw-r--r--   0        0        0      397 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/_chainable.py
--rw-r--r--   0        0        0      858 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/_generic_client.py
--rw-r--r--   0        0        0     2362 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/_model.py
--rw-r--r--   0        0        0     3413 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/_paging.py
--rw-r--r--   0        0        0      727 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/comma_separatable.py
--rw-r--r--   0        0        0      246 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/endpoint.py
--rw-r--r--   0        0        0     1581 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/extra_permissive_model.py
--rw-r--r--   0        0        0      645 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/http.py
--rw-r--r--   0        0        0      744 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/httpx.py
--rw-r--r--   0        0        0     1971 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/oauth.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/oauth1/__init__.py
--rw-r--r--   0        0        0     2037 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/oauth1/oauth1_access_token.py
--rw-r--r--   0        0        0     3474 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/oauth1/oauth1_authorization.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/oauth2/__init__.py
--rw-r--r--   0        0        0     1975 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/oauth2/oauth2_access_token.py
--rw-r--r--   0        0        0     3593 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/oauth2/oauth2_authorization.py
--rw-r--r--   0        0        0       74 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/pagination_token.py
--rw-r--r--   0        0        0       66 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_cashtag.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_dm_conversation/__init__.py
--rw-r--r--   0        0        0      337 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_dm_conversation/dm_conversation.py
--rw-r--r--   0        0        0      212 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_dm_conversation/dm_conversation_attachment.py
--rw-r--r--   0        0        0       75 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_dm_conversation/dm_conversation_id.py
--rw-r--r--   0        0        0      624 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_dm_conversation/dm_conversation_message.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_dm_event/__init__.py
--rw-r--r--   0        0        0      342 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_dm_event/dm_event_expansion.py
--rw-r--r--   0        0        0      448 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_dm_event/dm_event_field.py
--rw-r--r--   0        0        0       68 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_dm_event/dm_event_id.py
--rw-r--r--   0        0        0      249 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_dm_event/dm_event_type.py
--rw-r--r--   0        0        0      368 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_domain.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_entity/__init__.py
--rw-r--r--   0        0        0      286 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_entity/entity.py
--rw-r--r--   0        0        0       67 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_entity/entity_id.py
--rw-r--r--   0        0        0       69 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_entity/entity_name.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_geo/__init__.py
--rw-r--r--   0        0        0      220 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_geo/geo.py
--rw-r--r--   0        0        0       66 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_hashtag.py
--rw-r--r--   0        0        0      773 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_language.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_list/__init__.py
--rw-r--r--   0        0        0       65 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_list/list_id.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_media/__init__.py
--rw-r--r--   0        0        0     1386 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_media/media.py
--rw-r--r--   0        0        0      581 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_media/media_field.py
--rw-r--r--   0        0        0      111 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_media/media_id.py
--rw-r--r--   0        0        0       67 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_media/media_key.py
--rw-r--r--   0        0        0      376 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_media/media_non_public_metrics.py
--rw-r--r--   0        0        0      411 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_media/media_organic_metrics.py
--rw-r--r--   0        0        0      412 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_media/media_promoted_metrics.py
--rw-r--r--   0        0        0      190 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_media/media_public_metrics.py
--rw-r--r--   0        0        0      211 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_media/media_variants.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_place/__init__.py
--rw-r--r--   0        0        0      933 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_place/place.py
--rw-r--r--   0        0        0     2723 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_place/place_country_code.py
--rw-r--r--   0        0        0      359 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_place/place_field.py
--rw-r--r--   0        0        0       72 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_place/place_full_name.py
--rw-r--r--   0        0        0      105 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_place/place_id.py
--rw-r--r--   0        0        0       68 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_place/place_name.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_poll/__init__.py
--rw-r--r--   0        0        0      593 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_poll/poll.py
--rw-r--r--   0        0        0      283 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_poll/poll_field.py
--rw-r--r--   0        0        0       65 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_poll/poll_id.py
--rw-r--r--   0        0        0      164 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_poll/poll_option.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet.py
--rw-r--r--   0        0        0      392 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet_entities.py
--rw-r--r--   0        0        0      913 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet_entities_description.py
--rw-r--r--   0        0        0      237 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet_entities_description_cashtag.py
--rw-r--r--   0        0        0      237 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet_entities_description_hashtag.py
--rw-r--r--   0        0        0      246 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet_entities_description_mention.py
--rw-r--r--   0        0        0      258 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet_entities_description_url.py
--rw-r--r--   0        0        0      338 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet_entities_url.py
--rw-r--r--   0        0        0      254 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet_includes.py
--rw-r--r--   0        0        0      219 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet_public_metrics.py
--rw-r--r--   0        0        0      382 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet_withheld.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_rule/__init__.py
--rw-r--r--   0        0        0      311 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_rule/rule.py
--rw-r--r--   0        0        0       65 2023-05-22 12:26:39.011759 twitter_api_py-0.7.3/twitter_api/types/v2_rule/rule_id.py
--rw-r--r--   0        0        0       66 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_rule/rule_tag.py
--rw-r--r--   0        0        0     1411 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_scope.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/__init__.py
--rw-r--r--   0        0        0      873 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/_and_operator.py
--rw-r--r--   0        0        0      440 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/_markable_operator.py
--rw-r--r--   0        0        0      521 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/_not_operator.py
--rw-r--r--   0        0        0      662 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/_or_operator.py
--rw-r--r--   0        0        0      700 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/bounding_box_operator.py
--rw-r--r--   0        0        0      339 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/cashtag_operator.py
--rw-r--r--   0        0        0     1361 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/context_operator.py
--rw-r--r--   0        0        0      380 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/conversation_id_operator.py
--rw-r--r--   0        0        0      341 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/entity_operator.py
--rw-r--r--   0        0        0      424 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/from_user_operator.py
--rw-r--r--   0        0        0     1547 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/group_operator.py
--rw-r--r--   0        0        0      219 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/has_cashtags_operator.py
--rw-r--r--   0        0        0      209 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/has_geo_operator.py
--rw-r--r--   0        0        0      219 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/has_hashtags_operator.py
--rw-r--r--   0        0        0      215 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/has_images_operator.py
--rw-r--r--   0        0        0      213 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/has_links_operator.py
--rw-r--r--   0        0        0      213 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/has_media_operator.py
--rw-r--r--   0        0        0      219 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/has_mentions_operator.py
--rw-r--r--   0        0        0      222 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/has_video_link_operator.py
--rw-r--r--   0        0        0      339 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/hashtag_operator.py
--rw-r--r--   0        0        0      349 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/in_reply_to_tweet_id_operator.py
--rw-r--r--   0        0        0      442 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/is_nullcast_operator.py
--rw-r--r--   0        0        0      211 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/is_quote_operator.py
--rw-r--r--   0        0        0      211 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/is_reply_operator.py
--rw-r--r--   0        0        0      215 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/is_retweet_operator.py
--rw-r--r--   0        0        0      217 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/is_verified_operator.py
--rw-r--r--   0        0        0      658 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/keyword_operator.py
--rw-r--r--   0        0        0      339 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/lang_operator.py
--rw-r--r--   0        0        0      317 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/list_operator.py
--rw-r--r--   0        0        0      349 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/mention_operator.py
--rw-r--r--   0        0        0     2670 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/operator.py
--rw-r--r--   0        0        0      370 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/place_country_operator.py
--rw-r--r--   0        0        0      544 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/place_operator.py
--rw-r--r--   0        0        0     1328 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/point_radius_operator.py
--rw-r--r--   0        0        0      354 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/quotes_of_tweet_id_operator.py
--rw-r--r--   0        0        0      433 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/retweets_of_operator.py
--rw-r--r--   0        0        0      350 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/retweets_of_tweet_id_operator.py
--rw-r--r--   0        0        0      420 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/to_user_operator.py
--rw-r--r--   0        0        0      262 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/url_operator.py
--rw-r--r--   0        0        0     2495 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/search_query.py
--rw-r--r--   0        0        0    14382 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_search_query/search_query_builder.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/__init__.py
--rw-r--r--   0        0        0     7856 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet.py
--rw-r--r--   0        0        0      309 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_attachments.py
--rw-r--r--   0        0        0      267 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_context_annotation.py
--rw-r--r--   0        0        0      314 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_edit_controls.py
--rw-r--r--   0        0        0      720 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_entities.py
--rw-r--r--   0        0        0      333 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_entities_annotation.py
--rw-r--r--   0        0        0      247 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_entities_cashtag.py
--rw-r--r--   0        0        0      247 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_entities_hashtag.py
--rw-r--r--   0        0        0      313 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_entities_mention.py
--rw-r--r--   0        0        0      415 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_entities_url.py
--rw-r--r--   0        0        0      643 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_expansion.py
--rw-r--r--   0        0        0     1921 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_field.py
--rw-r--r--   0        0        0      288 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_geo.py
--rw-r--r--   0        0        0      231 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_geo_coordinates.py
--rw-r--r--   0        0        0      111 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_id.py
--rw-r--r--   0        0        0      287 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_non_public_metrics.py
--rw-r--r--   0        0        0      285 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_organic_metrics.py
--rw-r--r--   0        0        0      286 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_promoted_metrics.py
--rw-r--r--   0        0        0      437 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_public_metrics.py
--rw-r--r--   0        0        0      267 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_referenced_tweet.py
--rw-r--r--   0        0        0     7079 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_response_body.py
--rw-r--r--   0        0        0      417 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_withheld.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_user/__init__.py
--rw-r--r--   0        0        0      969 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_user/user.py
--rw-r--r--   0        0        0      168 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_user/user_expantion.py
--rw-r--r--   0        0        0      619 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_user/user_field.py
--rw-r--r--   0        0        0       65 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_user/user_id.py
--rw-r--r--   0        0        0      108 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_user/user_verified_type.py
--rw-r--r--   0        0        0      139 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/types/v2_user/username.py
--rw-r--r--   0        0        0        0 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/utils/__init__.py
--rw-r--r--   0        0        0      123 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/utils/_datetime.py
--rw-r--r--   0        0        0      716 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/utils/_functional.py
--rw-r--r--   0        0        0      904 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/utils/_oauth.py
--rw-r--r--   0        0        0      790 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/utils/json.py
--rw-r--r--   0        0        0      630 2023-05-22 12:26:39.015760 twitter_api_py-0.7.3/twitter_api/warning.py
--rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 twitter_api_py-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-05-24 12:21:32.986128 twitter_api_py-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2126 2023-05-24 12:21:32.986128 twitter_api_py-0.8.0/README.md
+-rw-r--r--   0        0        0     1672 2023-05-24 12:21:33.018128 twitter_api_py-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      480 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/__init__.py
+-rw-r--r--   0        0        0     1041 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
+-rw-r--r--   0        0        0      311 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
+-rw-r--r--   0        0        0      311 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_real_client.py
+-rw-r--r--   0        0        0     1388 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
+-rw-r--r--   0        0        0      306 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
+-rw-r--r--   0        0        0      808 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
+-rw-r--r--   0        0        0      315 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
+-rw-r--r--   0        0        0      315 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_real_client.py
+-rw-r--r--   0        0        0     1211 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
+-rw-r--r--   0        0        0      311 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
+-rw-r--r--   0        0        0      311 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_real_client.py
+-rw-r--r--   0        0        0      831 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
+-rw-r--r--   0        0        0      306 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
+-rw-r--r--   0        0        0      306 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_real_client.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
+-rw-r--r--   0        0        0     1140 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
+-rw-r--r--   0        0        0      462 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
+-rw-r--r--   0        0        0      793 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
+-rw-r--r--   0        0        0      444 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
+-rw-r--r--   0        0        0      722 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
+-rw-r--r--   0        0        0      392 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
+-rw-r--r--   0        0        0      798 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
+-rw-r--r--   0        0        0      501 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
+-rw-r--r--   0        0        0      751 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
+-rw-r--r--   0        0        0      648 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/session_resources.py
+-rw-r--r--   0        0        0      357 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
+-rw-r--r--   0        0        0     1596 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
+-rw-r--r--   0        0        0     1875 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
+-rw-r--r--   0        0        0     4005 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
+-rw-r--r--   0        0        0     1103 2023-05-24 12:21:33.038128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth1_session.py
+-rw-r--r--   0        0        0     1716 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
+-rw-r--r--   0        0        0     3466 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
+-rw-r--r--   0        0        0      823 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth2_session.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/request/__init__.py
+-rw-r--r--   0        0        0     1375 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/request/request_async_client.py
+-rw-r--r--   0        0        0      460 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/request/request_async_mock_client.py
+-rw-r--r--   0        0        0     5306 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/request/request_async_real_client.py
+-rw-r--r--   0        0        0     1786 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/request/request_client.py
+-rw-r--r--   0        0        0     3832 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/request/request_mock_client.py
+-rw-r--r--   0        0        0     7358 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/request/request_real_client.py
+-rw-r--r--   0        0        0    32384 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/twitter_api_async_client.py
+-rw-r--r--   0        0        0    15048 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/twitter_api_async_mock_client.py
+-rw-r--r--   0        0        0    14661 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/twitter_api_async_real_client.py
+-rw-r--r--   0        0        0    32143 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/twitter_api_client.py
+-rw-r--r--   0        0        0    27423 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/twitter_api_mock_client.py
+-rw-r--r--   0        0        0    13652 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/client/twitter_api_real_client.py
+-rw-r--r--   0        0        0    11214 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/error.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/__init__.py
+-rw-r--r--   0        0        0      603 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/manager/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
+-rw-r--r--   0        0        0     1301 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/manager/mixins/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/manager/mixins/dict_rate_limit_checker_mixin.py
+-rw-r--r--   0        0        0      672 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/manager/mixins/raise_rate_limit_handler_mixin.py
+-rw-r--r--   0        0        0     3287 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/manager/mixins/sleep_rate_limit_handler_mixin.py
+-rw-r--r--   0        0        0      908 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
+-rw-r--r--   0        0        0     1358 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/manager/rate_limit_manager.py
+-rw-r--r--   0        0        0     3751 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/rate_limit.py
+-rw-r--r--   0        0        0      291 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/rate_limit_info.py
+-rw-r--r--   0        0        0      102 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/rate_limit/rate_limit_target.py
+-rw-r--r--   0        0        0      281 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/api_resources.py
+-rw-r--r--   0        0        0      437 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/oauth2_invalidate_token/__init__.py
+-rw-r--r--   0        0        0     2331 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
+-rw-r--r--   0        0        0      332 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/oauth2_token/__init__.py
+-rw-r--r--   0        0        0     2223 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/oauth2_token/post_oauth2_token.py
+-rw-r--r--   0        0        0      522 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversation_messages/__init__.py
+-rw-r--r--   0        0        0     2370 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
+-rw-r--r--   0        0        0      422 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversations/__init__.py
+-rw-r--r--   0        0        0     2199 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py
+-rw-r--r--   0        0        0      654 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
+-rw-r--r--   0        0        0     8744 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
+-rw-r--r--   0        0        0      657 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py
+-rw-r--r--   0        0        0     2444 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
+-rw-r--r--   0        0        0      429 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     1492 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweet/delete_v2_tweet.py
+-rw-r--r--   0        0        0     3142 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweet/get_v2_tweet.py
+-rw-r--r--   0        0        0      439 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweet_retweeted_by/__init__.py
+-rw-r--r--   0        0        0     6310 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
+-rw-r--r--   0        0        0      428 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets/__init__.py
+-rw-r--r--   0        0        0     3007 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets/get_v2_tweets.py
+-rw-r--r--   0        0        0     2956 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets/post_v2_tweets.py
+-rw-r--r--   0        0        0      419 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_all/__init__.py
+-rw-r--r--   0        0        0     5815 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
+-rw-r--r--   0        0        0      452 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_recent/__init__.py
+-rw-r--r--   0        0        0     5914 2023-05-24 12:21:33.042128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
+-rw-r--r--   0        0        0      452 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_stream/__init__.py
+-rw-r--r--   0        0        0     3669 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
+-rw-r--r--   0        0        0      751 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py
+-rw-r--r--   0        0        0     2164 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0     3149 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0      286 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user/__init__.py
+-rw-r--r--   0        0        0     2833 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user/get_v2_user.py
+-rw-r--r--   0        0        0      382 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user_followers/__init__.py
+-rw-r--r--   0        0        0     6259 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user_followers/get_v2_user_followers.py
+-rw-r--r--   0        0        0      387 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user_following/__init__.py
+-rw-r--r--   0        0        0     1944 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user_following/post_v2_user_following.py
+-rw-r--r--   0        0        0      402 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user_liked_tweets/__init__.py
+-rw-r--r--   0        0        0     7680 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
+-rw-r--r--   0        0        0      378 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user_retweets/__init__.py
+-rw-r--r--   0        0        0     1946 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py
+-rw-r--r--   0        0        0      342 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user_tweets/__init__.py
+-rw-r--r--   0        0        0     8089 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py
+-rw-r--r--   0        0        0      290 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_users/__init__.py
+-rw-r--r--   0        0        0     2733 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_users/get_v2_users.py
+-rw-r--r--   0        0        0      310 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_users_by/__init__.py
+-rw-r--r--   0        0        0     2808 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_users_by/get_v2_users_by.py
+-rw-r--r--   0        0        0      407 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_users_by_username/__init__.py
+-rw-r--r--   0        0        0     3078 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/_chainable.py
+-rw-r--r--   0        0        0      858 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/_generic_client.py
+-rw-r--r--   0        0        0     2362 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/_model.py
+-rw-r--r--   0        0        0     3317 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/_paging.py
+-rw-r--r--   0        0        0      727 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/comma_separatable.py
+-rw-r--r--   0        0        0      246 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/endpoint.py
+-rw-r--r--   0        0        0     1581 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/extra_permissive_model.py
+-rw-r--r--   0        0        0      645 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/http.py
+-rw-r--r--   0        0        0      744 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/httpx.py
+-rw-r--r--   0        0        0     1971 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/oauth.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/oauth1/__init__.py
+-rw-r--r--   0        0        0     2037 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/oauth1/oauth1_access_token.py
+-rw-r--r--   0        0        0     3474 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/oauth1/oauth1_authorization.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/oauth2/__init__.py
+-rw-r--r--   0        0        0     1975 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/oauth2/oauth2_access_token.py
+-rw-r--r--   0        0        0     3593 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/oauth2/oauth2_authorization.py
+-rw-r--r--   0        0        0       74 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/pagination_token.py
+-rw-r--r--   0        0        0       66 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_cashtag.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_dm_conversation/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_dm_conversation/dm_conversation.py
+-rw-r--r--   0        0        0      212 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_dm_conversation/dm_conversation_attachment.py
+-rw-r--r--   0        0        0       75 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_dm_conversation/dm_conversation_id.py
+-rw-r--r--   0        0        0      624 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_dm_conversation/dm_conversation_message.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_dm_event/__init__.py
+-rw-r--r--   0        0        0      342 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_dm_event/dm_event_expansion.py
+-rw-r--r--   0        0        0      448 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_dm_event/dm_event_field.py
+-rw-r--r--   0        0        0       68 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_dm_event/dm_event_id.py
+-rw-r--r--   0        0        0      249 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_dm_event/dm_event_type.py
+-rw-r--r--   0        0        0      368 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_domain.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_entity/__init__.py
+-rw-r--r--   0        0        0      286 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_entity/entity.py
+-rw-r--r--   0        0        0       67 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_entity/entity_id.py
+-rw-r--r--   0        0        0       69 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_entity/entity_name.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_geo/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_geo/geo.py
+-rw-r--r--   0        0        0       66 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_hashtag.py
+-rw-r--r--   0        0        0      773 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_language.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_list/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_list/list_id.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_media/__init__.py
+-rw-r--r--   0        0        0     1386 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_media/media.py
+-rw-r--r--   0        0        0      581 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_media/media_field.py
+-rw-r--r--   0        0        0      111 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_media/media_id.py
+-rw-r--r--   0        0        0       67 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_media/media_key.py
+-rw-r--r--   0        0        0      376 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_media/media_non_public_metrics.py
+-rw-r--r--   0        0        0      411 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_media/media_organic_metrics.py
+-rw-r--r--   0        0        0      412 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_media/media_promoted_metrics.py
+-rw-r--r--   0        0        0      190 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_media/media_public_metrics.py
+-rw-r--r--   0        0        0      211 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_media/media_variants.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_place/__init__.py
+-rw-r--r--   0        0        0      933 2023-05-24 12:21:33.046128 twitter_api_py-0.8.0/twitter_api/types/v2_place/place.py
+-rw-r--r--   0        0        0     2723 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_place/place_country_code.py
+-rw-r--r--   0        0        0      359 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_place/place_field.py
+-rw-r--r--   0        0        0       72 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_place/place_full_name.py
+-rw-r--r--   0        0        0      105 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_place/place_id.py
+-rw-r--r--   0        0        0       68 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_place/place_name.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_poll/__init__.py
+-rw-r--r--   0        0        0      593 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_poll/poll.py
+-rw-r--r--   0        0        0      283 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_poll/poll_field.py
+-rw-r--r--   0        0        0       65 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_poll/poll_id.py
+-rw-r--r--   0        0        0      164 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_poll/poll_option.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet.py
+-rw-r--r--   0        0        0      392 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet_entities.py
+-rw-r--r--   0        0        0      913 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet_entities_description.py
+-rw-r--r--   0        0        0      237 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet_entities_description_cashtag.py
+-rw-r--r--   0        0        0      237 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet_entities_description_hashtag.py
+-rw-r--r--   0        0        0      246 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet_entities_description_mention.py
+-rw-r--r--   0        0        0      258 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet_entities_description_url.py
+-rw-r--r--   0        0        0      338 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet_entities_url.py
+-rw-r--r--   0        0        0      254 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet_includes.py
+-rw-r--r--   0        0        0      219 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet_public_metrics.py
+-rw-r--r--   0        0        0      382 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_rule/__init__.py
+-rw-r--r--   0        0        0      311 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_rule/rule.py
+-rw-r--r--   0        0        0       65 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_rule/rule_id.py
+-rw-r--r--   0        0        0       66 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_rule/rule_tag.py
+-rw-r--r--   0        0        0     1411 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_scope.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/__init__.py
+-rw-r--r--   0        0        0      873 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/_and_operator.py
+-rw-r--r--   0        0        0      440 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/_markable_operator.py
+-rw-r--r--   0        0        0      521 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/_not_operator.py
+-rw-r--r--   0        0        0      662 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/_or_operator.py
+-rw-r--r--   0        0        0      700 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/bounding_box_operator.py
+-rw-r--r--   0        0        0      339 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/cashtag_operator.py
+-rw-r--r--   0        0        0     1361 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/context_operator.py
+-rw-r--r--   0        0        0      380 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/conversation_id_operator.py
+-rw-r--r--   0        0        0      341 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/entity_operator.py
+-rw-r--r--   0        0        0      424 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/from_user_operator.py
+-rw-r--r--   0        0        0     1547 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/group_operator.py
+-rw-r--r--   0        0        0      219 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/has_cashtags_operator.py
+-rw-r--r--   0        0        0      209 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/has_geo_operator.py
+-rw-r--r--   0        0        0      219 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/has_hashtags_operator.py
+-rw-r--r--   0        0        0      215 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/has_images_operator.py
+-rw-r--r--   0        0        0      213 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/has_links_operator.py
+-rw-r--r--   0        0        0      213 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/has_media_operator.py
+-rw-r--r--   0        0        0      219 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/has_mentions_operator.py
+-rw-r--r--   0        0        0      222 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/has_video_link_operator.py
+-rw-r--r--   0        0        0      339 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/hashtag_operator.py
+-rw-r--r--   0        0        0      349 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/in_reply_to_tweet_id_operator.py
+-rw-r--r--   0        0        0      442 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/is_nullcast_operator.py
+-rw-r--r--   0        0        0      211 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/is_quote_operator.py
+-rw-r--r--   0        0        0      211 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/is_reply_operator.py
+-rw-r--r--   0        0        0      215 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/is_retweet_operator.py
+-rw-r--r--   0        0        0      217 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/is_verified_operator.py
+-rw-r--r--   0        0        0      658 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/keyword_operator.py
+-rw-r--r--   0        0        0      339 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/lang_operator.py
+-rw-r--r--   0        0        0      317 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/list_operator.py
+-rw-r--r--   0        0        0      349 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/mention_operator.py
+-rw-r--r--   0        0        0     2670 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/operator.py
+-rw-r--r--   0        0        0      370 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/place_country_operator.py
+-rw-r--r--   0        0        0      544 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/place_operator.py
+-rw-r--r--   0        0        0     1328 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/point_radius_operator.py
+-rw-r--r--   0        0        0      354 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/quotes_of_tweet_id_operator.py
+-rw-r--r--   0        0        0      433 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/retweets_of_operator.py
+-rw-r--r--   0        0        0      350 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/retweets_of_tweet_id_operator.py
+-rw-r--r--   0        0        0      420 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/to_user_operator.py
+-rw-r--r--   0        0        0      262 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/url_operator.py
+-rw-r--r--   0        0        0     2495 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/search_query.py
+-rw-r--r--   0        0        0    14382 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_search_query/search_query_builder.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     7856 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet.py
+-rw-r--r--   0        0        0      309 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_attachments.py
+-rw-r--r--   0        0        0      267 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_context_annotation.py
+-rw-r--r--   0        0        0      314 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_edit_controls.py
+-rw-r--r--   0        0        0      720 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_entities.py
+-rw-r--r--   0        0        0      333 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_entities_annotation.py
+-rw-r--r--   0        0        0      247 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_entities_cashtag.py
+-rw-r--r--   0        0        0      247 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_entities_hashtag.py
+-rw-r--r--   0        0        0      313 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_entities_mention.py
+-rw-r--r--   0        0        0      415 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_entities_url.py
+-rw-r--r--   0        0        0      643 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_expansion.py
+-rw-r--r--   0        0        0     1921 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_field.py
+-rw-r--r--   0        0        0      288 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_geo.py
+-rw-r--r--   0        0        0      231 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_geo_coordinates.py
+-rw-r--r--   0        0        0      111 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_id.py
+-rw-r--r--   0        0        0      287 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_non_public_metrics.py
+-rw-r--r--   0        0        0      285 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_organic_metrics.py
+-rw-r--r--   0        0        0      286 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_promoted_metrics.py
+-rw-r--r--   0        0        0      437 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_public_metrics.py
+-rw-r--r--   0        0        0      267 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_referenced_tweet.py
+-rw-r--r--   0        0        0     7079 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_response_body.py
+-rw-r--r--   0        0        0      417 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_user/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_user/user.py
+-rw-r--r--   0        0        0      168 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_user/user_expantion.py
+-rw-r--r--   0        0        0      619 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_user/user_field.py
+-rw-r--r--   0        0        0       65 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_user/user_id.py
+-rw-r--r--   0        0        0      108 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_user/user_verified_type.py
+-rw-r--r--   0        0        0      139 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/types/v2_user/username.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/utils/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/utils/_datetime.py
+-rw-r--r--   0        0        0      716 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/utils/_functional.py
+-rw-r--r--   0        0        0      904 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/utils/_oauth.py
+-rw-r--r--   0        0        0      790 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/utils/json.py
+-rw-r--r--   0        0        0      630 2023-05-24 12:21:33.050128 twitter_api_py-0.8.0/twitter_api/warning.py
+-rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 twitter_api_py-0.8.0/PKG-INFO
```

### Comparing `twitter_api_py-0.7.3/LICENSE` & `twitter_api_py-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/README.md` & `twitter_api_py-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/pyproject.toml` & `twitter_api_py-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["yassun4dev <yassun4dev@outlook.com>"]
 description = "Twitter API Client by Typed Python."
 name = "twitter-api-py"
 packages = [{ include = "twitter_api" }]
 readme = "README.md"
-version = "0.7.3"
+version = "0.8.0"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/twitter-api-py"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Software Development :: Libraries",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
```

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/session_resources.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/session_resources.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth1_real_session.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth1_real_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth1_session.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth1_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth2_real_session.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth2_real_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/oauth_session/twitter_oauth2_session.py` & `twitter_api_py-0.8.0/twitter_api/client/oauth_session/twitter_oauth2_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/request/request_async_client.py` & `twitter_api_py-0.8.0/twitter_api/client/request/request_async_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/request/request_async_real_client.py` & `twitter_api_py-0.8.0/twitter_api/client/request/request_async_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/request/request_client.py` & `twitter_api_py-0.8.0/twitter_api/client/request/request_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/request/request_mock_client.py` & `twitter_api_py-0.8.0/twitter_api/client/request/request_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/request/request_real_client.py` & `twitter_api_py-0.8.0/twitter_api/client/request/request_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/twitter_api_async_client.py` & `twitter_api_py-0.8.0/twitter_api/client/twitter_api_async_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/twitter_api_async_mock_client.py` & `twitter_api_py-0.8.0/twitter_api/client/twitter_api_async_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/twitter_api_async_real_client.py` & `twitter_api_py-0.8.0/twitter_api/client/twitter_api_async_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/twitter_api_client.py` & `twitter_api_py-0.8.0/twitter_api/client/twitter_api_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/twitter_api_mock_client.py` & `twitter_api_py-0.8.0/twitter_api/client/twitter_api_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/client/twitter_api_real_client.py` & `twitter_api_py-0.8.0/twitter_api/client/twitter_api_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/error.py` & `twitter_api_py-0.8.0/twitter_api/error.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/rate_limit/manager/__init__.py` & `twitter_api_py-0.8.0/twitter_api/rate_limit/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/rate_limit/manager/dict_rate_limit_manager.py` & `twitter_api_py-0.8.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py` & `twitter_api_py-0.8.0/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/rate_limit/manager/mixins/dict_rate_limit_checker_mixin.py` & `twitter_api_py-0.8.0/twitter_api/rate_limit/manager/mixins/dict_rate_limit_checker_mixin.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/rate_limit/manager/mixins/raise_rate_limit_handler_mixin.py` & `twitter_api_py-0.8.0/twitter_api/rate_limit/manager/mixins/raise_rate_limit_handler_mixin.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/rate_limit/manager/mixins/sleep_rate_limit_handler_mixin.py` & `twitter_api_py-0.8.0/twitter_api/rate_limit/manager/mixins/sleep_rate_limit_handler_mixin.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py` & `twitter_api_py-0.8.0/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/rate_limit/manager/rate_limit_manager.py` & `twitter_api_py-0.8.0/twitter_api/rate_limit/manager/rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/rate_limit/rate_limit.py` & `twitter_api_py-0.8.0/twitter_api/rate_limit/rate_limit.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py` & `twitter_api_py-0.8.0/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/oauth2_token/post_oauth2_token.py` & `twitter_api_py-0.8.0/twitter_api/resources/oauth2_token/post_oauth2_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversation_messages/__init__.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversation_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from pydantic import Field
 from typing_extensions import AsyncGenerator, NotRequired, Self, TypedDict, override
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types._paging import (
     PageResponseBody,
-    aget_collected_paging_response_body,
-    aget_paging_response_body_iter,
-    get_collected_paging_response_body,
-    get_paging_response_body_iter,
+    aget_paging_all,
+    aget_paging_iter,
+    get_paging_all,
+    get_paging_iter,
 )
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.v2_dm_conversation.dm_conversation_id import DmConversationId
 from twitter_api.types.v2_dm_event.dm_event_expansion import DmEventExpansion
@@ -158,47 +158,47 @@
         return self.request_client.get(
             endpoint=ENDPOINT,
             url=ENDPOINT.url.replace(":participant_id", participant_id),
             query=_make_query(query) if query is not None else None,
             response_body_type=GetV2DmConversationsWithParticipantDmEventsResponseBody,
         )
 
-    def get_paging_response_body_iter(
+    def get_paging_iter(
         self,
         participant_id: UserId,
         query: Optional[
             GetV2DmConversationsWithParticipantDmEventsQueryParameters
         ] = None,
     ) -> Generator[GetV2DmConversationsWithParticipantDmEventsResponseBody, None, None]:
         """
         DM の参加者のイベント情報を返す。
 
         ページングされた API のレスポンスをイテレータで返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/likes/api-reference/get-users-participant_id-liked_tweets
         """
-        return get_paging_response_body_iter(
+        return get_paging_iter(
             partial(self.get, participant_id), query, "pagination_token"
         )
 
-    def get_collected_paging_response_body(
+    def get_paging_all(
         self,
         participant_id: UserId,
         query: Optional[
             GetV2DmConversationsWithParticipantDmEventsQueryParameters
         ] = None,
     ) -> GetV2DmConversationsWithParticipantDmEventsResponseBody:
         """
         DM の参加者のイベント情報を返す。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/likes/api-reference/get-users-participant_id-liked_tweets
         """
-        return get_collected_paging_response_body(
+        return get_paging_all(
             partial(self.get, participant_id), query, "pagination_token"
         )
 
 
 class AsyncGetV2DmConversationsWithParticipantDmEventsResources(
     GetV2DmConversationsWithParticipantDmEventsResources
 ):
@@ -212,29 +212,29 @@
     ) -> GetV2DmConversationsWithParticipantDmEventsResponseBody:
         return super().get(
             participant_id,
             query,
         )
 
     @override
-    async def get_paging_response_body_iter(
+    async def get_paging_iter(
         self,
         participant_id: UserId,
         query: Optional[
             GetV2DmConversationsWithParticipantDmEventsQueryParameters
         ] = None,
     ) -> AsyncGenerator[GetV2DmConversationsWithParticipantDmEventsResponseBody, None]:
-        return aget_paging_response_body_iter(
+        return aget_paging_iter(
             partial(self.get, participant_id), query, "pagination_token"
         )
 
     @override
-    async def get_collected_paging_response_body(
+    async def get_paging_all(
         self,
         participant_id: UserId,
         query: Optional[
             GetV2DmConversationsWithParticipantDmEventsQueryParameters
         ] = None,
     ) -> GetV2DmConversationsWithParticipantDmEventsResponseBody:
-        return await aget_collected_paging_response_body(
+        return await aget_paging_all(
             partial(self.get, participant_id), query, "pagination_token"
         )
```

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_tweet/delete_v2_tweet.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_tweet/delete_v2_tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_tweet/get_v2_tweet.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_tweet/get_v2_tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from pydantic import Field
 from typing_extensions import AsyncGenerator, NotRequired, Self, TypedDict, override
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types._paging import (
     PageResponseBody,
-    aget_collected_paging_response_body,
-    aget_paging_response_body_iter,
-    get_collected_paging_response_body,
-    get_paging_response_body_iter,
+    aget_paging_all,
+    aget_paging_iter,
+    get_paging_all,
+    get_paging_iter,
 )
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.v2_retweet.retweet import Retweet
 from twitter_api.types.v2_scope import oauth2_scopes
@@ -109,61 +109,53 @@
         return self.request_client.get(
             endpoint=ENDPOINT,
             response_body_type=GetV2TweetRetweetedByResponseBody,
             url=ENDPOINT.url.replace(":id", id),
             query=_make_query(query) if query is not None else None,
         )
 
-    def get_paging_response_body_iter(
+    def get_paging_iter(
         self, id: TweetId, query: Optional[GetV2TweetRetweetedByQueryParameters] = None
     ) -> Generator[GetV2TweetRetweetedByResponseBody, None, None]:
         """
         リツイートされたツイートの一覧を取得する。
 
         ページングされた API のレスポンスをイテレータで返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/retweets/api-reference/get-tweets-id-retweeted_by
         """
-        return get_paging_response_body_iter(
-            partial(self.get, id), query, "pagination_token"
-        )
+        return get_paging_iter(partial(self.get, id), query, "pagination_token")
 
-    def get_collected_paging_response_body(
+    def get_paging_all(
         self, id: TweetId, query: Optional[GetV2TweetRetweetedByQueryParameters] = None
     ) -> GetV2TweetRetweetedByResponseBody:
         """
         リツイートされたツイートの一覧を取得する。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/retweets/api-reference/get-tweets-id-retweeted_by
         """
-        return get_collected_paging_response_body(
-            partial(self.get, id), query, "pagination_token"
-        )
+        return get_paging_all(partial(self.get, id), query, "pagination_token")
 
 
 class AsyncGetV2TweetRetweetedByResources(GetV2TweetRetweetedByResources):
     @override
     async def get(
         self, id: TweetId, query: Optional[GetV2TweetRetweetedByQueryParameters] = None
     ) -> GetV2TweetRetweetedByResponseBody:
         return super().get(
             id,
             query,
         )
 
     @override
-    async def get_paging_response_body_iter(
+    async def get_paging_iter(
         self, id: TweetId, query: Optional[GetV2TweetRetweetedByQueryParameters] = None
     ) -> AsyncGenerator[GetV2TweetRetweetedByResponseBody, None]:
-        return aget_paging_response_body_iter(
-            partial(self.get, id), query, "pagination_token"
-        )
+        return aget_paging_iter(partial(self.get, id), query, "pagination_token")
 
     @override
-    async def get_collected_paging_response_body(
+    async def get_paging_all(
         self, id: TweetId, query: Optional[GetV2TweetRetweetedByQueryParameters] = None
     ) -> GetV2TweetRetweetedByResponseBody:
-        return await aget_collected_paging_response_body(
-            partial(self.get, id), query, "pagination_token"
-        )
+        return await aget_paging_all(partial(self.get, id), query, "pagination_token")
```

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_tweets/get_v2_tweets.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_tweets/get_v2_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_tweets/post_v2_tweets.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_tweets/post_v2_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_user_followers/get_v2_user_followers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,140 +1,171 @@
-from datetime import datetime
-from typing import Generator, Optional, Union
-from urllib import parse
+from functools import partial
+from typing import Generator, Optional
 
-from typing_extensions import AsyncGenerator, Literal, NotRequired, TypedDict, override
+from pydantic import Field
+from typing_extensions import AsyncGenerator, NotRequired, Self, TypedDict, override
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types._paging import (
-    aget_collected_paging_response_body,
-    aget_paging_response_body_iter,
-    get_collected_paging_response_body,
-    get_paging_response_body_iter,
+    PageResponseBody,
+    aget_paging_all,
+    aget_paging_iter,
+    get_paging_all,
+    get_paging_iter,
 )
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.pagination_token import PaginationToken
-from twitter_api.types.v2_media.media_field import MediaField
-from twitter_api.types.v2_place.place_field import PlaceField
-from twitter_api.types.v2_poll.poll_field import PollField
 from twitter_api.types.v2_scope import oauth2_scopes
-from twitter_api.types.v2_search_query.search_query import SearchQuery
-from twitter_api.types.v2_tweet.tweet_expansion import TweetExpansion
+from twitter_api.types.v2_tweet.tweet import Tweet
 from twitter_api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.types.v2_tweet.tweet_id import TweetId
-from twitter_api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
+from twitter_api.types.v2_user.user import User
+from twitter_api.types.v2_user.user_expantion import UserExpansion
 from twitter_api.types.v2_user.user_field import UserField
-from twitter_api.utils._datetime import rfc3339
-from twitter_api.utils._functional import map_optional
+from twitter_api.types.v2_user.user_id import UserId
 
-ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/all")
+ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/:id/followers")
 
-GetV2TweetsSearchAllQueryParameters = TypedDict(
-    "GetV2TweetsSearchAllQueryParameters",
+GetV2UserFollowersQueryParameters = TypedDict(
+    "GetV2UserFollowersQueryParameters",
     {
-        "query": Union[SearchQuery, str],
-        "start_time": NotRequired[Optional[datetime]],
-        "end_time": NotRequired[Optional[datetime]],
-        "since_id": NotRequired[Optional[TweetId]],
-        "until_id": NotRequired[Optional[TweetId]],
-        "sort_order": NotRequired[Optional[Literal["recency", "relevancy"]]],
-        "next_token": NotRequired[Optional[PaginationToken]],
+        "expansions": NotRequired[Optional[CommaSeparatable[UserExpansion]]],
+        "pagination_token": NotRequired[Optional[str]],
         "max_results": NotRequired[Optional[int]],
-        "expansions": NotRequired[Optional[CommaSeparatable[TweetExpansion]]],
-        "place.fields": NotRequired[Optional[CommaSeparatable[PlaceField]]],
-        "media.fields": NotRequired[Optional[CommaSeparatable[MediaField]]],
-        "poll.fields": NotRequired[Optional[CommaSeparatable[PollField]]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
     },
 )
 
 
-def _make_query(query: GetV2TweetsSearchAllQueryParameters) -> dict:
+def _make_query(query: GetV2UserFollowersQueryParameters) -> dict:
     return {
-        "query": parse.quote(str(query["query"])),
-        "start_time": map_optional(rfc3339, query.get("start_time")),
-        "end_time": map_optional(rfc3339, query.get("end_time")),
-        "since_id": query.get("since_id"),
-        "until_id": query.get("until_id"),
-        "sort_order": query.get("sort_order"),
-        "next_token": query.get("next_token"),
-        "max_results": query.get("expansions"),
         "expansions": comma_separated_str(query.get("expansions")),
-        "place.fields": query.get("place.fields"),
-        "media.fields": query.get("media.fields"),
-        "poll.fields": query.get("poll.fields"),
+        "pagination_token": query.get("pagination_token"),
+        "max_results": query.get("max_results"),
         "tweet.fields": comma_separated_str(query.get("tweet.fields")),
         "user.fields": comma_separated_str(query.get("user.fields")),
     }
 
 
-class GetV2TweetsSearchAllResponseBody(TweetsSearchResponseBody):
-    pass
+class GetV2UserFollowersResponseBodyMeta(ExtraPermissiveModel):
+    result_count: int
+    next_token: Optional[PaginationToken] = None
+    previous_token: Optional[PaginationToken] = None
 
+    def extend(self, other: Self) -> None:
+        self.result_count += other.result_count
+        self.next_token = None
+        self.previous_token = None
 
-class GetV2TweetsSearchAllResources(ApiResources):
+
+class GetV2UserFollowersResponseBodyIncludes(ExtraPermissiveModel):
+    tweets: list[Tweet] = Field(default_factory=list)
+
+    def extend(self, other: Self) -> None:
+        self.tweets.extend(other.tweets)
+
+
+class GetV2UserFollowersResponseBody(ExtraPermissiveModel, PageResponseBody):
+    data: list[User] = Field(default_factory=list)
+    meta: GetV2UserFollowersResponseBodyMeta
+    includes: GetV2UserFollowersResponseBodyIncludes = Field(
+        default_factory=GetV2UserFollowersResponseBodyIncludes,
+    )
+    errors: Optional[list[dict]] = None
+
+    @property
+    def meta_next_token(self) -> Optional[PaginationToken]:
+        return self.meta.next_token
+
+    def extend(self, other: Self) -> None:
+        self.data.extend(other.data)
+        self.meta.extend(other.meta)
+        self.includes.extend(other.includes)
+
+        if other.errors is not None:
+            if self.errors is not None:
+                self.errors.extend(other.errors)
+            else:
+                self.errors = other.errors
+
+
+class GetV2UserFollowersResources(ApiResources):
     @oauth2_scopes(
         "tweet.read",
         "users.read",
+        "follows.read",
     )
-    @rate_limit(ENDPOINT, "app", requests=300, mins=15)
-    @rate_limit(ENDPOINT, "app", requests=1, seconds=1)
+    @rate_limit(ENDPOINT, "app", requests=15, mins=15)
+    @rate_limit(ENDPOINT, "user", requests=15, mins=15)
     def get(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> GetV2TweetsSearchAllResponseBody:
+        self,
+        id: UserId,
+        query: Optional[GetV2UserFollowersQueryParameters] = None,
+    ) -> GetV2UserFollowersResponseBody:
         """
-        ツイートの一覧を検索する。
+        ユーザのフォロワーの一覧を取得する。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-all
+        refer: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/get-users-id-followers
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
-            response_body_type=GetV2TweetsSearchAllResponseBody,
+            url=ENDPOINT.url.replace(":id", id),
             query=_make_query(query) if query is not None else None,
+            response_body_type=GetV2UserFollowersResponseBody,
         )
 
-    def get_paging_response_body_iter(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> Generator[GetV2TweetsSearchAllResponseBody, None, None]:
+    def get_paging_iter(
+        self,
+        id: UserId,
+        query: Optional[GetV2UserFollowersQueryParameters] = None,
+    ) -> Generator[GetV2UserFollowersResponseBody, None, None]:
         """
-        ツイートの一覧を検索する。
+        ユーザのフォロワーの一覧を取得する。
 
         ページングされた API のレスポンスをイテレータで返す。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-all
+        refer: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/get-users-id-followers
         """
-        return get_paging_response_body_iter(self.get, query, "next_token")
+        return get_paging_iter(partial(self.get, id), query, "pagination_token")
 
-    def get_collected_paging_response_body(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> GetV2TweetsSearchAllResponseBody:
+    def get_paging_all(
+        self,
+        id: UserId,
+        query: Optional[GetV2UserFollowersQueryParameters] = None,
+    ) -> GetV2UserFollowersResponseBody:
         """
-        ツイートの一覧を検索する。
+        ユーザのフォロワーの一覧を取得する。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-all
+        refer: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/get-users-id-followers
         """
-        return get_collected_paging_response_body(self.get, query, "next_token")
+        return get_paging_all(partial(self.get, id), query, "pagination_token")
 
 
-class AsyncGetV2TweetsSearchAllResources(GetV2TweetsSearchAllResources):
+class AsyncGetV2UserFollowersResources(GetV2UserFollowersResources):
     @override
     async def get(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> GetV2TweetsSearchAllResponseBody:
-        return super().get(query)
+        self,
+        id: UserId,
+        query: Optional[GetV2UserFollowersQueryParameters] = None,
+    ) -> GetV2UserFollowersResponseBody:
+        return super().get(id, query)
 
     @override
-    async def get_paging_response_body_iter(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> AsyncGenerator[GetV2TweetsSearchAllResponseBody, None]:
-        return aget_paging_response_body_iter(self.get, query, "next_token")
+    async def get_paging_iter(
+        self,
+        id: UserId,
+        query: Optional[GetV2UserFollowersQueryParameters] = None,
+    ) -> AsyncGenerator[GetV2UserFollowersResponseBody, None]:
+        return aget_paging_iter(partial(self.get, id), query, "pagination_token")
 
     @override
-    async def get_collected_paging_response_body(
-        self, query: GetV2TweetsSearchAllQueryParameters
-    ) -> GetV2TweetsSearchAllResponseBody:
-        return await aget_collected_paging_response_body(self.get, query, "next_token")
+    async def get_paging_all(
+        self,
+        id: UserId,
+        query: Optional[GetV2UserFollowersQueryParameters] = None,
+    ) -> GetV2UserFollowersResponseBody:
+        return await aget_paging_all(partial(self.get, id), query, "pagination_token")
```

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from typing import Generator, Optional, Union
 
 from typing_extensions import AsyncGenerator, Literal, NotRequired, TypedDict, override
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types._paging import (
-    aget_collected_paging_response_body,
-    aget_paging_response_body_iter,
-    get_collected_paging_response_body,
-    get_paging_response_body_iter,
+    aget_paging_all,
+    aget_paging_iter,
+    get_paging_all,
+    get_paging_iter,
 )
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.v2_media.media_field import MediaField
 from twitter_api.types.v2_place.place_field import PlaceField
 from twitter_api.types.v2_poll.poll_field import PollField
@@ -90,50 +90,50 @@
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
             response_body_type=GetV2TweetsSearchRecentResponseBody,
             query=_make_query(query) if query is not None else None,
         )
 
-    def get_paging_response_body_iter(
+    def get_paging_iter(
         self, query: GetV2TweetsSearchRecentQueryParameters
     ) -> Generator[GetV2TweetsSearchRecentResponseBody, None, None]:
         """
         ツイートの一覧を検索する。
 
         ページングされた API のレスポンスをイテレータで返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-recent
         """
-        return get_paging_response_body_iter(self.get, query, "next_token")
+        return get_paging_iter(self.get, query, "next_token")
 
-    def get_collected_paging_response_body(
+    def get_paging_all(
         self, query: GetV2TweetsSearchRecentQueryParameters
     ) -> GetV2TweetsSearchRecentResponseBody:
         """
         ツイートの一覧を検索する。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-recent
         """
-        return get_collected_paging_response_body(self.get, query, "next_token")
+        return get_paging_all(self.get, query, "next_token")
 
 
 class AsyncGetV2TweetsSearchRecentResources(GetV2TweetsSearchRecentResources):
     @override
     async def get(
         self, query: GetV2TweetsSearchRecentQueryParameters
     ) -> GetV2TweetsSearchRecentResponseBody:
         return super().get(query)
 
     @override
-    async def get_paging_response_body_iter(
+    async def get_paging_iter(
         self, query: GetV2TweetsSearchRecentQueryParameters
     ) -> AsyncGenerator[GetV2TweetsSearchRecentResponseBody, None]:
-        return aget_paging_response_body_iter(self.get, query, "next_token")
+        return aget_paging_iter(self.get, query, "next_token")
 
     @override
-    async def get_collected_paging_response_body(
+    async def get_paging_all(
         self, query: GetV2TweetsSearchRecentQueryParameters
     ) -> GetV2TweetsSearchRecentResponseBody:
-        return await aget_collected_paging_response_body(self.get, query, "next_token")
+        return await aget_paging_all(self.get, query, "next_token")
```

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_user/get_v2_user.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_user/get_v2_user.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_user_followers/get_v2_user_followers.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,125 @@
+from datetime import datetime
 from functools import partial
 from typing import Generator, Optional
 
 from pydantic import Field
-from typing_extensions import AsyncGenerator, NotRequired, Self, TypedDict, override
+from typing_extensions import (
+    AsyncGenerator,
+    Literal,
+    NotRequired,
+    Self,
+    TypedDict,
+    override,
+)
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types._paging import (
     PageResponseBody,
-    aget_collected_paging_response_body,
-    aget_paging_response_body_iter,
-    get_collected_paging_response_body,
-    get_paging_response_body_iter,
+    aget_paging_all,
+    aget_paging_iter,
+    get_paging_all,
+    get_paging_iter,
 )
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.pagination_token import PaginationToken
+from twitter_api.types.v2_media.media import Media
+from twitter_api.types.v2_media.media_field import MediaField
+from twitter_api.types.v2_place.place import Place
+from twitter_api.types.v2_place.place_field import PlaceField
+from twitter_api.types.v2_poll.poll import Poll
+from twitter_api.types.v2_poll.poll_field import PollField
 from twitter_api.types.v2_scope import oauth2_scopes
 from twitter_api.types.v2_tweet.tweet import Tweet
 from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.types.v2_user.user import User
 from twitter_api.types.v2_user.user_expantion import UserExpansion
 from twitter_api.types.v2_user.user_field import UserField
 from twitter_api.types.v2_user.user_id import UserId
+from twitter_api.utils._datetime import rfc3339
+from twitter_api.utils._functional import map_optional
 
-ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/:id/followers")
+ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/:id/tweets")
 
-GetV2UserFollowersQueryParameters = TypedDict(
-    "GetV2UserFollowersQueryParameters",
+GetV2UserTweetsQueryParameters = TypedDict(
+    "GetV2UserTweetsQueryParameters",
     {
+        "start_time": NotRequired[Optional[datetime]],
+        "end_time": NotRequired[Optional[datetime]],
+        "since_id": NotRequired[Optional[TweetId]],
+        "until_id": NotRequired[Optional[TweetId]],
+        "exclude": NotRequired[Optional[Literal["retweets", "replies"]]],
         "expansions": NotRequired[Optional[CommaSeparatable[UserExpansion]]],
         "pagination_token": NotRequired[Optional[str]],
         "max_results": NotRequired[Optional[int]],
+        "media.fields": NotRequired[Optional[CommaSeparatable[MediaField]]],
+        "place.fields": NotRequired[Optional[CommaSeparatable[PlaceField]]],
+        "poll.fields": NotRequired[Optional[CommaSeparatable[PollField]]],
         "tweet.fields": NotRequired[Optional[CommaSeparatable[TweetField]]],
         "user.fields": NotRequired[Optional[CommaSeparatable[UserField]]],
     },
 )
 
 
-def _make_query(query: GetV2UserFollowersQueryParameters) -> dict:
+def _make_query(query: GetV2UserTweetsQueryParameters) -> dict:
     return {
+        "start_time": map_optional(rfc3339, query.get("start_time")),
+        "end_time": map_optional(rfc3339, query.get("end_time")),
+        "since_id": query.get("since_id"),
+        "until_id": query.get("until_id"),
+        "exclude": query.get("exclude"),
         "expansions": comma_separated_str(query.get("expansions")),
         "pagination_token": query.get("pagination_token"),
         "max_results": query.get("max_results"),
+        "media.fields": comma_separated_str(query.get("media.fields")),
+        "place.fields": comma_separated_str(query.get("place.fields")),
+        "poll.fields": comma_separated_str(query.get("poll.fields")),
         "tweet.fields": comma_separated_str(query.get("tweet.fields")),
         "user.fields": comma_separated_str(query.get("user.fields")),
     }
 
 
-class GetV2UserFollowersResponseBodyMeta(ExtraPermissiveModel):
+class GetV2UserTweetsResponseBodyIncludes(ExtraPermissiveModel):
+    users: list[User] = Field(default_factory=list)
+    tweets: list[Tweet] = Field(default_factory=list)
+    places: list[Place] = Field(default_factory=list)
+    media: list[Media] = Field(default_factory=list)
+    polls: list[Poll] = Field(default_factory=list)
+
+    def extend(self, other: Self) -> None:
+        self.users.extend(other.users)
+        self.tweets.extend(other.tweets)
+        self.places.extend(other.places)
+        self.media.extend(other.media)
+        self.polls.extend(other.polls)
+
+
+class GetV2UserTweetsResponseBodyMeta(ExtraPermissiveModel):
     result_count: int
+    oldest_id: TweetId
+    newest_id: TweetId
     next_token: Optional[PaginationToken] = None
     previous_token: Optional[PaginationToken] = None
 
     def extend(self, other: Self) -> None:
         self.result_count += other.result_count
         self.next_token = None
         self.previous_token = None
 
 
-class GetV2UserFollowersResponseBodyIncludes(ExtraPermissiveModel):
-    tweets: list[Tweet] = Field(default_factory=list)
-
-    def extend(self, other: Self) -> None:
-        self.tweets.extend(other.tweets)
-
-
-class GetV2UserFollowersResponseBody(ExtraPermissiveModel, PageResponseBody):
-    data: list[User] = Field(default_factory=list)
-    meta: GetV2UserFollowersResponseBodyMeta
-    includes: GetV2UserFollowersResponseBodyIncludes = Field(
-        default_factory=GetV2UserFollowersResponseBodyIncludes,
+class GetV2UserTweetsResponseBody(ExtraPermissiveModel, PageResponseBody):
+    data: list[Tweet]
+    includes: GetV2UserTweetsResponseBodyIncludes = Field(
+        default_factory=GetV2UserTweetsResponseBodyIncludes,
     )
+    meta: GetV2UserTweetsResponseBodyMeta
     errors: Optional[list[dict]] = None
 
     @property
     def meta_next_token(self) -> Optional[PaginationToken]:
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
@@ -87,93 +130,84 @@
         if other.errors is not None:
             if self.errors is not None:
                 self.errors.extend(other.errors)
             else:
                 self.errors = other.errors
 
 
-class GetV2UserFollowersResources(ApiResources):
+class GetV2UserTweetsResources(ApiResources):
     @oauth2_scopes(
         "tweet.read",
         "users.read",
-        "follows.read",
     )
-    @rate_limit(ENDPOINT, "app", requests=15, mins=15)
-    @rate_limit(ENDPOINT, "user", requests=15, mins=15)
+    @rate_limit(ENDPOINT, "app", requests=1500, mins=15)
+    @rate_limit(ENDPOINT, "user", requests=900, mins=15)
     def get(
         self,
         id: UserId,
-        query: Optional[GetV2UserFollowersQueryParameters] = None,
-    ) -> GetV2UserFollowersResponseBody:
+        query: Optional[GetV2UserTweetsQueryParameters] = None,
+    ) -> GetV2UserTweetsResponseBody:
         """
-        ユーザのフォロワーの一覧を取得する。
+        ユーザのツイートの一覧を取得する。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/get-users-id-followers
+        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/timelines/api-reference/get-users-id-tweets
         """
         return self.request_client.get(
             endpoint=ENDPOINT,
             url=ENDPOINT.url.replace(":id", id),
             query=_make_query(query) if query is not None else None,
-            response_body_type=GetV2UserFollowersResponseBody,
+            response_body_type=GetV2UserTweetsResponseBody,
         )
 
-    def get_paging_response_body_iter(
+    def get_paging_iter(
         self,
         id: UserId,
-        query: Optional[GetV2UserFollowersQueryParameters] = None,
-    ) -> Generator[GetV2UserFollowersResponseBody, None, None]:
+        query: Optional[GetV2UserTweetsQueryParameters] = None,
+    ) -> Generator[GetV2UserTweetsResponseBody, None, None]:
         """
-        ユーザのフォロワーの一覧を取得する。
+        ユーザのツイートの一覧を取得する。
 
         ページングされた API のレスポンスをイテレータで返す。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/get-users-id-followers
+        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/timelines/api-reference/get-users-id-tweets
         """
-        return get_paging_response_body_iter(
-            partial(self.get, id), query, "pagination_token"
-        )
+        return get_paging_iter(partial(self.get, id), query, "pagination_token")
 
-    def get_collected_paging_response_body(
+    def get_paging_all(
         self,
         id: UserId,
-        query: Optional[GetV2UserFollowersQueryParameters] = None,
-    ) -> GetV2UserFollowersResponseBody:
+        query: Optional[GetV2UserTweetsQueryParameters] = None,
+    ) -> GetV2UserTweetsResponseBody:
         """
-        ユーザのフォロワーの一覧を取得する。
+        ユーザのツイートの一覧を取得する。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
-        refer: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/get-users-id-followers
+        refer: https://developer.twitter.com/en/docs/twitter-api/tweets/timelines/api-reference/get-users-id-tweets
         """
-        return get_collected_paging_response_body(
-            partial(self.get, id), query, "pagination_token"
-        )
+        return get_paging_all(partial(self.get, id), query, "pagination_token")
 
 
-class AsyncGetV2UserFollowersResources(GetV2UserFollowersResources):
+class AsyncGetV2UserTweetsResources(GetV2UserTweetsResources):
     @override
     async def get(
         self,
         id: UserId,
-        query: Optional[GetV2UserFollowersQueryParameters] = None,
-    ) -> GetV2UserFollowersResponseBody:
+        query: Optional[GetV2UserTweetsQueryParameters] = None,
+    ) -> GetV2UserTweetsResponseBody:
         return super().get(id, query)
 
     @override
-    async def get_paging_response_body_iter(
+    async def get_paging_iter(
         self,
         id: UserId,
-        query: Optional[GetV2UserFollowersQueryParameters] = None,
-    ) -> AsyncGenerator[GetV2UserFollowersResponseBody, None]:
-        return aget_paging_response_body_iter(
-            partial(self.get, id), query, "pagination_token"
-        )
+        query: Optional[GetV2UserTweetsQueryParameters] = None,
+    ) -> AsyncGenerator[GetV2UserTweetsResponseBody, None]:
+        return aget_paging_iter(partial(self.get, id), query, "pagination_token")
 
     @override
-    async def get_collected_paging_response_body(
+    async def get_paging_all(
         self,
         id: UserId,
-        query: Optional[GetV2UserFollowersQueryParameters] = None,
-    ) -> GetV2UserFollowersResponseBody:
-        return await aget_collected_paging_response_body(
-            partial(self.get, id), query, "pagination_token"
-        )
+        query: Optional[GetV2UserTweetsQueryParameters] = None,
+    ) -> GetV2UserTweetsResponseBody:
+        return await aget_paging_all(partial(self.get, id), query, "pagination_token")
```

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_user_following/post_v2_user_following.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_user_following/post_v2_user_following.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from pydantic import Field
 from typing_extensions import AsyncGenerator, NotRequired, Self, TypedDict, override
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types._paging import (
     PageResponseBody,
-    aget_collected_paging_response_body,
-    aget_paging_response_body_iter,
-    get_collected_paging_response_body,
-    get_paging_response_body_iter,
+    aget_paging_all,
+    aget_paging_iter,
+    get_paging_all,
+    get_paging_iter,
 )
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.v2_media.media import Media
 from twitter_api.types.v2_media.media_field import MediaField
@@ -137,68 +137,60 @@
         return self.request_client.get(
             endpoint=ENDPOINT,
             url=ENDPOINT.url.replace(":id", id),
             query=_make_query(query) if query is not None else None,
             response_body_type=GetV2UserLikedTweetsResponseBody,
         )
 
-    def get_paging_response_body_iter(
+    def get_paging_iter(
         self,
         id: UserId,
         query: Optional[GetV2UserLikedTweetsQueryParameters] = None,
     ) -> Generator[GetV2UserLikedTweetsResponseBody, None, None]:
         """
         ユーザが「いいね」をしているツイートの一覧を取得する。
 
         ページングされた API のレスポンスをイテレータで返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/likes/api-reference/get-users-id-liked_tweets
         """
-        return get_paging_response_body_iter(
-            partial(self.get, id), query, "pagination_token"
-        )
+        return get_paging_iter(partial(self.get, id), query, "pagination_token")
 
-    def get_collected_paging_response_body(
+    def get_paging_all(
         self,
         id: UserId,
         query: Optional[GetV2UserLikedTweetsQueryParameters] = None,
     ) -> GetV2UserLikedTweetsResponseBody:
         """
         ユーザが「いいね」をしているツイートの一覧を取得する。
 
         ページングされた API のレスポンスをまとめて一つのレスポンスとして返す。
 
         refer: https://developer.twitter.com/en/docs/twitter-api/tweets/likes/api-reference/get-users-id-liked_tweets
         """
-        return get_collected_paging_response_body(
-            partial(self.get, id), query, "pagination_token"
-        )
+        return get_paging_all(partial(self.get, id), query, "pagination_token")
 
 
 class AsyncGetV2UserLikedTweetsResources(GetV2UserLikedTweetsResources):
     @override
     async def get(
         self,
         id: UserId,
         query: Optional[GetV2UserLikedTweetsQueryParameters] = None,
     ) -> GetV2UserLikedTweetsResponseBody:
         return super().get(id, query)
 
     @override
-    async def get_paging_response_body_iter(
+    async def get_paging_iter(
         self,
         id: UserId,
         query: Optional[GetV2UserLikedTweetsQueryParameters] = None,
     ) -> AsyncGenerator[GetV2UserLikedTweetsResponseBody, None]:
-        return aget_paging_response_body_iter(
-            partial(self.get, id), query, "pagination_token"
-        )
+        return aget_paging_iter(partial(self.get, id), query, "pagination_token")
 
     @override
-    async def get_collected_paging_response_body(
+    async def get_paging_all(
         self,
         id: UserId,
         query: Optional[GetV2UserLikedTweetsQueryParameters] = None,
     ) -> GetV2UserLikedTweetsResponseBody:
-        return await aget_collected_paging_response_body(
-            partial(self.get, id), query, "pagination_token"
-        )
+        return await aget_paging_all(partial(self.get, id), query, "pagination_token")
```

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_users/get_v2_users.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_users/get_v2_users.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_users_by/get_v2_users_by.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_users_by/get_v2_users_by.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py` & `twitter_api_py-0.8.0/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/_generic_client.py` & `twitter_api_py-0.8.0/twitter_api/types/_generic_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/_model.py` & `twitter_api_py-0.8.0/twitter_api/types/_model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/_paging.py` & `twitter_api_py-0.8.0/twitter_api/types/_paging.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 AnyPageResponseBody = TypeVar(
     "AnyPageResponseBody",
     bound=PageResponseBody,
 )
 
 
-def get_paging_response_body_iter(
+def get_paging_iter(
     get_func: Callable[
         [AnyQueryParameters],
         AnyPageResponseBody,
     ],
     query: Optional[AnyQueryParameters],
     pagination_token_key: str,
 ) -> Generator[AnyPageResponseBody, None, None]:
@@ -48,35 +48,35 @@
 
         next_token = response_body.meta_next_token
 
         if next_token is None:
             return
 
 
-def get_collected_paging_response_body(
+def get_paging_all(
     get_func: Callable[
         [AnyQueryParameters],
         AnyPageResponseBody,
     ],
     query: Optional[AnyQueryParameters],
     pagination_token_key: str,
 ) -> AnyPageResponseBody:
     """
     ページングされたレスポンスを返す API に対して、最後までデータを読み取り、結合した状態で返す。
     """
-    paging = get_paging_response_body_iter(get_func, query, pagination_token_key)
+    paging = get_paging_iter(get_func, query, pagination_token_key)
     first = next(paging)
 
     for page in paging:
         first.extend(page)
 
     return first
 
 
-async def aget_paging_response_body_iter(
+async def aget_paging_iter(
     get_func: Callable[
         [AnyQueryParameters],
         Coroutine[Any, Any, AnyPageResponseBody],
     ],
     query: Optional[AnyQueryParameters],
     pagination_token_key: str,
 ) -> AsyncGenerator[AnyPageResponseBody, None]:
@@ -95,25 +95,25 @@
 
         next_token = response_body.meta_next_token
 
         if next_token is None:
             return
 
 
-async def aget_collected_paging_response_body(
+async def aget_paging_all(
     get_func: Callable[
         [AnyQueryParameters],
         Coroutine[Any, Any, AnyPageResponseBody],
     ],
     query: Optional[AnyQueryParameters],
     pagination_token_key: str,
 ) -> AnyPageResponseBody:
     """
     ページングされたレスポンスを返す API に対して、最後までデータを読み取り、結合した状態で返す。
     """
-    paging = aget_paging_response_body_iter(get_func, query, pagination_token_key)
+    paging = aget_paging_iter(get_func, query, pagination_token_key)
     first = await paging.__anext__()
 
     async for page in paging:
         first.extend(page)
 
     return first
```

### Comparing `twitter_api_py-0.7.3/twitter_api/types/comma_separatable.py` & `twitter_api_py-0.8.0/twitter_api/types/comma_separatable.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/extra_permissive_model.py` & `twitter_api_py-0.8.0/twitter_api/types/extra_permissive_model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/http.py` & `twitter_api_py-0.8.0/twitter_api/types/http.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/httpx.py` & `twitter_api_py-0.8.0/twitter_api/types/httpx.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/oauth.py` & `twitter_api_py-0.8.0/twitter_api/types/oauth.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/oauth1/oauth1_access_token.py` & `twitter_api_py-0.8.0/twitter_api/types/oauth1/oauth1_access_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/oauth1/oauth1_authorization.py` & `twitter_api_py-0.8.0/twitter_api/types/oauth1/oauth1_authorization.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/oauth2/oauth2_access_token.py` & `twitter_api_py-0.8.0/twitter_api/types/oauth2/oauth2_access_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/oauth2/oauth2_authorization.py` & `twitter_api_py-0.8.0/twitter_api/types/oauth2/oauth2_authorization.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_dm_conversation/dm_conversation_message.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_dm_conversation/dm_conversation_message.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_language.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_language.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_media/media.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_media/media.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_media/media_field.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_media/media_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_place/place.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_place/place.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_place/place_country_code.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_place/place_country_code.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_poll/poll.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_poll/poll.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_retweet/retweet_entities_description.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_retweet/retweet_entities_description.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_scope.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_scope.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/_and_operator.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/_and_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/_not_operator.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/_not_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/_or_operator.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/_or_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/bounding_box_operator.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/bounding_box_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/context_operator.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/context_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/group_operator.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/group_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/keyword_operator.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/keyword_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/operator.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/place_operator.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/place_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/operators/point_radius_operator.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/operators/point_radius_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/search_query.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/search_query.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_search_query/search_query_builder.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_search_query/search_query_builder.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_entities.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_entities.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_expansion.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_expansion.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_field.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_tweet/tweet_response_body.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_tweet/tweet_response_body.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_user/user.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_user/user.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/types/v2_user/user_field.py` & `twitter_api_py-0.8.0/twitter_api/types/v2_user/user_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/utils/_functional.py` & `twitter_api_py-0.8.0/twitter_api/utils/_functional.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/utils/_oauth.py` & `twitter_api_py-0.8.0/twitter_api/utils/_oauth.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/utils/json.py` & `twitter_api_py-0.8.0/twitter_api/utils/json.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/twitter_api/warning.py` & `twitter_api_py-0.8.0/twitter_api/warning.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.3/PKG-INFO` & `twitter_api_py-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-py
-Version: 0.7.3
+Version: 0.8.0
 Summary: Twitter API Client by Typed Python.
 Home-page: https://github.com/yassun4dev/twitter-api-py
 License: BSD-3-Clause
 Author: yassun4dev
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

