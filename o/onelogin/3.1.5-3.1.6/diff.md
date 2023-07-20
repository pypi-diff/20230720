# Comparing `tmp/onelogin-3.1.5.tar.gz` & `tmp/onelogin-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onelogin-3.1.5.tar", last modified: Thu May 11 21:26:38 2023, max compression
+gzip compressed data, was "onelogin-3.1.6.tar", last modified: Thu Jul 20 18:22:35 2023, max compression
```

## Comparing `onelogin-3.1.5.tar` & `onelogin-3.1.6.tar`

### file list

```diff
@@ -1,388 +1,1019 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:26:38.762802 onelogin-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-11 21:26:38.762802 onelogin-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   100299 2023-05-11 21:26:26.000000 onelogin-3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:26:38.698801 onelogin-3.1.5/onelogin/
--rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:26:38.706801 onelogin-3.1.5/onelogin/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28353 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/api_auth_claims_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29286 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/api_auth_client_apps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28131 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/api_auth_scopes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32755 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/api_authorization_server_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    79163 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/app_rules_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    48923 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/apps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37636 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/branding_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/branding_service_smtp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57905 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/branding_service_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22235 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/groups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/invite_links_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    74904 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/multi_factor_authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    49416 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/multi_factor_authentication_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20597 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/o_auth2_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    70685 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/privileges_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   110315 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/roles_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28128 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/saml_assertions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    76539 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/smart_hooks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    78713 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/user_mappings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   117402 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/users_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55073 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/users_v2_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    51421 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api/vigilance_ai_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29944 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:26:38.738801 onelogin-3.1.5/onelogin/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/action_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/activate_mfa_factors_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/add_client_app201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/add_client_app_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/add_privilege_to_role201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/add_privilege_to_role_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/add_roles_to_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/alt_err.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/app_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/app_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/assign_users_to_privilege_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/auth_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/auth_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/auth_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/auth_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/auth_server_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/brand_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/brand_background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/brand_background_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/brand_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/brand_logo_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/brand_req.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/client_app_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/clock_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/configuration_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/configuration_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/create_app200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/create_app_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/create_device_verification201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/create_device_verification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/create_factor_registration201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/create_factor_registration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/create_privilege200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/create_role201_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/email_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/enforcement_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/enforcement_point_resources_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/enroll_mfa_factor200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    14697 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/generate_mf_atoken200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/generate_mf_atoken_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/generate_otp201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/generate_otp_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/generate_saml_assert200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/generate_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/generic_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/generic_app_provisioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_assigned_user200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_auth_factors200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_authentication_devices200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_custom_attributes200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_email_settings200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_email_settings200_response_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_enrolled_factors200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_enrolled_factors200_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_enrolled_factors200_response_data_otp_devices_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_event_by_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_event_types200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_event_types200_response_data_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_events200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_events200_response_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_groups200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_invite_link200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_invite_link_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_mfa_factors200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_mfa_factors200_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_mfa_factors200_response_data_auth_factors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_rate_limit200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_risk_score200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_risk_score_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_risk_scores200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_risk_scores200_response_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_role_apps200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_role_by_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_role_by_id200_response_data_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_role_by_name200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_role_by_name200_response_data_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_role_by_name200_response_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_user_apps200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_user_roles200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/get_user_verification200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/hook_envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/hook_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/hook_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/hook_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/list_conditions200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/list_mapping_action_values200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/list_mapping_conditions200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/list_mapping_conditions_operators200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/list_mapping_contion_values200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/list_mappings_actions200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/list_message_templates200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/list_privelege_roles200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/list_privilege_roles200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/lock_account_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/message_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/message_template_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/message_template_template_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/message_template_template_one_of1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/oauth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/oidc_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/oidc_app_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/otp_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/privilege.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/privilege_privilege.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/privilege_privilege_statement_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/remove_role_users_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/remove_user_role_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/remove_user_role_request_role_id_array_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/request_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/revoke_tokens_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/risk_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/risk_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/risk_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/rule_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/rule_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/saml_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/saml_app_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/saml_app_all_of_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/saml_app_all_of_parameters_saml_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/saml_assert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/saml_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/send_invite_link200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/send_invite_link_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/set_user_state_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/sso_saml_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/token_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/track_risk_event_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/update_client_app_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/update_environment_variable_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/update_password_insecure_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/update_password_secure_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/update_privilege200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/update_risk_rule_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/update_role200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/ver_factor_saml200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/verb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/verify_mfa_factor_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/verify_user_registration200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/verify_user_registration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/models/verify_user_verification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-11 21:26:26.000000 onelogin-3.1.5/onelogin/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:26:38.698801 onelogin-3.1.5/onelogin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-11 21:26:38.000000 onelogin-3.1.5/onelogin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-05-11 21:26:38.000000 onelogin-3.1.5/onelogin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:26:38.000000 onelogin-3.1.5/onelogin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 21:26:38.000000 onelogin-3.1.5/onelogin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 21:26:38.000000 onelogin-3.1.5/onelogin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-11 21:26:26.000000 onelogin-3.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 21:26:38.762802 onelogin-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-11 21:26:26.000000 onelogin-3.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:26:38.762802 onelogin-3.1.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_action_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_activate_mfa_factors_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_add_client_app201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_add_client_app_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_add_privilege_to_role201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_add_privilege_to_role_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_add_roles_to_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_alt_err.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_api_auth_claims_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_api_auth_client_apps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_api_auth_scopes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_api_authorization_server_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_app_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_app_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_app_rules_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_apps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_assign_users_to_privilege_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_auth_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_auth_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_auth_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_auth_server_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_brand_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_brand_background.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_brand_background_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_brand_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_brand_logo_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_brand_req.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_branding_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_branding_service_smtp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_branding_service_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_client_app_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_clock_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_configuration_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_configuration_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_create_app200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_create_app_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_create_device_verification201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_create_device_verification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_create_factor_registration201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_create_factor_registration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_create_privilege200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_create_role201_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_email_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_enforcement_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_enforcement_point_resources_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_enroll_mfa_factor200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_generate_mf_atoken200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_generate_mf_atoken_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_generate_otp201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_generate_otp_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_generate_saml_assert200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_generate_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_generic_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_generic_app_provisioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_assigned_user200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_auth_factors200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_authentication_devices200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_custom_attributes200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_email_settings200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_email_settings200_response_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_enrolled_factors200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_enrolled_factors200_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_enrolled_factors200_response_data_otp_devices_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_event_by_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_event_types200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_event_types200_response_data_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_events200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_events200_response_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_groups200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_invite_link200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_invite_link_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_mfa_factors200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_mfa_factors200_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_mfa_factors200_response_data_auth_factors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_rate_limit200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_risk_score200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_risk_score_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_risk_scores200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_risk_scores200_response_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_role_apps200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_role_by_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_role_by_id200_response_data_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_role_by_name200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_role_by_name200_response_data_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_role_by_name200_response_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_user_apps200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_user_roles200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_get_user_verification200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_hook_envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_hook_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_hook_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_hook_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_invite_links_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_list_conditions200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_list_mapping_action_values200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_list_mapping_conditions200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_list_mapping_conditions_operators200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_list_mapping_contion_values200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_list_mappings_actions200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_list_message_templates200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_list_privelege_roles200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_list_privilege_roles200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_lock_account_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_message_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_message_template_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_message_template_template_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_message_template_template_one_of1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_multi_factor_authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_multi_factor_authentication_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_o_auth2_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_oauth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_oidc_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_oidc_app_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_otp_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_privilege.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_privilege_privilege.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_privilege_privilege_statement_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_privileges_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_remove_role_users_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_remove_user_role_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_remove_user_role_request_role_id_array_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_request_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_revoke_tokens_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_risk_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_risk_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_risk_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_roles_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_rule_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_rule_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_saml_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_saml_app_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_saml_app_all_of_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_saml_app_all_of_parameters_saml_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_saml_assert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_saml_assertions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_saml_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_send_invite_link200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_send_invite_link_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_set_user_state_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_smart_hooks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_sso_saml_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_token_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_track_risk_event_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_update_client_app_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_update_environment_variable_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_update_password_insecure_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_update_password_secure_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_update_privilege200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_update_risk_rule_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_update_role200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_user_mappings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_users_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_users_v2_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_ver_factor_saml200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_verb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_verify_mfa_factor_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_verify_user_registration200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_verify_user_registration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_verify_user_verification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-11 21:26:26.000000 onelogin-3.1.5/test/test_vigilance_ai_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.404764 onelogin-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-20 18:22:35.404764 onelogin-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43820 2023-07-20 18:22:25.000000 onelogin-3.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.292762 onelogin-3.1.6/onelogin/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58440 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.296762 onelogin-3.1.6/onelogin/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/path_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.308762 onelogin-3.1.6/onelogin/apis/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_events_event_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_events_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_groups_group_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_invites_get_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_invites_send_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_privileges_privilege_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_privileges_privilege_id_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_privileges_privilege_id_roles_role_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_privileges_privilege_id_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_privileges_privilege_id_users_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_roles_role_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_saml_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_saml_assertion_verify_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_custom_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_set_password_clear_text_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_set_password_using_salt_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_add_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_auth_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_lock_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_mfa_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_otp_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_otp_devices_device_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_otp_devices_device_id_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_otp_devices_device_id_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_remove_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_1_users_user_id_set_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_api_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_api_authorizations_api_auth_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_api_authorizations_api_auth_id_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_api_authorizations_api_auth_id_claims_claim_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_api_authorizations_api_auth_id_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_api_authorizations_api_auth_id_clients_client_app_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_api_authorizations_api_auth_id_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_api_authorizations_api_auth_id_scopes_scope_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps_app_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps_app_id_parameters_parameter_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps_app_id_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps_app_id_rules_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps_app_id_rules_actions_rule_action_value_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps_app_id_rules_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps_app_id_rules_conditions_rule_condition_value_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps_app_id_rules_conditions_rule_condition_value_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps_app_id_rules_rule_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps_app_id_rules_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_apps_app_id_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_branding_brands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_branding_brands_brand_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_branding_brands_brand_id_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_branding_brands_brand_id_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_branding_brands_brand_id_templates_template_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_branding_brands_brand_id_templates_template_type_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_branding_brands_master_templates_template_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_branding_email_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_hooks_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_hooks_envs_envvar_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_hooks_hook_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_hooks_hook_id_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mappings_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mappings_actions_mapping_action_value_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mappings_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mappings_conditions_mapping_condition_value_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mappings_conditions_mapping_condition_value_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mappings_mapping_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mappings_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mfa_users_user_id_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mfa_users_user_id_devices_device_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mfa_users_user_id_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mfa_users_user_id_mfa_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mfa_users_user_id_registrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mfa_users_user_id_registrations_registration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mfa_users_user_id_verifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_mfa_users_user_id_verifications_verification_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_risk_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_risk_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_risk_rules_rule_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_risk_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_risk_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_roles_role_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_roles_role_id_admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_roles_role_id_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_roles_role_id_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_saml_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_saml_assertion_verify_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_users_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/api_2_users_user_id_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/auth_oauth2_revoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/auth_oauth2_v2_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/paths/auth_rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tag_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.312762 onelogin-3.1.6/onelogin/apis/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/api_auth_claims_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/api_auth_client_apps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/api_auth_scopes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/api_authorization_server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/app_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/apps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/branding_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/branding_service_smtp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/branding_service_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/invite_links_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/multi_factor_authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/multi_factor_authentication_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/o_auth2_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/privileges_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/saml_assertions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/smart_hooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/user_mappings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/users_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/users_v2_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/apis/tags/vigilance_ai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16658 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.320762 onelogin-3.1.6/onelogin/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/action_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/alt_err.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/app_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/app_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/auth_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/auth_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/auth_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/auth_server_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30787 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/brand_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/brand_req.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/client_app_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/clock_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/configuration_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/configuration_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/email_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/enforcement_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123473 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/generic_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/hook_envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/hook_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/hook_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19303 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/message_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/oauth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/oidc_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/otp_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37016 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/privilege.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/request_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/risk_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/risk_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/risk_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/rule_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/rule_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12290 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/saml_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/saml_assert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/saml_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/token_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25842 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/model/verb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.320762 onelogin-3.1.6/onelogin/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.320762 onelogin-3.1.6/onelogin/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.320762 onelogin-3.1.6/onelogin/paths/api_1_events/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_events/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.320762 onelogin-3.1.6/onelogin/paths/api_1_events_event_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_events_event_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_events_event_id/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.320762 onelogin-3.1.6/onelogin/paths/api_1_events_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_events_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_events_types/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.320762 onelogin-3.1.6/onelogin/paths/api_1_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_groups/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.320762 onelogin-3.1.6/onelogin/paths/api_1_groups_group_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_groups_group_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_groups_group_id/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.320762 onelogin-3.1.6/onelogin/paths/api_1_invites_get_invite_link/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_invites_get_invite_link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_invites_get_invite_link/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.320762 onelogin-3.1.6/onelogin/paths/api_1_invites_send_invite_link/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_invites_send_invite_link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_invites_send_invite_link/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.320762 onelogin-3.1.6/onelogin/paths/api_1_privileges/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_roles/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19729 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_roles/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_roles_role_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_roles_role_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_roles_role_id/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_users/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18563 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_users/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_users/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_users_user_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_users_user_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_privileges_privilege_id_users_user_id/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22173 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_roles/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_roles_role_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_roles_role_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_roles_role_id/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_saml_assertion/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_saml_assertion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_saml_assertion/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_saml_assertion_verify_factor/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_saml_assertion_verify_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_saml_assertion_verify_factor/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_users/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20466 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_users_custom_attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_custom_attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12756 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_custom_attributes/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.324763 onelogin-3.1.6/onelogin/paths/api_1_users_set_password_clear_text_user_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_set_password_clear_text_user_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_set_password_clear_text_user_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_set_password_using_salt_user_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_set_password_using_salt_user_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20338 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_set_password_using_salt_user_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19096 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_add_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_add_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19132 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_add_roles/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27101 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_apps/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_auth_factor/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_auth_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21362 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_auth_factor/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_lock_user/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_lock_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_lock_user/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_logout/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_logout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_logout/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_mfa_token/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_mfa_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_mfa_token/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27264 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27373 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices_device_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices_device_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices_device_id/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices_device_id_trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices_device_id_trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35361 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices_device_id_trigger/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices_device_id_verify/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices_device_id_verify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_otp_devices_device_id_verify/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.328763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_remove_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_remove_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22194 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_remove_roles/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.332763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14757 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_roles/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.332763 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_set_state/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_set_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_1_users_user_id_set_state/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.332763 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.332763 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12206 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17745 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.332763 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_claims/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_claims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_claims/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_claims/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.332763 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_claims_claim_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_claims_claim_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_claims_claim_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_claims_claim_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.332763 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_clients/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23420 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_clients/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.332763 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_clients_client_app_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_clients_client_app_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_clients_client_app_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23269 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_clients_client_app_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.332763 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_scopes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_scopes/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_scopes/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.332763 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_scopes_scope_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_scopes_scope_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_scopes_scope_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_api_authorizations_api_auth_id_scopes_scope_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19993 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14936 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_parameters_parameter_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_parameters_parameter_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_parameters_parameter_id/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_actions/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_actions_rule_action_value_values/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_actions_rule_action_value_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_actions_rule_action_value_values/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_conditions/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_conditions_rule_condition_value_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_conditions_rule_condition_value_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_conditions_rule_condition_value_operators/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_conditions_rule_condition_value_values/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_conditions_rule_condition_value_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_conditions_rule_condition_value_values/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_rule_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_rule_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_rule_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_rule_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_rule_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_sort/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_rules_sort/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_users/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_apps_app_id_users/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.336763 onelogin-3.1.6/onelogin/paths/api_2_branding_brands/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.340763 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.340763 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_apps/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.340763 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16862 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17642 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.340763 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates_template_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates_template_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates_template_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates_template_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates_template_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.340763 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates_template_type_locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates_template_type_locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates_template_type_locale/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_brand_id_templates_template_type_locale/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.340763 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_master_templates_template_type/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_master_templates_template_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10845 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_brands_master_templates_template_type/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.340763 onelogin-3.1.6/onelogin/paths/api_2_branding_email_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_email_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_email_settings/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_email_settings/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_branding_email_settings/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.340763 onelogin-3.1.6/onelogin/paths/api_2_connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_connectors/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.340763 onelogin-3.1.6/onelogin/paths/api_2_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12996 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_hooks_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_envs/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_envs/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_hooks_envs_envvar_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_envs_envvar_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_envs_envvar_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_envs_envvar_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17581 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_envs_envvar_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_hooks_hook_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_hook_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_hook_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10654 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_hook_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_hook_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_hooks_hook_id_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_hook_id_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_hooks_hook_id_logs/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_mappings_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_actions/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_mappings_actions_mapping_action_value_values/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_actions_mapping_action_value_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13995 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_actions_mapping_action_value_values/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_mappings_conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_conditions/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_mappings_conditions_mapping_condition_value_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_conditions_mapping_condition_value_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_conditions_mapping_condition_value_operators/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_mappings_conditions_mapping_condition_value_values/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_conditions_mapping_condition_value_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_conditions_mapping_condition_value_values/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_mappings_mapping_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_mapping_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_mapping_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_mapping_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17562 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_mapping_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.344763 onelogin-3.1.6/onelogin/paths/api_2_mappings_sort/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mappings_sort/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15791 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_devices/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_devices_device_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_devices_device_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_devices_device_id/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_factors/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_factors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_factors/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_mfa_token/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_mfa_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23558 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_mfa_token/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_registrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_registrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28524 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_registrations/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_registrations_registration_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_registrations_registration_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_registrations_registration_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23882 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_registrations_registration_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_verifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_verifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27527 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_verifications/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_verifications_verification_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_verifications_verification_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_verifications_verification_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20635 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_mfa_users_user_id_verifications_verification_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_risk_events/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_events/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_risk_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_rules/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_rules/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_risk_rules_rule_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_rules_rule_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_rules_rule_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_rules_rule_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17060 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_rules_rule_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.348763 onelogin-3.1.6/onelogin/paths/api_2_risk_scores/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_scores/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.352763 onelogin-3.1.6/onelogin/paths/api_2_risk_verify/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_verify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23707 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_risk_verify/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.352763 onelogin-3.1.6/onelogin/paths/api_2_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.352763 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16566 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.352763 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_admins/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_admins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_admins/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_admins/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_admins/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.352763 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_apps/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_apps/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.352763 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_users/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17432 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_users/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_users/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_roles_role_id_users/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.352763 onelogin-3.1.6/onelogin/paths/api_2_saml_assertion/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_saml_assertion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18102 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_saml_assertion/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.352763 onelogin-3.1.6/onelogin/paths/api_2_saml_assertion_verify_factor/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_saml_assertion_verify_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_saml_assertion_verify_factor/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.352763 onelogin-3.1.6/onelogin/paths/api_2_users/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18327 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_users/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16341 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_users/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.356763 onelogin-3.1.6/onelogin/paths/api_2_users_user_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_users_user_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_users_user_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_users_user_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19048 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_users_user_id/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.356763 onelogin-3.1.6/onelogin/paths/api_2_users_user_id_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_users_user_id_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27106 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/api_2_users_user_id_apps/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.356763 onelogin-3.1.6/onelogin/paths/auth_oauth2_revoke/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/auth_oauth2_revoke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/auth_oauth2_revoke/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.356763 onelogin-3.1.6/onelogin/paths/auth_oauth2_v2_token/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/auth_oauth2_v2_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/auth_oauth2_v2_token/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.356763 onelogin-3.1.6/onelogin/paths/auth_rate_limit/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/auth_rate_limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/paths/auth_rate_limit/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97602 2023-07-20 18:22:25.000000 onelogin-3.1.6/onelogin/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.296762 onelogin-3.1.6/onelogin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-20 18:22:35.000000 onelogin-3.1.6/onelogin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42715 2023-07-20 18:22:35.000000 onelogin-3.1.6/onelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:22:35.000000 onelogin-3.1.6/onelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 18:22:35.000000 onelogin-3.1.6/onelogin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 18:22:35.000000 onelogin-3.1.6/onelogin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 18:22:35.404764 onelogin-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 18:22:25.000000 onelogin-3.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.284762 onelogin-3.1.6/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.368763 onelogin-3.1.6/test/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_action_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_alt_err.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_app_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_app_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_auth_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_auth_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_auth_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_auth_server_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_brand_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_brand_req.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_client_app_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_clock_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_configuration_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_configuration_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_email_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_enforcement_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_generic_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_hook_envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_hook_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_hook_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_message_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_oauth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_oidc_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_otp_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_request_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_risk_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_risk_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_risk_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_rule_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_rule_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_saml_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_saml_assert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_saml_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_token_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_models/test_verb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.368763 onelogin-3.1.6/test/test_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.368763 onelogin-3.1.6/test/test_paths/test_api_1_events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_events/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.368763 onelogin-3.1.6/test/test_paths/test_api_1_events_event_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_events_event_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_events_event_id/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.368763 onelogin-3.1.6/test/test_paths/test_api_1_events_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_events_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_events_types/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.368763 onelogin-3.1.6/test/test_paths/test_api_1_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_groups/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.368763 onelogin-3.1.6/test/test_paths/test_api_1_groups_group_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_groups_group_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_groups_group_id/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.368763 onelogin-3.1.6/test/test_paths/test_api_1_invites_get_invite_link/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_invites_get_invite_link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_invites_get_invite_link/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.368763 onelogin-3.1.6/test/test_paths/test_api_1_invites_send_invite_link/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_invites_send_invite_link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_invites_send_invite_link/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.368763 onelogin-3.1.6/test/test_paths/test_api_1_privileges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.368763 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.372763 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_roles/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_roles/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.372763 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_roles_role_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_roles_role_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_roles_role_id/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.372763 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_users/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_users/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.372763 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_users_user_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_users_user_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_users_user_id/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.372763 onelogin-3.1.6/test/test_paths/test_api_1_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_roles/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.372763 onelogin-3.1.6/test/test_paths/test_api_1_roles_role_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_roles_role_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_roles_role_id/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.372763 onelogin-3.1.6/test/test_paths/test_api_1_saml_assertion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_saml_assertion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_saml_assertion/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.372763 onelogin-3.1.6/test/test_paths/test_api_1_saml_assertion_verify_factor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_saml_assertion_verify_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_saml_assertion_verify_factor/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.372763 onelogin-3.1.6/test/test_paths/test_api_1_users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.372763 onelogin-3.1.6/test/test_paths/test_api_1_users_custom_attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_custom_attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_custom_attributes/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.372763 onelogin-3.1.6/test/test_paths/test_api_1_users_set_password_clear_text_user_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_set_password_clear_text_user_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_set_password_clear_text_user_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.376763 onelogin-3.1.6/test/test_paths/test_api_1_users_set_password_using_salt_user_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_set_password_using_salt_user_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_set_password_using_salt_user_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.376763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.376763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_add_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_add_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_add_roles/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.376763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_apps/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.376763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_auth_factor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_auth_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_auth_factor/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.376763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_lock_user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_lock_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_lock_user/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.376763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_logout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_logout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_logout/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.376763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_mfa_token/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_mfa_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_mfa_token/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.376763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.376763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices_device_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices_device_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices_device_id/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.376763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices_device_id_trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices_device_id_trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices_device_id_trigger/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.380763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices_device_id_verify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices_device_id_verify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_otp_devices_device_id_verify/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.380763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_remove_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_remove_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_remove_roles/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.380763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_roles/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.380763 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_set_state/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_set_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_set_state/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.380763 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.380763 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.380763 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_claims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_claims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_claims/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_claims/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.380763 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_claims_claim_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_claims_claim_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_claims_claim_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_claims_claim_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.380763 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_clients/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_clients/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.384763 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_clients_client_app_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_clients_client_app_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_clients_client_app_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_clients_client_app_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.384763 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_scopes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_scopes/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_scopes/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.384763 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_scopes_scope_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_scopes_scope_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_scopes_scope_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_scopes_scope_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.384763 onelogin-3.1.6/test/test_paths/test_api_2_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.384763 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.384763 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_parameters_parameter_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_parameters_parameter_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_parameters_parameter_id/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.384763 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.384763 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_actions/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.384763 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_actions_rule_action_value_values/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_actions_rule_action_value_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_actions_rule_action_value_values/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.384763 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_conditions/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.388764 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_conditions_rule_condition_value_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_conditions_rule_condition_value_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_conditions_rule_condition_value_operators/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.388764 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_conditions_rule_condition_value_values/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_conditions_rule_condition_value_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_conditions_rule_condition_value_values/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.388764 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_rule_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_rule_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_rule_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_rule_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_rule_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.388764 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_sort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_rules_sort/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.388764 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_users/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.388764 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.388764 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.388764 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_apps/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.388764 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates_template_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates_template_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates_template_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates_template_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates_template_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates_template_type_locale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates_template_type_locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates_template_type_locale/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id_templates_template_type_locale/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_master_templates_template_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_master_templates_template_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_master_templates_template_type/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_branding_email_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_email_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_email_settings/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_email_settings/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_branding_email_settings/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_connectors/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_hooks_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_envs/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_envs/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_hooks_envs_envvar_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_envs_envvar_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_envs_envvar_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_envs_envvar_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_envs_envvar_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_hooks_hook_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_hook_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_hook_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_hook_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_hook_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_hooks_hook_id_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_hook_id_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_hooks_hook_id_logs/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_mappings_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_actions/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.392763 onelogin-3.1.6/test/test_paths/test_api_2_mappings_actions_mapping_action_value_values/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_actions_mapping_action_value_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_actions_mapping_action_value_values/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mappings_conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_conditions/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mappings_conditions_mapping_condition_value_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_conditions_mapping_condition_value_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_conditions_mapping_condition_value_operators/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mappings_conditions_mapping_condition_value_values/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_conditions_mapping_condition_value_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_conditions_mapping_condition_value_values/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mappings_mapping_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_mapping_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_mapping_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_mapping_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_mapping_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mappings_sort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mappings_sort/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_devices/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_devices_device_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_devices_device_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_devices_device_id/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_factors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_factors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_factors/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_mfa_token/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_mfa_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_mfa_token/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_registrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_registrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_registrations/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_registrations_registration_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_registrations_registration_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_registrations_registration_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_registrations_registration_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_verifications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_verifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_verifications/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_verifications_verification_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_verifications_verification_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_verifications_verification_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_verifications_verification_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_risk_events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_events/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_risk_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_rules/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_rules/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.396763 onelogin-3.1.6/test/test_paths/test_api_2_risk_rules_rule_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_rules_rule_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_rules_rule_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_rules_rule_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_rules_rule_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.400764 onelogin-3.1.6/test/test_paths/test_api_2_risk_scores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_scores/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.400764 onelogin-3.1.6/test/test_paths/test_api_2_risk_verify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_verify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_risk_verify/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.400764 onelogin-3.1.6/test/test_paths/test_api_2_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.400764 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.400764 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_admins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_admins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_admins/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_admins/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_admins/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.400764 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_apps/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_apps/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.400764 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_users/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_users/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_roles_role_id_users/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.400764 onelogin-3.1.6/test/test_paths/test_api_2_saml_assertion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_saml_assertion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_saml_assertion/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.400764 onelogin-3.1.6/test/test_paths/test_api_2_saml_assertion_verify_factor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_saml_assertion_verify_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_saml_assertion_verify_factor/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.404764 onelogin-3.1.6/test/test_paths/test_api_2_users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_users/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_users/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.404764 onelogin-3.1.6/test/test_paths/test_api_2_users_user_id/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_users_user_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_users_user_id/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_users_user_id/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_users_user_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.404764 onelogin-3.1.6/test/test_paths/test_api_2_users_user_id_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_users_user_id_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_api_2_users_user_id_apps/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.404764 onelogin-3.1.6/test/test_paths/test_auth_oauth2_revoke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_auth_oauth2_revoke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_auth_oauth2_revoke/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.404764 onelogin-3.1.6/test/test_paths/test_auth_oauth2_v2_token/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_auth_oauth2_v2_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_auth_oauth2_v2_token/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:35.404764 onelogin-3.1.6/test/test_paths/test_auth_rate_limit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_auth_rate_limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-20 18:22:25.000000 onelogin-3.1.6/test/test_paths/test_auth_rate_limit/test_get.py
```

### Comparing `onelogin-3.1.5/onelogin/configuration.py` & `onelogin-3.1.6/onelogin/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,84 @@
-
 # coding: utf-8
 
 """
     OneLogin API
 
     OpenAPI Specification for OneLogin  # noqa: E501
 
     The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-import http.client as httplib
+from http import client as http_client
 from onelogin.exceptions import ApiValueError
 
+
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems'
+    'minLength', 'pattern', 'maxItems', 'minItems',
+    'uniqueItems', 'maxProperties', 'minProperties',
 }
 
 class Configuration(object):
-    """This class contains various settings of the API client.
+    """NOTE: This class is auto generated by OpenAPI Generator
 
-    :param host: Base url.
+    Ref: https://openapi-generator.tech
+    Do not edit the class manually.
+
+    :param host: Base url
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication.
-    :param password: Password for HTTP basic authentication.
-    :param access_token: Access token.
+    :param username: Username for HTTP basic authentication
+    :param password: Password for HTTP basic authentication
+    :param discard_unknown_keys: Boolean value indicating whether to discard
+      unknown properties. A server may send a response that includes additional
+      properties that are not known by the client in the following scenarios:
+      1. The OpenAPI document is incomplete, i.e. it does not match the server
+         implementation.
+      2. The client was generated using an older version of the OpenAPI document
+         and the server has been upgraded since then.
+      If a schema in the OpenAPI document defines the additionalProperties attribute,
+      then all undeclared properties received by the server are injected into the
+      additional properties map. In that case, there are undeclared properties, and
+      nothing to discard.
+    :param disabled_client_side_validations (string): Comma-separated list of
+      JSON schema validation keywords to disable JSON schema structural validation
+      rules. The following keywords may be specified: multipleOf, maximum,
+      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
+      maxItems, minItems.
+      By default, the validation is performed for data generated locally by the client
+      and data received from the server, independent of any validation performed by
+      the server side. If the input data does not satisfy the JSON schema validation
+      rules specified in the OpenAPI document, an exception is raised.
+      If disabled_client_side_validations is set, structural validation is
+      disabled. This can be useful to troubleshoot data validation problem, such as
+      when the OpenAPI document validation rules do not match the actual API data
+      received by the server.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
-    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
-      in PEM format.
 
     :Example:
 
     HTTP Basic Authentication Example.
     Given the following security scheme in the OpenAPI specification:
       components:
         securitySchemes:
@@ -71,22 +93,27 @@
     password='the-password',
 )
 
     """
 
     _default = None
 
-    def __init__(self, host=None,
-                 api_key=None, api_key_prefix=None,
-                 username=None, password=None,
-                 access_token=None,
-                 server_index=None, server_variables=None,
-                 server_operation_index=None, server_operation_variables=None,
-                 ssl_ca_cert=None,
-                 ):
+    def __init__(
+        self,
+        host=None,
+        username=None,
+        password=None,
+        discard_unknown_keys=False,
+        disabled_client_side_validations="",
+        server_index=None,
+        server_variables=None,
+        server_operation_index=None,
+        server_operation_variables=None,
+        access_token=None,
+    ):
         """Constructor
         """
         self._base_path = "https://your-api-subdomain.onelogin.com" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
@@ -96,36 +123,22 @@
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.api_key = {}
-        if api_key:
-            self.api_key = api_key
-        """dict to store API key(s)
-        """
-        self.api_key_prefix = {}
-        if api_key_prefix:
-            self.api_key_prefix = api_key_prefix
-        """dict to store API prefix (e.g. Bearer)
-        """
-        self.refresh_api_key_hook = None
-        """function hook to refresh API key if expired
-        """
         self.username = username
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
-        self.access_token = access_token
-        """Access token
-        """
+        self.discard_unknown_keys = discard_unknown_keys
+        self.disabled_client_side_validations = disabled_client_side_validations
         self.access_token = None
         """access token for OAuth/Bearer
         """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("onelogin")
@@ -147,15 +160,15 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = ssl_ca_cert
+        self.ssl_ca_cert = None
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -187,25 +200,16 @@
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
+        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
-        """Options to pass down to the underlying urllib3 socket
-        """
-
-        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
-        """datetime format
-        """
-
-        self.date_format = "%Y-%m-%d"
-        """date format
-        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
@@ -215,49 +219,46 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
+        if name == 'disabled_client_side_validations':
+            s = set(filter(None, value.split(',')))
+            for v in s:
+                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
+                    raise ApiValueError(
+                        "Invalid keyword: '{0}''".format(v))
+            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = default
+        cls._default = copy.deepcopy(default)
 
     @classmethod
     def get_default_copy(cls):
-        """Deprecated. Please use `get_default` instead.
-
-        Deprecated. Please use `get_default` instead.
-
-        :return: The configuration object.
-        """
-        return cls.get_default()
-
-    @classmethod
-    def get_default(cls):
-        """Return the default configuration.
+        """Return new instance of configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration.
+        configuration passed by the set_default method.
 
         :return: The configuration object.
         """
-        if cls._default is None:
-            cls._default = Configuration()
-        return cls._default
+        if cls._default is not None:
+            return copy.deepcopy(cls._default)
+        return Configuration()
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -303,23 +304,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on httplib debug
-            httplib.HTTPConnection.debuglevel = 1
+            # turn on http_client debug
+            http_client.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off httplib debug
-            httplib.HTTPConnection.debuglevel = 0
+            # turn off http_client debug
+            http_client.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -399,15 +400,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.1.1\n"\
-               "SDK Package Version: 3.1.5".\
+               "SDK Package Version: 3.1.6".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `onelogin-3.1.5/onelogin/exceptions.py` & `onelogin-3.1.6/onelogin/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 """
     OneLogin API
 
     OpenAPI Specification for OneLogin  # noqa: E501
 
     The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
+import dataclasses
+import typing
+
+from urllib3._collections import HTTPHeaderDict
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
@@ -95,27 +97,34 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
-class ApiException(OpenApiException):
+T = typing.TypeVar("T")
 
-    def __init__(self, status=None, reason=None, http_resp=None):
-        if http_resp:
-            self.status = http_resp.status
-            self.reason = http_resp.reason
-            self.body = http_resp.data
-            self.headers = http_resp.getheaders()
-        else:
-            self.status = status
-            self.reason = reason
-            self.body = None
-            self.headers = None
+
+@dataclasses.dataclass
+class ApiException(OpenApiException, typing.Generic[T]):
+    status: int
+    reason: str
+    api_response: typing.Optional[T] = None
+
+    @property
+    def body(self) -> typing.Union[str, bytes, None]:
+        if not self.api_response:
+            return None
+        return self.api_response.response.data
+
+    @property
+    def headers(self) -> typing.Optional[HTTPHeaderDict]:
+        if not self.api_response:
+            return None
+        return self.api_response.response.getheaders()
 
     def __str__(self):
         """Custom error messages for exception"""
         error_message = "({0})\n"\
                         "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(
@@ -123,38 +132,14 @@
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
-class NotFoundException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(NotFoundException, self).__init__(status, reason, http_resp)
-
-
-class UnauthorizedException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(UnauthorizedException, self).__init__(status, reason, http_resp)
-
-
-class ForbiddenException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ForbiddenException, self).__init__(status, reason, http_resp)
-
-
-class ServiceException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ServiceException, self).__init__(status, reason, http_resp)
-
-
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
             result += "[{0}]".format(pth)
         else:
```

### Comparing `onelogin-3.1.5/setup.py` & `onelogin-3.1.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,44 +2,46 @@
 
 """
     OneLogin API
 
     OpenAPI Specification for OneLogin  # noqa: E501
 
     The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 from setuptools import setup, find_packages  # noqa: H301
 
+NAME = "onelogin"
+VERSION = "3.1.6"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
-NAME = "onelogin"
-VERSION = "3.1.5"
 
-PYTHON_REQUIRES = ">=3.7"
-with open("requirements.txt") as f:
-    requirements = f.read().splitlines()
+REQUIRES = [
+    "certifi >= 14.5.14",
+    "frozendict ~= 2.3.4",
+    "python-dateutil ~= 2.7.0",
+    "setuptools >= 21.0.0",
+    "typing_extensions ~= 4.3.0",
+    "urllib3 ~= 1.26.7",
+]
 
 setup(
     name=NAME,
     version=VERSION,
     description="OneLogin API",
     author="OneLogin",
     author_email="team@openapitools.org",
     url="",
     keywords=["OpenAPI", "OpenAPI-Generator", "OneLogin API"],
-    install_requires=requirements,
+    python_requires=">=3.7",
+    install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
-    long_description_content_type='text/markdown',
     long_description="""\
     OpenAPI Specification for OneLogin  # noqa: E501
     """
 )
```

### Comparing `onelogin-3.1.5/test/test_action_obj.py` & `onelogin-3.1.6/test/test_paths/test_api_2_mappings_actions_mapping_action_value_values/test_get.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.action_obj import ActionObj  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_mappings_actions_mapping_action_value_values import get  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
+
 
-class TestActionObj(unittest.TestCase):
-    """ActionObj unit test stubs"""
+class TestApi2MappingsActionsMappingActionValueValues(ApiTestMixin, unittest.TestCase):
+    """
+    Api2MappingsActionsMappingActionValueValues unit test stubs
+        List Actions Values  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test ActionObj
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `ActionObj`
-        """
-        model = onelogin.models.action_obj.ActionObj()  # noqa: E501
-        if include_optional :
-            return ActionObj(
-                action = '', 
-                value = [
-                    '2'
-                    ]
-            )
-        else :
-            return ActionObj(
-        )
-        """
-
-    def testActionObj(self):
-        """Test ActionObj"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_alt_err.py` & `onelogin-3.1.6/test/test_paths/test_api_2_saml_assertion_verify_factor/test_post.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.alt_err import AltErr  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_saml_assertion_verify_factor import post  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
+
 
-class TestAltErr(unittest.TestCase):
-    """AltErr unit test stubs"""
+class TestApi2SamlAssertionVerifyFactor(ApiTestMixin, unittest.TestCase):
+    """
+    Api2SamlAssertionVerifyFactor unit test stubs
+        Verify Factor SAML  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test AltErr
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `AltErr`
-        """
-        model = onelogin.models.alt_err.AltErr()  # noqa: E501
-        if include_optional :
-            return AltErr(
-                status_code = 200, 
-                name = 'Success', 
-                message = 'Settings Updated'
-            )
-        else :
-            return AltErr(
-        )
-        """
-
-    def testAltErr(self):
-        """Test AltErr"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_api_auth_claims_api.py` & `onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_clients_client_app_id/test_delete.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.api.api_auth_claims_api import APIAuthClaimsApi  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_api_authorizations_api_auth_id_clients_client_app_id import delete  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
 
-class TestAPIAuthClaimsApi(unittest.TestCase):
-    """APIAuthClaimsApi unit test stubs"""
+class TestApi2ApiAuthorizationsApiAuthIdClientsClientAppId(ApiTestMixin, unittest.TestCase):
+    """
+    Api2ApiAuthorizationsApiAuthIdClientsClientAppId unit test stubs
+        Remove Client App  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        self.api = onelogin.api.api_auth_claims_api.APIAuthClaimsApi()  # noqa: E501
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_create_auth_claim(self):
-        """Test case for create_auth_claim
+    response_status = 200
 
-        Create Api Auth Server Claim  # noqa: E501
-        """
-        pass
-
-    def test_delete_auth_claim(self):
-        """Test case for delete_auth_claim
 
-        Delete Api Auth Server Claim  # noqa: E501
-        """
-        pass
-
-    def test_get_authclaims(self):
-        """Test case for get_authclaims
-
-        Get Api Auth Server claims  # noqa: E501
-        """
-        pass
-
-    def test_update_claim(self):
-        """Test case for update_claim
-
-        Update Api Auth Server Claim  # noqa: E501
-        """
-        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_api_auth_client_apps_api.py` & `onelogin-3.1.6/onelogin/apis/tags/api_auth_client_apps_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,60 +2,28 @@
 
 """
     OneLogin API
 
     OpenAPI Specification for OneLogin  # noqa: E501
 
     The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
+from onelogin.paths.api_2_api_authorizations_api_auth_id_clients.post import AddClientApp
+from onelogin.paths.api_2_api_authorizations_api_auth_id_clients_client_app_id.delete import DeleteClientApp
+from onelogin.paths.api_2_api_authorizations_api_auth_id_clients.get import ListClientApps
+from onelogin.paths.api_2_api_authorizations_api_auth_id_clients_client_app_id.put import UpdateClientApp
 
-import unittest
-
-import onelogin
-from onelogin.api.api_auth_client_apps_api import APIAuthClientAppsApi  # noqa: E501
-from onelogin.rest import ApiException
-
-
-class TestAPIAuthClientAppsApi(unittest.TestCase):
-    """APIAuthClientAppsApi unit test stubs"""
-
-    def setUp(self):
-        self.api = onelogin.api.api_auth_client_apps_api.APIAuthClientAppsApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_add_client_app(self):
-        """Test case for add_client_app
 
-        Add Client App  # noqa: E501
-        """
-        pass
+class APIAuthClientAppsApi(
+    AddClientApp,
+    DeleteClientApp,
+    ListClientApps,
+    UpdateClientApp,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
 
-    def test_delete_client_app(self):
-        """Test case for delete_client_app
-
-        Remove Client App  # noqa: E501
-        """
-        pass
-
-    def test_list_client_apps(self):
-        """Test case for list_client_apps
-
-        List Clients Apps  # noqa: E501
-        """
-        pass
-
-    def test_update_client_app(self):
-        """Test case for update_client_app
-
-        Update Client App  # noqa: E501
-        """
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+    Do not edit the class manually.
+    """
+    pass
```

### Comparing `onelogin-3.1.5/test/test_api_auth_scopes_api.py` & `onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_scopes_scope_id/test_delete.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,40 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
+from unittest.mock import patch
 
-import onelogin
-from onelogin.api.api_auth_scopes_api import APIAuthScopesApi  # noqa: E501
-from onelogin.rest import ApiException
-
-
-class TestAPIAuthScopesApi(unittest.TestCase):
-    """APIAuthScopesApi unit test stubs"""
+import urllib3
 
-    def setUp(self):
-        self.api = onelogin.api.api_auth_scopes_api.APIAuthScopesApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_create_scope(self):
-        """Test case for create_scope
+import onelogin
+from onelogin.paths.api_2_api_authorizations_api_auth_id_scopes_scope_id import delete  # noqa: E501
+from onelogin import configuration, schemas, api_client
 
-        Create Api Auth Server Scope  # noqa: E501
-        """
-        pass
+from .. import ApiTestMixin
 
-    def test_delete_scope(self):
-        """Test case for delete_scope
 
+class TestApi2ApiAuthorizationsApiAuthIdScopesScopeId(ApiTestMixin, unittest.TestCase):
+    """
+    Api2ApiAuthorizationsApiAuthIdScopesScopeId unit test stubs
         Delete Api Auth Server Scope  # noqa: E501
-        """
-        pass
+    """
+    _configuration = configuration.Configuration()
 
-    def test_get_scopes(self):
-        """Test case for get_scopes
+    def setUp(self):
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
-        Get Api Auth Server Scopes  # noqa: E501
-        """
+    def tearDown(self):
         pass
 
-    def test_update_scope(self):
-        """Test case for update_scope
-
-        Update Api Auth Server Scope  # noqa: E501
-        """
-        pass
+    response_status = 204
+    response_body = ''
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_auth_id.py` & `onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id/test_delete.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,40 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.auth_id import AuthId  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_1_privileges_privilege_id import delete  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
-class TestAuthId(unittest.TestCase):
-    """AuthId unit test stubs"""
+
+class TestApi1PrivilegesPrivilegeId(ApiTestMixin, unittest.TestCase):
+    """
+    Api1PrivilegesPrivilegeId unit test stubs
+        Delete a Privilege  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test AuthId
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `AuthId`
-        """
-        model = onelogin.models.auth_id.AuthId()  # noqa: E501
-        if include_optional :
-            return AuthId(
-                id = 323005
-            )
-        else :
-            return AuthId(
-        )
-        """
-
-    def testAuthId(self):
-        """Test AuthId"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    response_status = 204
+    response_body = ''
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_auth_method.py` & `onelogin-3.1.6/test/test_paths/test_api_1_users_user_id_apps/test_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.auth_method import AuthMethod  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_1_users_user_id_apps import get  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
+
 
-class TestAuthMethod(unittest.TestCase):
-    """AuthMethod unit test stubs"""
+class TestApi1UsersUserIdApps(ApiTestMixin, unittest.TestCase):
+    """
+    Api1UsersUserIdApps unit test stubs
+        Get Apps for a User  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testAuthMethod(self):
-        """Test AuthMethod"""
-        # inst = AuthMethod()
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_branding_service_smtp_api.py` & `onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id/test_delete.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,40 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.api.branding_service_smtp_api import BrandingServiceSMTPApi  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_branding_brands_brand_id import delete  # noqa: E501
+from onelogin import configuration, schemas, api_client
 
+from .. import ApiTestMixin
 
-class TestBrandingServiceSMTPApi(unittest.TestCase):
-    """BrandingServiceSMTPApi unit test stubs"""
+
+class TestApi2BrandingBrandsBrandId(ApiTestMixin, unittest.TestCase):
+    """
+    Api2BrandingBrandsBrandId unit test stubs
+        Delete Brand  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        self.api = onelogin.api.branding_service_smtp_api.BrandingServiceSMTPApi()  # noqa: E501
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_delete_email_settings(self):
-        """Test case for delete_email_settings
-
-        Delete Custom Email Settings  # noqa: E501
-        """
-        pass
-
-    def test_get_email_settings(self):
-        """Test case for get_email_settings
-
-        Get Email Settings  # noqa: E501
-        """
-        pass
-
-    def test_update_email_settings(self):
-        """Test case for update_email_settings
-
-        Update Email Settings  # noqa: E501
-        """
-        pass
+    response_status = 204
+    response_body = ''
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_condition.py` & `onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_roles/test_get.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.condition import Condition  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_1_privileges_privilege_id_roles import get  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
+
 
-class TestCondition(unittest.TestCase):
-    """Condition unit test stubs"""
+class TestApi1PrivilegesPrivilegeIdRoles(ApiTestMixin, unittest.TestCase):
+    """
+    Api1PrivilegesPrivilegeIdRoles unit test stubs
+        Get Roles assigned to Privilege  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test Condition
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `Condition`
-        """
-        model = onelogin.models.condition.Condition()  # noqa: E501
-        if include_optional :
-            return Condition(
-                source = 'last_login', 
-                operator = '>', 
-                value = '90'
-            )
-        else :
-            return Condition(
-        )
-        """
-
-    def testCondition(self):
-        """Test Condition"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_configuration_saml.py` & `onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id_parameters_parameter_id/test_delete.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,40 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.configuration_saml import ConfigurationSaml  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_apps_app_id_parameters_parameter_id import delete  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
-class TestConfigurationSaml(unittest.TestCase):
-    """ConfigurationSaml unit test stubs"""
+
+class TestApi2AppsAppIdParametersParameterId(ApiTestMixin, unittest.TestCase):
+    """
+    Api2AppsAppIdParametersParameterId unit test stubs
+        Delete Parameter from App  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test ConfigurationSaml
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `ConfigurationSaml`
-        """
-        model = onelogin.models.configuration_saml.ConfigurationSaml()  # noqa: E501
-        if include_optional :
-            return ConfigurationSaml(
-                signature_algorithm = 'SHA-512', 
-                certificate_id = 123456
-            )
-        else :
-            return ConfigurationSaml(
-        )
-        """
-
-    def testConfigurationSaml(self):
-        """Test ConfigurationSaml"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    response_status = 204
+    response_body = ''
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_device.py` & `onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_registrations_registration_id/test_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.device import Device  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_mfa_users_user_id_registrations_registration_id import get  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
+
 
-class TestDevice(unittest.TestCase):
-    """Device unit test stubs"""
+class TestApi2MfaUsersUserIdRegistrationsRegistrationId(ApiTestMixin, unittest.TestCase):
+    """
+    Api2MfaUsersUserIdRegistrationsRegistrationId unit test stubs
+        Get User Registration  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test Device
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `Device`
-        """
-        model = onelogin.models.device.Device()  # noqa: E501
-        if include_optional :
-            return Device(
-                device_id = 654984, 
-                device_type = 'Google Authenticator'
-            )
-        else :
-            return Device(
-        )
-        """
-
-    def testDevice(self):
-        """Test Device"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_events_api.py` & `onelogin-3.1.6/test/test_paths/test_auth_rate_limit/test_get.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.api.events_api import EventsApi  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.auth_rate_limit import get  # noqa: E501
+from onelogin import configuration, schemas, api_client
 
+from .. import ApiTestMixin
 
-class TestEventsApi(unittest.TestCase):
-    """EventsApi unit test stubs"""
+
+class TestAuthRateLimit(ApiTestMixin, unittest.TestCase):
+    """
+    AuthRateLimit unit test stubs
+        Get Rate Limit  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        self.api = onelogin.api.events_api.EventsApi()  # noqa: E501
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_get_event_by_id(self):
-        """Test case for get_event_by_id
-
-        Get Event by ID  # noqa: E501
-        """
-        pass
-
-    def test_get_event_types(self):
-        """Test case for get_event_types
+    response_status = 200
 
-        Get Event Types  # noqa: E501
-        """
-        pass
 
-    def test_get_events(self):
-        """Test case for get_events
-
-        Get Events  # noqa: E501
-        """
-        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_group.py` & `onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id/test_delete.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,40 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.group import Group  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_api_authorizations_api_auth_id import delete  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
-class TestGroup(unittest.TestCase):
-    """Group unit test stubs"""
+
+class TestApi2ApiAuthorizationsApiAuthId(ApiTestMixin, unittest.TestCase):
+    """
+    Api2ApiAuthorizationsApiAuthId unit test stubs
+        Delete Api Auth Server  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test Group
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `Group`
-        """
-        model = onelogin.models.group.Group()  # noqa: E501
-        if include_optional :
-            return Group(
-                id = 425741, 
-                name = 'group.security.policy.default', 
-                reference = 'null'
-            )
-        else :
-            return Group(
-        )
-        """
-
-    def testGroup(self):
-        """Test Group"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    response_status = 204
+    response_body = ''
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_groups_api.py` & `onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id/test_get.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.api.groups_api import GroupsApi  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_api_authorizations_api_auth_id import get  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
 
-class TestGroupsApi(unittest.TestCase):
-    """GroupsApi unit test stubs"""
+class TestApi2ApiAuthorizationsApiAuthId(ApiTestMixin, unittest.TestCase):
+    """
+    Api2ApiAuthorizationsApiAuthId unit test stubs
+        Get Api Auth Server  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        self.api = onelogin.api.groups_api.GroupsApi()  # noqa: E501
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_get_group_by_id(self):
-        """Test case for get_group_by_id
+    response_status = 200
 
-        Get Group by ID  # noqa: E501
-        """
-        pass
-
-    def test_get_groups(self):
-        """Test case for get_groups
 
-        Get Groups  # noqa: E501
-        """
-        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_invite_links_api.py` & `onelogin-3.1.6/test/test_paths/test_api_1_invites_get_invite_link/test_post.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.api.invite_links_api import InviteLinksApi  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_1_invites_get_invite_link import post  # noqa: E501
+from onelogin import configuration, schemas, api_client
 
+from .. import ApiTestMixin
 
-class TestInviteLinksApi(unittest.TestCase):
-    """InviteLinksApi unit test stubs"""
+
+class TestApi1InvitesGetInviteLink(ApiTestMixin, unittest.TestCase):
+    """
+    Api1InvitesGetInviteLink unit test stubs
+        Generate Invite Link  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        self.api = onelogin.api.invite_links_api.InviteLinksApi()  # noqa: E501
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_get_invite_link(self):
-        """Test case for get_invite_link
+    response_status = 200
 
-        Generate Invite Link  # noqa: E501
-        """
-        pass
 
-    def test_send_invite_link(self):
-        """Test case for send_invite_link
-
-        Send  Invite Link  # noqa: E501
-        """
-        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_o_auth2_api.py` & `onelogin-3.1.6/test/test_paths/test_api_2_branding_brands_brand_id/test_get.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.api.o_auth2_api import OAuth2Api  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_branding_brands_brand_id import get  # noqa: E501
+from onelogin import configuration, schemas, api_client
 
+from .. import ApiTestMixin
 
-class TestOAuth2Api(unittest.TestCase):
-    """OAuth2Api unit test stubs"""
+
+class TestApi2BrandingBrandsBrandId(ApiTestMixin, unittest.TestCase):
+    """
+    Api2BrandingBrandsBrandId unit test stubs
+        Get Brand  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        self.api = onelogin.api.o_auth2_api.OAuth2Api()  # noqa: E501
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_generate_token(self):
-        """Test case for generate_token
-
-        Generate Token  # noqa: E501
-        """
-        pass
-
-    def test_get_rate_limit(self):
-        """Test case for get_rate_limit
+    response_status = 200
 
-        Get Rate Limit  # noqa: E501
-        """
-        pass
 
-    def test_revoke_tokens(self):
-        """Test case for revoke_tokens
-
-        Revoke Tokens  # noqa: E501
-        """
-        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_saml_assertions_api.py` & `onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_claims_claim_id/test_put.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.api.saml_assertions_api import SAMLAssertionsApi  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_api_authorizations_api_auth_id_claims_claim_id import put  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
 
-class TestSAMLAssertionsApi(unittest.TestCase):
-    """SAMLAssertionsApi unit test stubs"""
+class TestApi2ApiAuthorizationsApiAuthIdClaimsClaimId(ApiTestMixin, unittest.TestCase):
+    """
+    Api2ApiAuthorizationsApiAuthIdClaimsClaimId unit test stubs
+        Update Api Auth Server Claim  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        self.api = onelogin.api.saml_assertions_api.SAMLAssertionsApi()  # noqa: E501
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_generate_saml_assert(self):
-        """Test case for generate_saml_assert
+    response_status = 200
 
-        Generate SAML Assertion  # noqa: E501
-        """
-        pass
-
-    def test_generate_saml_assert2(self):
-        """Test case for generate_saml_assert2
 
-        Generate SAML Assertion  # noqa: E501
-        """
-        pass
-
-    def test_ver_factor_saml(self):
-        """Test case for ver_factor_saml
-
-        Verify Factor SAML  # noqa: E501
-        """
-        pass
-
-    def test_ver_factor_saml2(self):
-        """Test case for ver_factor_saml2
-
-        Verify Factor SAML  # noqa: E501
-        """
-        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_scope.py` & `onelogin-3.1.6/test/test_paths/test_api_2_api_authorizations_api_auth_id_clients/test_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.scope import Scope  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_api_authorizations_api_auth_id_clients import get  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
+
 
-class TestScope(unittest.TestCase):
-    """Scope unit test stubs"""
+class TestApi2ApiAuthorizationsApiAuthIdClients(ApiTestMixin, unittest.TestCase):
+    """
+    Api2ApiAuthorizationsApiAuthIdClients unit test stubs
+        List Clients Apps  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test Scope
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `Scope`
-        """
-        model = onelogin.models.scope.Scope()  # noqa: E501
-        if include_optional :
-            return Scope(
-                id = 25, 
-                value = 'read:contacts', 
-                description = 'Read some contacts'
-            )
-        else :
-            return Scope(
-        )
-        """
-
-    def testScope(self):
-        """Test Scope"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_session.py` & `onelogin-3.1.6/test/test_paths/test_api_1_privileges_privilege_id_users/test_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.session import Session  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_1_privileges_privilege_id_users import get  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
+
 
-class TestSession(unittest.TestCase):
-    """Session unit test stubs"""
+class TestApi1PrivilegesPrivilegeIdUsers(ApiTestMixin, unittest.TestCase):
+    """
+    Api1PrivilegesPrivilegeIdUsers unit test stubs
+        Get Users assigned to a Privilege  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test Session
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `Session`
-        """
-        model = onelogin.models.session.Session()  # noqa: E501
-        if include_optional :
-            return Session(
-                id = ''
-            )
-        else :
-            return Session(
-        )
-        """
-
-    def testSession(self):
-        """Test Session"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_verb.py` & `onelogin-3.1.6/test/test_paths/test_api_2_apps_app_id/test_delete.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.verb import Verb  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_apps_app_id import delete  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
-class TestVerb(unittest.TestCase):
-    """Verb unit test stubs"""
+
+class TestApi2AppsAppId(ApiTestMixin, unittest.TestCase):
+    """
+    Api2AppsAppId unit test stubs
+        Delete App  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testVerb(self):
-        """Test Verb"""
-        # inst = Verb()
+    response_status = 204
+    response_body = ''
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `onelogin-3.1.5/test/test_verify_user_verification_request.py` & `onelogin-3.1.6/test/test_paths/test_api_2_mfa_users_user_id_verifications_verification_id/test_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,41 @@
 # coding: utf-8
 
 """
-    OneLogin API
 
-    OpenAPI Specification for OneLogin  # noqa: E501
 
-    The version of the OpenAPI document: 3.1.1
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import unittest
-import datetime
+from unittest.mock import patch
+
+import urllib3
 
 import onelogin
-from onelogin.models.verify_user_verification_request import VerifyUserVerificationRequest  # noqa: E501
-from onelogin.rest import ApiException
+from onelogin.paths.api_2_mfa_users_user_id_verifications_verification_id import get  # noqa: E501
+from onelogin import configuration, schemas, api_client
+
+from .. import ApiTestMixin
+
 
-class TestVerifyUserVerificationRequest(unittest.TestCase):
-    """VerifyUserVerificationRequest unit test stubs"""
+class TestApi2MfaUsersUserIdVerificationsVerificationId(ApiTestMixin, unittest.TestCase):
+    """
+    Api2MfaUsersUserIdVerificationsVerificationId unit test stubs
+        Get User Verification  # noqa: E501
+    """
+    _configuration = configuration.Configuration()
 
     def setUp(self):
-        pass
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test VerifyUserVerificationRequest
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `VerifyUserVerificationRequest`
-        """
-        model = onelogin.models.verify_user_verification_request.VerifyUserVerificationRequest()  # noqa: E501
-        if include_optional :
-            return VerifyUserVerificationRequest(
-                otp = '123456', 
-                device_id = 98765
-            )
-        else :
-            return VerifyUserVerificationRequest(
-        )
-        """
-
-    def testVerifyUserVerificationRequest(self):
-        """Test VerifyUserVerificationRequest"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    response_status = 200
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

