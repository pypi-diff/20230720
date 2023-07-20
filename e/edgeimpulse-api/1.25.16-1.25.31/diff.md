# Comparing `tmp/edgeimpulse_api-1.25.16.tar.gz` & `tmp/edgeimpulse_api-1.25.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse_api-1.25.16.tar", max compression
+gzip compressed data, was "edgeimpulse_api-1.25.31.tar", max compression
```

## Comparing `edgeimpulse_api-1.25.16.tar` & `edgeimpulse_api-1.25.31.tar`

### file list

```diff
@@ -1,779 +1,788 @@
--rw-r--r--   0        0        0      377 2023-05-16 14:36:24.095652 edgeimpulse_api-1.25.16/README.md
--rw-r--r--   0        0        0    74273 2023-07-03 10:35:44.903571 edgeimpulse_api-1.25.16/edgeimpulse_api/__init__.py
--rw-r--r--   0        0        0     2928 2023-07-03 10:35:21.195990 edgeimpulse_api-1.25.16/edgeimpulse_api/api/__init__.py
--rw-r--r--   0        0        0   237298 2023-07-03 10:35:20.539335 edgeimpulse_api-1.25.16/edgeimpulse_api/api/admin_api.py
--rw-r--r--   0        0        0   290922 2023-07-03 10:35:20.580355 edgeimpulse_api-1.25.16/edgeimpulse_api/api/allows_read_only_api.py
--rw-r--r--   0        0        0    11231 2023-07-03 10:35:20.606218 edgeimpulse_api-1.25.16/edgeimpulse_api/api/auth_api.py
--rw-r--r--   0        0        0     6235 2023-07-03 10:35:20.617093 edgeimpulse_api-1.25.16/edgeimpulse_api/api/cdn_api.py
--rw-r--r--   0        0        0    28575 2023-07-03 10:35:20.628327 edgeimpulse_api-1.25.16/edgeimpulse_api/api/classify_api.py
--rw-r--r--   0        0        0     7426 2023-07-03 10:35:20.640862 edgeimpulse_api-1.25.16/edgeimpulse_api/api/content_disposition_inline_api.py
--rw-r--r--   0        0        0    72480 2023-07-03 10:35:20.682703 edgeimpulse_api-1.25.16/edgeimpulse_api/api/deployment_api.py
--rw-r--r--   0        0        0    38974 2023-07-03 10:35:20.703717 edgeimpulse_api-1.25.16/edgeimpulse_api/api/devices_api.py
--rw-r--r--   0        0        0   130256 2023-07-03 10:35:20.656213 edgeimpulse_api-1.25.16/edgeimpulse_api/api/dsp_api.py
--rw-r--r--   0        0        0     6435 2023-07-03 10:35:20.714237 edgeimpulse_api-1.25.16/edgeimpulse_api/api/export_api.py
--rw-r--r--   0        0        0    11921 2023-07-03 10:35:20.724231 edgeimpulse_api-1.25.16/edgeimpulse_api/api/health_api.py
--rw-r--r--   0        0        0    49621 2023-07-03 10:35:20.734337 edgeimpulse_api-1.25.16/edgeimpulse_api/api/impulse_api.py
--rw-r--r--   0        0        0   232507 2023-07-03 10:35:20.754729 edgeimpulse_api-1.25.16/edgeimpulse_api/api/jobs_api.py
--rw-r--r--   0        0        0   141029 2023-07-03 10:35:20.773944 edgeimpulse_api-1.25.16/edgeimpulse_api/api/learn_api.py
--rw-r--r--   0        0        0     6483 2023-07-03 10:35:20.784987 edgeimpulse_api-1.25.16/edgeimpulse_api/api/login_api.py
--rw-r--r--   0        0        0    12006 2023-07-03 10:35:20.792984 edgeimpulse_api-1.25.16/edgeimpulse_api/api/metrics_api.py
--rw-r--r--   0        0        0    67457 2023-07-03 10:35:20.801804 edgeimpulse_api-1.25.16/edgeimpulse_api/api/optimization_api.py
--rw-r--r--   0        0        0   300920 2023-07-03 10:35:20.816178 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_allow_developer_profile_api.py
--rw-r--r--   0        0        0    63140 2023-07-03 10:35:20.832303 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_allow_guest_access_api.py
--rw-r--r--   0        0        0   141131 2023-07-03 10:35:20.843993 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_blocks_api.py
--rw-r--r--   0        0        0    91908 2023-07-03 10:35:20.856889 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_create_project_api.py
--rw-r--r--   0        0        0   255365 2023-07-03 10:35:20.879849 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_data_api.py
--rw-r--r--   0        0        0    80882 2023-07-03 10:35:20.896182 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_data_campaigns_api.py
--rw-r--r--   0        0        0    58218 2023-07-03 10:35:20.906058 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_jobs_api.py
--rw-r--r--   0        0        0    47178 2023-07-03 10:35:20.914397 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_pipelines_api.py
--rw-r--r--   0        0        0    45490 2023-07-03 10:35:20.932017 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_portals_api.py
--rw-r--r--   0        0        0   259735 2023-07-03 10:35:20.945083 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_requires_admin_api.py
--rw-r--r--   0        0        0   169682 2023-07-03 10:35:20.963012 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py
--rw-r--r--   0        0        0   293621 2023-07-03 10:35:20.981250 edgeimpulse_api-1.25.16/edgeimpulse_api/api/organizations_api.py
--rw-r--r--   0        0        0    54671 2023-07-03 10:35:20.996219 edgeimpulse_api-1.25.16/edgeimpulse_api/api/performance_calibration_api.py
--rw-r--r--   0        0        0    12662 2023-07-03 10:35:21.004986 edgeimpulse_api-1.25.16/edgeimpulse_api/api/project_requires_admin_api.py
--rw-r--r--   0        0        0   228112 2023-07-03 10:35:21.044608 edgeimpulse_api-1.25.16/edgeimpulse_api/api/projects_api.py
--rw-r--r--   0        0        0   366799 2023-07-03 10:35:21.067101 edgeimpulse_api-1.25.16/edgeimpulse_api/api/raw_data_api.py
--rw-r--r--   0        0        0    24481 2023-07-03 10:35:21.084166 edgeimpulse_api-1.25.16/edgeimpulse_api/api/requires_sudo_api.py
--rw-r--r--   0        0        0     7730 2023-07-03 10:35:21.092343 edgeimpulse_api-1.25.16/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py
--rw-r--r--   0        0        0    13690 2023-07-03 10:35:21.102033 edgeimpulse_api-1.25.16/edgeimpulse_api/api/supports_range_api.py
--rw-r--r--   0        0        0    35671 2023-07-03 10:35:21.111033 edgeimpulse_api-1.25.16/edgeimpulse_api/api/themes_api.py
--rw-r--r--   0        0        0    43486 2023-07-03 10:35:21.121332 edgeimpulse_api-1.25.16/edgeimpulse_api/api/third_party_auth_api.py
--rw-r--r--   0        0        0    45393 2023-07-03 10:35:21.131170 edgeimpulse_api-1.25.16/edgeimpulse_api/api/upload_portal_api.py
--rw-r--r--   0        0        0   197590 2023-07-03 10:35:21.147785 edgeimpulse_api-1.25.16/edgeimpulse_api/api/user_api.py
--rw-r--r--   0        0        0    42135 2023-07-03 10:35:21.164376 edgeimpulse_api-1.25.16/edgeimpulse_api/api/whitelabels_api.py
--rw-r--r--   0        0        0    29331 2023-07-03 10:35:21.202957 edgeimpulse_api-1.25.16/edgeimpulse_api/api_client.py
--rw-r--r--   0        0        0    15659 2023-07-03 10:35:21.186337 edgeimpulse_api-1.25.16/edgeimpulse_api/configuration.py
--rw-r--r--   0        0        0     5113 2023-07-03 10:35:21.198021 edgeimpulse_api-1.25.16/edgeimpulse_api/exceptions.py
--rw-r--r--   0        0        0    70891 2023-07-03 10:35:35.487751 edgeimpulse_api-1.25.16/edgeimpulse_api/models/__init__.py
--rw-r--r--   0        0        0     2897 2023-07-03 10:35:35.456524 edgeimpulse_api-1.25.16/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
--rw-r--r--   0        0        0     1882 2023-07-03 10:35:35.460504 edgeimpulse_api-1.25.16/edgeimpulse_api/models/activate_user_request.py
--rw-r--r--   0        0        0     2610 2023-07-03 10:35:34.530969 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_api_key_request.py
--rw-r--r--   0        0        0     1963 2023-07-03 10:35:34.856596 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_collaborator_request.py
--rw-r--r--   0        0        0     2223 2023-07-03 10:35:35.922581 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_hmac_key_request.py
--rw-r--r--   0        0        0     2299 2023-07-03 10:35:35.856339 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_member_request.py
--rw-r--r--   0        0        0     2418 2023-07-03 10:35:35.199915 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_api_key_request.py
--rw-r--r--   0        0        0     2806 2023-07-03 10:35:35.496152 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_bucket_request.py
--rw-r--r--   0        0        0     2656 2023-07-03 10:35:35.310912 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     2469 2023-07-03 10:35:34.636865 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2152 2023-07-03 10:35:35.494110 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     4230 2023-07-03 10:35:35.777242 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2359 2023-07-03 10:35:35.948176 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2042 2023-07-03 10:35:36.132583 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
--rw-r--r--   0        0        0     2269 2023-07-03 10:35:35.627327 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2816 2023-07-03 10:35:35.426807 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2248 2023-07-03 10:35:35.710139 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2054 2023-07-03 10:35:35.446416 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_secret_request.py
--rw-r--r--   0        0        0     2266 2023-07-03 10:35:35.729621 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_secret_response.py
--rw-r--r--   0        0        0     1949 2023-07-03 10:35:35.348216 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_secret_response_all_of.py
--rw-r--r--   0        0        0     4363 2023-07-03 10:35:34.998552 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     2339 2023-07-03 10:35:35.691610 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     4592 2023-07-03 10:35:34.592908 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_transformation_block_request.py
--rw-r--r--   0        0        0     2325 2023-07-03 10:35:36.156817 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2001 2023-07-03 10:35:35.128673 edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     1940 2023-07-03 10:35:35.238329 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
--rw-r--r--   0        0        0     1961 2023-07-03 10:35:35.913843 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
--rw-r--r--   0        0        0     2542 2023-07-03 10:35:36.113138 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_organization_user_request.py
--rw-r--r--   0        0        0     2246 2023-07-03 10:35:36.016782 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
--rw-r--r--   0        0        0     2146 2023-07-03 10:35:36.092826 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_project_user_request.py
--rw-r--r--   0        0        0     2097 2023-07-03 10:35:35.945859 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_user_request.py
--rw-r--r--   0        0        0     3876 2023-07-03 10:35:36.264917 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_api_organization.py
--rw-r--r--   0        0        0     2396 2023-07-03 10:35:34.918632 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_api_organization_all_of.py
--rw-r--r--   0        0        0     3459 2023-07-03 10:35:35.618137 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_api_project.py
--rw-r--r--   0        0        0     6652 2023-07-03 10:35:35.127545 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_api_user.py
--rw-r--r--   0        0        0     5098 2023-07-03 10:35:36.085751 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_api_user_all_of.py
--rw-r--r--   0        0        0     2262 2023-07-03 10:35:35.712326 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_create_organization_request.py
--rw-r--r--   0        0        0     2546 2023-07-03 10:35:35.491925 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_data_migration_response.py
--rw-r--r--   0        0        0     2222 2023-07-03 10:35:35.934421 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
--rw-r--r--   0        0        0     2735 2023-07-03 10:35:35.714372 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_data_migrations_response.py
--rw-r--r--   0        0        0     2428 2023-07-03 10:35:35.006087 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
--rw-r--r--   0        0        0     2318 2023-07-03 10:35:35.665269 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
--rw-r--r--   0        0        0     2022 2023-07-03 10:35:35.285904 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
--rw-r--r--   0        0        0     2217 2023-07-03 10:35:35.896634 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_metrics_response.py
--rw-r--r--   0        0        0     1910 2023-07-03 10:35:35.652816 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
--rw-r--r--   0        0        0     3046 2023-07-03 10:35:35.560238 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_organizations_response.py
--rw-r--r--   0        0        0     2746 2023-07-03 10:35:36.356570 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
--rw-r--r--   0        0        0     3409 2023-07-03 10:35:35.587556 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
--rw-r--r--   0        0        0     2243 2023-07-03 10:35:35.451204 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
--rw-r--r--   0        0        0     1947 2023-07-03 10:35:35.556217 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
--rw-r--r--   0        0        0     2914 2023-07-03 10:35:35.947023 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_sso_settings_response.py
--rw-r--r--   0        0        0     2614 2023-07-03 10:35:35.764696 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
--rw-r--r--   0        0        0     2096 2023-07-03 10:35:35.326566 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
--rw-r--r--   0        0        0     2208 2023-07-03 10:35:36.058500 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_ids_response.py
--rw-r--r--   0        0        0     1901 2023-07-03 10:35:35.928311 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
--rw-r--r--   0        0        0     2245 2023-07-03 10:35:36.230980 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_metrics_response.py
--rw-r--r--   0        0        0     1938 2023-07-03 10:35:35.078246 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_metrics_response_all_of.py
--rw-r--r--   0        0        0     2452 2023-07-03 10:35:34.581344 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_response.py
--rw-r--r--   0        0        0     2128 2023-07-03 10:35:35.581180 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_response_all_of.py
--rw-r--r--   0        0        0     2807 2023-07-03 10:35:35.265479 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_users_response.py
--rw-r--r--   0        0        0     2500 2023-07-03 10:35:36.224632 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_users_response_all_of.py
--rw-r--r--   0        0        0     3087 2023-07-03 10:35:35.590881 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
--rw-r--r--   0        0        0     2445 2023-07-03 10:35:35.645564 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_list_projects.py
--rw-r--r--   0        0        0     2836 2023-07-03 10:35:35.629794 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_list_projects_response.py
--rw-r--r--   0        0        0     7695 2023-07-03 10:35:35.334421 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_organization_info_response.py
--rw-r--r--   0        0        0     3752 2023-07-03 10:35:35.758956 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_organization_info_response_all_of.py
--rw-r--r--   0        0        0     2158 2023-07-03 10:35:36.259666 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_toggle_data_migration_request.py
--rw-r--r--   0        0        0     3269 2023-07-03 10:35:36.439539 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_update_organization_request.py
--rw-r--r--   0        0        0     2015 2023-07-03 10:35:35.944502 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_update_user_permissions_request.py
--rw-r--r--   0        0        0     2661 2023-07-03 10:35:36.455973 edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_update_user_request.py
--rw-r--r--   0        0        0     2525 2023-07-03 10:35:35.893738 edgeimpulse_api-1.25.16/edgeimpulse_api/models/akida_edge_learning_config.py
--rw-r--r--   0        0        0     3630 2023-07-03 10:35:34.785647 edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_model_metadata.py
--rw-r--r--   0        0        0     2151 2023-07-03 10:35:35.361014 edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_model_metadata_clusters_inner.py
--rw-r--r--   0        0        0     4011 2023-07-03 10:35:36.205225 edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_model_metadata_response.py
--rw-r--r--   0        0        0     4079 2023-07-03 10:35:34.934937 edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_response.py
--rw-r--r--   0        0        0     3812 2023-07-03 10:35:35.749049 edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_response_all_of.py
--rw-r--r--   0        0        0     2044 2023-07-03 10:35:35.215762 edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_response_all_of_axes.py
--rw-r--r--   0        0        0     3029 2023-07-03 10:35:35.844644 edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_trained_features_response.py
--rw-r--r--   0        0        0     2729 2023-07-03 10:35:35.931620 edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2375 2023-07-03 10:35:34.956033 edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0      506 2023-07-03 10:35:35.588837 edgeimpulse_api-1.25.16/edgeimpulse_api/models/augmentation_policy_image_enum.py
--rw-r--r--   0        0        0     3635 2023-07-03 10:35:35.341583 edgeimpulse_api-1.25.16/edgeimpulse_api/models/augmentation_policy_spectrogram.py
--rw-r--r--   0        0        0     1895 2023-07-03 10:35:34.747691 edgeimpulse_api-1.25.16/edgeimpulse_api/models/autotune_dsp_request.py
--rw-r--r--   0        0        0     2044 2023-07-03 10:35:35.794746 edgeimpulse_api-1.25.16/edgeimpulse_api/models/bounding_box.py
--rw-r--r--   0        0        0     2151 2023-07-03 10:35:34.818125 edgeimpulse_api-1.25.16/edgeimpulse_api/models/bounding_box_with_score.py
--rw-r--r--   0        0        0     2197 2023-07-03 10:35:35.358588 edgeimpulse_api-1.25.16/edgeimpulse_api/models/build_on_device_model_request.py
--rw-r--r--   0        0        0     2433 2023-07-03 10:35:34.847672 edgeimpulse_api-1.25.16/edgeimpulse_api/models/build_organization_on_device_model_request.py
--rw-r--r--   0        0        0     2041 2023-07-03 10:35:35.229849 edgeimpulse_api-1.25.16/edgeimpulse_api/models/change_password_request.py
--rw-r--r--   0        0        0     3701 2023-07-03 10:35:35.697672 edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response.py
--rw-r--r--   0        0        0     3394 2023-07-03 10:35:36.282159 edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response_all_of.py
--rw-r--r--   0        0        0     3769 2023-07-03 10:35:35.499521 edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
--rw-r--r--   0        0        0     2055 2023-07-03 10:35:36.149255 edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
--rw-r--r--   0        0        0     3255 2023-07-03 10:35:34.522037 edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response_page.py
--rw-r--r--   0        0        0     2948 2023-07-03 10:35:34.640900 edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response_page_all_of.py
--rw-r--r--   0        0        0     3932 2023-07-03 10:35:34.828028 edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_sample_response.py
--rw-r--r--   0        0        0     3644 2023-07-03 10:35:34.735204 edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_sample_response_all_of.py
--rw-r--r--   0        0        0     4783 2023-07-03 10:35:35.292676 edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_sample_response_classification.py
--rw-r--r--   0        0        0     2755 2023-07-03 10:35:34.803909 edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_sample_response_classification_details.py
--rw-r--r--   0        0        0     3004 2023-07-03 10:35:35.681278 edgeimpulse_api-1.25.16/edgeimpulse_api/models/convert_user_request.py
--rw-r--r--   0        0        0     2183 2023-07-03 10:35:35.850115 edgeimpulse_api-1.25.16/edgeimpulse_api/models/count_samples_response.py
--rw-r--r--   0        0        0     1859 2023-07-03 10:35:34.605721 edgeimpulse_api-1.25.16/edgeimpulse_api/models/count_samples_response_all_of.py
--rw-r--r--   0        0        0     2255 2023-07-03 10:35:35.743566 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_block_version_response.py
--rw-r--r--   0        0        0     1938 2023-07-03 10:35:36.206884 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_block_version_response_all_of.py
--rw-r--r--   0        0        0     2404 2023-07-03 10:35:35.308347 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_developer_profile_response.py
--rw-r--r--   0        0        0     2125 2023-07-03 10:35:34.588896 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_developer_profile_response_all_of.py
--rw-r--r--   0        0        0     2387 2023-07-03 10:35:35.707609 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_device_request.py
--rw-r--r--   0        0        0     2491 2023-07-03 10:35:34.860002 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_evaluation_user_response.py
--rw-r--r--   0        0        0     2185 2023-07-03 10:35:35.421260 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
--rw-r--r--   0        0        0     2600 2023-07-03 10:35:35.205992 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_portal_request.py
--rw-r--r--   0        0        0     2830 2023-07-03 10:35:36.040335 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_portal_response.py
--rw-r--r--   0        0        0     2551 2023-07-03 10:35:35.098721 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     1990 2023-07-03 10:35:36.115011 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_request.py
--rw-r--r--   0        0        0     2454 2023-07-03 10:35:36.080960 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_response.py
--rw-r--r--   0        0        0     2148 2023-07-03 10:35:35.966261 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_response_all_of.py
--rw-r--r--   0        0        0     2185 2023-07-03 10:35:35.340290 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_pipeline_response.py
--rw-r--r--   0        0        0     2254 2023-07-03 10:35:34.501636 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_project_request.py
--rw-r--r--   0        0        0     2378 2023-07-03 10:35:35.395092 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_project_response.py
--rw-r--r--   0        0        0     2072 2023-07-03 10:35:36.134773 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_project_response_all_of.py
--rw-r--r--   0        0        0     2276 2023-07-03 10:35:36.097505 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_signed_upload_link_request.py
--rw-r--r--   0        0        0     2414 2023-07-03 10:35:36.007569 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_signed_upload_link_response.py
--rw-r--r--   0        0        0     2135 2023-07-03 10:35:34.905251 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
--rw-r--r--   0        0        0     2413 2023-07-03 10:35:36.241097 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_third_party_auth_request.py
--rw-r--r--   0        0        0     2450 2023-07-03 10:35:34.938337 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_third_party_auth_response.py
--rw-r--r--   0        0        0     2144 2023-07-03 10:35:34.631227 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     3835 2023-07-03 10:35:35.350876 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_request.py
--rw-r--r--   0        0        0     2393 2023-07-03 10:35:35.181483 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_response.py
--rw-r--r--   0        0        0     2114 2023-07-03 10:35:35.252639 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_response_all_of.py
--rw-r--r--   0        0        0     2919 2023-07-03 10:35:35.526088 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_third_party_request.py
--rw-r--r--   0        0        0     2672 2023-07-03 10:35:36.166104 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_third_party_response.py
--rw-r--r--   0        0        0     2393 2023-07-03 10:35:35.357246 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_third_party_response_all_of.py
--rw-r--r--   0        0        0     4157 2023-07-03 10:35:34.584732 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_whitelabel_request.py
--rw-r--r--   0        0        0     2438 2023-07-03 10:35:35.367827 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_whitelabel_response.py
--rw-r--r--   0        0        0     2121 2023-07-03 10:35:34.813898 edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2051 2023-07-03 10:35:36.258146 edgeimpulse_api-1.25.16/edgeimpulse_api/models/crop_sample_request.py
--rw-r--r--   0        0        0     2248 2023-07-03 10:35:35.708986 edgeimpulse_api-1.25.16/edgeimpulse_api/models/crop_sample_response.py
--rw-r--r--   0        0        0     1943 2023-07-03 10:35:35.329900 edgeimpulse_api-1.25.16/edgeimpulse_api/models/crop_sample_response_all_of.py
--rw-r--r--   0        0        0     4054 2023-07-03 10:35:34.569732 edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign.py
--rw-r--r--   0        0        0     2851 2023-07-03 10:35:35.866600 edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_dashboard.py
--rw-r--r--   0        0        0     2786 2023-07-03 10:35:35.184440 edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_graph.py
--rw-r--r--   0        0        0     3352 2023-07-03 10:35:35.405262 edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
--rw-r--r--   0        0        0     2047 2023-07-03 10:35:36.387448 edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
--rw-r--r--   0        0        0     1934 2023-07-03 10:35:36.136628 edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_link.py
--rw-r--r--   0        0        0     1957 2023-07-03 10:35:35.403679 edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_query.py
--rw-r--r--   0        0        0     3292 2023-07-03 10:35:35.781242 edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_explorer_predictions_response.py
--rw-r--r--   0        0        0     3003 2023-07-03 10:35:34.836243 edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
--rw-r--r--   0        0        0     2838 2023-07-03 10:35:36.145732 edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_explorer_settings.py
--rw-r--r--   0        0        0     2149 2023-07-03 10:35:36.402482 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dataset_ratio_data.py
--rw-r--r--   0        0        0     2111 2023-07-03 10:35:35.524804 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dataset_ratio_data_ratio.py
--rw-r--r--   0        0        0     1898 2023-07-03 10:35:34.714936 edgeimpulse_api-1.25.16/edgeimpulse_api/models/delete_portal_file_request.py
--rw-r--r--   0        0        0     2230 2023-07-03 10:35:35.228253 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dependency_data.py
--rw-r--r--   0        0        0     2280 2023-07-03 10:35:35.537119 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
--rw-r--r--   0        0        0     2408 2023-07-03 10:35:35.400915 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
--rw-r--r--   0        0        0     2155 2023-07-03 10:35:36.215116 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
--rw-r--r--   0        0        0     2484 2023-07-03 10:35:35.949323 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
--rw-r--r--   0        0        0     2344 2023-07-03 10:35:35.831337 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
--rw-r--r--   0        0        0     2780 2023-07-03 10:35:35.785377 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
--rw-r--r--   0        0        0     2200 2023-07-03 10:35:35.417168 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
--rw-r--r--   0        0        0     4355 2023-07-03 10:35:36.098974 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_request.py
--rw-r--r--   0        0        0     2833 2023-07-03 10:35:35.315770 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
--rw-r--r--   0        0        0     8503 2023-07-03 10:35:36.431101 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
--rw-r--r--   0        0        0     8065 2023-07-03 10:35:36.186138 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
--rw-r--r--   0        0        0     5950 2023-07-03 10:35:35.432752 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deployment_target.py
--rw-r--r--   0        0        0     1926 2023-07-03 10:35:35.884837 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deployment_target_badge.py
--rw-r--r--   0        0        0      679 2023-07-03 10:35:34.788933 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deployment_target_engine.py
--rw-r--r--   0        0        0     2702 2023-07-03 10:35:35.818597 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deployment_targets_response.py
--rw-r--r--   0        0        0     2395 2023-07-03 10:35:35.301565 edgeimpulse_api-1.25.16/edgeimpulse_api/models/deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     1983 2023-07-03 10:35:35.531920 edgeimpulse_api-1.25.16/edgeimpulse_api/models/development_board.py
--rw-r--r--   0        0        0     2831 2023-07-03 10:35:35.412919 edgeimpulse_api-1.25.16/edgeimpulse_api/models/development_boards_response.py
--rw-r--r--   0        0        0     2531 2023-07-03 10:35:34.850732 edgeimpulse_api-1.25.16/edgeimpulse_api/models/development_boards_response_all_of.py
--rw-r--r--   0        0        0     2030 2023-07-03 10:35:36.419102 edgeimpulse_api-1.25.16/edgeimpulse_api/models/development_keys.py
--rw-r--r--   0        0        0     2400 2023-07-03 10:35:36.120939 edgeimpulse_api-1.25.16/edgeimpulse_api/models/development_keys_response.py
--rw-r--r--   0        0        0     3677 2023-07-03 10:35:35.236367 edgeimpulse_api-1.25.16/edgeimpulse_api/models/device.py
--rw-r--r--   0        0        0     2199 2023-07-03 10:35:35.408240 edgeimpulse_api-1.25.16/edgeimpulse_api/models/device_name_response.py
--rw-r--r--   0        0        0     1920 2023-07-03 10:35:35.570509 edgeimpulse_api-1.25.16/edgeimpulse_api/models/device_name_response_all_of.py
--rw-r--r--   0        0        0     2231 2023-07-03 10:35:36.073400 edgeimpulse_api-1.25.16/edgeimpulse_api/models/device_sensors_inner.py
--rw-r--r--   0        0        0     2094 2023-07-03 10:35:35.363577 edgeimpulse_api-1.25.16/edgeimpulse_api/models/download.py
--rw-r--r--   0        0        0     1912 2023-07-03 10:35:35.309671 edgeimpulse_api-1.25.16/edgeimpulse_api/models/download_portal_file_request.py
--rw-r--r--   0        0        0     2260 2023-07-03 10:35:35.881068 edgeimpulse_api-1.25.16/edgeimpulse_api/models/download_portal_file_response.py
--rw-r--r--   0        0        0     1954 2023-07-03 10:35:36.193552 edgeimpulse_api-1.25.16/edgeimpulse_api/models/download_portal_file_response_all_of.py
--rw-r--r--   0        0        0     2724 2023-07-03 10:35:36.004920 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_autotuner_results.py
--rw-r--r--   0        0        0     2417 2023-07-03 10:35:35.585958 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
--rw-r--r--   0        0        0     1968 2023-07-03 10:35:35.683870 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
--rw-r--r--   0        0        0     2870 2023-07-03 10:35:34.790839 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_block.py
--rw-r--r--   0        0        0     1834 2023-07-03 10:35:34.505615 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_config_request.py
--rw-r--r--   0        0        0     3092 2023-07-03 10:35:35.809859 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_config_response.py
--rw-r--r--   0        0        0     2813 2023-07-03 10:35:35.789357 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_config_response_all_of.py
--rw-r--r--   0        0        0     3016 2023-07-03 10:35:35.290592 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_importance_response.py
--rw-r--r--   0        0        0     2728 2023-07-03 10:35:34.992019 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
--rw-r--r--   0        0        0     2058 2023-07-03 10:35:34.808996 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
--rw-r--r--   0        0        0     2572 2023-07-03 10:35:36.014381 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
--rw-r--r--   0        0        0     2216 2023-07-03 10:35:35.194497 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_labels_response.py
--rw-r--r--   0        0        0     1920 2023-07-03 10:35:34.485360 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
--rw-r--r--   0        0        0     2294 2023-07-03 10:35:35.513496 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_group.py
--rw-r--r--   0        0        0     3779 2023-07-03 10:35:35.782652 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_group_item.py
--rw-r--r--   0        0        0     2190 2023-07-03 10:35:34.908328 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
--rw-r--r--   0        0        0     2195 2023-07-03 10:35:35.117826 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_group_item_show_if.py
--rw-r--r--   0        0        0     4410 2023-07-03 10:35:36.101691 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_info.py
--rw-r--r--   0        0        0     2210 2023-07-03 10:35:35.921383 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_info_features.py
--rw-r--r--   0        0        0     1885 2023-07-03 10:35:35.409891 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_info_performance.py
--rw-r--r--   0        0        0     5144 2023-07-03 10:35:35.903167 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_metadata.py
--rw-r--r--   0        0        0     2025 2023-07-03 10:35:35.700144 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
--rw-r--r--   0        0        0     2566 2023-07-03 10:35:36.410192 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_metadata_output_config.py
--rw-r--r--   0        0        0     2531 2023-07-03 10:35:35.116223 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
--rw-r--r--   0        0        0     5502 2023-07-03 10:35:35.905893 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_metadata_response.py
--rw-r--r--   0        0        0     3019 2023-07-03 10:35:35.657478 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_performance_all_variants_response.py
--rw-r--r--   0        0        0     2729 2023-07-03 10:35:34.830182 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2278 2023-07-03 10:35:35.820700 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
--rw-r--r--   0        0        0     4639 2023-07-03 10:35:36.422702 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_graph.py
--rw-r--r--   0        0        0     1899 2023-07-03 10:35:35.223945 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
--rw-r--r--   0        0        0     2677 2023-07-03 10:35:35.508051 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_request_with_features.py
--rw-r--r--   0        0        0     2151 2023-07-03 10:35:35.519004 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_request_without_features.py
--rw-r--r--   0        0        0     2030 2023-07-03 10:35:35.069362 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
--rw-r--r--   0        0        0     3513 2023-07-03 10:35:35.686837 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_response.py
--rw-r--r--   0        0        0     3234 2023-07-03 10:35:34.603211 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_response_all_of.py
--rw-r--r--   0        0        0     1969 2023-07-03 10:35:36.235623 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
--rw-r--r--   0        0        0     4142 2023-07-03 10:35:34.753053 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_response_with_sample.py
--rw-r--r--   0        0        0     3875 2023-07-03 10:35:36.237330 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
--rw-r--r--   0        0        0     3342 2023-07-03 10:35:35.131752 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_sample_features_response.py
--rw-r--r--   0        0        0     3042 2023-07-03 10:35:35.595768 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
--rw-r--r--   0        0        0     2748 2023-07-03 10:35:35.858124 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
--rw-r--r--   0        0        0     2213 2023-07-03 10:35:35.997727 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
--rw-r--r--   0        0        0     3353 2023-07-03 10:35:34.944890 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_trained_features_response.py
--rw-r--r--   0        0        0     3053 2023-07-03 10:35:35.319749 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2773 2023-07-03 10:35:35.608751 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     2205 2023-07-03 10:35:34.864870 edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
--rw-r--r--   0        0        0     1893 2023-07-03 10:35:36.128310 edgeimpulse_api-1.25.16/edgeimpulse_api/models/edit_sample_label_request.py
--rw-r--r--   0        0        0     2397 2023-07-03 10:35:35.387558 edgeimpulse_api-1.25.16/edgeimpulse_api/models/entitlement_limits.py
--rw-r--r--   0        0        0     2656 2023-07-03 10:35:35.430530 edgeimpulse_api-1.25.16/edgeimpulse_api/models/evaluate_job_response.py
--rw-r--r--   0        0        0     2349 2023-07-03 10:35:35.168658 edgeimpulse_api-1.25.16/edgeimpulse_api/models/evaluate_job_response_all_of.py
--rw-r--r--   0        0        0     2099 2023-07-03 10:35:34.700134 edgeimpulse_api-1.25.16/edgeimpulse_api/models/evaluate_result_value.py
--rw-r--r--   0        0        0     2511 2023-07-03 10:35:34.990069 edgeimpulse_api-1.25.16/edgeimpulse_api/models/export_get_url_response.py
--rw-r--r--   0        0        0     2244 2023-07-03 10:35:34.596426 edgeimpulse_api-1.25.16/edgeimpulse_api/models/export_get_url_response_all_of.py
--rw-r--r--   0        0        0     2116 2023-07-03 10:35:35.827183 edgeimpulse_api-1.25.16/edgeimpulse_api/models/export_keras_block_data_request.py
--rw-r--r--   0        0        0     2373 2023-07-03 10:35:35.031931 edgeimpulse_api-1.25.16/edgeimpulse_api/models/export_original_data_request.py
--rw-r--r--   0        0        0     2021 2023-07-03 10:35:35.725131 edgeimpulse_api-1.25.16/edgeimpulse_api/models/export_wav_data_request.py
--rw-r--r--   0        0        0     2206 2023-07-03 10:35:35.823156 edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_segment_sample_request.py
--rw-r--r--   0        0        0     2804 2023-07-03 10:35:36.313826 edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_segment_sample_response.py
--rw-r--r--   0        0        0     2497 2023-07-03 10:35:35.610550 edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_segment_sample_response_all_of.py
--rw-r--r--   0        0        0     2090 2023-07-03 10:35:35.626169 edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
--rw-r--r--   0        0        0     2665 2023-07-03 10:35:35.246931 edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_user_response.py
--rw-r--r--   0        0        0     2358 2023-07-03 10:35:36.321557 edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_user_response_all_of.py
--rw-r--r--   0        0        0     2322 2023-07-03 10:35:35.084787 edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_user_response_all_of_users.py
--rw-r--r--   0        0        0     2507 2023-07-03 10:35:35.719441 edgeimpulse_api-1.25.16/edgeimpulse_api/models/generate_features_request.py
--rw-r--r--   0        0        0     2083 2023-07-03 10:35:35.125507 edgeimpulse_api-1.25.16/edgeimpulse_api/models/generic_api_response.py
--rw-r--r--   0        0        0     2764 2023-07-03 10:35:36.061485 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_imported_from_response.py
--rw-r--r--   0        0        0     2457 2023-07-03 10:35:35.860802 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
--rw-r--r--   0        0        0     2156 2023-07-03 10:35:36.426713 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
--rw-r--r--   0        0        0     2698 2023-07-03 10:35:36.110146 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_third_party_auth_response.py
--rw-r--r--   0        0        0     2391 2023-07-03 10:35:36.212777 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     2713 2023-07-03 10:35:35.419669 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_whitelabels_response.py
--rw-r--r--   0        0        0     2406 2023-07-03 10:35:34.604611 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
--rw-r--r--   0        0        0     3385 2023-07-03 10:35:36.083196 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_auto_segmenter_response.py
--rw-r--r--   0        0        0     3108 2023-07-03 10:35:35.974639 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py
--rw-r--r--   0        0        0     2610 2023-07-03 10:35:36.435083 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py
--rw-r--r--   0        0        0     1968 2023-07-03 10:35:35.754222 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py
--rw-r--r--   0        0        0     3400 2023-07-03 10:35:35.191825 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_data_explorer_features_response.py
--rw-r--r--   0        0        0     3122 2023-07-03 10:35:35.530250 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0     3752 2023-07-03 10:35:36.316708 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_data_explorer_settings_response.py
--rw-r--r--   0        0        0     2402 2023-07-03 10:35:36.111666 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
--rw-r--r--   0        0        0     2349 2023-07-03 10:35:35.828311 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_deployment_response.py
--rw-r--r--   0        0        0     2071 2023-07-03 10:35:36.239084 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_deployment_response_all_of.py
--rw-r--r--   0        0        0     2434 2023-07-03 10:35:35.599752 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_device_response.py
--rw-r--r--   0        0        0     2137 2023-07-03 10:35:36.077973 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_device_response_all_of.py
--rw-r--r--   0        0        0     3930 2023-07-03 10:35:36.062938 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_impulse_blocks_response.py
--rw-r--r--   0        0        0     3630 2023-07-03 10:35:34.939909 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
--rw-r--r--   0        0        0     2454 2023-07-03 10:35:34.557712 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_impulse_response.py
--rw-r--r--   0        0        0     2157 2023-07-03 10:35:35.953519 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_impulse_response_all_of.py
--rw-r--r--   0        0        0     2374 2023-07-03 10:35:35.503430 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_job_response.py
--rw-r--r--   0        0        0     2077 2023-07-03 10:35:36.009432 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_job_response_all_of.py
--rw-r--r--   0        0        0     2650 2023-07-03 10:35:34.503900 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_jwt_request.py
--rw-r--r--   0        0        0     2431 2023-07-03 10:35:35.447606 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_jwt_response.py
--rw-r--r--   0        0        0     2152 2023-07-03 10:35:34.657408 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_jwt_response_all_of.py
--rw-r--r--   0        0        0     2977 2023-07-03 10:35:34.729631 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_last_deployment_build_response.py
--rw-r--r--   0        0        0     2699 2023-07-03 10:35:35.514635 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
--rw-r--r--   0        0        0     2869 2023-07-03 10:35:36.119748 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
--rw-r--r--   0        0        0     2572 2023-07-03 10:35:36.352662 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_notes_response.py
--rw-r--r--   0        0        0     2265 2023-07-03 10:35:35.969223 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_notes_response_all_of.py
--rw-r--r--   0        0        0     2701 2023-07-03 10:35:35.018347 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2377 2023-07-03 10:35:34.668272 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     2890 2023-07-03 10:35:35.160987 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
--rw-r--r--   0        0        0     2583 2023-07-03 10:35:35.175455 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
--rw-r--r--   0        0        0     3158 2023-07-03 10:35:35.943287 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2939 2023-07-03 10:35:35.833881 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaigns_response.py
--rw-r--r--   0        0        0     2632 2023-07-03 10:35:35.555102 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
--rw-r--r--   0        0        0     2921 2023-07-03 10:35:36.181616 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
--rw-r--r--   0        0        0     2561 2023-07-03 10:35:36.379365 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_item_response.py
--rw-r--r--   0        0        0     2237 2023-07-03 10:35:36.144376 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
--rw-r--r--   0        0        0     3411 2023-07-03 10:35:35.225468 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
--rw-r--r--   0        0        0     3111 2023-07-03 10:35:34.906847 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
--rw-r--r--   0        0        0     3398 2023-07-03 10:35:35.443687 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
--rw-r--r--   0        0        0     2576 2023-07-03 10:35:35.622807 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_dataset_response.py
--rw-r--r--   0        0        0     2252 2023-07-03 10:35:35.659952 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
--rw-r--r--   0        0        0     2603 2023-07-03 10:35:35.985173 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_pipelines_response.py
--rw-r--r--   0        0        0     2279 2023-07-03 10:35:34.736939 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     3670 2023-07-03 10:35:36.178614 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_portal_response.py
--rw-r--r--   0        0        0     3391 2023-07-03 10:35:34.926866 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2323 2023-07-03 10:35:35.280533 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_projects_data_count_response.py
--rw-r--r--   0        0        0     2905 2023-07-03 10:35:34.695967 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
--rw-r--r--   0        0        0     2598 2023-07-03 10:35:35.489533 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
--rw-r--r--   0        0        0     3012 2023-07-03 10:35:35.558735 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
--rw-r--r--   0        0        0     2712 2023-07-03 10:35:34.853653 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
--rw-r--r--   0        0        0     2722 2023-07-03 10:35:34.616211 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
--rw-r--r--   0        0        0     2425 2023-07-03 10:35:36.161633 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
--rw-r--r--   0        0        0     2922 2023-07-03 10:35:35.144665 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
--rw-r--r--   0        0        0     2615 2023-07-03 10:35:35.434603 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
--rw-r--r--   0        0        0     3151 2023-07-03 10:35:34.479981 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_status_response.py
--rw-r--r--   0        0        0     2884 2023-07-03 10:35:35.490781 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
--rw-r--r--   0        0        0     3761 2023-07-03 10:35:35.572609 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_pretrained_model_response.py
--rw-r--r--   0        0        0     3483 2023-07-03 10:35:35.954935 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3861 2023-07-03 10:35:35.138716 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
--rw-r--r--   0        0        0     2978 2023-07-03 10:35:35.441011 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
--rw-r--r--   0        0        0     3058 2023-07-03 10:35:35.129887 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
--rw-r--r--   0        0        0     2397 2023-07-03 10:35:35.190631 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_public_metrics_response.py
--rw-r--r--   0        0        0     2073 2023-07-03 10:35:35.723679 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_public_metrics_response_all_of.py
--rw-r--r--   0        0        0     2767 2023-07-03 10:35:35.593590 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_sample_metadata_response.py
--rw-r--r--   0        0        0     3044 2023-07-03 10:35:36.389473 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_sample_response.py
--rw-r--r--   0        0        0     2462 2023-07-03 10:35:36.057080 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_syntiant_posterior_response.py
--rw-r--r--   0        0        0     2184 2023-07-03 10:35:36.011918 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
--rw-r--r--   0        0        0     2414 2023-07-03 10:35:35.422724 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_theme_response.py
--rw-r--r--   0        0        0     2117 2023-07-03 10:35:35.366424 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_theme_response_all_of.py
--rw-r--r--   0        0        0     2592 2023-07-03 10:35:35.318492 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_themes_response.py
--rw-r--r--   0        0        0     2285 2023-07-03 10:35:36.175707 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_themes_response_all_of.py
--rw-r--r--   0        0        0     2495 2023-07-03 10:35:35.740790 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_third_party_auth_response.py
--rw-r--r--   0        0        0     2171 2023-07-03 10:35:34.855197 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     2703 2023-07-03 10:35:35.739645 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_user_need_to_set_password_response.py
--rw-r--r--   0        0        0     2436 2023-07-03 10:35:35.702155 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
--rw-r--r--   0        0        0     7717 2023-07-03 10:35:35.140790 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_user_response.py
--rw-r--r--   0        0        0     5708 2023-07-03 10:35:35.643112 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_user_response_all_of.py
--rw-r--r--   0        0        0     2395 2023-07-03 10:35:36.100266 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
--rw-r--r--   0        0        0     2307 2023-07-03 10:35:35.501975 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_whitelabel_domain_response.py
--rw-r--r--   0        0        0     2021 2023-07-03 10:35:35.492959 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
--rw-r--r--   0        0        0     2514 2023-07-03 10:35:35.625019 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_whitelabel_response.py
--rw-r--r--   0        0        0     2217 2023-07-03 10:35:35.755656 edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2776 2023-07-03 10:35:35.221310 edgeimpulse_api-1.25.16/edgeimpulse_api/models/has_data_explorer_features_response.py
--rw-r--r--   0        0        0     2498 2023-07-03 10:35:35.848936 edgeimpulse_api-1.25.16/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0      526 2023-07-03 10:35:35.241968 edgeimpulse_api-1.25.16/edgeimpulse_api/models/image_input_scaling.py
--rw-r--r--   0        0        0     3738 2023-07-03 10:35:35.035443 edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse.py
--rw-r--r--   0        0        0     6723 2023-07-03 10:35:34.985148 edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse_block_version.py
--rw-r--r--   0        0        0     6814 2023-07-03 10:35:35.890930 edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse_dsp_block.py
--rw-r--r--   0        0        0     1967 2023-07-03 10:35:35.935465 edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse_dsp_block_organization.py
--rw-r--r--   0        0        0     8976 2023-07-03 10:35:35.805728 edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse_input_block.py
--rw-r--r--   0        0        0     5612 2023-07-03 10:35:35.602735 edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse_learn_block.py
--rw-r--r--   0        0        0     2463 2023-07-03 10:35:36.342239 edgeimpulse_api-1.25.16/edgeimpulse_api/models/input_block.py
--rw-r--r--   0        0        0     2323 2023-07-03 10:35:35.545391 edgeimpulse_api-1.25.16/edgeimpulse_api/models/invite_organization_member_request.py
--rw-r--r--   0        0        0     3668 2023-07-03 10:35:35.324515 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job.py
--rw-r--r--   0        0        0     4699 2023-07-03 10:35:34.639617 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_details.py
--rw-r--r--   0        0        0     2736 2023-07-03 10:35:36.391127 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_details_all_of.py
--rw-r--r--   0        0        0     2613 2023-07-03 10:35:35.568085 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_details_response.py
--rw-r--r--   0        0        0     2316 2023-07-03 10:35:35.726891 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_details_response_all_of.py
--rw-r--r--   0        0        0     2257 2023-07-03 10:35:34.833070 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_failure_details.py
--rw-r--r--   0        0        0     2657 2023-07-03 10:35:35.887754 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_logs_response.py
--rw-r--r--   0        0        0     2350 2023-07-03 10:35:34.483815 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_logs_response_all_of.py
--rw-r--r--   0        0        0     3297 2023-07-03 10:35:36.450937 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_metrics_response.py
--rw-r--r--   0        0        0     3007 2023-07-03 10:35:35.842338 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_metrics_response_all_of.py
--rw-r--r--   0        0        0      516 2023-07-03 10:35:34.766537 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_parent_type_enum.py
--rw-r--r--   0        0        0     2944 2023-07-03 10:35:34.936869 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_state.py
--rw-r--r--   0        0        0     1966 2023-07-03 10:35:35.584643 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_state_execution_details.py
--rw-r--r--   0        0        0     2965 2023-07-03 10:35:35.344730 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_step.py
--rw-r--r--   0        0        0     2713 2023-07-03 10:35:35.900379 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_summary_response.py
--rw-r--r--   0        0        0     2406 2023-07-03 10:35:34.638154 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_summary_response_all_of.py
--rw-r--r--   0        0        0     2089 2023-07-03 10:35:36.197847 edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_summary_response_all_of_summary.py
--rw-r--r--   0        0        0     2510 2023-07-03 10:35:36.245438 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_layer.py
--rw-r--r--   0        0        0     2093 2023-07-03 10:35:36.275303 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_layer_input.py
--rw-r--r--   0        0        0     2101 2023-07-03 10:35:36.002575 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_layer_output.py
--rw-r--r--   0        0        0     5431 2023-07-03 10:35:35.814231 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_metadata.py
--rw-r--r--   0        0        0     5164 2023-07-03 10:35:36.047229 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_metadata_all_of.py
--rw-r--r--   0        0        0     4792 2023-07-03 10:35:35.535621 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_metadata_metrics.py
--rw-r--r--   0        0        0     3228 2023-07-03 10:35:35.837656 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
--rw-r--r--   0        0        0     2497 2023-07-03 10:35:35.797893 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
--rw-r--r--   0        0        0      562 2023-07-03 10:35:35.937674 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_type_enum.py
--rw-r--r--   0        0        0     9842 2023-07-03 10:35:34.515985 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_response.py
--rw-r--r--   0        0        0     9575 2023-07-03 10:35:35.189333 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_response_all_of.py
--rw-r--r--   0        0        0     3392 2023-07-03 10:35:35.940049 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_visual_layer.py
--rw-r--r--   0        0        0     2310 2023-07-03 10:35:35.741927 edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_visual_layer_type.py
--rw-r--r--   0        0        0     2529 2023-07-03 10:35:34.578572 edgeimpulse_api-1.25.16/edgeimpulse_api/models/last_modification_date_response.py
--rw-r--r--   0        0        0     2239 2023-07-03 10:35:34.996812 edgeimpulse_api-1.25.16/edgeimpulse_api/models/last_modification_date_response_all_of.py
--rw-r--r--   0        0        0     2633 2023-07-03 10:35:35.768873 edgeimpulse_api-1.25.16/edgeimpulse_api/models/latency_device.py
--rw-r--r--   0        0        0     2424 2023-07-03 10:35:34.800432 edgeimpulse_api-1.25.16/edgeimpulse_api/models/learn_block.py
--rw-r--r--   0        0        0      883 2023-07-03 10:35:36.054903 edgeimpulse_api-1.25.16/edgeimpulse_api/models/learn_block_type.py
--rw-r--r--   0        0        0     2788 2023-07-03 10:35:35.918083 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_api_keys_response.py
--rw-r--r--   0        0        0     2488 2023-07-03 10:35:34.841042 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2682 2023-07-03 10:35:36.051072 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2630 2023-07-03 10:35:35.795948 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_devices_response.py
--rw-r--r--   0        0        0     2333 2023-07-03 10:35:34.492991 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_devices_response_all_of.py
--rw-r--r--   0        0        0     2726 2023-07-03 10:35:35.282093 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_email_response.py
--rw-r--r--   0        0        0     2426 2023-07-03 10:35:35.511280 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_email_response_all_of.py
--rw-r--r--   0        0        0     2918 2023-07-03 10:35:35.631687 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_email_response_all_of_emails.py
--rw-r--r--   0        0        0     2813 2023-07-03 10:35:35.982581 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_hmac_keys_response.py
--rw-r--r--   0        0        0     2513 2023-07-03 10:35:35.564591 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
--rw-r--r--   0        0        0     2381 2023-07-03 10:35:35.385272 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
--rw-r--r--   0        0        0     2745 2023-07-03 10:35:34.561902 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_jobs_response.py
--rw-r--r--   0        0        0     2445 2023-07-03 10:35:35.428445 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_jobs_response_all_of.py
--rw-r--r--   0        0        0     2200 2023-07-03 10:35:35.650183 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_models_response.py
--rw-r--r--   0        0        0     1910 2023-07-03 10:35:36.415774 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_models_response_all_of.py
--rw-r--r--   0        0        0     2921 2023-07-03 10:35:36.154348 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_api_keys_response.py
--rw-r--r--   0        0        0     2621 2023-07-03 10:35:35.030369 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2760 2023-07-03 10:35:35.213279 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2857 2023-07-03 10:35:35.208148 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_response.py
--rw-r--r--   0        0        0     2550 2023-07-03 10:35:36.328173 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
--rw-r--r--   0        0        0     2995 2023-07-03 10:35:36.252495 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py
--rw-r--r--   0        0        0     2902 2023-07-03 10:35:35.751056 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_user_response.py
--rw-r--r--   0        0        0     2595 2023-07-03 10:35:35.615749 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
--rw-r--r--   0        0        0     2760 2023-07-03 10:35:35.170892 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
--rw-r--r--   0        0        0     3310 2023-07-03 10:35:35.829549 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_data_response.py
--rw-r--r--   0        0        0     3031 2023-07-03 10:35:34.902041 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_data_response_all_of.py
--rw-r--r--   0        0        0     3430 2023-07-03 10:35:36.378082 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
--rw-r--r--   0        0        0     2887 2023-07-03 10:35:36.167334 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
--rw-r--r--   0        0        0     2587 2023-07-03 10:35:34.862934 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
--rw-r--r--   0        0        0     2824 2023-07-03 10:35:35.331220 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
--rw-r--r--   0        0        0     2524 2023-07-03 10:35:36.122120 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
--rw-r--r--   0        0        0     3353 2023-07-03 10:35:35.275958 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_files_response.py
--rw-r--r--   0        0        0     3074 2023-07-03 10:35:35.802607 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_files_response_all_of.py
--rw-r--r--   0        0        0     2792 2023-07-03 10:35:35.270380 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_pipelines_response.py
--rw-r--r--   0        0        0     2485 2023-07-03 10:35:34.834571 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     2857 2023-07-03 10:35:35.628554 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_portals_response.py
--rw-r--r--   0        0        0     2550 2023-07-03 10:35:35.811090 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_portals_response_all_of.py
--rw-r--r--   0        0        0     2744 2023-07-03 10:35:36.138828 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
--rw-r--r--   0        0        0     3449 2023-07-03 10:35:35.092646 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_projects_data_response.py
--rw-r--r--   0        0        0     3142 2023-07-03 10:35:35.248542 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
--rw-r--r--   0        0        0     2271 2023-07-03 10:35:35.415019 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
--rw-r--r--   0        0        0     2723 2023-07-03 10:35:35.623960 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_projects_response.py
--rw-r--r--   0        0        0     2416 2023-07-03 10:35:35.375759 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_projects_response_all_of.py
--rw-r--r--   0        0        0     2857 2023-07-03 10:35:34.716271 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_secrets_response.py
--rw-r--r--   0        0        0     2550 2023-07-03 10:35:34.776969 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
--rw-r--r--   0        0        0     2265 2023-07-03 10:35:36.117155 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
--rw-r--r--   0        0        0     3103 2023-07-03 10:35:35.173847 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
--rw-r--r--   0        0        0     2803 2023-07-03 10:35:36.172784 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
--rw-r--r--   0        0        0     3055 2023-07-03 10:35:35.462086 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2755 2023-07-03 10:35:35.704642 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2786 2023-07-03 10:35:35.847522 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organizations_response.py
--rw-r--r--   0        0        0     2486 2023-07-03 10:35:36.443066 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organizations_response_all_of.py
--rw-r--r--   0        0        0     1937 2023-07-03 10:35:35.382910 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_portal_files_in_folder_request.py
--rw-r--r--   0        0        0     2713 2023-07-03 10:35:35.933104 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_portal_files_in_folder_response.py
--rw-r--r--   0        0        0     2416 2023-07-03 10:35:35.437864 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2290 2023-07-03 10:35:35.735120 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_projects.py
--rw-r--r--   0        0        0     2681 2023-07-03 10:35:36.432650 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_projects_response.py
--rw-r--r--   0        0        0     2553 2023-07-03 10:35:35.557419 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_public_projects.py
--rw-r--r--   0        0        0     2944 2023-07-03 10:35:35.083131 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_public_projects_response.py
--rw-r--r--   0        0        0     2815 2023-07-03 10:35:35.783857 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_public_versions_response.py
--rw-r--r--   0        0        0     2508 2023-07-03 10:35:35.728501 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_public_versions_response_all_of.py
--rw-r--r--   0        0        0     2290 2023-07-03 10:35:36.210982 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2754 2023-07-03 10:35:35.048427 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_samples_response.py
--rw-r--r--   0        0        0     2454 2023-07-03 10:35:35.369279 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_samples_response_all_of.py
--rw-r--r--   0        0        0     3933 2023-07-03 10:35:35.306111 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_versions_response.py
--rw-r--r--   0        0        0     3633 2023-07-03 10:35:34.812379 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_versions_response_all_of.py
--rw-r--r--   0        0        0     2353 2023-07-03 10:35:36.344934 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
--rw-r--r--   0        0        0     2053 2023-07-03 10:35:35.231931 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
--rw-r--r--   0        0        0     3960 2023-07-03 10:35:35.204803 edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2900 2023-07-03 10:35:36.196544 edgeimpulse_api-1.25.16/edgeimpulse_api/models/log_stdout_response.py
--rw-r--r--   0        0        0     2600 2023-07-03 10:35:36.248358 edgeimpulse_api-1.25.16/edgeimpulse_api/models/log_stdout_response_all_of.py
--rw-r--r--   0        0        0     2441 2023-07-03 10:35:35.289195 edgeimpulse_api-1.25.16/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
--rw-r--r--   0        0        0     2191 2023-07-03 10:35:35.423854 edgeimpulse_api-1.25.16/edgeimpulse_api/models/log_website_pageview_request.py
--rw-r--r--   0        0        0     2217 2023-07-03 10:35:34.689267 edgeimpulse_api-1.25.16/edgeimpulse_api/models/login_response.py
--rw-r--r--   0        0        0     1911 2023-07-03 10:35:35.898004 edgeimpulse_api-1.25.16/edgeimpulse_api/models/login_response_all_of.py
--rw-r--r--   0        0        0     2430 2023-07-03 10:35:36.227889 edgeimpulse_api-1.25.16/edgeimpulse_api/models/migration.py
--rw-r--r--   0        0        0     2521 2023-07-03 10:35:36.088309 edgeimpulse_api-1.25.16/edgeimpulse_api/models/model_prediction.py
--rw-r--r--   0        0        0     2895 2023-07-03 10:35:35.732879 edgeimpulse_api-1.25.16/edgeimpulse_api/models/model_result.py
--rw-r--r--   0        0        0     5046 2023-07-03 10:35:36.279843 edgeimpulse_api-1.25.16/edgeimpulse_api/models/model_variant_stats.py
--rw-r--r--   0        0        0     2128 2023-07-03 10:35:35.717470 edgeimpulse_api-1.25.16/edgeimpulse_api/models/move_raw_data_request.py
--rw-r--r--   0        0        0     2687 2023-07-03 10:35:36.255128 edgeimpulse_api-1.25.16/edgeimpulse_api/models/note.py
--rw-r--r--   0        0        0     2221 2023-07-03 10:35:35.721492 edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_auto_label_request.py
--rw-r--r--   0        0        0     2994 2023-07-03 10:35:35.678540 edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_auto_label_response.py
--rw-r--r--   0        0        0     2705 2023-07-03 10:35:35.080426 edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
--rw-r--r--   0        0        0     2275 2023-07-03 10:35:36.318434 edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
--rw-r--r--   0        0        0     2368 2023-07-03 10:35:36.000143 edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_label_queue_count_response.py
--rw-r--r--   0        0        0     2051 2023-07-03 10:35:35.283644 edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
--rw-r--r--   0        0        0     2887 2023-07-03 10:35:36.407012 edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_label_queue_response.py
--rw-r--r--   0        0        0     2580 2023-07-03 10:35:36.089477 edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
--rw-r--r--   0        0        0      621 2023-07-03 10:35:36.153005 edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_last_layer.py
--rw-r--r--   0        0        0     6418 2023-07-03 10:35:35.868551 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_config.py
--rw-r--r--   0        0        0     6871 2023-07-03 10:35:36.398918 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_config_response.py
--rw-r--r--   0        0        0     1920 2023-07-03 10:35:35.792640 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_config_response_all_of.py
--rw-r--r--   0        0        0     2067 2023-07-03 10:35:35.787407 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_config_target_device.py
--rw-r--r--   0        0        0     2271 2023-07-03 10:35:34.609950 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_dsp_parameters_response.py
--rw-r--r--   0        0        0     1964 2023-07-03 10:35:36.234515 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
--rw-r--r--   0        0        0     2756 2023-07-03 10:35:36.233400 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_space_response.py
--rw-r--r--   0        0        0     2456 2023-07-03 10:35:34.549553 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_space_response_all_of.py
--rw-r--r--   0        0        0     4897 2023-07-03 10:35:35.150920 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_state_response.py
--rw-r--r--   0        0        0     4618 2023-07-03 10:35:35.436420 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_state_response_all_of.py
--rw-r--r--   0        0        0     3419 2023-07-03 10:35:35.197711 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_state_response_all_of_status.py
--rw-r--r--   0        0        0     2366 2023-07-03 10:35:36.125409 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
--rw-r--r--   0        0        0     2760 2023-07-03 10:35:35.950510 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
--rw-r--r--   0        0        0     2463 2023-07-03 10:35:36.376321 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
--rw-r--r--   0        0        0     4682 2023-07-03 10:35:35.505896 edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
--rw-r--r--   0        0        0     3774 2023-07-03 10:35:35.257234 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization.py
--rw-r--r--   0        0        0     2359 2023-07-03 10:35:35.938759 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_add_data_folder_request.py
--rw-r--r--   0        0        0     2498 2023-07-03 10:35:36.465021 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_add_data_folder_response.py
--rw-r--r--   0        0        0     2209 2023-07-03 10:35:36.375013 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
--rw-r--r--   0        0        0     2549 2023-07-03 10:35:35.226896 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_add_dataset_request.py
--rw-r--r--   0        0        0     2460 2023-07-03 10:35:35.911210 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
--rw-r--r--   0        0        0     8598 2023-07-03 10:35:36.019352 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project.py
--rw-r--r--   0        0        0     5176 2023-07-03 10:35:35.583483 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_request.py
--rw-r--r--   0        0        0     2543 2023-07-03 10:35:34.885536 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_response.py
--rw-r--r--   0        0        0     2237 2023-07-03 10:35:36.400415 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_response_all_of.py
--rw-r--r--   0        0        0     2704 2023-07-03 10:35:36.466671 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_status_response.py
--rw-r--r--   0        0        0     2407 2023-07-03 10:35:35.550399 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
--rw-r--r--   0        0        0     2501 2023-07-03 10:35:35.202434 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_transformation_summary.py
--rw-r--r--   0        0        0     9325 2023-07-03 10:35:35.637095 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_with_files.py
--rw-r--r--   0        0        0     2558 2023-07-03 10:35:35.899184 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
--rw-r--r--   0        0        0     3034 2023-07-03 10:35:36.384148 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
--rw-r--r--   0        0        0     2559 2023-07-03 10:35:36.200635 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_campaign_diff_request.py
--rw-r--r--   0        0        0     2327 2023-07-03 10:35:35.607411 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
--rw-r--r--   0        0        0     3041 2023-07-03 10:35:36.267817 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_campaign_diff_response.py
--rw-r--r--   0        0        0     2741 2023-07-03 10:35:35.915840 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
--rw-r--r--   0        0        0     2468 2023-07-03 10:35:34.497024 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
--rw-r--r--   0        0        0     3476 2023-07-03 10:35:35.298656 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_item.py
--rw-r--r--   0        0        0     2103 2023-07-03 10:35:35.279157 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_item_files_inner.py
--rw-r--r--   0        0        0     3529 2023-07-03 10:35:36.036498 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_dataset.py
--rw-r--r--   0        0        0     2767 2023-07-03 10:35:35.267176 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_dataset_bucket.py
--rw-r--r--   0        0        0     4689 2023-07-03 10:35:34.708775 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_deploy_block.py
--rw-r--r--   0        0        0     3646 2023-07-03 10:35:35.865286 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_dsp_block.py
--rw-r--r--   0        0        0     3037 2023-07-03 10:35:36.013237 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_get_create_projects_response.py
--rw-r--r--   0        0        0     2737 2023-07-03 10:35:35.336911 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
--rw-r--r--   0        0        0     5707 2023-07-03 10:35:36.217658 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
--rw-r--r--   0        0        0     6331 2023-07-03 10:35:35.656282 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response.py
--rw-r--r--   0        0        0     6041 2023-07-03 10:35:35.746091 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response_all_of.py
--rw-r--r--   0        0        0     3915 2023-07-03 10:35:36.190325 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
--rw-r--r--   0        0        0     2267 2023-07-03 10:35:35.527794 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
--rw-r--r--   0        0        0     2338 2023-07-03 10:35:35.425618 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
--rw-r--r--   0        0        0     2458 2023-07-03 10:35:34.717927 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
--rw-r--r--   0        0        0      525 2023-07-03 10:35:36.222086 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_member_role.py
--rw-r--r--   0        0        0     2639 2023-07-03 10:35:35.613097 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_metrics_response.py
--rw-r--r--   0        0        0     2315 2023-07-03 10:35:34.941318 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_metrics_response_all_of.py
--rw-r--r--   0        0        0     3453 2023-07-03 10:35:34.994535 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
--rw-r--r--   0        0        0     6132 2023-07-03 10:35:35.951999 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline.py
--rw-r--r--   0        0        0     2595 2023-07-03 10:35:35.730911 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
--rw-r--r--   0        0        0     2275 2023-07-03 10:35:36.256418 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
--rw-r--r--   0        0        0     2314 2023-07-03 10:35:35.397260 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_item_count.py
--rw-r--r--   0        0        0     4109 2023-07-03 10:35:35.621117 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_run.py
--rw-r--r--   0        0        0     5213 2023-07-03 10:35:35.263608 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_run_step.py
--rw-r--r--   0        0        0     4813 2023-07-03 10:35:36.065950 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_step.py
--rw-r--r--   0        0        0     2351 2023-07-03 10:35:35.222588 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
--rw-r--r--   0        0        0     2344 2023-07-03 10:35:36.220248 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
--rw-r--r--   0        0        0     2037 2023-07-03 10:35:35.698857 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_projects_data_batch_request.py
--rw-r--r--   0        0        0     4932 2023-07-03 10:35:35.321626 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_transfer_learning_block.py
--rw-r--r--   0        0        0      611 2023-07-03 10:35:36.103021 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
--rw-r--r--   0        0        0     5168 2023-07-03 10:35:35.772623 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_transformation_block.py
--rw-r--r--   0        0        0     3907 2023-07-03 10:35:34.487318 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_update_pipeline_body.py
--rw-r--r--   0        0        0     4225 2023-07-03 10:35:36.263663 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_user.py
--rw-r--r--   0        0        0     2294 2023-07-03 10:35:35.596954 edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_user_all_of.py
--rw-r--r--   0        0        0     2104 2023-07-03 10:35:34.651563 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_detection.py
--rw-r--r--   0        0        0     3434 2023-07-03 10:35:35.540409 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_false_positive.py
--rw-r--r--   0        0        0     3770 2023-07-03 10:35:35.517542 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_ground_truth.py
--rw-r--r--   0        0        0     2477 2023-07-03 10:35:34.693686 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
--rw-r--r--   0        0        0     4880 2023-07-03 10:35:34.625342 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_parameter_set.py
--rw-r--r--   0        0        0     2255 2023-07-03 10:35:35.870067 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
--rw-r--r--   0        0        0     4092 2023-07-03 10:35:34.874621 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
--rw-r--r--   0        0        0     3007 2023-07-03 10:35:36.412277 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_parameters.py
--rw-r--r--   0        0        0     2585 2023-07-03 10:35:35.402603 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_parameters_standard.py
--rw-r--r--   0        0        0     2250 2023-07-03 10:35:35.647504 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_raw_detection.py
--rw-r--r--   0        0        0     2366 2023-07-03 10:35:36.060053 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
--rw-r--r--   0        0        0     2412 2023-07-03 10:35:35.901530 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
--rw-r--r--   0        0        0     2106 2023-07-03 10:35:35.114182 edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
--rw-r--r--   0        0        0     1574 2023-07-03 10:35:35.186605 edgeimpulse_api-1.25.16/edgeimpulse_api/models/permission.py
--rw-r--r--   0        0        0     2211 2023-07-03 10:35:36.015584 edgeimpulse_api-1.25.16/edgeimpulse_api/models/portal_file.py
--rw-r--r--   0        0        0     2413 2023-07-03 10:35:35.300195 edgeimpulse_api-1.25.16/edgeimpulse_api/models/portal_info_response.py
--rw-r--r--   0        0        0     2666 2023-07-03 10:35:35.606297 edgeimpulse_api-1.25.16/edgeimpulse_api/models/pretrained_model_tensor.py
--rw-r--r--   0        0        0     2955 2023-07-03 10:35:35.854508 edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_info.py
--rw-r--r--   0        0        0     2640 2023-07-03 10:35:35.548165 edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_info_memory.py
--rw-r--r--   0        0        0     1918 2023-07-03 10:35:35.790872 edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_info_memory_eon.py
--rw-r--r--   0        0        0     2065 2023-07-03 10:35:35.533605 edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_info_memory_tflite.py
--rw-r--r--   0        0        0     4335 2023-07-03 10:35:36.140733 edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_table.py
--rw-r--r--   0        0        0     2780 2023-07-03 10:35:35.393458 edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_table_mcu.py
--rw-r--r--   0        0        0     2565 2023-07-03 10:35:35.605093 edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_table_mcu_memory.py
--rw-r--r--   0        0        0     2250 2023-07-03 10:35:35.459110 edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_table_mpu.py
--rw-r--r--   0        0        0     2201 2023-07-03 10:35:36.105623 edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_tf_lite_request.py
--rw-r--r--   0        0        0     3292 2023-07-03 10:35:35.753096 edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_tf_lite_response.py
--rw-r--r--   0        0        0     6139 2023-07-03 10:35:36.351174 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project.py
--rw-r--r--   0        0        0     3888 2023-07-03 10:35:35.327922 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_collaborator.py
--rw-r--r--   0        0        0     1895 2023-07-03 10:35:35.907885 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_collaborator_all_of.py
--rw-r--r--   0        0        0     2416 2023-07-03 10:35:36.158569 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_data_axes_summary_response.py
--rw-r--r--   0        0        0     2116 2023-07-03 10:35:34.642174 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
--rw-r--r--   0        0        0     2281 2023-07-03 10:35:35.553630 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_data_interval_response.py
--rw-r--r--   0        0        0     1964 2023-07-03 10:35:35.193013 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_data_interval_response_all_of.py
--rw-r--r--   0        0        0     2235 2023-07-03 10:35:34.831564 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_data_summary.py
--rw-r--r--   0        0        0     6854 2023-07-03 10:35:36.091091 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_deployment_target.py
--rw-r--r--   0        0        0     2706 2023-07-03 10:35:36.273356 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_deployment_target_all_of.py
--rw-r--r--   0        0        0     2780 2023-07-03 10:35:35.695639 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_deployment_targets_response.py
--rw-r--r--   0        0        0     2473 2023-07-03 10:35:34.725411 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     2680 2023-07-03 10:35:34.794794 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_downloads_response.py
--rw-r--r--   0        0        0     2373 2023-07-03 10:35:35.515793 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_downloads_response_all_of.py
--rw-r--r--   0        0        0    13550 2023-07-03 10:35:36.370522 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response.py
--rw-r--r--   0        0        0    13283 2023-07-03 10:35:36.396690 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of.py
--rw-r--r--   0        0        0     3130 2023-07-03 10:35:34.539034 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
--rw-r--r--   0        0        0     2723 2023-07-03 10:35:36.262235 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
--rw-r--r--   0        0        0     2997 2023-07-03 10:35:35.693540 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
--rw-r--r--   0        0        0     2979 2023-07-03 10:35:35.169829 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
--rw-r--r--   0        0        0     2339 2023-07-03 10:35:36.130502 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_experiments.py
--rw-r--r--   0        0        0     2285 2023-07-03 10:35:36.202100 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_impulse.py
--rw-r--r--   0        0        0     2726 2023-07-03 10:35:35.689822 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_performance.py
--rw-r--r--   0        0        0     1977 2023-07-03 10:35:36.250494 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_readme.py
--rw-r--r--   0        0        0     2225 2023-07-03 10:35:35.845968 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
--rw-r--r--   0        0        0     2735 2023-07-03 10:35:35.142198 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_urls.py
--rw-r--r--   0        0        0     2478 2023-07-03 10:35:34.957726 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_summary_response.py
--rw-r--r--   0        0        0     2172 2023-07-03 10:35:35.296014 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_summary_response_all_of.py
--rw-r--r--   0        0        0     3554 2023-07-03 10:35:34.691690 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_private_data.py
--rw-r--r--   0        0        0     4396 2023-07-03 10:35:34.674346 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_public_data.py
--rw-r--r--   0        0        0     1928 2023-07-03 10:35:35.669293 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_public_data_readme.py
--rw-r--r--   0        0        0     2404 2023-07-03 10:35:36.253937 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_sample_metadata.py
--rw-r--r--   0        0        0     2670 2023-07-03 10:35:35.179098 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_training_data_summary_response.py
--rw-r--r--   0        0        0     2353 2023-07-03 10:35:36.232191 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
--rw-r--r--   0        0        0     2316 2023-07-03 10:35:35.406597 edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_version_request.py
--rw-r--r--   0        0        0     2664 2023-07-03 10:35:34.969909 edgeimpulse_api-1.25.16/edgeimpulse_api/models/raw_sample_data.py
--rw-r--r--   0        0        0     3440 2023-07-03 10:35:36.348993 edgeimpulse_api-1.25.16/edgeimpulse_api/models/raw_sample_payload.py
--rw-r--r--   0        0        0     2537 2023-07-03 10:35:36.421071 edgeimpulse_api-1.25.16/edgeimpulse_api/models/rebalance_dataset_response.py
--rw-r--r--   0        0        0     1984 2023-07-03 10:35:35.575965 edgeimpulse_api-1.25.16/edgeimpulse_api/models/remove_collaborator_request.py
--rw-r--r--   0        0        0     1805 2023-07-03 10:35:35.874213 edgeimpulse_api-1.25.16/edgeimpulse_api/models/remove_member_request.py
--rw-r--r--   0        0        0     1867 2023-07-03 10:35:35.465008 edgeimpulse_api-1.25.16/edgeimpulse_api/models/rename_device_request.py
--rw-r--r--   0        0        0     2081 2023-07-03 10:35:35.365059 edgeimpulse_api-1.25.16/edgeimpulse_api/models/rename_portal_file_request.py
--rw-r--r--   0        0        0     1867 2023-07-03 10:35:36.339018 edgeimpulse_api-1.25.16/edgeimpulse_api/models/rename_sample_request.py
--rw-r--r--   0        0        0     1873 2023-07-03 10:35:34.802210 edgeimpulse_api-1.25.16/edgeimpulse_api/models/request_reset_password_request.py
--rw-r--r--   0        0        0     2031 2023-07-03 10:35:36.353936 edgeimpulse_api-1.25.16/edgeimpulse_api/models/reset_password_request.py
--rw-r--r--   0        0        0     1985 2023-07-03 10:35:35.654628 edgeimpulse_api-1.25.16/edgeimpulse_api/models/restore_project_from_public_request.py
--rw-r--r--   0        0        0     2265 2023-07-03 10:35:36.243597 edgeimpulse_api-1.25.16/edgeimpulse_api/models/restore_project_request.py
--rw-r--r--   0        0        0     2244 2023-07-03 10:35:35.807031 edgeimpulse_api-1.25.16/edgeimpulse_api/models/run_auto_segmenter_request.py
--rw-r--r--   0        0        0     2669 2023-07-03 10:35:36.308282 edgeimpulse_api-1.25.16/edgeimpulse_api/models/run_organization_pipeline_response.py
--rw-r--r--   0        0        0     2352 2023-07-03 10:35:34.719602 edgeimpulse_api-1.25.16/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
--rw-r--r--   0        0        0     9637 2023-07-03 10:35:35.941959 edgeimpulse_api-1.25.16/edgeimpulse_api/models/sample.py
--rw-r--r--   0        0        0     2443 2023-07-03 10:35:35.028330 edgeimpulse_api-1.25.16/edgeimpulse_api/models/sample_bounding_boxes_request.py
--rw-r--r--   0        0        0     2000 2023-07-03 10:35:34.857938 edgeimpulse_api-1.25.16/edgeimpulse_api/models/sample_metadata.py
--rw-r--r--   0        0        0     2539 2023-07-03 10:35:34.599207 edgeimpulse_api-1.25.16/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py
--rw-r--r--   0        0        0     2085 2023-07-03 10:35:35.245691 edgeimpulse_api-1.25.16/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py
--rw-r--r--   0        0        0     2355 2023-07-03 10:35:35.658623 edgeimpulse_api-1.25.16/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py
--rw-r--r--   0        0        0     2038 2023-07-03 10:35:35.338950 edgeimpulse_api-1.25.16/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py
--rw-r--r--   0        0        0     2756 2023-07-03 10:35:34.912783 edgeimpulse_api-1.25.16/edgeimpulse_api/models/save_pretrained_model_request.py
--rw-r--r--   0        0        0     3327 2023-07-03 10:35:35.521629 edgeimpulse_api-1.25.16/edgeimpulse_api/models/score_trial_response.py
--rw-r--r--   0        0        0     3003 2023-07-03 10:35:36.463332 edgeimpulse_api-1.25.16/edgeimpulse_api/models/score_trial_response_all_of.py
--rw-r--r--   0        0        0     2240 2023-07-03 10:35:35.453333 edgeimpulse_api-1.25.16/edgeimpulse_api/models/score_trial_response_all_of_latency.py
--rw-r--r--   0        0        0     1914 2023-07-03 10:35:36.208869 edgeimpulse_api-1.25.16/edgeimpulse_api/models/score_trial_response_all_of_ram.py
--rw-r--r--   0        0        0     2405 2023-07-03 10:35:35.219191 edgeimpulse_api-1.25.16/edgeimpulse_api/models/segment_sample_request.py
--rw-r--r--   0        0        0     2055 2023-07-03 10:35:36.382019 edgeimpulse_api-1.25.16/edgeimpulse_api/models/segment_sample_request_segments_inner.py
--rw-r--r--   0        0        0     3364 2023-07-03 10:35:35.800364 edgeimpulse_api-1.25.16/edgeimpulse_api/models/send_user_feedback_request.py
--rw-r--r--   0        0        0     1981 2023-07-03 10:35:34.894950 edgeimpulse_api-1.25.16/edgeimpulse_api/models/sensor.py
--rw-r--r--   0        0        0     2142 2023-07-03 10:35:36.155545 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_anomaly_parameter_request.py
--rw-r--r--   0        0        0     8028 2023-07-03 10:35:35.033862 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_keras_parameter_request.py
--rw-r--r--   0        0        0     1893 2023-07-03 10:35:36.340554 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_member_datasets_request.py
--rw-r--r--   0        0        0     1905 2023-07-03 10:35:36.069124 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_member_role_request.py
--rw-r--r--   0        0        0     2219 2023-07-03 10:35:36.147496 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_optimize_space_request.py
--rw-r--r--   0        0        0     2254 2023-07-03 10:35:36.164754 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_optimize_space_request_all_of.py
--rw-r--r--   0        0        0     1923 2023-07-03 10:35:36.445320 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_organization_data_dataset_request.py
--rw-r--r--   0        0        0     1974 2023-07-03 10:35:35.379949 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_project_compute_time_request.py
--rw-r--r--   0        0        0     2011 2023-07-03 10:35:35.688414 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_project_dsp_file_size_request.py
--rw-r--r--   0        0        0     1919 2023-07-03 10:35:35.089547 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_sample_metadata_request.py
--rw-r--r--   0        0        0     1915 2023-07-03 10:35:35.640124 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_syntiant_posterior_request.py
--rw-r--r--   0        0        0     2140 2023-07-03 10:35:35.448965 edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_user_password_request.py
--rw-r--r--   0        0        0     2536 2023-07-03 10:35:35.135182 edgeimpulse_api-1.25.16/edgeimpulse_api/models/socket_token_response.py
--rw-r--r--   0        0        0     2239 2023-07-03 10:35:36.064317 edgeimpulse_api-1.25.16/edgeimpulse_api/models/socket_token_response_all_of.py
--rw-r--r--   0        0        0     2059 2023-07-03 10:35:34.572783 edgeimpulse_api-1.25.16/edgeimpulse_api/models/socket_token_response_all_of_token.py
--rw-r--r--   0        0        0     1971 2023-07-03 10:35:35.195707 edgeimpulse_api-1.25.16/edgeimpulse_api/models/split_sample_in_frames_request.py
--rw-r--r--   0        0        0     2110 2023-07-03 10:35:35.023261 edgeimpulse_api-1.25.16/edgeimpulse_api/models/staff_info.py
--rw-r--r--   0        0        0     2226 2023-07-03 10:35:35.763161 edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_job_response.py
--rw-r--r--   0        0        0     1909 2023-07-03 10:35:34.607058 edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_job_response_all_of.py
--rw-r--r--   0        0        0     2883 2023-07-03 10:35:35.542700 edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_performance_calibration_request.py
--rw-r--r--   0        0        0     2838 2023-07-03 10:35:35.995434 edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_sampling_request.py
--rw-r--r--   0        0        0     2189 2023-07-03 10:35:35.923683 edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_sampling_response.py
--rw-r--r--   0        0        0     1892 2023-07-03 10:35:35.674409 edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_sampling_response_all_of.py
--rw-r--r--   0        0        0     2492 2023-07-03 10:35:35.661170 edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_training_request_anomaly.py
--rw-r--r--   0        0        0     1967 2023-07-03 10:35:34.738437 edgeimpulse_api-1.25.16/edgeimpulse_api/models/store_segment_length_request.py
--rw-r--r--   0        0        0     3460 2023-07-03 10:35:36.151482 edgeimpulse_api-1.25.16/edgeimpulse_api/models/structured_classify_result.py
--rw-r--r--   0        0        0     2433 2023-07-03 10:35:34.547530 edgeimpulse_api-1.25.16/edgeimpulse_api/models/test_pretrained_model_request.py
--rw-r--r--   0        0        0     3074 2023-07-03 10:35:36.203382 edgeimpulse_api-1.25.16/edgeimpulse_api/models/test_pretrained_model_response.py
--rw-r--r--   0        0        0     2784 2023-07-03 10:35:35.863635 edgeimpulse_api-1.25.16/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3251 2023-07-03 10:35:35.122206 edgeimpulse_api-1.25.16/edgeimpulse_api/models/theme.py
--rw-r--r--   0        0        0     2239 2023-07-03 10:35:35.598101 edgeimpulse_api-1.25.16/edgeimpulse_api/models/theme_colors.py
--rw-r--r--   0        0        0     2764 2023-07-03 10:35:35.390024 edgeimpulse_api-1.25.16/edgeimpulse_api/models/theme_favicon.py
--rw-r--r--   0        0        0     2721 2023-07-03 10:35:35.463604 edgeimpulse_api-1.25.16/edgeimpulse_api/models/theme_logos.py
--rw-r--r--   0        0        0     2245 2023-07-03 10:35:35.354126 edgeimpulse_api-1.25.16/edgeimpulse_api/models/third_party_auth.py
--rw-r--r--   0        0        0     1921 2023-07-03 10:35:35.172214 edgeimpulse_api-1.25.16/edgeimpulse_api/models/time_series_data_point.py
--rw-r--r--   0        0        0     2031 2023-07-03 10:35:35.359839 edgeimpulse_api-1.25.16/edgeimpulse_api/models/track_objects_request.py
--rw-r--r--   0        0        0     2736 2023-07-03 10:35:35.779441 edgeimpulse_api-1.25.16/edgeimpulse_api/models/track_objects_response.py
--rw-r--r--   0        0        0     2436 2023-07-03 10:35:35.303481 edgeimpulse_api-1.25.16/edgeimpulse_api/models/track_objects_response_all_of.py
--rw-r--r--   0        0        0     5295 2023-07-03 10:35:35.259534 edgeimpulse_api-1.25.16/edgeimpulse_api/models/transfer_learning_model.py
--rw-r--r--   0        0        0     2012 2023-07-03 10:35:34.977873 edgeimpulse_api-1.25.16/edgeimpulse_api/models/transfer_ownership_organization_request.py
--rw-r--r--   0        0        0     2585 2023-07-03 10:35:36.108145 edgeimpulse_api-1.25.16/edgeimpulse_api/models/transformation_block_additional_mount_point.py
--rw-r--r--   0        0        0      588 2023-07-03 10:35:36.118573 edgeimpulse_api-1.25.16/edgeimpulse_api/models/transformation_job_status_enum.py
--rw-r--r--   0        0        0     2578 2023-07-03 10:35:35.824754 edgeimpulse_api-1.25.16/edgeimpulse_api/models/tuner_create_trial_impulse.py
--rw-r--r--   0        0        0     2570 2023-07-03 10:35:34.608555 edgeimpulse_api-1.25.16/edgeimpulse_api/models/tuner_space_impulse.py
--rw-r--r--   0        0        0     3661 2023-07-03 10:35:36.260979 edgeimpulse_api-1.25.16/edgeimpulse_api/models/tuner_trial.py
--rw-r--r--   0        0        0     2304 2023-07-03 10:35:35.391492 edgeimpulse_api-1.25.16/edgeimpulse_api/models/tuner_trial_blocks_inner.py
--rw-r--r--   0        0        0     2028 2023-07-03 10:35:35.268784 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_job_request.py
--rw-r--r--   0        0        0     2281 2023-07-03 10:35:35.313681 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_add_collaborator_request.py
--rw-r--r--   0        0        0     2882 2023-07-03 10:35:35.826033 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_bucket_request.py
--rw-r--r--   0        0        0     2578 2023-07-03 10:35:36.229669 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_create_empty_project_request.py
--rw-r--r--   0        0        0     2428 2023-07-03 10:35:34.545079 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_create_project_request.py
--rw-r--r--   0        0        0     2764 2023-07-03 10:35:35.919962 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     4154 2023-07-03 10:35:35.993011 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2158 2023-07-03 10:35:36.168932 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_data_item_request.py
--rw-r--r--   0        0        0     2624 2023-07-03 10:35:36.334233 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_dataset_request.py
--rw-r--r--   0        0        0     2881 2023-07-03 10:35:36.373732 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2724 2023-07-03 10:35:35.362156 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_portal_response.py
--rw-r--r--   0        0        0     2445 2023-07-03 10:35:35.862144 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2582 2023-07-03 10:35:35.989553 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_request.py
--rw-r--r--   0        0        0     4439 2023-07-03 10:35:36.123596 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     4734 2023-07-03 10:35:36.170857 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_transformation_block_request.py
--rw-r--r--   0        0        0     8081 2023-07-03 10:35:35.761765 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_project_request.py
--rw-r--r--   0        0        0     1877 2023-07-03 10:35:35.439361 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_project_tags_request.py
--rw-r--r--   0        0        0     2259 2023-07-03 10:35:35.152139 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_theme_colors_request.py
--rw-r--r--   0        0        0     2895 2023-07-03 10:35:35.149079 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_theme_logos_request.py
--rw-r--r--   0        0        0     2205 2023-07-03 10:35:35.925613 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_third_party_auth_request.py
--rw-r--r--   0        0        0     2603 2023-07-03 10:35:35.037526 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_user_request.py
--rw-r--r--   0        0        0     1886 2023-07-03 10:35:35.512259 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_version_request.py
--rw-r--r--   0        0        0     2393 2023-07-03 10:35:35.081681 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
--rw-r--r--   0        0        0     2237 2023-07-03 10:35:34.682887 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
--rw-r--r--   0        0        0     2125 2023-07-03 10:35:36.277563 edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
--rw-r--r--   0        0        0     2168 2023-07-03 10:35:35.738513 edgeimpulse_api-1.25.16/edgeimpulse_api/models/upload_asset_response.py
--rw-r--r--   0        0        0     1882 2023-07-03 10:35:35.342935 edgeimpulse_api-1.25.16/edgeimpulse_api/models/upload_asset_response_all_of.py
--rw-r--r--   0        0        0     2199 2023-07-03 10:35:34.601894 edgeimpulse_api-1.25.16/edgeimpulse_api/models/upload_readme_image_response.py
--rw-r--r--   0        0        0     2185 2023-07-03 10:35:35.803808 edgeimpulse_api-1.25.16/edgeimpulse_api/models/upload_user_photo_response.py
--rw-r--r--   0        0        0     1872 2023-07-03 10:35:35.840048 edgeimpulse_api-1.25.16/edgeimpulse_api/models/upload_user_photo_response_all_of.py
--rw-r--r--   0        0        0     3673 2023-07-03 10:35:34.739982 edgeimpulse_api-1.25.16/edgeimpulse_api/models/user.py
--rw-r--r--   0        0        0     1991 2023-07-03 10:35:35.287724 edgeimpulse_api-1.25.16/edgeimpulse_api/models/user_by_third_party_activation_request.py
--rw-r--r--   0        0        0     2192 2023-07-03 10:35:36.285262 edgeimpulse_api-1.25.16/edgeimpulse_api/models/user_experiment.py
--rw-r--r--   0        0        0     2709 2023-07-03 10:35:35.509964 edgeimpulse_api-1.25.16/edgeimpulse_api/models/user_organization.py
--rw-r--r--   0        0        0     1844 2023-07-03 10:35:35.852376 edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_dsp_block_url_request.py
--rw-r--r--   0        0        0     2604 2023-07-03 10:35:36.198987 edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_dsp_block_url_response.py
--rw-r--r--   0        0        0     2307 2023-07-03 10:35:35.961299 edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
--rw-r--r--   0        0        0     2407 2023-07-03 10:35:36.142018 edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
--rw-r--r--   0        0        0     2708 2023-07-03 10:35:35.398752 edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_organization_bucket_request.py
--rw-r--r--   0        0        0     2897 2023-07-03 10:35:35.936543 edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_organization_bucket_response.py
--rw-r--r--   0        0        0     2597 2023-07-03 10:35:36.287299 edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2187 2023-07-03 10:35:34.481968 edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
--rw-r--r--   0        0        0     1937 2023-07-03 10:35:36.094909 edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_reset_password_request.py
--rw-r--r--   0        0        0     5638 2023-07-03 10:35:35.808644 edgeimpulse_api-1.25.16/edgeimpulse_api/models/whitelabel.py
--rw-r--r--   0        0        0     2534 2023-07-03 10:35:34.536669 edgeimpulse_api-1.25.16/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
--rw-r--r--   0        0        0     2120 2023-07-03 10:35:35.352094 edgeimpulse_api-1.25.16/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
--rw-r--r--   0        0        0     2885 2023-07-03 10:35:36.270909 edgeimpulse_api-1.25.16/edgeimpulse_api/models/window_settings_response.py
--rw-r--r--   0        0        0     2585 2023-07-03 10:35:34.582891 edgeimpulse_api-1.25.16/edgeimpulse_api/models/window_settings_response_all_of.py
--rw-r--r--   0        0        0     2848 2023-07-03 10:35:34.713734 edgeimpulse_api-1.25.16/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
--rw-r--r--   0        0        0    12674 2023-07-03 10:35:21.206690 edgeimpulse_api-1.25.16/edgeimpulse_api/rest.py
--rw-r--r--   0        0        0      973 2023-07-03 10:40:44.951068 edgeimpulse_api-1.25.16/pyproject.toml
--rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 edgeimpulse_api-1.25.16/PKG-INFO
+-rw-r--r--   0        0        0      377 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/README.md
+-rw-r--r--   0        0        0    75024 2023-07-20 19:25:10.562599 edgeimpulse_api-1.25.31/edgeimpulse_api/__init__.py
+-rw-r--r--   0        0        0     2928 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/__init__.py
+-rw-r--r--   0        0        0   263386 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/admin_api.py
+-rw-r--r--   0        0        0   291873 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/allows_read_only_api.py
+-rw-r--r--   0        0        0    11231 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/auth_api.py
+-rw-r--r--   0        0        0     6235 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/cdn_api.py
+-rw-r--r--   0        0        0    28575 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/classify_api.py
+-rw-r--r--   0        0        0     7426 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/content_disposition_inline_api.py
+-rw-r--r--   0        0        0    72480 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/deployment_api.py
+-rw-r--r--   0        0        0    38974 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/devices_api.py
+-rw-r--r--   0        0        0   131256 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/dsp_api.py
+-rw-r--r--   0        0        0     6435 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/export_api.py
+-rw-r--r--   0        0        0    11921 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/health_api.py
+-rw-r--r--   0        0        0    49621 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/impulse_api.py
+-rw-r--r--   0        0        0   232507 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/jobs_api.py
+-rw-r--r--   0        0        0   147712 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/learn_api.py
+-rw-r--r--   0        0        0     6483 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/login_api.py
+-rw-r--r--   0        0        0    12006 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/metrics_api.py
+-rw-r--r--   0        0        0    67457 2023-07-20 19:24:45.255041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/optimization_api.py
+-rw-r--r--   0        0        0   300920 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_allow_developer_profile_api.py
+-rw-r--r--   0        0        0    63140 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_allow_guest_access_api.py
+-rw-r--r--   0        0        0   141131 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_blocks_api.py
+-rw-r--r--   0        0        0    91908 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_create_project_api.py
+-rw-r--r--   0        0        0   255365 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_data_api.py
+-rw-r--r--   0        0        0    80882 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_data_campaigns_api.py
+-rw-r--r--   0        0        0    58218 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_jobs_api.py
+-rw-r--r--   0        0        0    47178 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_pipelines_api.py
+-rw-r--r--   0        0        0    45490 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_portals_api.py
+-rw-r--r--   0        0        0   266354 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_requires_admin_api.py
+-rw-r--r--   0        0        0   176301 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py
+-rw-r--r--   0        0        0   300240 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/organizations_api.py
+-rw-r--r--   0        0        0    54671 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/performance_calibration_api.py
+-rw-r--r--   0        0        0    12662 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/project_requires_admin_api.py
+-rw-r--r--   0        0        0   228112 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/projects_api.py
+-rw-r--r--   0        0        0   366799 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/raw_data_api.py
+-rw-r--r--   0        0        0    24481 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/requires_sudo_api.py
+-rw-r--r--   0        0        0     7730 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py
+-rw-r--r--   0        0        0    13690 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/supports_range_api.py
+-rw-r--r--   0        0        0    35671 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/themes_api.py
+-rw-r--r--   0        0        0    43486 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/third_party_auth_api.py
+-rw-r--r--   0        0        0    45393 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/upload_portal_api.py
+-rw-r--r--   0        0        0   197590 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/user_api.py
+-rw-r--r--   0        0        0    42135 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api/whitelabels_api.py
+-rw-r--r--   0        0        0    29331 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/api_client.py
+-rw-r--r--   0        0        0    15659 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/configuration.py
+-rw-r--r--   0        0        0     5113 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/exceptions.py
+-rw-r--r--   0        0        0    71642 2023-07-20 19:24:45.259041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/__init__.py
+-rw-r--r--   0        0        0     2897 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
+-rw-r--r--   0        0        0     1882 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/activate_user_request.py
+-rw-r--r--   0        0        0     2610 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_api_key_request.py
+-rw-r--r--   0        0        0     1963 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_collaborator_request.py
+-rw-r--r--   0        0        0     2223 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_hmac_key_request.py
+-rw-r--r--   0        0        0     2299 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_member_request.py
+-rw-r--r--   0        0        0     2418 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2806 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_bucket_request.py
+-rw-r--r--   0        0        0     2656 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     2469 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2152 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     4230 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2359 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2042 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
+-rw-r--r--   0        0        0     2269 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2816 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2248 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2054 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_secret_request.py
+-rw-r--r--   0        0        0     2266 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_secret_response.py
+-rw-r--r--   0        0        0     1949 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_secret_response_all_of.py
+-rw-r--r--   0        0        0     4588 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     2339 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     4592 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     2325 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2001 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     1940 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
+-rw-r--r--   0        0        0     1961 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
+-rw-r--r--   0        0        0     2542 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_organization_user_request.py
+-rw-r--r--   0        0        0     2246 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
+-rw-r--r--   0        0        0     2146 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_project_user_request.py
+-rw-r--r--   0        0        0     2097 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_user_request.py
+-rw-r--r--   0        0        0     4696 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_api_organization.py
+-rw-r--r--   0        0        0     2396 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_api_organization_all_of.py
+-rw-r--r--   0        0        0     3459 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_api_project.py
+-rw-r--r--   0        0        0     7268 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_api_user.py
+-rw-r--r--   0        0        0     5714 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_api_user_all_of.py
+-rw-r--r--   0        0        0     2262 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_create_organization_request.py
+-rw-r--r--   0        0        0     2742 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_create_user_trial_request.py
+-rw-r--r--   0        0        0     2546 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_data_migration_response.py
+-rw-r--r--   0        0        0     2222 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
+-rw-r--r--   0        0        0     2735 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_data_migrations_response.py
+-rw-r--r--   0        0        0     2428 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
+-rw-r--r--   0        0        0     2318 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
+-rw-r--r--   0        0        0     2022 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
+-rw-r--r--   0        0        0     2217 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_metrics_response.py
+-rw-r--r--   0        0        0     1910 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3046 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_organizations_response.py
+-rw-r--r--   0        0        0     2746 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
+-rw-r--r--   0        0        0     3409 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
+-rw-r--r--   0        0        0     2243 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
+-rw-r--r--   0        0        0     1947 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
+-rw-r--r--   0        0        0     2914 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_sso_settings_response.py
+-rw-r--r--   0        0        0     2614 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
+-rw-r--r--   0        0        0     2096 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
+-rw-r--r--   0        0        0     2208 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_ids_response.py
+-rw-r--r--   0        0        0     1901 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
+-rw-r--r--   0        0        0     2245 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_metrics_response.py
+-rw-r--r--   0        0        0     1938 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_metrics_response_all_of.py
+-rw-r--r--   0        0        0     2452 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_response.py
+-rw-r--r--   0        0        0     2128 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_response_all_of.py
+-rw-r--r--   0        0        0     2507 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_trial_response.py
+-rw-r--r--   0        0        0     2183 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
+-rw-r--r--   0        0        0     2807 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_users_response.py
+-rw-r--r--   0        0        0     2500 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_users_response_all_of.py
+-rw-r--r--   0        0        0     3087 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
+-rw-r--r--   0        0        0     2445 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_list_projects.py
+-rw-r--r--   0        0        0     2836 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_list_projects_response.py
+-rw-r--r--   0        0        0     7695 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_organization_info_response.py
+-rw-r--r--   0        0        0     3752 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_organization_info_response_all_of.py
+-rw-r--r--   0        0        0     2158 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_toggle_data_migration_request.py
+-rw-r--r--   0        0        0     3269 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_update_organization_request.py
+-rw-r--r--   0        0        0     2015 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_update_user_permissions_request.py
+-rw-r--r--   0        0        0     2661 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_update_user_request.py
+-rw-r--r--   0        0        0     2365 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_update_user_trial_request.py
+-rw-r--r--   0        0        0     2525 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/akida_edge_learning_config.py
+-rw-r--r--   0        0        0     5499 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_model_metadata.py
+-rw-r--r--   0        0        0     5221 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
+-rw-r--r--   0        0        0     2151 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
+-rw-r--r--   0        0        0     4079 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_response.py
+-rw-r--r--   0        0        0     3812 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_response_all_of.py
+-rw-r--r--   0        0        0     2044 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_response_all_of_axes.py
+-rw-r--r--   0        0        0     3029 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_trained_features_response.py
+-rw-r--r--   0        0        0     2729 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2375 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0      506 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/augmentation_policy_image_enum.py
+-rw-r--r--   0        0        0     3635 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/augmentation_policy_spectrogram.py
+-rw-r--r--   0        0        0     1895 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/autotune_dsp_request.py
+-rw-r--r--   0        0        0     2044 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/bounding_box.py
+-rw-r--r--   0        0        0     2151 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/bounding_box_with_score.py
+-rw-r--r--   0        0        0     2197 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/build_on_device_model_request.py
+-rw-r--r--   0        0        0     2433 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/build_organization_on_device_model_request.py
+-rw-r--r--   0        0        0     2041 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/change_password_request.py
+-rw-r--r--   0        0        0     3701 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response.py
+-rw-r--r--   0        0        0     3394 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response_all_of.py
+-rw-r--r--   0        0        0     3769 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
+-rw-r--r--   0        0        0     2055 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
+-rw-r--r--   0        0        0     3255 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response_page.py
+-rw-r--r--   0        0        0     2948 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response_page_all_of.py
+-rw-r--r--   0        0        0     3932 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_sample_response.py
+-rw-r--r--   0        0        0     3644 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_sample_response_all_of.py
+-rw-r--r--   0        0        0     4783 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_sample_response_classification.py
+-rw-r--r--   0        0        0     2755 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_sample_response_classification_details.py
+-rw-r--r--   0        0        0     3004 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/convert_user_request.py
+-rw-r--r--   0        0        0     2183 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/count_samples_response.py
+-rw-r--r--   0        0        0     1859 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/count_samples_response_all_of.py
+-rw-r--r--   0        0        0     2255 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_block_version_response.py
+-rw-r--r--   0        0        0     1938 2023-07-20 19:24:45.263041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_block_version_response_all_of.py
+-rw-r--r--   0        0        0     2404 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_developer_profile_response.py
+-rw-r--r--   0        0        0     2125 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_developer_profile_response_all_of.py
+-rw-r--r--   0        0        0     2387 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_device_request.py
+-rw-r--r--   0        0        0     2491 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_evaluation_user_response.py
+-rw-r--r--   0        0        0     2185 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
+-rw-r--r--   0        0        0     2600 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_portal_request.py
+-rw-r--r--   0        0        0     2830 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_portal_response.py
+-rw-r--r--   0        0        0     2551 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     1990 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_request.py
+-rw-r--r--   0        0        0     2454 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_response.py
+-rw-r--r--   0        0        0     2148 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_response_all_of.py
+-rw-r--r--   0        0        0     2185 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_pipeline_response.py
+-rw-r--r--   0        0        0     2254 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_project_request.py
+-rw-r--r--   0        0        0     2378 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_project_response.py
+-rw-r--r--   0        0        0     2072 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_project_response_all_of.py
+-rw-r--r--   0        0        0     2276 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_signed_upload_link_request.py
+-rw-r--r--   0        0        0     2414 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_signed_upload_link_response.py
+-rw-r--r--   0        0        0     2135 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
+-rw-r--r--   0        0        0     2413 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_third_party_auth_request.py
+-rw-r--r--   0        0        0     2450 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_third_party_auth_response.py
+-rw-r--r--   0        0        0     2144 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     3835 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_request.py
+-rw-r--r--   0        0        0     2393 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_response.py
+-rw-r--r--   0        0        0     2114 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_response_all_of.py
+-rw-r--r--   0        0        0     2919 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_third_party_request.py
+-rw-r--r--   0        0        0     2672 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_third_party_response.py
+-rw-r--r--   0        0        0     2393 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_third_party_response_all_of.py
+-rw-r--r--   0        0        0     4157 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_whitelabel_request.py
+-rw-r--r--   0        0        0     2438 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_whitelabel_response.py
+-rw-r--r--   0        0        0     2121 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2051 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/crop_sample_request.py
+-rw-r--r--   0        0        0     2248 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/crop_sample_response.py
+-rw-r--r--   0        0        0     1943 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/crop_sample_response_all_of.py
+-rw-r--r--   0        0        0     4054 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign.py
+-rw-r--r--   0        0        0     2851 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_dashboard.py
+-rw-r--r--   0        0        0     2786 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_graph.py
+-rw-r--r--   0        0        0     3352 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
+-rw-r--r--   0        0        0     2047 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
+-rw-r--r--   0        0        0     1934 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_link.py
+-rw-r--r--   0        0        0     1957 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_query.py
+-rw-r--r--   0        0        0     3292 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_explorer_predictions_response.py
+-rw-r--r--   0        0        0     3003 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
+-rw-r--r--   0        0        0     2838 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_explorer_settings.py
+-rw-r--r--   0        0        0     2149 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dataset_ratio_data.py
+-rw-r--r--   0        0        0     2111 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dataset_ratio_data_ratio.py
+-rw-r--r--   0        0        0     1898 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/delete_portal_file_request.py
+-rw-r--r--   0        0        0     2230 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dependency_data.py
+-rw-r--r--   0        0        0     2280 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
+-rw-r--r--   0        0        0     2408 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
+-rw-r--r--   0        0        0     2155 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
+-rw-r--r--   0        0        0     2484 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
+-rw-r--r--   0        0        0     2344 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
+-rw-r--r--   0        0        0     2780 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
+-rw-r--r--   0        0        0     2200 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
+-rw-r--r--   0        0        0     4355 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_request.py
+-rw-r--r--   0        0        0     2833 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
+-rw-r--r--   0        0        0     8503 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
+-rw-r--r--   0        0        0     8065 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
+-rw-r--r--   0        0        0     5950 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deployment_target.py
+-rw-r--r--   0        0        0     1926 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deployment_target_badge.py
+-rw-r--r--   0        0        0      679 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deployment_target_engine.py
+-rw-r--r--   0        0        0     2702 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deployment_targets_response.py
+-rw-r--r--   0        0        0     2395 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     1983 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/development_board.py
+-rw-r--r--   0        0        0     2831 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/development_boards_response.py
+-rw-r--r--   0        0        0     2531 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/development_boards_response_all_of.py
+-rw-r--r--   0        0        0     2030 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/development_keys.py
+-rw-r--r--   0        0        0     2400 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/development_keys_response.py
+-rw-r--r--   0        0        0     3677 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/device.py
+-rw-r--r--   0        0        0     2199 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/device_name_response.py
+-rw-r--r--   0        0        0     1920 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/device_name_response_all_of.py
+-rw-r--r--   0        0        0     2231 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/device_sensors_inner.py
+-rw-r--r--   0        0        0     2094 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/download.py
+-rw-r--r--   0        0        0     1912 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/download_portal_file_request.py
+-rw-r--r--   0        0        0     2260 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/download_portal_file_response.py
+-rw-r--r--   0        0        0     1954 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/download_portal_file_response_all_of.py
+-rw-r--r--   0        0        0     2724 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_autotuner_results.py
+-rw-r--r--   0        0        0     2417 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
+-rw-r--r--   0        0        0     1968 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
+-rw-r--r--   0        0        0     2870 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_block.py
+-rw-r--r--   0        0        0     1834 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_config_request.py
+-rw-r--r--   0        0        0     3092 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_config_response.py
+-rw-r--r--   0        0        0     2813 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_config_response_all_of.py
+-rw-r--r--   0        0        0     3016 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_importance_response.py
+-rw-r--r--   0        0        0     2728 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
+-rw-r--r--   0        0        0     2058 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
+-rw-r--r--   0        0        0     2572 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
+-rw-r--r--   0        0        0     2216 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_labels_response.py
+-rw-r--r--   0        0        0     1920 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
+-rw-r--r--   0        0        0     2294 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_group.py
+-rw-r--r--   0        0        0     3779 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_group_item.py
+-rw-r--r--   0        0        0     2190 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
+-rw-r--r--   0        0        0     2195 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_group_item_show_if.py
+-rw-r--r--   0        0        0     4410 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_info.py
+-rw-r--r--   0        0        0     2210 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_info_features.py
+-rw-r--r--   0        0        0     1885 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_info_performance.py
+-rw-r--r--   0        0        0     5144 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_metadata.py
+-rw-r--r--   0        0        0     2025 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
+-rw-r--r--   0        0        0     2566 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_metadata_output_config.py
+-rw-r--r--   0        0        0     2531 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
+-rw-r--r--   0        0        0     5502 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_metadata_response.py
+-rw-r--r--   0        0        0     3019 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_performance_all_variants_response.py
+-rw-r--r--   0        0        0     2729 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2278 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
+-rw-r--r--   0        0        0     4639 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_graph.py
+-rw-r--r--   0        0        0     1899 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
+-rw-r--r--   0        0        0     2677 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_request_with_features.py
+-rw-r--r--   0        0        0     2151 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_request_without_features.py
+-rw-r--r--   0        0        0     2030 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
+-rw-r--r--   0        0        0     3513 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_response.py
+-rw-r--r--   0        0        0     3234 2023-07-20 19:24:45.267041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_response_all_of.py
+-rw-r--r--   0        0        0     1969 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
+-rw-r--r--   0        0        0     4142 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_response_with_sample.py
+-rw-r--r--   0        0        0     3875 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
+-rw-r--r--   0        0        0     3342 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_sample_features_response.py
+-rw-r--r--   0        0        0     3042 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
+-rw-r--r--   0        0        0     2748 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2213 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     3353 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_trained_features_response.py
+-rw-r--r--   0        0        0     3053 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2773 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2205 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     1893 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/edit_sample_label_request.py
+-rw-r--r--   0        0        0     3697 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/enterprise_trial.py
+-rw-r--r--   0        0        0     2397 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/entitlement_limits.py
+-rw-r--r--   0        0        0     2178 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/entity_created_response.py
+-rw-r--r--   0        0        0     2656 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/evaluate_job_response.py
+-rw-r--r--   0        0        0     2349 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/evaluate_job_response_all_of.py
+-rw-r--r--   0        0        0     2099 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/evaluate_result_value.py
+-rw-r--r--   0        0        0     2511 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/export_get_url_response.py
+-rw-r--r--   0        0        0     2244 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/export_get_url_response_all_of.py
+-rw-r--r--   0        0        0     2116 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/export_keras_block_data_request.py
+-rw-r--r--   0        0        0     2373 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/export_original_data_request.py
+-rw-r--r--   0        0        0     2021 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/export_wav_data_request.py
+-rw-r--r--   0        0        0     2206 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_segment_sample_request.py
+-rw-r--r--   0        0        0     2804 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_segment_sample_response.py
+-rw-r--r--   0        0        0     2497 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_segment_sample_response_all_of.py
+-rw-r--r--   0        0        0     2090 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
+-rw-r--r--   0        0        0     2665 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_user_response.py
+-rw-r--r--   0        0        0     2358 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_user_response_all_of.py
+-rw-r--r--   0        0        0     2322 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_user_response_all_of_users.py
+-rw-r--r--   0        0        0     2507 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/generate_features_request.py
+-rw-r--r--   0        0        0     2083 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/generic_api_response.py
+-rw-r--r--   0        0        0     2764 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_imported_from_response.py
+-rw-r--r--   0        0        0     2457 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
+-rw-r--r--   0        0        0     2156 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
+-rw-r--r--   0        0        0     2698 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_third_party_auth_response.py
+-rw-r--r--   0        0        0     2391 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     2713 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_whitelabels_response.py
+-rw-r--r--   0        0        0     2406 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
+-rw-r--r--   0        0        0     3385 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_auto_segmenter_response.py
+-rw-r--r--   0        0        0     3108 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py
+-rw-r--r--   0        0        0     2610 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py
+-rw-r--r--   0        0        0     1968 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py
+-rw-r--r--   0        0        0     3400 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_data_explorer_features_response.py
+-rw-r--r--   0        0        0     3122 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0     3752 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_data_explorer_settings_response.py
+-rw-r--r--   0        0        0     2402 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
+-rw-r--r--   0        0        0     2349 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_deployment_response.py
+-rw-r--r--   0        0        0     2071 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_deployment_response_all_of.py
+-rw-r--r--   0        0        0     2434 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_device_response.py
+-rw-r--r--   0        0        0     2137 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_device_response_all_of.py
+-rw-r--r--   0        0        0     3930 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_impulse_blocks_response.py
+-rw-r--r--   0        0        0     3630 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2454 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_impulse_response.py
+-rw-r--r--   0        0        0     2157 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_impulse_response_all_of.py
+-rw-r--r--   0        0        0     2374 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_job_response.py
+-rw-r--r--   0        0        0     2077 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_job_response_all_of.py
+-rw-r--r--   0        0        0     2650 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_jwt_request.py
+-rw-r--r--   0        0        0     2431 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_jwt_response.py
+-rw-r--r--   0        0        0     2152 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_jwt_response_all_of.py
+-rw-r--r--   0        0        0     2977 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_last_deployment_build_response.py
+-rw-r--r--   0        0        0     2699 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
+-rw-r--r--   0        0        0     2869 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
+-rw-r--r--   0        0        0     2572 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_notes_response.py
+-rw-r--r--   0        0        0     2265 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_notes_response_all_of.py
+-rw-r--r--   0        0        0     2701 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2377 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     2890 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
+-rw-r--r--   0        0        0     2583 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
+-rw-r--r--   0        0        0     3158 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2939 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaigns_response.py
+-rw-r--r--   0        0        0     2632 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
+-rw-r--r--   0        0        0     2921 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
+-rw-r--r--   0        0        0     2561 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_item_response.py
+-rw-r--r--   0        0        0     2237 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
+-rw-r--r--   0        0        0     3411 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
+-rw-r--r--   0        0        0     3111 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
+-rw-r--r--   0        0        0     3398 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
+-rw-r--r--   0        0        0     2576 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_dataset_response.py
+-rw-r--r--   0        0        0     2252 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
+-rw-r--r--   0        0        0     2603 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2279 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     3670 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_portal_response.py
+-rw-r--r--   0        0        0     3391 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2323 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_projects_data_count_response.py
+-rw-r--r--   0        0        0     2905 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
+-rw-r--r--   0        0        0     2598 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
+-rw-r--r--   0        0        0     3012 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
+-rw-r--r--   0        0        0     2712 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
+-rw-r--r--   0        0        0     2722 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
+-rw-r--r--   0        0        0     2425 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2922 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
+-rw-r--r--   0        0        0     2615 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
+-rw-r--r--   0        0        0     3151 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_status_response.py
+-rw-r--r--   0        0        0     2884 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
+-rw-r--r--   0        0        0     3761 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_pretrained_model_response.py
+-rw-r--r--   0        0        0     3483 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3861 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
+-rw-r--r--   0        0        0     2978 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
+-rw-r--r--   0        0        0     3058 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
+-rw-r--r--   0        0        0     2397 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_public_metrics_response.py
+-rw-r--r--   0        0        0     2073 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_public_metrics_response_all_of.py
+-rw-r--r--   0        0        0     2767 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_sample_metadata_response.py
+-rw-r--r--   0        0        0     3044 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_sample_response.py
+-rw-r--r--   0        0        0     2462 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_syntiant_posterior_response.py
+-rw-r--r--   0        0        0     2184 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
+-rw-r--r--   0        0        0     2414 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_theme_response.py
+-rw-r--r--   0        0        0     2117 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_theme_response_all_of.py
+-rw-r--r--   0        0        0     2592 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_themes_response.py
+-rw-r--r--   0        0        0     2285 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_themes_response_all_of.py
+-rw-r--r--   0        0        0     2495 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_third_party_auth_response.py
+-rw-r--r--   0        0        0     2171 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     2703 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_user_need_to_set_password_response.py
+-rw-r--r--   0        0        0     2436 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
+-rw-r--r--   0        0        0     7717 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_user_response.py
+-rw-r--r--   0        0        0     5708 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_user_response_all_of.py
+-rw-r--r--   0        0        0     2395 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
+-rw-r--r--   0        0        0     2307 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_whitelabel_domain_response.py
+-rw-r--r--   0        0        0     2021 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
+-rw-r--r--   0        0        0     2514 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_whitelabel_response.py
+-rw-r--r--   0        0        0     2217 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2776 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/has_data_explorer_features_response.py
+-rw-r--r--   0        0        0     2498 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0      526 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/image_input_scaling.py
+-rw-r--r--   0        0        0     3738 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse.py
+-rw-r--r--   0        0        0     6723 2023-07-20 19:24:45.271041 edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse_block_version.py
+-rw-r--r--   0        0        0     6814 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse_dsp_block.py
+-rw-r--r--   0        0        0     1967 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse_dsp_block_organization.py
+-rw-r--r--   0        0        0     8958 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse_input_block.py
+-rw-r--r--   0        0        0     5612 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse_learn_block.py
+-rw-r--r--   0        0        0     2445 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/input_block.py
+-rw-r--r--   0        0        0     2323 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/invite_organization_member_request.py
+-rw-r--r--   0        0        0     3668 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job.py
+-rw-r--r--   0        0        0     4699 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_details.py
+-rw-r--r--   0        0        0     2736 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_details_all_of.py
+-rw-r--r--   0        0        0     2613 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_details_response.py
+-rw-r--r--   0        0        0     2316 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_details_response_all_of.py
+-rw-r--r--   0        0        0     2257 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_failure_details.py
+-rw-r--r--   0        0        0     2657 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_logs_response.py
+-rw-r--r--   0        0        0     2350 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_logs_response_all_of.py
+-rw-r--r--   0        0        0     3297 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_metrics_response.py
+-rw-r--r--   0        0        0     3007 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_metrics_response_all_of.py
+-rw-r--r--   0        0        0      516 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_parent_type_enum.py
+-rw-r--r--   0        0        0     2944 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_state.py
+-rw-r--r--   0        0        0     1966 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_state_execution_details.py
+-rw-r--r--   0        0        0     2965 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_step.py
+-rw-r--r--   0        0        0     2713 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_summary_response.py
+-rw-r--r--   0        0        0     2406 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_summary_response_all_of.py
+-rw-r--r--   0        0        0     2089 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_summary_response_all_of_summary.py
+-rw-r--r--   0        0        0     2510 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_layer.py
+-rw-r--r--   0        0        0     2093 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_layer_input.py
+-rw-r--r--   0        0        0     2101 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_layer_output.py
+-rw-r--r--   0        0        0     5431 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_metadata.py
+-rw-r--r--   0        0        0     5164 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_metadata_all_of.py
+-rw-r--r--   0        0        0     4792 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_metadata_metrics.py
+-rw-r--r--   0        0        0     3228 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
+-rw-r--r--   0        0        0     2497 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
+-rw-r--r--   0        0        0      562 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_type_enum.py
+-rw-r--r--   0        0        0     9842 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_response.py
+-rw-r--r--   0        0        0     9575 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_response_all_of.py
+-rw-r--r--   0        0        0     3392 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_visual_layer.py
+-rw-r--r--   0        0        0     2310 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_visual_layer_type.py
+-rw-r--r--   0        0        0     2529 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/last_modification_date_response.py
+-rw-r--r--   0        0        0     2239 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/last_modification_date_response_all_of.py
+-rw-r--r--   0        0        0     2633 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/latency_device.py
+-rw-r--r--   0        0        0     2424 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/learn_block.py
+-rw-r--r--   0        0        0      883 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/learn_block_type.py
+-rw-r--r--   0        0        0     2788 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     2488 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2682 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2630 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_devices_response.py
+-rw-r--r--   0        0        0     2333 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_devices_response_all_of.py
+-rw-r--r--   0        0        0     2726 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_email_response.py
+-rw-r--r--   0        0        0     2426 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_email_response_all_of.py
+-rw-r--r--   0        0        0     2918 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_email_response_all_of_emails.py
+-rw-r--r--   0        0        0     2813 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_hmac_keys_response.py
+-rw-r--r--   0        0        0     2513 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
+-rw-r--r--   0        0        0     2381 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
+-rw-r--r--   0        0        0     2745 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_jobs_response.py
+-rw-r--r--   0        0        0     2445 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_jobs_response_all_of.py
+-rw-r--r--   0        0        0     2200 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_models_response.py
+-rw-r--r--   0        0        0     1910 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_models_response_all_of.py
+-rw-r--r--   0        0        0     2921 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_api_keys_response.py
+-rw-r--r--   0        0        0     2621 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2760 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2857 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_response.py
+-rw-r--r--   0        0        0     2550 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
+-rw-r--r--   0        0        0     2995 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py
+-rw-r--r--   0        0        0     2902 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_user_response.py
+-rw-r--r--   0        0        0     2595 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
+-rw-r--r--   0        0        0     2760 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
+-rw-r--r--   0        0        0     3310 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_data_response.py
+-rw-r--r--   0        0        0     3031 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_data_response_all_of.py
+-rw-r--r--   0        0        0     3430 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2887 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
+-rw-r--r--   0        0        0     2587 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2824 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
+-rw-r--r--   0        0        0     2524 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3353 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_files_response.py
+-rw-r--r--   0        0        0     3074 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_files_response_all_of.py
+-rw-r--r--   0        0        0     2792 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2485 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     2857 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_portals_response.py
+-rw-r--r--   0        0        0     2550 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_portals_response_all_of.py
+-rw-r--r--   0        0        0     2744 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
+-rw-r--r--   0        0        0     3449 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_projects_data_response.py
+-rw-r--r--   0        0        0     3142 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
+-rw-r--r--   0        0        0     2271 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
+-rw-r--r--   0        0        0     2723 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_projects_response.py
+-rw-r--r--   0        0        0     2416 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_projects_response_all_of.py
+-rw-r--r--   0        0        0     2857 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_secrets_response.py
+-rw-r--r--   0        0        0     2550 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
+-rw-r--r--   0        0        0     2265 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
+-rw-r--r--   0        0        0     3103 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
+-rw-r--r--   0        0        0     2803 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3055 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2755 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2786 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organizations_response.py
+-rw-r--r--   0        0        0     2486 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organizations_response_all_of.py
+-rw-r--r--   0        0        0     1937 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_portal_files_in_folder_request.py
+-rw-r--r--   0        0        0     2713 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_portal_files_in_folder_response.py
+-rw-r--r--   0        0        0     2416 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2290 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_projects.py
+-rw-r--r--   0        0        0     2681 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_projects_response.py
+-rw-r--r--   0        0        0     2553 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_public_projects.py
+-rw-r--r--   0        0        0     2944 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_public_projects_response.py
+-rw-r--r--   0        0        0     2815 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_public_versions_response.py
+-rw-r--r--   0        0        0     2508 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_public_versions_response_all_of.py
+-rw-r--r--   0        0        0     2290 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2754 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_samples_response.py
+-rw-r--r--   0        0        0     2454 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_samples_response_all_of.py
+-rw-r--r--   0        0        0     3933 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_versions_response.py
+-rw-r--r--   0        0        0     3633 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_versions_response_all_of.py
+-rw-r--r--   0        0        0     2353 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
+-rw-r--r--   0        0        0     2053 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
+-rw-r--r--   0        0        0     3960 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2900 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/log_stdout_response.py
+-rw-r--r--   0        0        0     2600 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/log_stdout_response_all_of.py
+-rw-r--r--   0        0        0     2441 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
+-rw-r--r--   0        0        0     2191 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/log_website_pageview_request.py
+-rw-r--r--   0        0        0     2217 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/login_response.py
+-rw-r--r--   0        0        0     1911 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/login_response_all_of.py
+-rw-r--r--   0        0        0     2430 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/migration.py
+-rw-r--r--   0        0        0     2521 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/model_prediction.py
+-rw-r--r--   0        0        0     2895 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/model_result.py
+-rw-r--r--   0        0        0     5046 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/model_variant_stats.py
+-rw-r--r--   0        0        0     2128 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/move_raw_data_request.py
+-rw-r--r--   0        0        0     2687 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/note.py
+-rw-r--r--   0        0        0     2221 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_auto_label_request.py
+-rw-r--r--   0        0        0     2994 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_auto_label_response.py
+-rw-r--r--   0        0        0     2705 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
+-rw-r--r--   0        0        0     2275 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
+-rw-r--r--   0        0        0     2368 2023-07-20 19:24:45.275040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_label_queue_count_response.py
+-rw-r--r--   0        0        0     2051 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
+-rw-r--r--   0        0        0     2887 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_label_queue_response.py
+-rw-r--r--   0        0        0     2580 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
+-rw-r--r--   0        0        0      621 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_last_layer.py
+-rw-r--r--   0        0        0     6418 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_config.py
+-rw-r--r--   0        0        0     6871 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_config_response.py
+-rw-r--r--   0        0        0     1920 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_config_response_all_of.py
+-rw-r--r--   0        0        0     2067 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_config_target_device.py
+-rw-r--r--   0        0        0     2271 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_dsp_parameters_response.py
+-rw-r--r--   0        0        0     1964 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_space_response.py
+-rw-r--r--   0        0        0     2456 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_space_response_all_of.py
+-rw-r--r--   0        0        0     4897 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_state_response.py
+-rw-r--r--   0        0        0     4618 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_state_response_all_of.py
+-rw-r--r--   0        0        0     3419 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_state_response_all_of_status.py
+-rw-r--r--   0        0        0     2366 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
+-rw-r--r--   0        0        0     2760 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
+-rw-r--r--   0        0        0     2463 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
+-rw-r--r--   0        0        0     4717 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
+-rw-r--r--   0        0        0     4594 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization.py
+-rw-r--r--   0        0        0     2359 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_add_data_folder_request.py
+-rw-r--r--   0        0        0     2498 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_add_data_folder_response.py
+-rw-r--r--   0        0        0     2209 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
+-rw-r--r--   0        0        0     2549 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_add_dataset_request.py
+-rw-r--r--   0        0        0     2460 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
+-rw-r--r--   0        0        0     8598 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project.py
+-rw-r--r--   0        0        0     5176 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_request.py
+-rw-r--r--   0        0        0     2543 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_response.py
+-rw-r--r--   0        0        0     2237 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_response_all_of.py
+-rw-r--r--   0        0        0     2704 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_status_response.py
+-rw-r--r--   0        0        0     2407 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
+-rw-r--r--   0        0        0     2501 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_transformation_summary.py
+-rw-r--r--   0        0        0     9493 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_with_files.py
+-rw-r--r--   0        0        0     2744 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
+-rw-r--r--   0        0        0     3034 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
+-rw-r--r--   0        0        0     2559 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_campaign_diff_request.py
+-rw-r--r--   0        0        0     2327 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
+-rw-r--r--   0        0        0     3041 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_campaign_diff_response.py
+-rw-r--r--   0        0        0     2741 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
+-rw-r--r--   0        0        0     2468 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
+-rw-r--r--   0        0        0     3476 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_item.py
+-rw-r--r--   0        0        0     2103 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_item_files_inner.py
+-rw-r--r--   0        0        0     3529 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_dataset.py
+-rw-r--r--   0        0        0     2767 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_dataset_bucket.py
+-rw-r--r--   0        0        0     4689 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_deploy_block.py
+-rw-r--r--   0        0        0     3646 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_dsp_block.py
+-rw-r--r--   0        0        0     3037 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_get_create_projects_response.py
+-rw-r--r--   0        0        0     2737 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
+-rw-r--r--   0        0        0     5707 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
+-rw-r--r--   0        0        0     6331 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response.py
+-rw-r--r--   0        0        0     6041 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response_all_of.py
+-rw-r--r--   0        0        0     3915 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
+-rw-r--r--   0        0        0     2267 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
+-rw-r--r--   0        0        0     2338 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
+-rw-r--r--   0        0        0     2458 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
+-rw-r--r--   0        0        0      525 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_member_role.py
+-rw-r--r--   0        0        0     2639 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_metrics_response.py
+-rw-r--r--   0        0        0     2315 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3453 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
+-rw-r--r--   0        0        0     6132 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline.py
+-rw-r--r--   0        0        0     2595 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
+-rw-r--r--   0        0        0     2275 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
+-rw-r--r--   0        0        0     2314 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_item_count.py
+-rw-r--r--   0        0        0     4109 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_run.py
+-rw-r--r--   0        0        0     5213 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_run_step.py
+-rw-r--r--   0        0        0     4813 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_step.py
+-rw-r--r--   0        0        0     2351 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
+-rw-r--r--   0        0        0     2344 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
+-rw-r--r--   0        0        0     2037 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_projects_data_batch_request.py
+-rw-r--r--   0        0        0     5146 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_transfer_learning_block.py
+-rw-r--r--   0        0        0      611 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
+-rw-r--r--   0        0        0     5168 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_transformation_block.py
+-rw-r--r--   0        0        0     3907 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_update_pipeline_body.py
+-rw-r--r--   0        0        0     4225 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_user.py
+-rw-r--r--   0        0        0     2294 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_user_all_of.py
+-rw-r--r--   0        0        0     2104 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_detection.py
+-rw-r--r--   0        0        0     3434 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_false_positive.py
+-rw-r--r--   0        0        0     3770 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_ground_truth.py
+-rw-r--r--   0        0        0     2477 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
+-rw-r--r--   0        0        0     4880 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_parameter_set.py
+-rw-r--r--   0        0        0     2255 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
+-rw-r--r--   0        0        0     4092 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
+-rw-r--r--   0        0        0     3007 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_parameters.py
+-rw-r--r--   0        0        0     2585 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_parameters_standard.py
+-rw-r--r--   0        0        0     2250 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_raw_detection.py
+-rw-r--r--   0        0        0     2366 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
+-rw-r--r--   0        0        0     2412 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
+-rw-r--r--   0        0        0     2106 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
+-rw-r--r--   0        0        0     1629 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/permission.py
+-rw-r--r--   0        0        0     2211 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/portal_file.py
+-rw-r--r--   0        0        0     2413 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/portal_info_response.py
+-rw-r--r--   0        0        0     2666 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/pretrained_model_tensor.py
+-rw-r--r--   0        0        0     2955 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_info.py
+-rw-r--r--   0        0        0     2640 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_info_memory.py
+-rw-r--r--   0        0        0     1918 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_info_memory_eon.py
+-rw-r--r--   0        0        0     2065 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_info_memory_tflite.py
+-rw-r--r--   0        0        0     4335 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_table.py
+-rw-r--r--   0        0        0     2780 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_table_mcu.py
+-rw-r--r--   0        0        0     2565 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_table_mcu_memory.py
+-rw-r--r--   0        0        0     2250 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_table_mpu.py
+-rw-r--r--   0        0        0     2201 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_tf_lite_request.py
+-rw-r--r--   0        0        0     3292 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_tf_lite_response.py
+-rw-r--r--   0        0        0     6139 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project.py
+-rw-r--r--   0        0        0     3888 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_collaborator.py
+-rw-r--r--   0        0        0     1895 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_collaborator_all_of.py
+-rw-r--r--   0        0        0     2416 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_data_axes_summary_response.py
+-rw-r--r--   0        0        0     2116 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
+-rw-r--r--   0        0        0     2281 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_data_interval_response.py
+-rw-r--r--   0        0        0     1964 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_data_interval_response_all_of.py
+-rw-r--r--   0        0        0     2235 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_data_summary.py
+-rw-r--r--   0        0        0     6854 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_deployment_target.py
+-rw-r--r--   0        0        0     2706 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_deployment_target_all_of.py
+-rw-r--r--   0        0        0     2780 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_deployment_targets_response.py
+-rw-r--r--   0        0        0     2473 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     2680 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_downloads_response.py
+-rw-r--r--   0        0        0     2373 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_downloads_response_all_of.py
+-rw-r--r--   0        0        0    13550 2023-07-20 19:24:45.279040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response.py
+-rw-r--r--   0        0        0    13283 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of.py
+-rw-r--r--   0        0        0     3130 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
+-rw-r--r--   0        0        0     2723 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
+-rw-r--r--   0        0        0     2997 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
+-rw-r--r--   0        0        0     2979 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
+-rw-r--r--   0        0        0     2339 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_experiments.py
+-rw-r--r--   0        0        0     2285 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_impulse.py
+-rw-r--r--   0        0        0     2726 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_performance.py
+-rw-r--r--   0        0        0     1977 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_readme.py
+-rw-r--r--   0        0        0     2225 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
+-rw-r--r--   0        0        0     2735 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_urls.py
+-rw-r--r--   0        0        0     2478 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_summary_response.py
+-rw-r--r--   0        0        0     2172 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_summary_response_all_of.py
+-rw-r--r--   0        0        0     3554 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_private_data.py
+-rw-r--r--   0        0        0     4127 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_public_data.py
+-rw-r--r--   0        0        0     1928 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_public_data_readme.py
+-rw-r--r--   0        0        0     2404 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_sample_metadata.py
+-rw-r--r--   0        0        0     2670 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_training_data_summary_response.py
+-rw-r--r--   0        0        0     2353 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
+-rw-r--r--   0        0        0      606 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_type.py
+-rw-r--r--   0        0        0     2316 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_version_request.py
+-rw-r--r--   0        0        0     2664 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/raw_sample_data.py
+-rw-r--r--   0        0        0     3440 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/raw_sample_payload.py
+-rw-r--r--   0        0        0     2537 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/rebalance_dataset_response.py
+-rw-r--r--   0        0        0     1984 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/remove_collaborator_request.py
+-rw-r--r--   0        0        0     1805 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/remove_member_request.py
+-rw-r--r--   0        0        0     1867 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/rename_device_request.py
+-rw-r--r--   0        0        0     2081 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/rename_portal_file_request.py
+-rw-r--r--   0        0        0     1867 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/rename_sample_request.py
+-rw-r--r--   0        0        0     1873 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/request_reset_password_request.py
+-rw-r--r--   0        0        0     2031 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/reset_password_request.py
+-rw-r--r--   0        0        0     1985 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/restore_project_from_public_request.py
+-rw-r--r--   0        0        0     2265 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/restore_project_request.py
+-rw-r--r--   0        0        0     2244 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/run_auto_segmenter_request.py
+-rw-r--r--   0        0        0     2669 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/run_organization_pipeline_response.py
+-rw-r--r--   0        0        0     2352 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
+-rw-r--r--   0        0        0     9637 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/sample.py
+-rw-r--r--   0        0        0     2443 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/sample_bounding_boxes_request.py
+-rw-r--r--   0        0        0     2000 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/sample_metadata.py
+-rw-r--r--   0        0        0     2539 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py
+-rw-r--r--   0        0        0     2085 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py
+-rw-r--r--   0        0        0     2355 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py
+-rw-r--r--   0        0        0     2038 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/save_pretrained_model_request.py
+-rw-r--r--   0        0        0     3327 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/score_trial_response.py
+-rw-r--r--   0        0        0     3003 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/score_trial_response_all_of.py
+-rw-r--r--   0        0        0     2240 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/score_trial_response_all_of_latency.py
+-rw-r--r--   0        0        0     1914 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/score_trial_response_all_of_ram.py
+-rw-r--r--   0        0        0     2405 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/segment_sample_request.py
+-rw-r--r--   0        0        0     2055 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/segment_sample_request_segments_inner.py
+-rw-r--r--   0        0        0     3364 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/send_user_feedback_request.py
+-rw-r--r--   0        0        0     1981 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/sensor.py
+-rw-r--r--   0        0        0     2142 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_anomaly_parameter_request.py
+-rw-r--r--   0        0        0     8028 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_keras_parameter_request.py
+-rw-r--r--   0        0        0     1893 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_member_datasets_request.py
+-rw-r--r--   0        0        0     1905 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_member_role_request.py
+-rw-r--r--   0        0        0     2219 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_optimize_space_request.py
+-rw-r--r--   0        0        0     2254 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_optimize_space_request_all_of.py
+-rw-r--r--   0        0        0     1923 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_organization_data_dataset_request.py
+-rw-r--r--   0        0        0     1974 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_project_compute_time_request.py
+-rw-r--r--   0        0        0     2011 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_project_dsp_file_size_request.py
+-rw-r--r--   0        0        0     1919 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_sample_metadata_request.py
+-rw-r--r--   0        0        0     1915 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_syntiant_posterior_request.py
+-rw-r--r--   0        0        0     2140 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_user_password_request.py
+-rw-r--r--   0        0        0     2536 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/socket_token_response.py
+-rw-r--r--   0        0        0     2239 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/socket_token_response_all_of.py
+-rw-r--r--   0        0        0     2059 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/socket_token_response_all_of_token.py
+-rw-r--r--   0        0        0     1971 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/split_sample_in_frames_request.py
+-rw-r--r--   0        0        0     2110 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/staff_info.py
+-rw-r--r--   0        0        0     2226 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_job_response.py
+-rw-r--r--   0        0        0     1909 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_job_response_all_of.py
+-rw-r--r--   0        0        0     2883 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_performance_calibration_request.py
+-rw-r--r--   0        0        0     2838 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_sampling_request.py
+-rw-r--r--   0        0        0     2189 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_sampling_response.py
+-rw-r--r--   0        0        0     1892 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_sampling_response_all_of.py
+-rw-r--r--   0        0        0     2795 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_training_request_anomaly.py
+-rw-r--r--   0        0        0     1967 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/store_segment_length_request.py
+-rw-r--r--   0        0        0     3460 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/structured_classify_result.py
+-rw-r--r--   0        0        0     2433 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/test_pretrained_model_request.py
+-rw-r--r--   0        0        0     3074 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/test_pretrained_model_response.py
+-rw-r--r--   0        0        0     2784 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3251 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/theme.py
+-rw-r--r--   0        0        0     2239 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/theme_colors.py
+-rw-r--r--   0        0        0     2764 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/theme_favicon.py
+-rw-r--r--   0        0        0     2721 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/theme_logos.py
+-rw-r--r--   0        0        0     2245 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/third_party_auth.py
+-rw-r--r--   0        0        0     1921 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/time_series_data_point.py
+-rw-r--r--   0        0        0     2031 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/track_objects_request.py
+-rw-r--r--   0        0        0     2736 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/track_objects_response.py
+-rw-r--r--   0        0        0     2436 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/track_objects_response_all_of.py
+-rw-r--r--   0        0        0     5295 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/transfer_learning_model.py
+-rw-r--r--   0        0        0     2012 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/transfer_ownership_organization_request.py
+-rw-r--r--   0        0        0     2585 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/transformation_block_additional_mount_point.py
+-rw-r--r--   0        0        0      588 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/transformation_job_status_enum.py
+-rw-r--r--   0        0        0     2578 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/tuner_create_trial_impulse.py
+-rw-r--r--   0        0        0     2570 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/tuner_space_impulse.py
+-rw-r--r--   0        0        0     4257 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/tuner_trial.py
+-rw-r--r--   0        0        0     2304 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/tuner_trial_blocks_inner.py
+-rw-r--r--   0        0        0     1935 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
+-rw-r--r--   0        0        0     2028 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_job_request.py
+-rw-r--r--   0        0        0     2281 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_add_collaborator_request.py
+-rw-r--r--   0        0        0     2882 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_bucket_request.py
+-rw-r--r--   0        0        0     2578 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_create_empty_project_request.py
+-rw-r--r--   0        0        0     2428 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_create_project_request.py
+-rw-r--r--   0        0        0     2764 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     4154 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2158 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_data_item_request.py
+-rw-r--r--   0        0        0     2624 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_dataset_request.py
+-rw-r--r--   0        0        0     2881 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2724 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_portal_response.py
+-rw-r--r--   0        0        0     2445 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2582 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_request.py
+-rw-r--r--   0        0        0     4664 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     4734 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     8081 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_project_request.py
+-rw-r--r--   0        0        0     1877 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_project_tags_request.py
+-rw-r--r--   0        0        0     2259 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_theme_colors_request.py
+-rw-r--r--   0        0        0     2895 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_theme_logos_request.py
+-rw-r--r--   0        0        0     2205 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_third_party_auth_request.py
+-rw-r--r--   0        0        0     2603 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_user_request.py
+-rw-r--r--   0        0        0     1886 2023-07-20 19:24:45.283040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_version_request.py
+-rw-r--r--   0        0        0     2393 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
+-rw-r--r--   0        0        0     2237 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
+-rw-r--r--   0        0        0     2125 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
+-rw-r--r--   0        0        0     2059 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_whitelabel_request.py
+-rw-r--r--   0        0        0     2168 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/upload_asset_response.py
+-rw-r--r--   0        0        0     1882 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/upload_asset_response_all_of.py
+-rw-r--r--   0        0        0     2199 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/upload_readme_image_response.py
+-rw-r--r--   0        0        0     2185 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/upload_user_photo_response.py
+-rw-r--r--   0        0        0     1872 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/upload_user_photo_response_all_of.py
+-rw-r--r--   0        0        0     3673 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/user.py
+-rw-r--r--   0        0        0     1991 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/user_by_third_party_activation_request.py
+-rw-r--r--   0        0        0     2192 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/user_experiment.py
+-rw-r--r--   0        0        0     3200 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/user_organization.py
+-rw-r--r--   0        0        0     1844 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_dsp_block_url_request.py
+-rw-r--r--   0        0        0     2604 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_dsp_block_url_response.py
+-rw-r--r--   0        0        0     2307 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
+-rw-r--r--   0        0        0     2407 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
+-rw-r--r--   0        0        0     2708 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_organization_bucket_request.py
+-rw-r--r--   0        0        0     2897 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_organization_bucket_response.py
+-rw-r--r--   0        0        0     2597 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2187 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
+-rw-r--r--   0        0        0     1937 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_reset_password_request.py
+-rw-r--r--   0        0        0     5887 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/whitelabel.py
+-rw-r--r--   0        0        0     2534 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
+-rw-r--r--   0        0        0     2120 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
+-rw-r--r--   0        0        0     2885 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/window_settings_response.py
+-rw-r--r--   0        0        0     2585 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/window_settings_response_all_of.py
+-rw-r--r--   0        0        0     2848 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
+-rw-r--r--   0        0        0    12674 2023-07-20 19:24:45.287040 edgeimpulse_api-1.25.31/edgeimpulse_api/rest.py
+-rw-r--r--   0        0        0      968 2023-07-20 19:25:10.562599 edgeimpulse_api-1.25.31/pyproject.toml
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 edgeimpulse_api-1.25.31/PKG-INFO
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/__init__.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.25.16" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+__version__ = "1.25.31" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 
 # import apis into sdk package
 from edgeimpulse_api.api.admin_api import AdminApi
 from edgeimpulse_api.api.allows_read_only_api import AllowsReadOnlyApi
 from edgeimpulse_api.api.auth_api import AuthApi
 from edgeimpulse_api.api.cdn_api import CDNApi
 from edgeimpulse_api.api.classify_api import ClassifyApi
@@ -102,14 +102,15 @@
 from edgeimpulse_api.models.admin_add_user_request import AdminAddUserRequest
 from edgeimpulse_api.models.admin_api_organization import AdminApiOrganization
 from edgeimpulse_api.models.admin_api_organization_all_of import AdminApiOrganizationAllOf
 from edgeimpulse_api.models.admin_api_project import AdminApiProject
 from edgeimpulse_api.models.admin_api_user import AdminApiUser
 from edgeimpulse_api.models.admin_api_user_all_of import AdminApiUserAllOf
 from edgeimpulse_api.models.admin_create_organization_request import AdminCreateOrganizationRequest
+from edgeimpulse_api.models.admin_create_user_trial_request import AdminCreateUserTrialRequest
 from edgeimpulse_api.models.admin_get_data_migration_response import AdminGetDataMigrationResponse
 from edgeimpulse_api.models.admin_get_data_migration_response_all_of import AdminGetDataMigrationResponseAllOf
 from edgeimpulse_api.models.admin_get_data_migrations_response import AdminGetDataMigrationsResponse
 from edgeimpulse_api.models.admin_get_data_migrations_response_all_of import AdminGetDataMigrationsResponseAllOf
 from edgeimpulse_api.models.admin_get_disallowed_email_domains_response import AdminGetDisallowedEmailDomainsResponse
 from edgeimpulse_api.models.admin_get_disallowed_email_domains_response_all_of import AdminGetDisallowedEmailDomainsResponseAllOf
 from edgeimpulse_api.models.admin_get_metrics_response import AdminGetMetricsResponse
@@ -124,29 +125,32 @@
 from edgeimpulse_api.models.admin_get_sso_settings_response_all_of_sso_whitelist import AdminGetSSOSettingsResponseAllOfSsoWhitelist
 from edgeimpulse_api.models.admin_get_user_ids_response import AdminGetUserIdsResponse
 from edgeimpulse_api.models.admin_get_user_ids_response_all_of import AdminGetUserIdsResponseAllOf
 from edgeimpulse_api.models.admin_get_user_metrics_response import AdminGetUserMetricsResponse
 from edgeimpulse_api.models.admin_get_user_metrics_response_all_of import AdminGetUserMetricsResponseAllOf
 from edgeimpulse_api.models.admin_get_user_response import AdminGetUserResponse
 from edgeimpulse_api.models.admin_get_user_response_all_of import AdminGetUserResponseAllOf
+from edgeimpulse_api.models.admin_get_user_trial_response import AdminGetUserTrialResponse
+from edgeimpulse_api.models.admin_get_user_trial_response_all_of import AdminGetUserTrialResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response import AdminGetUsersResponse
 from edgeimpulse_api.models.admin_get_users_response_all_of import AdminGetUsersResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response_all_of_users import AdminGetUsersResponseAllOfUsers
 from edgeimpulse_api.models.admin_list_projects import AdminListProjects
 from edgeimpulse_api.models.admin_list_projects_response import AdminListProjectsResponse
 from edgeimpulse_api.models.admin_organization_info_response import AdminOrganizationInfoResponse
 from edgeimpulse_api.models.admin_organization_info_response_all_of import AdminOrganizationInfoResponseAllOf
 from edgeimpulse_api.models.admin_toggle_data_migration_request import AdminToggleDataMigrationRequest
 from edgeimpulse_api.models.admin_update_organization_request import AdminUpdateOrganizationRequest
 from edgeimpulse_api.models.admin_update_user_permissions_request import AdminUpdateUserPermissionsRequest
 from edgeimpulse_api.models.admin_update_user_request import AdminUpdateUserRequest
+from edgeimpulse_api.models.admin_update_user_trial_request import AdminUpdateUserTrialRequest
 from edgeimpulse_api.models.akida_edge_learning_config import AkidaEdgeLearningConfig
 from edgeimpulse_api.models.anomaly_model_metadata import AnomalyModelMetadata
-from edgeimpulse_api.models.anomaly_model_metadata_clusters_inner import AnomalyModelMetadataClustersInner
-from edgeimpulse_api.models.anomaly_model_metadata_response import AnomalyModelMetadataResponse
+from edgeimpulse_api.models.anomaly_model_metadata_all_of import AnomalyModelMetadataAllOf
+from edgeimpulse_api.models.anomaly_model_metadata_all_of_clusters import AnomalyModelMetadataAllOfClusters
 from edgeimpulse_api.models.anomaly_response import AnomalyResponse
 from edgeimpulse_api.models.anomaly_response_all_of import AnomalyResponseAllOf
 from edgeimpulse_api.models.anomaly_response_all_of_axes import AnomalyResponseAllOfAxes
 from edgeimpulse_api.models.anomaly_trained_features_response import AnomalyTrainedFeaturesResponse
 from edgeimpulse_api.models.anomaly_trained_features_response_all_of import AnomalyTrainedFeaturesResponseAllOf
 from edgeimpulse_api.models.anomaly_trained_features_response_all_of_data import AnomalyTrainedFeaturesResponseAllOfData
 from edgeimpulse_api.models.augmentation_policy_image_enum import AugmentationPolicyImageEnum
@@ -291,15 +295,17 @@
 from edgeimpulse_api.models.dsp_sample_features_response_all_of_data import DspSampleFeaturesResponseAllOfData
 from edgeimpulse_api.models.dsp_sample_features_response_all_of_sample import DspSampleFeaturesResponseAllOfSample
 from edgeimpulse_api.models.dsp_trained_features_response import DspTrainedFeaturesResponse
 from edgeimpulse_api.models.dsp_trained_features_response_all_of import DspTrainedFeaturesResponseAllOf
 from edgeimpulse_api.models.dsp_trained_features_response_all_of_data import DspTrainedFeaturesResponseAllOfData
 from edgeimpulse_api.models.dsp_trained_features_response_all_of_sample import DspTrainedFeaturesResponseAllOfSample
 from edgeimpulse_api.models.edit_sample_label_request import EditSampleLabelRequest
+from edgeimpulse_api.models.enterprise_trial import EnterpriseTrial
 from edgeimpulse_api.models.entitlement_limits import EntitlementLimits
+from edgeimpulse_api.models.entity_created_response import EntityCreatedResponse
 from edgeimpulse_api.models.evaluate_job_response import EvaluateJobResponse
 from edgeimpulse_api.models.evaluate_job_response_all_of import EvaluateJobResponseAllOf
 from edgeimpulse_api.models.evaluate_result_value import EvaluateResultValue
 from edgeimpulse_api.models.export_get_url_response import ExportGetUrlResponse
 from edgeimpulse_api.models.export_get_url_response_all_of import ExportGetUrlResponseAllOf
 from edgeimpulse_api.models.export_keras_block_data_request import ExportKerasBlockDataRequest
 from edgeimpulse_api.models.export_original_data_request import ExportOriginalDataRequest
@@ -666,14 +672,15 @@
 from edgeimpulse_api.models.project_info_summary_response_all_of import ProjectInfoSummaryResponseAllOf
 from edgeimpulse_api.models.project_private_data import ProjectPrivateData
 from edgeimpulse_api.models.project_public_data import ProjectPublicData
 from edgeimpulse_api.models.project_public_data_readme import ProjectPublicDataReadme
 from edgeimpulse_api.models.project_sample_metadata import ProjectSampleMetadata
 from edgeimpulse_api.models.project_training_data_summary_response import ProjectTrainingDataSummaryResponse
 from edgeimpulse_api.models.project_training_data_summary_response_all_of import ProjectTrainingDataSummaryResponseAllOf
+from edgeimpulse_api.models.project_type import ProjectType
 from edgeimpulse_api.models.project_version_request import ProjectVersionRequest
 from edgeimpulse_api.models.raw_sample_data import RawSampleData
 from edgeimpulse_api.models.raw_sample_payload import RawSamplePayload
 from edgeimpulse_api.models.rebalance_dataset_response import RebalanceDatasetResponse
 from edgeimpulse_api.models.remove_collaborator_request import RemoveCollaboratorRequest
 from edgeimpulse_api.models.remove_member_request import RemoveMemberRequest
 from edgeimpulse_api.models.rename_device_request import RenameDeviceRequest
@@ -744,14 +751,15 @@
 from edgeimpulse_api.models.transfer_ownership_organization_request import TransferOwnershipOrganizationRequest
 from edgeimpulse_api.models.transformation_block_additional_mount_point import TransformationBlockAdditionalMountPoint
 from edgeimpulse_api.models.transformation_job_status_enum import TransformationJobStatusEnum
 from edgeimpulse_api.models.tuner_create_trial_impulse import TunerCreateTrialImpulse
 from edgeimpulse_api.models.tuner_space_impulse import TunerSpaceImpulse
 from edgeimpulse_api.models.tuner_trial import TunerTrial
 from edgeimpulse_api.models.tuner_trial_blocks_inner import TunerTrialBlocksInner
+from edgeimpulse_api.models.tuner_trial_dsp_job_id import TunerTrialDspJobId
 from edgeimpulse_api.models.update_job_request import UpdateJobRequest
 from edgeimpulse_api.models.update_organization_add_collaborator_request import UpdateOrganizationAddCollaboratorRequest
 from edgeimpulse_api.models.update_organization_bucket_request import UpdateOrganizationBucketRequest
 from edgeimpulse_api.models.update_organization_create_empty_project_request import UpdateOrganizationCreateEmptyProjectRequest
 from edgeimpulse_api.models.update_organization_create_project_request import UpdateOrganizationCreateProjectRequest
 from edgeimpulse_api.models.update_organization_data_campaign_dashboard_request import UpdateOrganizationDataCampaignDashboardRequest
 from edgeimpulse_api.models.update_organization_data_campaign_request import UpdateOrganizationDataCampaignRequest
@@ -769,14 +777,15 @@
 from edgeimpulse_api.models.update_theme_logos_request import UpdateThemeLogosRequest
 from edgeimpulse_api.models.update_third_party_auth_request import UpdateThirdPartyAuthRequest
 from edgeimpulse_api.models.update_user_request import UpdateUserRequest
 from edgeimpulse_api.models.update_version_request import UpdateVersionRequest
 from edgeimpulse_api.models.update_whitelabel_default_deployment_target_request import UpdateWhitelabelDefaultDeploymentTargetRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_options_order_request import UpdateWhitelabelDeploymentOptionsOrderRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_targets_request import UpdateWhitelabelDeploymentTargetsRequest
+from edgeimpulse_api.models.update_whitelabel_request import UpdateWhitelabelRequest
 from edgeimpulse_api.models.upload_asset_response import UploadAssetResponse
 from edgeimpulse_api.models.upload_asset_response_all_of import UploadAssetResponseAllOf
 from edgeimpulse_api.models.upload_readme_image_response import UploadReadmeImageResponse
 from edgeimpulse_api.models.upload_user_photo_response import UploadUserPhotoResponse
 from edgeimpulse_api.models.upload_user_photo_response_all_of import UploadUserPhotoResponseAllOf
 from edgeimpulse_api.models.user import User
 from edgeimpulse_api.models.user_by_third_party_activation_request import UserByThirdPartyActivationRequest
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/__init__.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/admin_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/admin_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,32 +22,36 @@
 from typing import Optional
 
 from edgeimpulse_api.models.admin_add_disallowed_email_domain_request import AdminAddDisallowedEmailDomainRequest
 from edgeimpulse_api.models.admin_add_or_update_sso_domain_id_ps_request import AdminAddOrUpdateSSODomainIdPsRequest
 from edgeimpulse_api.models.admin_add_organization_user_request import AdminAddOrganizationUserRequest
 from edgeimpulse_api.models.admin_add_project_user_request import AdminAddProjectUserRequest
 from edgeimpulse_api.models.admin_create_organization_request import AdminCreateOrganizationRequest
+from edgeimpulse_api.models.admin_create_user_trial_request import AdminCreateUserTrialRequest
 from edgeimpulse_api.models.admin_get_data_migration_response import AdminGetDataMigrationResponse
 from edgeimpulse_api.models.admin_get_data_migrations_response import AdminGetDataMigrationsResponse
 from edgeimpulse_api.models.admin_get_disallowed_email_domains_response import AdminGetDisallowedEmailDomainsResponse
 from edgeimpulse_api.models.admin_get_metrics_response import AdminGetMetricsResponse
 from edgeimpulse_api.models.admin_get_organizations_response import AdminGetOrganizationsResponse
 from edgeimpulse_api.models.admin_get_sso_domain_id_ps_response import AdminGetSSODomainIdPsResponse
 from edgeimpulse_api.models.admin_get_sso_settings_response import AdminGetSSOSettingsResponse
 from edgeimpulse_api.models.admin_get_user_ids_response import AdminGetUserIdsResponse
 from edgeimpulse_api.models.admin_get_user_metrics_response import AdminGetUserMetricsResponse
 from edgeimpulse_api.models.admin_get_user_response import AdminGetUserResponse
+from edgeimpulse_api.models.admin_get_user_trial_response import AdminGetUserTrialResponse
 from edgeimpulse_api.models.admin_get_users_response import AdminGetUsersResponse
 from edgeimpulse_api.models.admin_list_projects_response import AdminListProjectsResponse
 from edgeimpulse_api.models.admin_organization_info_response import AdminOrganizationInfoResponse
 from edgeimpulse_api.models.admin_toggle_data_migration_request import AdminToggleDataMigrationRequest
 from edgeimpulse_api.models.admin_update_organization_request import AdminUpdateOrganizationRequest
 from edgeimpulse_api.models.admin_update_user_permissions_request import AdminUpdateUserPermissionsRequest
 from edgeimpulse_api.models.admin_update_user_request import AdminUpdateUserRequest
+from edgeimpulse_api.models.admin_update_user_trial_request import AdminUpdateUserTrialRequest
 from edgeimpulse_api.models.create_organization_response import CreateOrganizationResponse
+from edgeimpulse_api.models.entity_created_response import EntityCreatedResponse
 from edgeimpulse_api.models.find_user_response import FindUserResponse
 from edgeimpulse_api.models.generic_api_response import GenericApiResponse
 from edgeimpulse_api.models.job_details_response import JobDetailsResponse
 from edgeimpulse_api.models.job_logs_response import JobLogsResponse
 from edgeimpulse_api.models.job_metrics_response import JobMetricsResponse
 from edgeimpulse_api.models.job_parent_type_enum import JobParentTypeEnum
 from edgeimpulse_api.models.project_info_response import ProjectInfoResponse
@@ -917,14 +921,161 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def admin_create_user_trial(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_create_user_trial_request : AdminCreateUserTrialRequest, **kwargs) -> EntityCreatedResponse:  # noqa: E501
+        """Create user enterprise trial
+
+        Admin-only API to create an enterprise trial for a user.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param admin_create_user_trial_request: (required)
+        :type admin_create_user_trial_request: AdminCreateUserTrialRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: EntityCreatedResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._admin_create_user_trial_with_http_info(user_id, admin_create_user_trial_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _admin_create_user_trial_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_create_user_trial_request : AdminCreateUserTrialRequest, **kwargs):  # noqa: E501
+        """Create user enterprise trial 
+
+        Admin-only API to create an enterprise trial for a user.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param admin_create_user_trial_request: (required)
+        :type admin_create_user_trial_request: AdminCreateUserTrialRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(EntityCreatedResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'user_id',
+            'admin_create_user_trial_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method admin_create_user_trial" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['user_id']:
+            _path_params['userId'] = _params['user_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['admin_create_user_trial_request']:
+            _body_params = _params['admin_create_user_trial_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "EntityCreatedResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/admin/users/{userId}/trials', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def admin_delete_disallowed_email_domain(self, domain_name : Annotated[StrictStr, Field(..., description="Email domain name")], **kwargs) -> GenericApiResponse:  # noqa: E501
         """Delete disallowed email domain
 
         Admin-only API to delete an email domain from the list of disallowed email domains.
 
         :param domain_name: Email domain name (required)
         :type domain_name: str
@@ -1596,14 +1747,154 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def admin_delete_user_trial(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Delete user enterprise trial
+
+        Admin-only API to delete an enterprise trial for a user.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._admin_delete_user_trial_with_http_info(user_id, enterprise_trial_id, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _admin_delete_user_trial_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs):  # noqa: E501
+        """Delete user enterprise trial 
+
+        Admin-only API to delete an enterprise trial for a user.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'user_id',
+            'enterprise_trial_id'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method admin_delete_user_trial" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['user_id']:
+            _path_params['userId'] = _params['user_id']
+        if _params['enterprise_trial_id']:
+            _path_params['enterpriseTrialId'] = _params['enterprise_trial_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/admin/users/{userId}/trials/{enterpriseTrialId}', 'DELETE',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def admin_find_user(self, query : Annotated[StrictStr, Field(..., description="Part of e-mail address or username")], **kwargs) -> FindUserResponse:  # noqa: E501
         """Find a user
 
         DEPRECATED. Admin-only API to find a user by username or email address.
 
         :param query: Part of e-mail address or username (required)
         :type query: str
@@ -4046,14 +4337,154 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def admin_get_user_trial(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs) -> AdminGetUserTrialResponse:  # noqa: E501
+        """Get user enterprise trial
+
+        Admin-only API to get a specific enterprise trial.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: AdminGetUserTrialResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._admin_get_user_trial_with_http_info(user_id, enterprise_trial_id, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _admin_get_user_trial_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs):  # noqa: E501
+        """Get user enterprise trial 
+
+        Admin-only API to get a specific enterprise trial.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(AdminGetUserTrialResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'user_id',
+            'enterprise_trial_id'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method admin_get_user_trial" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['user_id']:
+            _path_params['userId'] = _params['user_id']
+        if _params['enterprise_trial_id']:
+            _path_params['enterpriseTrialId'] = _params['enterprise_trial_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "AdminGetUserTrialResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/admin/users/{userId}/trials/{enterpriseTrialId}', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def admin_get_users(self, active : Annotated[Optional[StrictInt], Field(description="Whether to search for entities (users, orgs) active in the last X days")] = None, tier : Annotated[Optional[StrictStr], Field(description="Whether to search for free, pro or enterprise entities (users, projects)")] = None, fields : Annotated[Optional[StrictStr], Field(description="Comma separated list of fields to fetch in a query")] = None, sort : Annotated[Optional[StrictStr], Field(description="Fields and order to sort query by")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, search : Annotated[Optional[StrictStr], Field(description="Search query")] = None, **kwargs) -> AdminGetUsersResponse:  # noqa: E501
         """Get all users
 
         Admin-only API to get the list of all registered users.
 
         :param active: Whether to search for entities (users, orgs) active in the last X days
         :type active: int
@@ -5360,14 +5791,168 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def admin_update_user_trial(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], admin_update_user_trial_request : AdminUpdateUserTrialRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Update user enterprise trial
+
+        Admin-only API to update an enterprise trial for a user.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
+        :param admin_update_user_trial_request: (required)
+        :type admin_update_user_trial_request: AdminUpdateUserTrialRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._admin_update_user_trial_with_http_info(user_id, enterprise_trial_id, admin_update_user_trial_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _admin_update_user_trial_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], admin_update_user_trial_request : AdminUpdateUserTrialRequest, **kwargs):  # noqa: E501
+        """Update user enterprise trial 
+
+        Admin-only API to update an enterprise trial for a user.
+
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
+        :param admin_update_user_trial_request: (required)
+        :type admin_update_user_trial_request: AdminUpdateUserTrialRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'user_id',
+            'enterprise_trial_id',
+            'admin_update_user_trial_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method admin_update_user_trial" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['user_id']:
+            _path_params['userId'] = _params['user_id']
+        if _params['enterprise_trial_id']:
+            _path_params['enterpriseTrialId'] = _params['enterprise_trial_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['admin_update_user_trial_request']:
+            _body_params = _params['admin_update_user_trial_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/admin/users/{userId}/trials/{enterpriseTrialId}', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/allows_read_only_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/allows_read_only_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr
 
 from typing import Optional
 
-from edgeimpulse_api.models.anomaly_model_metadata_response import AnomalyModelMetadataResponse
+from edgeimpulse_api.models.anomaly_model_metadata import AnomalyModelMetadata
 from edgeimpulse_api.models.anomaly_trained_features_response import AnomalyTrainedFeaturesResponse
 from edgeimpulse_api.models.classify_job_response import ClassifyJobResponse
 from edgeimpulse_api.models.classify_job_response_page import ClassifyJobResponsePage
 from edgeimpulse_api.models.classify_sample_response import ClassifySampleResponse
 from edgeimpulse_api.models.count_samples_response import CountSamplesResponse
 from edgeimpulse_api.models.dsp_metadata_response import DSPMetadataResponse
 from edgeimpulse_api.models.data_explorer_predictions_response import DataExplorerPredictionsResponse
@@ -1769,15 +1769,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_anomaly_metadata(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], learn_id : Annotated[StrictInt, Field(..., description="Learn Block ID, use the impulse functions to retrieve the ID")], **kwargs) -> AnomalyModelMetadataResponse:  # noqa: E501
+    def get_anomaly_metadata(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], learn_id : Annotated[StrictInt, Field(..., description="Learn Block ID, use the impulse functions to retrieve the ID")], **kwargs) -> AnomalyModelMetadata:  # noqa: E501
         """Anomaly metadata
 
         Get metadata about a trained anomaly block. Use the impulse blocks to find the learnId.
 
         :param project_id: Project ID (required)
         :type project_id: int
         :param learn_id: Learn Block ID, use the impulse functions to retrieve the ID (required)
@@ -1791,15 +1791,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: AnomalyModelMetadataResponse
+        :rtype: AnomalyModelMetadata
         """
         kwargs['_return_http_data_only'] = True
         return self._get_anomaly_metadata_with_http_info(project_id, learn_id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def _get_anomaly_metadata_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], learn_id : Annotated[StrictInt, Field(..., description="Learn Block ID, use the impulse functions to retrieve the ID")], **kwargs):  # noqa: E501
         """Anomaly metadata 
@@ -1827,15 +1827,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(AnomalyModelMetadataResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(AnomalyModelMetadata, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'project_id',
             'learn_id'
@@ -1888,15 +1888,15 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "AnomalyModelMetadataResponse",
+            '200': "AnomalyModelMetadata",
         }
 
         return self.api_client.call_api(
             '/api/{projectId}/training/anomaly/{learnId}/metadata', 'GET',
             _path_params,
             _query_params,
             _header_params,
@@ -2462,23 +2462,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_dsp_metadata(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], dsp_id : Annotated[StrictInt, Field(..., description="DSP Block ID, use the impulse functions to retrieve the ID")], **kwargs) -> DSPMetadataResponse:  # noqa: E501
+    def get_dsp_metadata(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], dsp_id : Annotated[StrictInt, Field(..., description="DSP Block ID, use the impulse functions to retrieve the ID")], exclude_included_samples : Annotated[Optional[StrictBool], Field(description="Whether to exclude 'includedSamples' in the response (as these can slow down requests significantly).")] = None, **kwargs) -> DSPMetadataResponse:  # noqa: E501
         """Get metadata
 
         Retrieve the metadata from a generated DSP block.
 
         :param project_id: Project ID (required)
         :type project_id: int
         :param dsp_id: DSP Block ID, use the impulse functions to retrieve the ID (required)
         :type dsp_id: int
+        :param exclude_included_samples: Whether to exclude 'includedSamples' in the response (as these can slow down requests significantly).
+        :type exclude_included_samples: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -2487,26 +2489,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DSPMetadataResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._get_dsp_metadata_with_http_info(project_id, dsp_id, **kwargs)  # noqa: E501
+        return self._get_dsp_metadata_with_http_info(project_id, dsp_id, exclude_included_samples, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _get_dsp_metadata_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], dsp_id : Annotated[StrictInt, Field(..., description="DSP Block ID, use the impulse functions to retrieve the ID")], **kwargs):  # noqa: E501
+    def _get_dsp_metadata_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], dsp_id : Annotated[StrictInt, Field(..., description="DSP Block ID, use the impulse functions to retrieve the ID")], exclude_included_samples : Annotated[Optional[StrictBool], Field(description="Whether to exclude 'includedSamples' in the response (as these can slow down requests significantly).")] = None, **kwargs):  # noqa: E501
         """Get metadata 
 
         Retrieve the metadata from a generated DSP block.
 
         :param project_id: Project ID (required)
         :type project_id: int
         :param dsp_id: DSP Block ID, use the impulse functions to retrieve the ID (required)
         :type dsp_id: int
+        :param exclude_included_samples: Whether to exclude 'includedSamples' in the response (as these can slow down requests significantly).
+        :type exclude_included_samples: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -2527,15 +2531,16 @@
         :rtype: tuple(DSPMetadataResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'project_id',
-            'dsp_id'
+            'dsp_id',
+            'exclude_included_samples'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -2562,14 +2567,16 @@
         if _params['project_id']:
             _path_params['projectId'] = _params['project_id']
         if _params['dsp_id']:
             _path_params['dspId'] = _params['dsp_id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('exclude_included_samples') is not None:  # noqa: E501
+            _query_params.append(('excludeIncludedSamples', _params['exclude_included_samples']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/auth_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/cdn_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/cdn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/classify_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/classify_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/content_disposition_inline_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/content_disposition_inline_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/deployment_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/deployment_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/devices_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/devices_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/dsp_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/dsp_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1365,23 +1365,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_dsp_metadata(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], dsp_id : Annotated[StrictInt, Field(..., description="DSP Block ID, use the impulse functions to retrieve the ID")], **kwargs) -> DSPMetadataResponse:  # noqa: E501
+    def get_dsp_metadata(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], dsp_id : Annotated[StrictInt, Field(..., description="DSP Block ID, use the impulse functions to retrieve the ID")], exclude_included_samples : Annotated[Optional[StrictBool], Field(description="Whether to exclude 'includedSamples' in the response (as these can slow down requests significantly).")] = None, **kwargs) -> DSPMetadataResponse:  # noqa: E501
         """Get metadata
 
         Retrieve the metadata from a generated DSP block.
 
         :param project_id: Project ID (required)
         :type project_id: int
         :param dsp_id: DSP Block ID, use the impulse functions to retrieve the ID (required)
         :type dsp_id: int
+        :param exclude_included_samples: Whether to exclude 'includedSamples' in the response (as these can slow down requests significantly).
+        :type exclude_included_samples: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -1390,26 +1392,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DSPMetadataResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._get_dsp_metadata_with_http_info(project_id, dsp_id, **kwargs)  # noqa: E501
+        return self._get_dsp_metadata_with_http_info(project_id, dsp_id, exclude_included_samples, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _get_dsp_metadata_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], dsp_id : Annotated[StrictInt, Field(..., description="DSP Block ID, use the impulse functions to retrieve the ID")], **kwargs):  # noqa: E501
+    def _get_dsp_metadata_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], dsp_id : Annotated[StrictInt, Field(..., description="DSP Block ID, use the impulse functions to retrieve the ID")], exclude_included_samples : Annotated[Optional[StrictBool], Field(description="Whether to exclude 'includedSamples' in the response (as these can slow down requests significantly).")] = None, **kwargs):  # noqa: E501
         """Get metadata 
 
         Retrieve the metadata from a generated DSP block.
 
         :param project_id: Project ID (required)
         :type project_id: int
         :param dsp_id: DSP Block ID, use the impulse functions to retrieve the ID (required)
         :type dsp_id: int
+        :param exclude_included_samples: Whether to exclude 'includedSamples' in the response (as these can slow down requests significantly).
+        :type exclude_included_samples: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1430,15 +1434,16 @@
         :rtype: tuple(DSPMetadataResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'project_id',
-            'dsp_id'
+            'dsp_id',
+            'exclude_included_samples'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1465,14 +1470,16 @@
         if _params['project_id']:
             _path_params['projectId'] = _params['project_id']
         if _params['dsp_id']:
             _path_params['dspId'] = _params['dsp_id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('exclude_included_samples') is not None:  # noqa: E501
+            _query_params.append(('excludeIncludedSamples', _params['exclude_included_samples']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/export_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/health_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/health_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/impulse_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/impulse_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/jobs_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/learn_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/learn_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr
 
 from typing import Optional
 
-from edgeimpulse_api.models.anomaly_model_metadata_response import AnomalyModelMetadataResponse
+from edgeimpulse_api.models.anomaly_model_metadata import AnomalyModelMetadata
 from edgeimpulse_api.models.anomaly_response import AnomalyResponse
 from edgeimpulse_api.models.anomaly_trained_features_response import AnomalyTrainedFeaturesResponse
 from edgeimpulse_api.models.generic_api_response import GenericApiResponse
 from edgeimpulse_api.models.get_data_explorer_features_response import GetDataExplorerFeaturesResponse
 from edgeimpulse_api.models.get_pretrained_model_response import GetPretrainedModelResponse
 from edgeimpulse_api.models.keras_model_metadata import KerasModelMetadata
 from edgeimpulse_api.models.keras_response import KerasResponse
@@ -46,14 +46,168 @@
 class LearnApi(object):
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
+    def add_keras_files(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], learn_id : Annotated[StrictInt, Field(..., description="Learn Block ID, use the impulse functions to retrieve the ID")], zip : StrictStr, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Add Keras files
+
+        Add Keras block files with the contents of a zip. This is an internal API.
+
+        :param project_id: Project ID (required)
+        :type project_id: int
+        :param learn_id: Learn Block ID, use the impulse functions to retrieve the ID (required)
+        :type learn_id: int
+        :param zip: (required)
+        :type zip: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._add_keras_files_with_http_info(project_id, learn_id, zip, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _add_keras_files_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], learn_id : Annotated[StrictInt, Field(..., description="Learn Block ID, use the impulse functions to retrieve the ID")], zip : StrictStr, **kwargs):  # noqa: E501
+        """Add Keras files 
+
+        Add Keras block files with the contents of a zip. This is an internal API.
+
+        :param project_id: Project ID (required)
+        :type project_id: int
+        :param learn_id: Learn Block ID, use the impulse functions to retrieve the ID (required)
+        :type learn_id: int
+        :param zip: (required)
+        :type zip: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'project_id',
+            'learn_id',
+            'zip'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method add_keras_files" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['project_id']:
+            _path_params['projectId'] = _params['project_id']
+        if _params['learn_id']:
+            _path_params['learnId'] = _params['learn_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        if _params['zip']:
+            _files['zip'] = _params['zip']
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['multipart/form-data']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/{projectId}/training/keras/{learnId}/addFiles', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def anomaly_trained_features(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], learn_id : Annotated[StrictInt, Field(..., description="Learn Block ID, use the impulse functions to retrieve the ID")], feature_ax1 : Annotated[StrictInt, Field(..., description="Feature axis 1")], feature_ax2 : Annotated[StrictInt, Field(..., description="Feature axis 2")], **kwargs) -> AnomalyTrainedFeaturesResponse:  # noqa: E501
         """Trained features
 
         Get a sample of trained features, this extracts a number of samples and their features.
 
         :param project_id: Project ID (required)
         :type project_id: int
@@ -1054,15 +1208,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_anomaly_metadata(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], learn_id : Annotated[StrictInt, Field(..., description="Learn Block ID, use the impulse functions to retrieve the ID")], **kwargs) -> AnomalyModelMetadataResponse:  # noqa: E501
+    def get_anomaly_metadata(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], learn_id : Annotated[StrictInt, Field(..., description="Learn Block ID, use the impulse functions to retrieve the ID")], **kwargs) -> AnomalyModelMetadata:  # noqa: E501
         """Anomaly metadata
 
         Get metadata about a trained anomaly block. Use the impulse blocks to find the learnId.
 
         :param project_id: Project ID (required)
         :type project_id: int
         :param learn_id: Learn Block ID, use the impulse functions to retrieve the ID (required)
@@ -1076,15 +1230,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: AnomalyModelMetadataResponse
+        :rtype: AnomalyModelMetadata
         """
         kwargs['_return_http_data_only'] = True
         return self._get_anomaly_metadata_with_http_info(project_id, learn_id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def _get_anomaly_metadata_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], learn_id : Annotated[StrictInt, Field(..., description="Learn Block ID, use the impulse functions to retrieve the ID")], **kwargs):  # noqa: E501
         """Anomaly metadata 
@@ -1112,15 +1266,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(AnomalyModelMetadataResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(AnomalyModelMetadata, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'project_id',
             'learn_id'
@@ -1173,15 +1327,15 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "AnomalyModelMetadataResponse",
+            '200': "AnomalyModelMetadata",
         }
 
         return self.api_client.call_api(
             '/api/{projectId}/training/anomaly/{learnId}/metadata', 'GET',
             _path_params,
             _query_params,
             _header_params,
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/login_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/login_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/metrics_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/optimization_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/optimization_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_allow_developer_profile_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_allow_developer_profile_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_allow_guest_access_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_allow_guest_access_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_blocks_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_blocks_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_create_project_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_create_project_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_data_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_data_campaigns_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_data_campaigns_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_jobs_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_pipelines_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_pipelines_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_portals_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_portals_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_requires_admin_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_requires_admin_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 from edgeimpulse_api.models.update_organization_bucket_request import UpdateOrganizationBucketRequest
 from edgeimpulse_api.models.update_organization_request import UpdateOrganizationRequest
 from edgeimpulse_api.models.update_project_request import UpdateProjectRequest
 from edgeimpulse_api.models.update_theme_colors_request import UpdateThemeColorsRequest
 from edgeimpulse_api.models.update_whitelabel_default_deployment_target_request import UpdateWhitelabelDefaultDeploymentTargetRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_options_order_request import UpdateWhitelabelDeploymentOptionsOrderRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_targets_request import UpdateWhitelabelDeploymentTargetsRequest
+from edgeimpulse_api.models.update_whitelabel_request import UpdateWhitelabelRequest
 from edgeimpulse_api.models.upload_asset_response import UploadAssetResponse
 from edgeimpulse_api.models.whitelabel_admin_create_organization_request import WhitelabelAdminCreateOrganizationRequest
 
 from edgeimpulse_api.api_client import ApiClient
 from edgeimpulse_api.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
@@ -4624,14 +4625,161 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def whitelabel_admin_update_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], update_whitelabel_request : UpdateWhitelabelRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Update white label information
+
+        White label admin only API to update the white label information.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param update_whitelabel_request: (required)
+        :type update_whitelabel_request: UpdateWhitelabelRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._whitelabel_admin_update_info_with_http_info(organization_id, update_whitelabel_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _whitelabel_admin_update_info_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], update_whitelabel_request : UpdateWhitelabelRequest, **kwargs):  # noqa: E501
+        """Update white label information 
+
+        White label admin only API to update the white label information.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param update_whitelabel_request: (required)
+        :type update_whitelabel_request: UpdateWhitelabelRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'organization_id',
+            'update_whitelabel_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method whitelabel_admin_update_info" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['organization_id']:
+            _path_params['organizationId'] = _params['organization_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['update_whitelabel_request']:
+            _body_params = _params['update_whitelabel_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/organizations/{organizationId}/whitelabel', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from edgeimpulse_api.models.get_whitelabel_response import GetWhitelabelResponse
 from edgeimpulse_api.models.project_info_response import ProjectInfoResponse
 from edgeimpulse_api.models.update_project_request import UpdateProjectRequest
 from edgeimpulse_api.models.update_theme_colors_request import UpdateThemeColorsRequest
 from edgeimpulse_api.models.update_whitelabel_default_deployment_target_request import UpdateWhitelabelDefaultDeploymentTargetRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_options_order_request import UpdateWhitelabelDeploymentOptionsOrderRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_targets_request import UpdateWhitelabelDeploymentTargetsRequest
+from edgeimpulse_api.models.update_whitelabel_request import UpdateWhitelabelRequest
 from edgeimpulse_api.models.upload_asset_response import UploadAssetResponse
 from edgeimpulse_api.models.whitelabel_admin_create_organization_request import WhitelabelAdminCreateOrganizationRequest
 
 from edgeimpulse_api.api_client import ApiClient
 from edgeimpulse_api.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
@@ -2579,14 +2580,161 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def whitelabel_admin_update_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], update_whitelabel_request : UpdateWhitelabelRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Update white label information
+
+        White label admin only API to update the white label information.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param update_whitelabel_request: (required)
+        :type update_whitelabel_request: UpdateWhitelabelRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._whitelabel_admin_update_info_with_http_info(organization_id, update_whitelabel_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _whitelabel_admin_update_info_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], update_whitelabel_request : UpdateWhitelabelRequest, **kwargs):  # noqa: E501
+        """Update white label information 
+
+        White label admin only API to update the white label information.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param update_whitelabel_request: (required)
+        :type update_whitelabel_request: UpdateWhitelabelRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'organization_id',
+            'update_whitelabel_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method whitelabel_admin_update_info" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['organization_id']:
+            _path_params['organizationId'] = _params['organization_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['update_whitelabel_request']:
+            _body_params = _params['update_whitelabel_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/organizations/{organizationId}/whitelabel', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/organizations_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/organizations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 from edgeimpulse_api.models.set_member_role_request import SetMemberRoleRequest
 from edgeimpulse_api.models.update_organization_request import UpdateOrganizationRequest
 from edgeimpulse_api.models.update_project_request import UpdateProjectRequest
 from edgeimpulse_api.models.update_theme_colors_request import UpdateThemeColorsRequest
 from edgeimpulse_api.models.update_whitelabel_default_deployment_target_request import UpdateWhitelabelDefaultDeploymentTargetRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_options_order_request import UpdateWhitelabelDeploymentOptionsOrderRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_targets_request import UpdateWhitelabelDeploymentTargetsRequest
+from edgeimpulse_api.models.update_whitelabel_request import UpdateWhitelabelRequest
 from edgeimpulse_api.models.upload_asset_response import UploadAssetResponse
 from edgeimpulse_api.models.upload_readme_image_response import UploadReadmeImageResponse
 from edgeimpulse_api.models.whitelabel_admin_create_organization_request import WhitelabelAdminCreateOrganizationRequest
 
 from edgeimpulse_api.api_client import ApiClient
 from edgeimpulse_api.exceptions import (  # noqa: F401
     ApiTypeError,
@@ -5421,14 +5422,161 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def whitelabel_admin_update_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], update_whitelabel_request : UpdateWhitelabelRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Update white label information
+
+        White label admin only API to update the white label information.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param update_whitelabel_request: (required)
+        :type update_whitelabel_request: UpdateWhitelabelRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._whitelabel_admin_update_info_with_http_info(organization_id, update_whitelabel_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _whitelabel_admin_update_info_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], update_whitelabel_request : UpdateWhitelabelRequest, **kwargs):  # noqa: E501
+        """Update white label information 
+
+        White label admin only API to update the white label information.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param update_whitelabel_request: (required)
+        :type update_whitelabel_request: UpdateWhitelabelRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'organization_id',
+            'update_whitelabel_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method whitelabel_admin_update_info" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['organization_id']:
+            _path_params['organizationId'] = _params['organization_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['update_whitelabel_request']:
+            _body_params = _params['update_whitelabel_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/organizations/{organizationId}/whitelabel', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/performance_calibration_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/performance_calibration_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/project_requires_admin_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/project_requires_admin_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/projects_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/raw_data_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/raw_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/requires_sudo_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/requires_sudo_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/supports_range_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/supports_range_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/themes_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/themes_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/third_party_auth_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/third_party_auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/upload_portal_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/upload_portal_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/user_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/user_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api/whitelabels_api.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api/whitelabels_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/api_client.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/api_client.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/configuration.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/configuration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/exceptions.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/__init__.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 from edgeimpulse_api.models.admin_add_user_request import AdminAddUserRequest
 from edgeimpulse_api.models.admin_api_organization import AdminApiOrganization
 from edgeimpulse_api.models.admin_api_organization_all_of import AdminApiOrganizationAllOf
 from edgeimpulse_api.models.admin_api_project import AdminApiProject
 from edgeimpulse_api.models.admin_api_user import AdminApiUser
 from edgeimpulse_api.models.admin_api_user_all_of import AdminApiUserAllOf
 from edgeimpulse_api.models.admin_create_organization_request import AdminCreateOrganizationRequest
+from edgeimpulse_api.models.admin_create_user_trial_request import AdminCreateUserTrialRequest
 from edgeimpulse_api.models.admin_get_data_migration_response import AdminGetDataMigrationResponse
 from edgeimpulse_api.models.admin_get_data_migration_response_all_of import AdminGetDataMigrationResponseAllOf
 from edgeimpulse_api.models.admin_get_data_migrations_response import AdminGetDataMigrationsResponse
 from edgeimpulse_api.models.admin_get_data_migrations_response_all_of import AdminGetDataMigrationsResponseAllOf
 from edgeimpulse_api.models.admin_get_disallowed_email_domains_response import AdminGetDisallowedEmailDomainsResponse
 from edgeimpulse_api.models.admin_get_disallowed_email_domains_response_all_of import AdminGetDisallowedEmailDomainsResponseAllOf
 from edgeimpulse_api.models.admin_get_metrics_response import AdminGetMetricsResponse
@@ -69,29 +70,32 @@
 from edgeimpulse_api.models.admin_get_sso_settings_response_all_of_sso_whitelist import AdminGetSSOSettingsResponseAllOfSsoWhitelist
 from edgeimpulse_api.models.admin_get_user_ids_response import AdminGetUserIdsResponse
 from edgeimpulse_api.models.admin_get_user_ids_response_all_of import AdminGetUserIdsResponseAllOf
 from edgeimpulse_api.models.admin_get_user_metrics_response import AdminGetUserMetricsResponse
 from edgeimpulse_api.models.admin_get_user_metrics_response_all_of import AdminGetUserMetricsResponseAllOf
 from edgeimpulse_api.models.admin_get_user_response import AdminGetUserResponse
 from edgeimpulse_api.models.admin_get_user_response_all_of import AdminGetUserResponseAllOf
+from edgeimpulse_api.models.admin_get_user_trial_response import AdminGetUserTrialResponse
+from edgeimpulse_api.models.admin_get_user_trial_response_all_of import AdminGetUserTrialResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response import AdminGetUsersResponse
 from edgeimpulse_api.models.admin_get_users_response_all_of import AdminGetUsersResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response_all_of_users import AdminGetUsersResponseAllOfUsers
 from edgeimpulse_api.models.admin_list_projects import AdminListProjects
 from edgeimpulse_api.models.admin_list_projects_response import AdminListProjectsResponse
 from edgeimpulse_api.models.admin_organization_info_response import AdminOrganizationInfoResponse
 from edgeimpulse_api.models.admin_organization_info_response_all_of import AdminOrganizationInfoResponseAllOf
 from edgeimpulse_api.models.admin_toggle_data_migration_request import AdminToggleDataMigrationRequest
 from edgeimpulse_api.models.admin_update_organization_request import AdminUpdateOrganizationRequest
 from edgeimpulse_api.models.admin_update_user_permissions_request import AdminUpdateUserPermissionsRequest
 from edgeimpulse_api.models.admin_update_user_request import AdminUpdateUserRequest
+from edgeimpulse_api.models.admin_update_user_trial_request import AdminUpdateUserTrialRequest
 from edgeimpulse_api.models.akida_edge_learning_config import AkidaEdgeLearningConfig
 from edgeimpulse_api.models.anomaly_model_metadata import AnomalyModelMetadata
-from edgeimpulse_api.models.anomaly_model_metadata_clusters_inner import AnomalyModelMetadataClustersInner
-from edgeimpulse_api.models.anomaly_model_metadata_response import AnomalyModelMetadataResponse
+from edgeimpulse_api.models.anomaly_model_metadata_all_of import AnomalyModelMetadataAllOf
+from edgeimpulse_api.models.anomaly_model_metadata_all_of_clusters import AnomalyModelMetadataAllOfClusters
 from edgeimpulse_api.models.anomaly_response import AnomalyResponse
 from edgeimpulse_api.models.anomaly_response_all_of import AnomalyResponseAllOf
 from edgeimpulse_api.models.anomaly_response_all_of_axes import AnomalyResponseAllOfAxes
 from edgeimpulse_api.models.anomaly_trained_features_response import AnomalyTrainedFeaturesResponse
 from edgeimpulse_api.models.anomaly_trained_features_response_all_of import AnomalyTrainedFeaturesResponseAllOf
 from edgeimpulse_api.models.anomaly_trained_features_response_all_of_data import AnomalyTrainedFeaturesResponseAllOfData
 from edgeimpulse_api.models.augmentation_policy_image_enum import AugmentationPolicyImageEnum
@@ -236,15 +240,17 @@
 from edgeimpulse_api.models.dsp_sample_features_response_all_of_data import DspSampleFeaturesResponseAllOfData
 from edgeimpulse_api.models.dsp_sample_features_response_all_of_sample import DspSampleFeaturesResponseAllOfSample
 from edgeimpulse_api.models.dsp_trained_features_response import DspTrainedFeaturesResponse
 from edgeimpulse_api.models.dsp_trained_features_response_all_of import DspTrainedFeaturesResponseAllOf
 from edgeimpulse_api.models.dsp_trained_features_response_all_of_data import DspTrainedFeaturesResponseAllOfData
 from edgeimpulse_api.models.dsp_trained_features_response_all_of_sample import DspTrainedFeaturesResponseAllOfSample
 from edgeimpulse_api.models.edit_sample_label_request import EditSampleLabelRequest
+from edgeimpulse_api.models.enterprise_trial import EnterpriseTrial
 from edgeimpulse_api.models.entitlement_limits import EntitlementLimits
+from edgeimpulse_api.models.entity_created_response import EntityCreatedResponse
 from edgeimpulse_api.models.evaluate_job_response import EvaluateJobResponse
 from edgeimpulse_api.models.evaluate_job_response_all_of import EvaluateJobResponseAllOf
 from edgeimpulse_api.models.evaluate_result_value import EvaluateResultValue
 from edgeimpulse_api.models.export_get_url_response import ExportGetUrlResponse
 from edgeimpulse_api.models.export_get_url_response_all_of import ExportGetUrlResponseAllOf
 from edgeimpulse_api.models.export_keras_block_data_request import ExportKerasBlockDataRequest
 from edgeimpulse_api.models.export_original_data_request import ExportOriginalDataRequest
@@ -611,14 +617,15 @@
 from edgeimpulse_api.models.project_info_summary_response_all_of import ProjectInfoSummaryResponseAllOf
 from edgeimpulse_api.models.project_private_data import ProjectPrivateData
 from edgeimpulse_api.models.project_public_data import ProjectPublicData
 from edgeimpulse_api.models.project_public_data_readme import ProjectPublicDataReadme
 from edgeimpulse_api.models.project_sample_metadata import ProjectSampleMetadata
 from edgeimpulse_api.models.project_training_data_summary_response import ProjectTrainingDataSummaryResponse
 from edgeimpulse_api.models.project_training_data_summary_response_all_of import ProjectTrainingDataSummaryResponseAllOf
+from edgeimpulse_api.models.project_type import ProjectType
 from edgeimpulse_api.models.project_version_request import ProjectVersionRequest
 from edgeimpulse_api.models.raw_sample_data import RawSampleData
 from edgeimpulse_api.models.raw_sample_payload import RawSamplePayload
 from edgeimpulse_api.models.rebalance_dataset_response import RebalanceDatasetResponse
 from edgeimpulse_api.models.remove_collaborator_request import RemoveCollaboratorRequest
 from edgeimpulse_api.models.remove_member_request import RemoveMemberRequest
 from edgeimpulse_api.models.rename_device_request import RenameDeviceRequest
@@ -689,14 +696,15 @@
 from edgeimpulse_api.models.transfer_ownership_organization_request import TransferOwnershipOrganizationRequest
 from edgeimpulse_api.models.transformation_block_additional_mount_point import TransformationBlockAdditionalMountPoint
 from edgeimpulse_api.models.transformation_job_status_enum import TransformationJobStatusEnum
 from edgeimpulse_api.models.tuner_create_trial_impulse import TunerCreateTrialImpulse
 from edgeimpulse_api.models.tuner_space_impulse import TunerSpaceImpulse
 from edgeimpulse_api.models.tuner_trial import TunerTrial
 from edgeimpulse_api.models.tuner_trial_blocks_inner import TunerTrialBlocksInner
+from edgeimpulse_api.models.tuner_trial_dsp_job_id import TunerTrialDspJobId
 from edgeimpulse_api.models.update_job_request import UpdateJobRequest
 from edgeimpulse_api.models.update_organization_add_collaborator_request import UpdateOrganizationAddCollaboratorRequest
 from edgeimpulse_api.models.update_organization_bucket_request import UpdateOrganizationBucketRequest
 from edgeimpulse_api.models.update_organization_create_empty_project_request import UpdateOrganizationCreateEmptyProjectRequest
 from edgeimpulse_api.models.update_organization_create_project_request import UpdateOrganizationCreateProjectRequest
 from edgeimpulse_api.models.update_organization_data_campaign_dashboard_request import UpdateOrganizationDataCampaignDashboardRequest
 from edgeimpulse_api.models.update_organization_data_campaign_request import UpdateOrganizationDataCampaignRequest
@@ -714,14 +722,15 @@
 from edgeimpulse_api.models.update_theme_logos_request import UpdateThemeLogosRequest
 from edgeimpulse_api.models.update_third_party_auth_request import UpdateThirdPartyAuthRequest
 from edgeimpulse_api.models.update_user_request import UpdateUserRequest
 from edgeimpulse_api.models.update_version_request import UpdateVersionRequest
 from edgeimpulse_api.models.update_whitelabel_default_deployment_target_request import UpdateWhitelabelDefaultDeploymentTargetRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_options_order_request import UpdateWhitelabelDeploymentOptionsOrderRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_targets_request import UpdateWhitelabelDeploymentTargetsRequest
+from edgeimpulse_api.models.update_whitelabel_request import UpdateWhitelabelRequest
 from edgeimpulse_api.models.upload_asset_response import UploadAssetResponse
 from edgeimpulse_api.models.upload_asset_response_all_of import UploadAssetResponseAllOf
 from edgeimpulse_api.models.upload_readme_image_response import UploadReadmeImageResponse
 from edgeimpulse_api.models.upload_user_photo_response import UploadUserPhotoResponse
 from edgeimpulse_api.models.upload_user_photo_response_all_of import UploadUserPhotoResponseAllOf
 from edgeimpulse_api.models.user import User
 from edgeimpulse_api.models.user_by_third_party_activation_request import UserByThirdPartyActivationRequest
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/activate_user_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/activate_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_api_key_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_collaborator_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_hmac_key_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_hmac_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_member_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_api_key_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_bucket_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_deploy_block_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_dsp_block_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_dsp_block_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_secret_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_secret_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_secret_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_secret_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_secret_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_secret_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     object_detection_last_layer: Optional[ObjectDetectionLastLayer] = Field(None, alias="objectDetectionLastLayer")
     implementation_version: StrictInt = Field(..., alias="implementationVersion")
     is_public: Optional[StrictBool] = Field(None, alias="isPublic", description="Whether this block is publicly available to Edge Impulse users (if false, then only for members of the owning organization)")
     is_public_for_devices: Optional[List[StrictStr]] = Field(None, alias="isPublicForDevices", description="If `isPublic` is true, the list of devices (from latencyDevices) for which this model can be shown.")
     repository_url: Optional[StrictStr] = Field(None, alias="repositoryUrl", description="URL to the source code of this custom learn block.")
     parameters: Optional[List[Dict[str, Any]]] = Field(None, description="List of parameters, spec'ed according to https://docs.edgeimpulse.com/docs/tips-and-tricks/adding-parameters-to-custom-blocks")
     image_input_scaling: Optional[ImageInputScaling] = Field(None, alias="imageInputScaling")
-    __properties = ["name", "dockerContainer", "description", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "repositoryUrl", "parameters", "imageInputScaling"]
+    ind_requires_gpu: Optional[StrictBool] = Field(None, alias="indRequiresGpu", description="If set, requires this block to be scheduled on GPU.")
+    __properties = ["name", "dockerContainer", "description", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "repositoryUrl", "parameters", "imageInputScaling", "indRequiresGpu"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -78,11 +79,12 @@
             "operates_on": obj.get("operatesOn"),
             "object_detection_last_layer": obj.get("objectDetectionLastLayer"),
             "implementation_version": obj.get("implementationVersion"),
             "is_public": obj.get("isPublic"),
             "is_public_for_devices": obj.get("isPublicForDevices"),
             "repository_url": obj.get("repositoryUrl"),
             "parameters": obj.get("parameters"),
-            "image_input_scaling": obj.get("imageInputScaling")
+            "image_input_scaling": obj.get("imageInputScaling"),
+            "ind_requires_gpu": obj.get("indRequiresGpu")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_transformation_block_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_transformation_block_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_organization_user_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_organization_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_project_user_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_project_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_add_user_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_add_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_api_organization.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,88 +12,92 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
-from edgeimpulse_api.models.organization_user import OrganizationUser
-from edgeimpulse_api.models.project import Project
+from pydantic import BaseModel, Field, StrictInt, StrictStr
+from edgeimpulse_api.models.data_campaign_link import DataCampaignLink
+from edgeimpulse_api.models.data_campaign_query import DataCampaignQuery
 
-class AdminApiOrganization(BaseModel):
+class DataCampaign(BaseModel):
     id: StrictInt = ...
-    name: StrictStr = Field(..., description="EdgeImpulse Inc.")
+    data_campaign_dashboard_id: StrictInt = Field(..., alias="dataCampaignDashboardId")
+    created: datetime = ...
+    name: StrictStr = ...
+    description: StrictStr = ...
+    coordinator_uids: List[StrictInt] = Field(..., alias="coordinatorUids", description="List of user IDs that coordinate this campaign")
     logo: Optional[StrictStr] = None
-    header_img: Optional[StrictStr] = Field(None, alias="headerImg")
-    users: List[OrganizationUser] = ...
-    is_developer_profile: StrictBool = Field(..., alias="isDeveloperProfile")
-    whitelabel_id: Optional[StrictInt] = Field(..., alias="whitelabelId", description="Unique identifier of the white label this organization belongs to, if any.")
-    projects: List[Project] = Field(..., description="Array with organizational projects")
-    __properties = ["id", "name", "logo", "headerImg", "users", "isDeveloperProfile", "whitelabelId", "projects"]
+    queries: List[DataCampaignQuery] = ...
+    links: List[DataCampaignLink] = ...
+    datasets: List[StrictStr] = ...
+    pipeline_ids: List[StrictInt] = Field(..., alias="pipelineIds")
+    project_ids: List[StrictInt] = Field(..., alias="projectIds")
+    __properties = ["id", "dataCampaignDashboardId", "created", "name", "description", "coordinatorUids", "logo", "queries", "links", "datasets", "pipelineIds", "projectIds"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AdminApiOrganization:
-        """Create an instance of AdminApiOrganization from a JSON string"""
+    def from_json(cls, json_str: str) -> DataCampaign:
+        """Create an instance of DataCampaign from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in users (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in queries (list)
         _items = []
-        if self.users:
-            for _item in self.users:
+        if self.queries:
+            for _item in self.queries:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['users'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in projects (list)
+            _dict['queries'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in links (list)
         _items = []
-        if self.projects:
-            for _item in self.projects:
+        if self.links:
+            for _item in self.links:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['projects'] = _items
-        # set to None if whitelabel_id (nullable) is None
-        if self.whitelabel_id is None:
-            _dict['whitelabelId'] = None
-
+            _dict['links'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AdminApiOrganization:
-        """Create an instance of AdminApiOrganization from a dict"""
+    def from_dict(cls, obj: dict) -> DataCampaign:
+        """Create an instance of DataCampaign from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AdminApiOrganization.construct(**obj)
+            return DataCampaign.construct(**obj)
 
-        _obj = AdminApiOrganization.construct(**{
+        _obj = DataCampaign.construct(**{
             "id": obj.get("id"),
+            "data_campaign_dashboard_id": obj.get("dataCampaignDashboardId"),
+            "created": obj.get("created"),
             "name": obj.get("name"),
+            "description": obj.get("description"),
+            "coordinator_uids": obj.get("coordinatorUids"),
             "logo": obj.get("logo"),
-            "header_img": obj.get("headerImg"),
-            "users": [OrganizationUser.from_dict(_item) for _item in obj.get("users")] if obj.get("users") is not None else None,
-            "is_developer_profile": obj.get("isDeveloperProfile"),
-            "whitelabel_id": obj.get("whitelabelId"),
-            "projects": [Project.from_dict(_item) for _item in obj.get("projects")] if obj.get("projects") is not None else None
+            "queries": [DataCampaignQuery.from_dict(_item) for _item in obj.get("queries")] if obj.get("queries") is not None else None,
+            "links": [DataCampaignLink.from_dict(_item) for _item in obj.get("links")] if obj.get("links") is not None else None,
+            "datasets": obj.get("datasets"),
+            "pipeline_ids": obj.get("pipelineIds"),
+            "project_ids": obj.get("projectIds")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_api_organization_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_api_organization_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_api_project.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_api_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_api_user.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_api_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, validator
+from edgeimpulse_api.models.enterprise_trial import EnterpriseTrial
 from edgeimpulse_api.models.permission import Permission
 from edgeimpulse_api.models.project import Project
 from edgeimpulse_api.models.staff_info import StaffInfo
 from edgeimpulse_api.models.user_experiment import UserExperiment
 from edgeimpulse_api.models.user_organization import UserOrganization
 
 class AdminApiUser(BaseModel):
@@ -44,15 +45,16 @@
     projects: List[Project] = ...
     experiments: List[UserExperiment] = Field(..., description="Experiments the user has access to. Enabling experiments can only be done through a JWT token.")
     evaluation: Optional[StrictBool] = Field(None, description="Whether this is an ephemeral evaluation account.")
     ambassador: Optional[StrictBool] = Field(None, description="Whether this user is an ambassador.")
     show_imagine2022: StrictBool = Field(..., alias="showImagine2022", description="Whether to show the Imagine 2022 banner.")
     tier: StrictStr = Field(..., description="The user account tier.")
     suspended: StrictBool = Field(..., description="Whether the user is suspended.")
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "organizations", "projects", "experiments", "evaluation", "ambassador", "showImagine2022", "tier", "suspended"]
+    trials: List[EnterpriseTrial] = Field(..., description="Current, past or future enterprise trials.")
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "organizations", "projects", "experiments", "evaluation", "ambassador", "showImagine2022", "tier", "suspended", "trials"]
 
     @validator('tier')
     def tier_validate_enum(cls, v):
         if v not in ('free', 'pro'):
             raise ValueError("must validate the enum values ('free', 'pro')")
         return v
 
@@ -99,14 +101,21 @@
         # override the default output from pydantic by calling `to_dict()` of each item in experiments (list)
         _items = []
         if self.experiments:
             for _item in self.experiments:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['experiments'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in trials (list)
+        _items = []
+        if self.trials:
+            for _item in self.trials:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['trials'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> AdminApiUser:
         """Create an instance of AdminApiUser from a dict"""
         if obj is None:
             return None
@@ -132,11 +141,12 @@
             "organizations": [UserOrganization.from_dict(_item) for _item in obj.get("organizations")] if obj.get("organizations") is not None else None,
             "projects": [Project.from_dict(_item) for _item in obj.get("projects")] if obj.get("projects") is not None else None,
             "experiments": [UserExperiment.from_dict(_item) for _item in obj.get("experiments")] if obj.get("experiments") is not None else None,
             "evaluation": obj.get("evaluation"),
             "ambassador": obj.get("ambassador"),
             "show_imagine2022": obj.get("showImagine2022"),
             "tier": obj.get("tier"),
-            "suspended": obj.get("suspended")
+            "suspended": obj.get("suspended"),
+            "trials": [EnterpriseTrial.from_dict(_item) for _item in obj.get("trials")] if obj.get("trials") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_api_user_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_api_user_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
+from edgeimpulse_api.models.enterprise_trial import EnterpriseTrial
 from edgeimpulse_api.models.project import Project
 from edgeimpulse_api.models.user_experiment import UserExperiment
 from edgeimpulse_api.models.user_organization import UserOrganization
 
 class AdminApiUserAllOf(BaseModel):
     email: StrictStr = ...
     activated: StrictBool = ...
@@ -31,15 +32,16 @@
     experiments: List[UserExperiment] = Field(..., description="Experiments the user has access to. Enabling experiments can only be done through a JWT token.")
     evaluation: Optional[StrictBool] = Field(None, description="Whether this is an ephemeral evaluation account.")
     ambassador: Optional[StrictBool] = Field(None, description="Whether this user is an ambassador.")
     show_imagine2022: StrictBool = Field(..., alias="showImagine2022", description="Whether to show the Imagine 2022 banner.")
     tier: StrictStr = Field(..., description="The user account tier.")
     last_seen: Optional[datetime] = Field(None, alias="lastSeen")
     suspended: StrictBool = Field(..., description="Whether the user is suspended.")
-    __properties = ["email", "activated", "organizations", "projects", "experiments", "evaluation", "ambassador", "showImagine2022", "tier", "lastSeen", "suspended"]
+    trials: List[EnterpriseTrial] = Field(..., description="Current, past or future enterprise trials.")
+    __properties = ["email", "activated", "organizations", "projects", "experiments", "evaluation", "ambassador", "showImagine2022", "tier", "lastSeen", "suspended", "trials"]
 
     @validator('tier')
     def tier_validate_enum(cls, v):
         if v not in ('free', 'pro'):
             raise ValueError("must validate the enum values ('free', 'pro')")
         return v
 
@@ -83,14 +85,21 @@
         # override the default output from pydantic by calling `to_dict()` of each item in experiments (list)
         _items = []
         if self.experiments:
             for _item in self.experiments:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['experiments'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in trials (list)
+        _items = []
+        if self.trials:
+            for _item in self.trials:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['trials'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> AdminApiUserAllOf:
         """Create an instance of AdminApiUserAllOf from a dict"""
         if obj is None:
             return None
@@ -105,11 +114,12 @@
             "projects": [Project.from_dict(_item) for _item in obj.get("projects")] if obj.get("projects") is not None else None,
             "experiments": [UserExperiment.from_dict(_item) for _item in obj.get("experiments")] if obj.get("experiments") is not None else None,
             "evaluation": obj.get("evaluation"),
             "ambassador": obj.get("ambassador"),
             "show_imagine2022": obj.get("showImagine2022"),
             "tier": obj.get("tier"),
             "last_seen": obj.get("lastSeen"),
-            "suspended": obj.get("suspended")
+            "suspended": obj.get("suspended"),
+            "trials": [EnterpriseTrial.from_dict(_item) for _item in obj.get("trials")] if obj.get("trials") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_create_organization_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_data_migration_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_data_migration_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_data_migrations_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_data_migrations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_metrics_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_metrics_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_organizations_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_organizations_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_sso_settings_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_sso_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_ids_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_ids_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_metrics_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_metrics_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_user_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_users_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_users_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_users_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_users_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_get_users_response_all_of_users.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_users_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_list_projects.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_list_projects_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_organization_info_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_organization_info_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_toggle_data_migration_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_toggle_data_migration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_update_organization_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_update_user_permissions_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_update_user_permissions_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/admin_update_user_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/akida_edge_learning_config.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/akida_edge_learning_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_model_metadata.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_auto_segmenter_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,43 +12,44 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
+
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt
-from edgeimpulse_api.models.anomaly_model_metadata_clusters_inner import AnomalyModelMetadataClustersInner
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from edgeimpulse_api.models.get_auto_segmenter_response_all_of_clusters import GetAutoSegmenterResponseAllOfClusters
 
-class AnomalyModelMetadata(BaseModel):
-    created: datetime = Field(..., description="Date when the model was trained")
-    scale: List[float] = Field(..., description="Scale input for StandardScaler. Values are scaled like this (where `ix` is axis index): `input[ix] = (input[ix] - mean[ix]) / scale[ix];`")
-    mean: List[float] = Field(..., description="Mean input for StandardScaler. Values are scaled like this (where `ix` is axis index): `input[ix] = (input[ix] - mean[ix]) / scale[ix];`")
-    clusters: List[AnomalyModelMetadataClustersInner] = Field(..., description="Trained K-means clusters")
-    axes: List[StrictInt] = Field(..., description="Which axes were included during training (by index)")
-    default_minimum_confidence_rating: Optional[float] = Field(None, alias="defaultMinimumConfidenceRating", description="Default minimum confidence rating required before tagging as anomaly, based on scores of training data (GMM only).")
-    __properties = ["created", "scale", "mean", "clusters", "axes", "defaultMinimumConfidenceRating"]
+class GetAutoSegmenterResponse(BaseModel):
+    success: StrictBool = Field(..., description="Whether the operation succeeded")
+    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+    has_results: StrictBool = Field(..., alias="hasResults")
+    clusters: List[GetAutoSegmenterResponseAllOfClusters] = ...
+    sim_threshold: float = Field(..., alias="simThreshold")
+    min_object_size_px: StrictInt = Field(..., alias="minObjectSizePx")
+    which_items_to_include: StrictStr = Field(..., alias="whichItemsToInclude")
+    __properties = ["success", "error", "hasResults", "clusters", "simThreshold", "minObjectSizePx", "whichItemsToInclude"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AnomalyModelMetadata:
-        """Create an instance of AnomalyModelMetadata from a JSON string"""
+    def from_json(cls, json_str: str) -> GetAutoSegmenterResponse:
+        """Create an instance of GetAutoSegmenterResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -59,25 +60,26 @@
             for _item in self.clusters:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['clusters'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AnomalyModelMetadata:
-        """Create an instance of AnomalyModelMetadata from a dict"""
+    def from_dict(cls, obj: dict) -> GetAutoSegmenterResponse:
+        """Create an instance of GetAutoSegmenterResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AnomalyModelMetadata.construct(**obj)
+            return GetAutoSegmenterResponse.construct(**obj)
 
-        _obj = AnomalyModelMetadata.construct(**{
-            "created": obj.get("created"),
-            "scale": obj.get("scale"),
-            "mean": obj.get("mean"),
-            "clusters": [AnomalyModelMetadataClustersInner.from_dict(_item) for _item in obj.get("clusters")] if obj.get("clusters") is not None else None,
-            "axes": obj.get("axes"),
-            "default_minimum_confidence_rating": obj.get("defaultMinimumConfidenceRating")
+        _obj = GetAutoSegmenterResponse.construct(**{
+            "success": obj.get("success"),
+            "error": obj.get("error"),
+            "has_results": obj.get("hasResults"),
+            "clusters": [GetAutoSegmenterResponseAllOfClusters.from_dict(_item) for _item in obj.get("clusters")] if obj.get("clusters") is not None else None,
+            "sim_threshold": obj.get("simThreshold"),
+            "min_object_size_px": obj.get("minObjectSizePx"),
+            "which_items_to_include": obj.get("whichItemsToInclude")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_model_metadata_clusters_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import re  # noqa: F401
 import json
 
 
 from typing import List
 from pydantic import BaseModel, Field
 
-class AnomalyModelMetadataClustersInner(BaseModel):
+class AnomalyModelMetadataAllOfClusters(BaseModel):
     center: List[float] = Field(..., description="Center of each cluster (one value per axis)")
     max_error: float = Field(..., alias="maxError", description="Size of the cluster")
     __properties = ["center", "maxError"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
@@ -34,34 +34,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AnomalyModelMetadataClustersInner:
-        """Create an instance of AnomalyModelMetadataClustersInner from a JSON string"""
+    def from_json(cls, json_str: str) -> AnomalyModelMetadataAllOfClusters:
+        """Create an instance of AnomalyModelMetadataAllOfClusters from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AnomalyModelMetadataClustersInner:
-        """Create an instance of AnomalyModelMetadataClustersInner from a dict"""
+    def from_dict(cls, obj: dict) -> AnomalyModelMetadataAllOfClusters:
+        """Create an instance of AnomalyModelMetadataAllOfClusters from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AnomalyModelMetadataClustersInner.construct(**obj)
+            return AnomalyModelMetadataAllOfClusters.construct(**obj)
 
-        _obj = AnomalyModelMetadataClustersInner.construct(**{
+        _obj = AnomalyModelMetadataAllOfClusters.construct(**{
             "center": obj.get("center"),
             "max_error": obj.get("maxError")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_model_metadata_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,73 +15,69 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
-from edgeimpulse_api.models.anomaly_model_metadata_clusters_inner import AnomalyModelMetadataClustersInner
 
-class AnomalyModelMetadataResponse(BaseModel):
-    success: StrictBool = Field(..., description="Whether the operation succeeded")
-    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    created: datetime = Field(..., description="Date when the model was trained")
-    scale: List[float] = Field(..., description="Scale input for StandardScaler. Values are scaled like this (where `ix` is axis index): `input[ix] = (input[ix] - mean[ix]) / scale[ix];`")
-    mean: List[float] = Field(..., description="Mean input for StandardScaler. Values are scaled like this (where `ix` is axis index): `input[ix] = (input[ix] - mean[ix]) / scale[ix];`")
-    clusters: List[AnomalyModelMetadataClustersInner] = Field(..., description="Trained K-means clusters")
-    axes: List[StrictInt] = Field(..., description="Which axes were included during training (by index)")
-    default_minimum_confidence_rating: Optional[float] = Field(None, alias="defaultMinimumConfidenceRating", description="Default minimum confidence rating required before tagging as anomaly, based on scores of training data (GMM only).")
-    __properties = ["success", "error", "created", "scale", "mean", "clusters", "axes", "defaultMinimumConfidenceRating"]
+class Job(BaseModel):
+    id: StrictInt = Field(..., description="Job id, use this to refer back to the job. The web socket API also uses this ID.")
+    category: StrictStr = ...
+    key: StrictStr = Field(..., description="External job identifier, this can be used to categorize jobs, and recover job status. E.g. set this to 'keras-192' for a Keras learning block with ID 192. When a user refreshes the page you can check whether a job is active for this ID and re-attach. ")
+    created: datetime = Field(..., description="When the job was created.")
+    started: Optional[datetime] = Field(None, description="When the job was started.")
+    finished: Optional[datetime] = Field(None, description="When the job was finished.")
+    finished_successful: Optional[StrictBool] = Field(None, alias="finishedSuccessful", description="Whether the job finished successfully.")
+    job_notification_uids: List[StrictInt] = Field(..., alias="jobNotificationUids", description="The IDs of users who should be notified when a job is finished.")
+    additional_info: Optional[StrictStr] = Field(None, alias="additionalInfo", description="Additional metadata associated with this job.")
+    compute_time: Optional[float] = Field(None, alias="computeTime", description="Job duration time in seconds from start to finished, measured by k8s job watcher.")
+    __properties = ["id", "category", "key", "created", "started", "finished", "finishedSuccessful", "jobNotificationUids", "additionalInfo", "computeTime"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AnomalyModelMetadataResponse:
-        """Create an instance of AnomalyModelMetadataResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> Job:
+        """Create an instance of Job from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in clusters (list)
-        _items = []
-        if self.clusters:
-            for _item in self.clusters:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['clusters'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AnomalyModelMetadataResponse:
-        """Create an instance of AnomalyModelMetadataResponse from a dict"""
+    def from_dict(cls, obj: dict) -> Job:
+        """Create an instance of Job from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AnomalyModelMetadataResponse.construct(**obj)
+            return Job.construct(**obj)
 
-        _obj = AnomalyModelMetadataResponse.construct(**{
-            "success": obj.get("success"),
-            "error": obj.get("error"),
+        _obj = Job.construct(**{
+            "id": obj.get("id"),
+            "category": obj.get("category"),
+            "key": obj.get("key"),
             "created": obj.get("created"),
-            "scale": obj.get("scale"),
-            "mean": obj.get("mean"),
-            "clusters": [AnomalyModelMetadataClustersInner.from_dict(_item) for _item in obj.get("clusters")] if obj.get("clusters") is not None else None,
-            "axes": obj.get("axes"),
-            "default_minimum_confidence_rating": obj.get("defaultMinimumConfidenceRating")
+            "started": obj.get("started"),
+            "finished": obj.get("finished"),
+            "finished_successful": obj.get("finishedSuccessful"),
+            "job_notification_uids": obj.get("jobNotificationUids"),
+            "additional_info": obj.get("additionalInfo"),
+            "compute_time": obj.get("computeTime")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_response_all_of_axes.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_response_all_of_axes.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_trained_features_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/augmentation_policy_spectrogram.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/augmentation_policy_spectrogram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/autotune_dsp_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/autotune_dsp_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/bounding_box.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/bounding_box_with_score.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/bounding_box_with_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/build_on_device_model_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/build_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/build_organization_on_device_model_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/build_organization_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/change_password_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/change_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response_page.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response_page.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_job_response_page_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_job_response_page_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_sample_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_sample_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_sample_response_classification.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_sample_response_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/classify_sample_response_classification_details.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/classify_sample_response_classification_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/convert_user_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/convert_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/count_samples_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/count_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/count_samples_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/count_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_block_version_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_block_version_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_block_version_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_block_version_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_developer_profile_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_developer_profile_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_developer_profile_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_developer_profile_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_device_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_evaluation_user_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_evaluation_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_evaluation_user_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_evaluation_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_portal_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_portal_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_portal_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_portal_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_organization_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_organization_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_pipeline_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_project_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_project_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_project_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_signed_upload_link_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_signed_upload_link_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_signed_upload_link_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_signed_upload_link_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_third_party_auth_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_third_party_auth_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_third_party_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_third_party_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_third_party_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_third_party_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_user_third_party_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_user_third_party_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_whitelabel_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_whitelabel_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/create_whitelabel_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/create_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/crop_sample_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/crop_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/crop_sample_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/crop_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/crop_sample_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/crop_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/user.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,90 +14,83 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
-from edgeimpulse_api.models.data_campaign_link import DataCampaignLink
-from edgeimpulse_api.models.data_campaign_query import DataCampaignQuery
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from edgeimpulse_api.models.permission import Permission
+from edgeimpulse_api.models.staff_info import StaffInfo
 
-class DataCampaign(BaseModel):
+class User(BaseModel):
     id: StrictInt = ...
-    data_campaign_dashboard_id: StrictInt = Field(..., alias="dataCampaignDashboardId")
-    created: datetime = ...
+    username: StrictStr = ...
     name: StrictStr = ...
-    description: StrictStr = ...
-    coordinator_uids: List[StrictInt] = Field(..., alias="coordinatorUids", description="List of user IDs that coordinate this campaign")
-    logo: Optional[StrictStr] = None
-    queries: List[DataCampaignQuery] = ...
-    links: List[DataCampaignLink] = ...
-    datasets: List[StrictStr] = ...
-    pipeline_ids: List[StrictInt] = Field(..., alias="pipelineIds")
-    project_ids: List[StrictInt] = Field(..., alias="projectIds")
-    __properties = ["id", "dataCampaignDashboardId", "created", "name", "description", "coordinatorUids", "logo", "queries", "links", "datasets", "pipelineIds", "projectIds"]
+    email: StrictStr = ...
+    photo: Optional[StrictStr] = None
+    created: datetime = ...
+    last_seen: Optional[datetime] = Field(None, alias="lastSeen")
+    staff_info: StaffInfo = Field(..., alias="staffInfo")
+    pending: StrictBool = ...
+    last_tos_acceptance_date: Optional[datetime] = Field(None, alias="lastTosAcceptanceDate")
+    job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
+    permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
+    company_name: Optional[StrictStr] = Field(None, alias="companyName")
+    activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DataCampaign:
-        """Create an instance of DataCampaign from a JSON string"""
+    def from_json(cls, json_str: str) -> User:
+        """Create an instance of User from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in queries (list)
-        _items = []
-        if self.queries:
-            for _item in self.queries:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['queries'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in links (list)
-        _items = []
-        if self.links:
-            for _item in self.links:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['links'] = _items
+        # override the default output from pydantic by calling `to_dict()` of staff_info
+        if self.staff_info:
+            _dict['staffInfo'] = self.staff_info.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DataCampaign:
-        """Create an instance of DataCampaign from a dict"""
+    def from_dict(cls, obj: dict) -> User:
+        """Create an instance of User from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return DataCampaign.construct(**obj)
+            return User.construct(**obj)
 
-        _obj = DataCampaign.construct(**{
+        _obj = User.construct(**{
             "id": obj.get("id"),
-            "data_campaign_dashboard_id": obj.get("dataCampaignDashboardId"),
-            "created": obj.get("created"),
+            "username": obj.get("username"),
             "name": obj.get("name"),
-            "description": obj.get("description"),
-            "coordinator_uids": obj.get("coordinatorUids"),
-            "logo": obj.get("logo"),
-            "queries": [DataCampaignQuery.from_dict(_item) for _item in obj.get("queries")] if obj.get("queries") is not None else None,
-            "links": [DataCampaignLink.from_dict(_item) for _item in obj.get("links")] if obj.get("links") is not None else None,
-            "datasets": obj.get("datasets"),
-            "pipeline_ids": obj.get("pipelineIds"),
-            "project_ids": obj.get("projectIds")
+            "email": obj.get("email"),
+            "photo": obj.get("photo"),
+            "created": obj.get("created"),
+            "last_seen": obj.get("lastSeen"),
+            "staff_info": StaffInfo.from_dict(obj.get("staffInfo")) if obj.get("staffInfo") is not None else None,
+            "pending": obj.get("pending"),
+            "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
+            "job_title": obj.get("jobTitle"),
+            "permissions": obj.get("permissions"),
+            "company_name": obj.get("companyName"),
+            "activated": obj.get("activated")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_dashboard.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_dashboard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_graph.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_link.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_link.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_campaign_query.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_campaign_query.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_explorer_predictions_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_explorer_predictions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/data_explorer_settings.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/data_explorer_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dataset_ratio_data.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dataset_ratio_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dataset_ratio_data_ratio.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dataset_ratio_data_ratio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/delete_portal_file_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/delete_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dependency_data.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dependency_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_input_image.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_input_image.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_input_other.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_input_other.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deployment_target.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deployment_target_badge.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deployment_target_badge.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deployment_target_engine.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deployment_target_engine.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deployment_targets_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/deployment_targets_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/development_board.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/development_board.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/development_boards_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/development_boards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/development_boards_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/development_boards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/development_keys.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/development_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/development_keys_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/development_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/device.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/device_name_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/device_name_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/device_name_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/device_name_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/device_sensors_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/device_sensors_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/download.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/download.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/download_portal_file_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/download_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/download_portal_file_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/download_portal_file_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/download_portal_file_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/download_portal_file_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_autotuner_results.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_autotuner_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_autotuner_results_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_autotuner_results_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_block.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_config_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_config_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_config_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_config_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_importance_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_importance_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_labels_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_labels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_group.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_group.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_group_item.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_group_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_group_item_select_options_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_group_item_select_options_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_group_item_show_if.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_group_item_show_if.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_info.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_info_features.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_info_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_info_performance.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_info_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_metadata.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_metadata_output_config.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_metadata_output_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_metadata_output_config_shape.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_metadata_output_config_shape.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_metadata_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_performance_all_variants_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_performance_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_graph.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_graph_axis_labels.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_graph_axis_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_request_with_features.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_request_with_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_request_without_features.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_request_without_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_response_all_of_performance.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_response_with_sample.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_response_with_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_sample_features_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_sample_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_sample_features_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_sample_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_trained_features_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_trained_features_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/edit_sample_label_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/edit_sample_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/entitlement_limits.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/entitlement_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/evaluate_job_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/evaluate_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/evaluate_job_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/evaluate_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/evaluate_result_value.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/evaluate_result_value.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/export_get_url_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/export_get_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/export_get_url_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/export_get_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/export_keras_block_data_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/export_keras_block_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/export_original_data_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/export_original_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/export_wav_data_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/export_wav_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_segment_sample_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_segment_sample_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_segment_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_segment_sample_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_segment_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_user_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_user_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/find_user_response_all_of_users.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/find_user_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/generate_features_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/generate_features_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/generic_api_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/generic_api_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_imported_from_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_imported_from_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_imported_from_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_imported_from_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_third_party_auth_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_whitelabels_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_whitelabels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_auto_segmenter_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_portal_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,73 +13,61 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
-from edgeimpulse_api.models.get_auto_segmenter_response_all_of_clusters import GetAutoSegmenterResponseAllOfClusters
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class GetAutoSegmenterResponse(BaseModel):
+class UpdateOrganizationPortalResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    has_results: StrictBool = Field(..., alias="hasResults")
-    clusters: List[GetAutoSegmenterResponseAllOfClusters] = ...
-    sim_threshold: float = Field(..., alias="simThreshold")
-    min_object_size_px: StrictInt = Field(..., alias="minObjectSizePx")
-    which_items_to_include: StrictStr = Field(..., alias="whichItemsToInclude")
-    __properties = ["success", "error", "hasResults", "clusters", "simThreshold", "minObjectSizePx", "whichItemsToInclude"]
+    url: StrictStr = Field(..., description="URL to the portal")
+    signed_url: Optional[StrictStr] = Field(None, alias="signedUrl", description="pre-signed upload URL, only set if not using the Edge Impulse hosted bucket.")
+    bucket_bucket: Optional[StrictStr] = Field(None, alias="bucketBucket", description="Only set if not using the Edge Impulse hosted bucket.")
+    __properties = ["success", "error", "url", "signedUrl", "bucketBucket"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GetAutoSegmenterResponse:
-        """Create an instance of GetAutoSegmenterResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateOrganizationPortalResponse:
+        """Create an instance of UpdateOrganizationPortalResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in clusters (list)
-        _items = []
-        if self.clusters:
-            for _item in self.clusters:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['clusters'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetAutoSegmenterResponse:
-        """Create an instance of GetAutoSegmenterResponse from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateOrganizationPortalResponse:
+        """Create an instance of UpdateOrganizationPortalResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return GetAutoSegmenterResponse.construct(**obj)
+            return UpdateOrganizationPortalResponse.construct(**obj)
 
-        _obj = GetAutoSegmenterResponse.construct(**{
+        _obj = UpdateOrganizationPortalResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
-            "has_results": obj.get("hasResults"),
-            "clusters": [GetAutoSegmenterResponseAllOfClusters.from_dict(_item) for _item in obj.get("clusters")] if obj.get("clusters") is not None else None,
-            "sim_threshold": obj.get("simThreshold"),
-            "min_object_size_px": obj.get("minObjectSizePx"),
-            "which_items_to_include": obj.get("whichItemsToInclude")
+            "url": obj.get("url"),
+            "signed_url": obj.get("signedUrl"),
+            "bucket_bucket": obj.get("bucketBucket")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_data_explorer_features_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_data_explorer_settings_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_data_explorer_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_deployment_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_deployment_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_deployment_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_deployment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_device_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_device_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_device_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_device_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_impulse_blocks_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_impulse_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_impulse_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_impulse_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_impulse_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_impulse_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_job_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_job_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_jwt_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_jwt_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_jwt_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_jwt_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_jwt_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_jwt_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_last_deployment_build_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_last_deployment_build_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_notes_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_notes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_notes_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_notes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaign_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaigns_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaigns_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_item_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_item_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_item_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_dataset_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_dataset_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_dataset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_pipelines_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_portal_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_portal_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_organization_projects_data_count_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_organization_projects_data_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_parameters_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_status_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_pretrained_model_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_public_metrics_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_public_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_public_metrics_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_public_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_sample_metadata_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_sample_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_sample_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_syntiant_posterior_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_syntiant_posterior_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_theme_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_theme_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_theme_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_theme_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_themes_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_themes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_themes_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_themes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_third_party_auth_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_user_need_to_set_password_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_user_need_to_set_password_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_user_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_user_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_whitelabel_domain_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_whitelabel_domain_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_whitelabel_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/get_whitelabel_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/get_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/has_data_explorer_features_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/has_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/image_input_scaling.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/image_input_scaling.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse_block_version.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse_block_version.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse_dsp_block.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse_dsp_block_organization.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse_dsp_block_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse_input_block.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse_input_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     description: Optional[StrictStr] = Field(None, description="A short description of the block version, displayed in the block versioning UI")
     created_by: Optional[StrictStr] = Field(None, alias="createdBy", description="The system component that created the block version (createImpulse | clone | tuner). Cannot be set via API.")
     created_at: Optional[datetime] = Field(None, alias="createdAt", description="The datetime that the block version was created. Cannot be set via API.")
     __properties = ["id", "type", "name", "title", "windowSizeMs", "windowIncreaseMs", "frequencyHz", "classificationWindowIncreaseMs", "padZeros", "imageWidth", "imageHeight", "resizeMode", "resizeMethod", "cropAnchor", "primaryVersion", "baseBlockId", "tunerBaseBlockId", "tunerTemplateId", "tunerPrimary", "clonedFromBlockId", "mutated", "enabled", "db", "description", "createdBy", "createdAt"]
 
     @validator('type')
     def type_validate_enum(cls, v):
-        if v not in ('time-series', 'image', 'video'):
-            raise ValueError("must validate the enum values ('time-series', 'image', 'video')")
+        if v not in ('time-series', 'image'):
+            raise ValueError("must validate the enum values ('time-series', 'image')")
         return v
 
     @validator('resize_mode')
     def resize_mode_validate_enum(cls, v):
         if v is None:
             return v
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/impulse_learn_block.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/impulse_learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/input_block.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/input_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     description: StrictStr = ...
     name: StrictStr = ...
     recommended: Optional[StrictBool] = None
     __properties = ["type", "title", "author", "description", "name", "recommended"]
 
     @validator('type')
     def type_validate_enum(cls, v):
-        if v not in ('time-series', 'image', 'video'):
-            raise ValueError("must validate the enum values ('time-series', 'image', 'video')")
+        if v not in ('time-series', 'image'):
+            raise ValueError("must validate the enum values ('time-series', 'image')")
         return v
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/invite_organization_member_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/invite_organization_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_details.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,71 +13,85 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from edgeimpulse_api.models.job_state import JobState
 
-class Job(BaseModel):
+class JobDetails(BaseModel):
     id: StrictInt = Field(..., description="Job id, use this to refer back to the job. The web socket API also uses this ID.")
     category: StrictStr = ...
     key: StrictStr = Field(..., description="External job identifier, this can be used to categorize jobs, and recover job status. E.g. set this to 'keras-192' for a Keras learning block with ID 192. When a user refreshes the page you can check whether a job is active for this ID and re-attach. ")
     created: datetime = Field(..., description="When the job was created.")
     started: Optional[datetime] = Field(None, description="When the job was started.")
     finished: Optional[datetime] = Field(None, description="When the job was finished.")
     finished_successful: Optional[StrictBool] = Field(None, alias="finishedSuccessful", description="Whether the job finished successfully.")
     job_notification_uids: List[StrictInt] = Field(..., alias="jobNotificationUids", description="The IDs of users who should be notified when a job is finished.")
     additional_info: Optional[StrictStr] = Field(None, alias="additionalInfo", description="Additional metadata associated with this job.")
     compute_time: Optional[float] = Field(None, alias="computeTime", description="Job duration time in seconds from start to finished, measured by k8s job watcher.")
-    __properties = ["id", "category", "key", "created", "started", "finished", "finishedSuccessful", "jobNotificationUids", "additionalInfo", "computeTime"]
+    children_ids: Optional[List[StrictInt]] = Field(None, alias="childrenIds", description="List of jobs children isd triggered by this job")
+    states: List[JobState] = Field(..., description="List of states the job went through")
+    spec: Optional[Dict[str, Any]] = Field(None, description="Job specification (Kubernetes specification or other underlying engine)")
+    __properties = ["id", "category", "key", "created", "started", "finished", "finishedSuccessful", "jobNotificationUids", "additionalInfo", "computeTime", "childrenIds", "states", "spec"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Job:
-        """Create an instance of Job from a JSON string"""
+    def from_json(cls, json_str: str) -> JobDetails:
+        """Create an instance of JobDetails from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in states (list)
+        _items = []
+        if self.states:
+            for _item in self.states:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['states'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Job:
-        """Create an instance of Job from a dict"""
+    def from_dict(cls, obj: dict) -> JobDetails:
+        """Create an instance of JobDetails from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return Job.construct(**obj)
+            return JobDetails.construct(**obj)
 
-        _obj = Job.construct(**{
+        _obj = JobDetails.construct(**{
             "id": obj.get("id"),
             "category": obj.get("category"),
             "key": obj.get("key"),
             "created": obj.get("created"),
             "started": obj.get("started"),
             "finished": obj.get("finished"),
             "finished_successful": obj.get("finishedSuccessful"),
             "job_notification_uids": obj.get("jobNotificationUids"),
             "additional_info": obj.get("additionalInfo"),
-            "compute_time": obj.get("computeTime")
+            "compute_time": obj.get("computeTime"),
+            "children_ids": obj.get("childrenIds"),
+            "states": [JobState.from_dict(_item) for _item in obj.get("states")] if obj.get("states") is not None else None,
+            "spec": obj.get("spec")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_details_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_details_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_details_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_details_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_details_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_details_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_failure_details.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_failure_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_logs_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_logs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_logs_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_logs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_metrics_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_metrics_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_parent_type_enum.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_parent_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_state.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_state.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_state_execution_details.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_state_execution_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_step.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_summary_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_summary_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/job_summary_response_all_of_summary.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/job_summary_response_all_of_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_layer.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_layer_input.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_layer_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_layer_output.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_layer_output.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_metadata.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_metadata_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_metadata_metrics.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_metadata_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_model_type_enum.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_model_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_visual_layer.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_visual_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/keras_visual_layer_type.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/keras_visual_layer_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/last_modification_date_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/last_modification_date_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/last_modification_date_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/last_modification_date_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/latency_device.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/latency_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/learn_block.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/learn_block_type.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/learn_block_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_api_keys_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_api_keys_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_devices_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_devices_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_devices_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_devices_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_email_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_email_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_email_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_email_response_all_of_emails.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_email_response_all_of_emails.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_hmac_keys_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_hmac_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_hmac_keys_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_hmac_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_jobs_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_jobs_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_models_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_models_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_api_keys_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_user_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_data_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_data_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_data_response_all_of_data.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_deploy_blocks_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_deploy_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_dsp_blocks_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_dsp_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_files_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_files_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_files_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_files_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_pipelines_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_portals_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_portals_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_portals_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_portals_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_projects_data_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_projects_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_projects_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_projects_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_secrets_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_secrets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_secrets_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_secrets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organizations_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_organizations_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_portal_files_in_folder_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_portal_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_portal_files_in_folder_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_portal_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_projects.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_projects_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_public_projects.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_public_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_public_projects_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_public_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_public_versions_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_public_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_public_versions_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_public_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_samples_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_samples_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_versions_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_versions_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_versions_response_all_of_bucket.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_versions_response_all_of_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/list_versions_response_all_of_versions.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/list_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/log_stdout_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/log_stdout_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/log_stdout_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/log_stdout_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/log_website_pageview_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/log_website_pageview_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/login_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/login_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/login_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/login_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/migration.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/migration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/model_prediction.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/model_prediction.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/model_result.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/model_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/model_variant_stats.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/model_variant_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/move_raw_data_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/move_raw_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/note.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/note.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_auto_label_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_auto_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_auto_label_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_auto_label_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_label_queue_count_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_label_queue_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_label_queue_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_label_queue_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/object_detection_last_layer.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/object_detection_last_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_config.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_config_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_config_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_config_target_device.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_config_target_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_dsp_parameters_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_dsp_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_space_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_space_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_space_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_space_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_state_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_state_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_state_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_state_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_state_response_all_of_status.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_state_response_all_of_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_state_response_all_of_workers.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_state_response_all_of_workers.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_transfer_learning_models_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_transfer_learning_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from edgeimpulse_api.models.transfer_learning_model import TransferLearningModel
 
 class OptimizeTransferLearningModelsResponseAllOfModels(BaseModel):
     image: List[TransferLearningModel] = ...
-    object_detection: List[TransferLearningModel] = ...
+    object_detection: List[TransferLearningModel] = Field(..., alias="objectDetection")
     kws: List[TransferLearningModel] = ...
     regression: List[TransferLearningModel] = ...
     classification: List[TransferLearningModel] = ...
-    __properties = ["image", "object_detection", "kws", "regression", "classification"]
+    __properties = ["image", "objectDetection", "kws", "regression", "classification"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -61,15 +61,15 @@
             _dict['image'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in object_detection (list)
         _items = []
         if self.object_detection:
             for _item in self.object_detection:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['object_detection'] = _items
+            _dict['objectDetection'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in kws (list)
         _items = []
         if self.kws:
             for _item in self.kws:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['kws'] = _items
@@ -96,14 +96,14 @@
             return None
 
         if type(obj) is not dict:
             return OptimizeTransferLearningModelsResponseAllOfModels.construct(**obj)
 
         _obj = OptimizeTransferLearningModelsResponseAllOfModels.construct(**{
             "image": [TransferLearningModel.from_dict(_item) for _item in obj.get("image")] if obj.get("image") is not None else None,
-            "object_detection": [TransferLearningModel.from_dict(_item) for _item in obj.get("object_detection")] if obj.get("object_detection") is not None else None,
+            "object_detection": [TransferLearningModel.from_dict(_item) for _item in obj.get("objectDetection")] if obj.get("objectDetection") is not None else None,
             "kws": [TransferLearningModel.from_dict(_item) for _item in obj.get("kws")] if obj.get("kws") is not None else None,
             "regression": [TransferLearningModel.from_dict(_item) for _item in obj.get("regression")] if obj.get("regression") is not None else None,
             "classification": [TransferLearningModel.from_dict(_item) for _item in obj.get("classification")] if obj.get("classification") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/user_organization.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,88 +12,76 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import List, Optional
+from datetime import datetime
+from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
-from edgeimpulse_api.models.organization_user import OrganizationUser
-from edgeimpulse_api.models.project import Project
 
-class Organization(BaseModel):
+class UserOrganization(BaseModel):
     id: StrictInt = ...
-    name: StrictStr = Field(..., description="EdgeImpulse Inc.")
+    name: StrictStr = ...
     logo: Optional[StrictStr] = None
-    header_img: Optional[StrictStr] = Field(None, alias="headerImg")
-    users: List[OrganizationUser] = ...
     is_developer_profile: StrictBool = Field(..., alias="isDeveloperProfile")
-    whitelabel_id: Optional[StrictInt] = Field(..., alias="whitelabelId", description="Unique identifier of the white label this organization belongs to, if any.")
-    projects: Optional[List[Project]] = None
-    __properties = ["id", "name", "logo", "headerImg", "users", "isDeveloperProfile", "whitelabelId", "projects"]
+    whitelabel_id: Optional[StrictInt] = Field(..., alias="whitelabelId", description="Unique identifier of the white label this project belongs to, if any.")
+    is_admin: StrictBool = Field(..., alias="isAdmin", description="Whether the user is admin of this organization or not.")
+    created: datetime = Field(..., description="When the organization was created.")
+    trial_id: Optional[float] = Field(..., alias="trialId", description="Unique identifier of the trial this organization belongs to, if any.")
+    __properties = ["id", "name", "logo", "isDeveloperProfile", "whitelabelId", "isAdmin", "created", "trialId"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Organization:
-        """Create an instance of Organization from a JSON string"""
+    def from_json(cls, json_str: str) -> UserOrganization:
+        """Create an instance of UserOrganization from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in users (list)
-        _items = []
-        if self.users:
-            for _item in self.users:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['users'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in projects (list)
-        _items = []
-        if self.projects:
-            for _item in self.projects:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['projects'] = _items
         # set to None if whitelabel_id (nullable) is None
         if self.whitelabel_id is None:
             _dict['whitelabelId'] = None
 
+        # set to None if trial_id (nullable) is None
+        if self.trial_id is None:
+            _dict['trialId'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Organization:
-        """Create an instance of Organization from a dict"""
+    def from_dict(cls, obj: dict) -> UserOrganization:
+        """Create an instance of UserOrganization from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return Organization.construct(**obj)
+            return UserOrganization.construct(**obj)
 
-        _obj = Organization.construct(**{
+        _obj = UserOrganization.construct(**{
             "id": obj.get("id"),
             "name": obj.get("name"),
             "logo": obj.get("logo"),
-            "header_img": obj.get("headerImg"),
-            "users": [OrganizationUser.from_dict(_item) for _item in obj.get("users")] if obj.get("users") is not None else None,
             "is_developer_profile": obj.get("isDeveloperProfile"),
             "whitelabel_id": obj.get("whitelabelId"),
-            "projects": [Project.from_dict(_item) for _item in obj.get("projects")] if obj.get("projects") is not None else None
+            "is_admin": obj.get("isAdmin"),
+            "created": obj.get("created"),
+            "trial_id": obj.get("trialId")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_add_data_folder_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_add_data_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_add_data_folder_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_add_data_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_add_dataset_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_add_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_add_dataset_request_bucket.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_add_dataset_request_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_status_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_status_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_transformation_summary.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_transformation_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_with_files.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_with_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,16 @@
     email_recipient_uids: Optional[List[StrictInt]] = Field(None, alias="emailRecipientUids")
     pipeline_id: Optional[StrictInt] = Field(None, alias="pipelineId")
     pipeline_name: Optional[StrictStr] = Field(None, alias="pipelineName")
     pipeline_run_id: Optional[StrictInt] = Field(None, alias="pipelineRunId")
     pipeline_step: Optional[StrictInt] = Field(None, alias="pipelineStep")
     operates_on: StrictStr = Field(..., alias="operatesOn")
     files: List[OrganizationCreateProjectWithFilesAllOfFiles] = ...
-    __properties = ["id", "organizationId", "name", "uploadType", "status", "transformJobStatus", "uploadJobId", "uploadJobStatus", "uploadJobFilesUploaded", "projectOwner", "projectId", "projectName", "transformationBlockId", "builtinTransformationBlock", "transformationBlockName", "category", "created", "outputDatasetName", "outputDatasetBucketId", "outputDatasetBucketPath", "totalDownloadFileCount", "totalDownloadFileSize", "totalDownloadFileSizeString", "totalUploadFileCount", "transformationParallel", "transformationSummary", "inProgress", "label", "filterQuery", "emailRecipientUids", "pipelineId", "pipelineName", "pipelineRunId", "pipelineStep", "operatesOn", "files"]
+    file_count_for_filter: StrictInt = Field(..., alias="fileCountForFilter")
+    __properties = ["id", "organizationId", "name", "uploadType", "status", "transformJobStatus", "uploadJobId", "uploadJobStatus", "uploadJobFilesUploaded", "projectOwner", "projectId", "projectName", "transformationBlockId", "builtinTransformationBlock", "transformationBlockName", "category", "created", "outputDatasetName", "outputDatasetBucketId", "outputDatasetBucketPath", "totalDownloadFileCount", "totalDownloadFileSize", "totalDownloadFileSizeString", "totalUploadFileCount", "transformationParallel", "transformationSummary", "inProgress", "label", "filterQuery", "emailRecipientUids", "pipelineId", "pipelineName", "pipelineRunId", "pipelineStep", "operatesOn", "files", "fileCountForFilter"]
 
     @validator('upload_type')
     def upload_type_validate_enum(cls, v):
         if v not in ('dataset', 'project'):
             raise ValueError("must validate the enum values ('dataset', 'project')")
         return v
 
@@ -156,11 +157,12 @@
             "filter_query": obj.get("filterQuery"),
             "email_recipient_uids": obj.get("emailRecipientUids"),
             "pipeline_id": obj.get("pipelineId"),
             "pipeline_name": obj.get("pipelineName"),
             "pipeline_run_id": obj.get("pipelineRunId"),
             "pipeline_step": obj.get("pipelineStep"),
             "operates_on": obj.get("operatesOn"),
-            "files": [OrganizationCreateProjectWithFilesAllOfFiles.from_dict(_item) for _item in obj.get("files")] if obj.get("files") is not None else None
+            "files": [OrganizationCreateProjectWithFilesAllOfFiles.from_dict(_item) for _item in obj.get("files")] if obj.get("files") is not None else None,
+            "file_count_for_filter": obj.get("fileCountForFilter")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_with_files_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_with_files_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel
+from pydantic import BaseModel, Field, StrictInt
 from edgeimpulse_api.models.organization_create_project_with_files_all_of_files import OrganizationCreateProjectWithFilesAllOfFiles
 
 class OrganizationCreateProjectWithFilesAllOf(BaseModel):
     files: List[OrganizationCreateProjectWithFilesAllOfFiles] = ...
-    __properties = ["files"]
+    file_count_for_filter: StrictInt = Field(..., alias="fileCountForFilter")
+    __properties = ["files", "fileCountForFilter"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -63,11 +64,12 @@
         if obj is None:
             return None
 
         if type(obj) is not dict:
             return OrganizationCreateProjectWithFilesAllOf.construct(**obj)
 
         _obj = OrganizationCreateProjectWithFilesAllOf.construct(**{
-            "files": [OrganizationCreateProjectWithFilesAllOfFiles.from_dict(_item) for _item in obj.get("files")] if obj.get("files") is not None else None
+            "files": [OrganizationCreateProjectWithFilesAllOfFiles.from_dict(_item) for _item in obj.get("files")] if obj.get("files") is not None else None,
+            "file_count_for_filter": obj.get("fileCountForFilter")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_campaign_diff_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_campaign_diff_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_campaign_diff_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_campaign_diff_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_item.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_data_item_files_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_data_item_files_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_dataset.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_dataset_bucket.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_dataset_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_deploy_block.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_deploy_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_dsp_block.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_get_create_projects_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_get_create_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_member_role.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_member_role.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_metrics_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_metrics_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_item_count.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_item_count.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_run.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_run_step.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_run_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_pipeline_step.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_projects_data_batch_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_projects_data_batch_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_transfer_learning_block.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_transfer_learning_block.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     object_detection_last_layer: Optional[ObjectDetectionLastLayer] = Field(None, alias="objectDetectionLastLayer")
     implementation_version: StrictInt = Field(..., alias="implementationVersion")
     is_public: StrictBool = Field(..., alias="isPublic", description="Whether this block is publicly available to Edge Impulse users (if false, then only for members of the owning organization)")
     is_public_for_devices: List[StrictStr] = Field(..., alias="isPublicForDevices", description="If `isPublic` is true, the list of devices (from latencyDevices) for which this model can be shown.")
     repository_url: Optional[StrictStr] = Field(None, alias="repositoryUrl", description="URL to the source code of this custom learn block.")
     parameters: List[Dict[str, Any]] = Field(..., description="List of parameters, spec'ed according to https://docs.edgeimpulse.com/docs/tips-and-tricks/adding-parameters-to-custom-blocks")
     image_input_scaling: Optional[ImageInputScaling] = Field(None, alias="imageInputScaling")
-    __properties = ["id", "name", "dockerContainer", "dockerContainerManagedByEdgeImpulse", "created", "description", "userId", "userName", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "repositoryUrl", "parameters", "imageInputScaling"]
+    ind_requires_gpu: StrictBool = Field(..., alias="indRequiresGpu", description="If set, requires this block to be scheduled on GPU.")
+    __properties = ["id", "name", "dockerContainer", "dockerContainerManagedByEdgeImpulse", "created", "description", "userId", "userName", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "repositoryUrl", "parameters", "imageInputScaling", "indRequiresGpu"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -88,11 +89,12 @@
             "operates_on": obj.get("operatesOn"),
             "object_detection_last_layer": obj.get("objectDetectionLastLayer"),
             "implementation_version": obj.get("implementationVersion"),
             "is_public": obj.get("isPublic"),
             "is_public_for_devices": obj.get("isPublicForDevices"),
             "repository_url": obj.get("repositoryUrl"),
             "parameters": obj.get("parameters"),
-            "image_input_scaling": obj.get("imageInputScaling")
+            "image_input_scaling": obj.get("imageInputScaling"),
+            "ind_requires_gpu": obj.get("indRequiresGpu")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_transfer_learning_operates_on.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_transfer_learning_operates_on.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_transformation_block.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_update_pipeline_body.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_update_pipeline_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_user.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/organization_user_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/organization_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_detection.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_false_positive.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_false_positive.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_ground_truth.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_ground_truth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_parameter_set.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_parameter_set.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_parameters.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_parameters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_parameters_standard.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_parameters_standard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_raw_detection.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_raw_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/permission.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/permission.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     ADMINORGANIZATIONSREAD = 'admin:organizations:read'
     ADMINORGANIZATIONSWRITE = 'admin:organizations:write'
     ADMINORGANIZATIONSMEMBERSWRITE = 'admin:organizations:members:write'
     ADMINPROJECTSMEMBERSWRITE = 'admin:projects:members:write'
     ADMINPROJECTSREAD = 'admin:projects:read'
     ADMINPROJECTSWRITE = 'admin:projects:write'
     ADMINUSERSPERMISSIONSWRITE = 'admin:users:permissions:write'
+    ADMINUSERSTRIALSWRITE = 'admin:users:trials:write'
     ADMINUSERSREAD = 'admin:users:read'
     ADMINUSERSWRITE = 'admin:users:write'
     ADMINJOBSREAD = 'admin:jobs:read'
     PROJECTSLIMITSWRITE = 'projects:limits:write'
     PROJECTSTRAININGKERASWRITE = 'projects:training:keras:write'
     THIRDPARTYAUTHREAD = 'thirdpartyauth:read'
     THIRDPARTYAUTHWRITE = 'thirdpartyauth:write'
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/portal_file.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/portal_file.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/portal_info_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/portal_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/pretrained_model_tensor.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/pretrained_model_tensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_info.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_info_memory.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_info_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_info_memory_eon.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_info_memory_eon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_info_memory_tflite.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_info_memory_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_table.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_table.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_table_mcu.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_table_mcu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_table_mcu_memory.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_table_mcu_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_model_table_mpu.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_model_table_mpu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_tf_lite_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_tf_lite_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/profile_tf_lite_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/profile_tf_lite_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_collaborator.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_collaborator.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_collaborator_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_collaborator_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_data_axes_summary_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_data_axes_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_data_interval_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_data_interval_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_data_interval_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_data_interval_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_data_summary.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_data_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_deployment_target.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_deployment_target_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_deployment_target_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_deployment_targets_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_deployment_targets_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_downloads_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_downloads_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_downloads_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_downloads_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_compute_time.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_compute_time.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_experiments.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_experiments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_impulse.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_performance.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_readme.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_response_all_of_urls.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_response_all_of_urls.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_summary_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_info_summary_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_info_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_private_data.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_private_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_public_data.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_public_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,41 +14,36 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 from edgeimpulse_api.models.project_public_data_readme import ProjectPublicDataReadme
+from edgeimpulse_api.models.project_type import ProjectType
 
 class ProjectPublicData(BaseModel):
     id: StrictInt = ...
     name: StrictStr = ...
     description: StrictStr = ...
     created: datetime = ...
     owner: StrictStr = Field(..., description="User or organization that owns the project")
     owner_avatar: Optional[StrictStr] = Field(None, alias="ownerAvatar", description="URL to the project owner avatar, if any")
     public_url: StrictStr = Field(..., alias="publicUrl", description="URL of the latest public version of the project, if any")
-    project_type: StrictStr = Field(..., alias="projectType")
+    project_type: ProjectType = Field(..., alias="projectType")
     page_view_count: StrictInt = Field(..., alias="pageViewCount")
     clone_count: StrictInt = Field(..., alias="cloneCount")
     total_samples_count: Optional[StrictStr] = Field(None, alias="totalSamplesCount")
     training_accuracy: Optional[float] = Field(None, alias="trainingAccuracy")
     test_accuracy: Optional[float] = Field(None, alias="testAccuracy")
     readme: Optional[ProjectPublicDataReadme] = None
     tags: List[StrictStr] = Field(..., description="List of project tags")
     __properties = ["id", "name", "description", "created", "owner", "ownerAvatar", "publicUrl", "projectType", "pageViewCount", "cloneCount", "totalSamplesCount", "trainingAccuracy", "testAccuracy", "readme", "tags"]
 
-    @validator('project_type')
-    def project_type_validate_enum(cls, v):
-        if v not in ('kws', 'audio', 'object-detection', 'image', 'accelerometer', 'other'):
-            raise ValueError("must validate the enum values ('kws', 'audio', 'object-detection', 'image', 'accelerometer', 'other')")
-        return v
-
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_public_data_readme.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_public_data_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_sample_metadata.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_training_data_summary_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_training_data_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_training_data_summary_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_training_data_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/project_version_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/project_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/raw_sample_data.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/raw_sample_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/raw_sample_payload.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/raw_sample_payload.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/rebalance_dataset_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/rebalance_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/remove_collaborator_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/remove_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/remove_member_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/remove_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/rename_device_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/rename_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/rename_portal_file_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/rename_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/rename_sample_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/rename_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/request_reset_password_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/request_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/reset_password_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/restore_project_from_public_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/restore_project_from_public_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/restore_project_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/restore_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/run_auto_segmenter_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/run_auto_segmenter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/run_organization_pipeline_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/run_organization_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/sample.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/sample_bounding_boxes_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/sample_bounding_boxes_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/sample_metadata.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/save_pretrained_model_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/save_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/score_trial_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/score_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/score_trial_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/score_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/score_trial_response_all_of_latency.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/score_trial_response_all_of_latency.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/score_trial_response_all_of_ram.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/score_trial_response_all_of_ram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/segment_sample_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/segment_sample_request_segments_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/segment_sample_request_segments_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/send_user_feedback_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/send_user_feedback_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/sensor.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/sensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_anomaly_parameter_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_anomaly_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_keras_parameter_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_keras_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_member_datasets_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_member_datasets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_member_role_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_member_role_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_optimize_space_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_optimize_space_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_optimize_space_request_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_optimize_space_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_organization_data_dataset_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_organization_data_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_project_compute_time_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_project_compute_time_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_project_dsp_file_size_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_project_dsp_file_size_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_sample_metadata_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_sample_metadata_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_syntiant_posterior_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_syntiant_posterior_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/set_user_password_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/set_user_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/socket_token_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/socket_token_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/socket_token_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/socket_token_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/socket_token_response_all_of_token.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/socket_token_response_all_of_token.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/split_sample_in_frames_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/split_sample_in_frames_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/staff_info.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/staff_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_job_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_job_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_performance_calibration_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_performance_calibration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_sampling_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_sampling_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_sampling_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_sampling_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_sampling_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_sampling_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/start_training_request_anomaly.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/start_training_request_anomaly.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt
+from pydantic import BaseModel, Field, StrictBool, StrictInt
 
 class StartTrainingRequestAnomaly(BaseModel):
     axes: List[StrictInt] = Field(..., description="Which axes (indexes from DSP script) to include in the training set")
     cluster_count: Optional[StrictInt] = Field(None, alias="clusterCount", description="Number of clusters for K-means, or number of components for GMM")
     minimum_confidence_rating: float = Field(..., alias="minimumConfidenceRating", description="Minimum confidence rating required before tagging as anomaly")
-    __properties = ["axes", "clusterCount", "minimumConfidenceRating"]
+    skip_embeddings_and_memory: Optional[StrictBool] = Field(None, alias="skipEmbeddingsAndMemory", description="If set, skips creating embeddings and measuring memory (used in tests)")
+    __properties = ["axes", "clusterCount", "minimumConfidenceRating", "skipEmbeddingsAndMemory"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -59,11 +60,12 @@
 
         if type(obj) is not dict:
             return StartTrainingRequestAnomaly.construct(**obj)
 
         _obj = StartTrainingRequestAnomaly.construct(**{
             "axes": obj.get("axes"),
             "cluster_count": obj.get("clusterCount"),
-            "minimum_confidence_rating": obj.get("minimumConfidenceRating")
+            "minimum_confidence_rating": obj.get("minimumConfidenceRating"),
+            "skip_embeddings_and_memory": obj.get("skipEmbeddingsAndMemory")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/store_segment_length_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/store_segment_length_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/structured_classify_result.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/structured_classify_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/test_pretrained_model_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/test_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/test_pretrained_model_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/test_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/test_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/test_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/theme.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/theme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/theme_colors.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/theme_colors.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/theme_favicon.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/theme_favicon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/theme_logos.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/theme_logos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/third_party_auth.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/third_party_auth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/time_series_data_point.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/time_series_data_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/track_objects_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/track_objects_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/track_objects_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/track_objects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/track_objects_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/track_objects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/transfer_learning_model.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/transfer_ownership_organization_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/transfer_ownership_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/transformation_block_additional_mount_point.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/transformation_block_additional_mount_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/transformation_job_status_enum.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/transformation_job_status_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/tuner_create_trial_impulse.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/tuner_create_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/tuner_space_impulse.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/tuner_space_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/tuner_trial.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/tuner_trial.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,29 +16,32 @@
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 from edgeimpulse_api.models.tuner_trial_blocks_inner import TunerTrialBlocksInner
+from edgeimpulse_api.models.tuner_trial_dsp_job_id import TunerTrialDspJobId
 
 class TunerTrial(BaseModel):
     id: StrictStr = ...
     status: StrictStr = ...
     last_completed_epoch: Optional[datetime] = Field(None, alias="lastCompletedEpoch")
     last_completed_training: Optional[datetime] = Field(None, alias="lastCompletedTraining")
     retries: Optional[StrictInt] = None
     current_epoch: Optional[StrictInt] = Field(None, alias="currentEpoch")
     worker_id: Optional[StrictStr] = Field(None, alias="workerId")
     blocks: Optional[List[TunerTrialBlocksInner]] = None
     impulse: Optional[Dict[str, Any]] = None
     experiment: Optional[StrictStr] = None
     original_trial_id: Optional[StrictStr] = None
     model: Optional[Dict[str, Any]] = None
-    __properties = ["id", "status", "lastCompletedEpoch", "lastCompletedTraining", "retries", "currentEpoch", "workerId", "blocks", "impulse", "experiment", "original_trial_id", "model"]
+    dsp_job_id: Optional[TunerTrialDspJobId] = Field(None, alias="dspJobId")
+    learn_job_id: Optional[float] = Field(None, alias="learnJobId")
+    __properties = ["id", "status", "lastCompletedEpoch", "lastCompletedTraining", "retries", "currentEpoch", "workerId", "blocks", "impulse", "experiment", "original_trial_id", "model", "dspJobId", "learnJobId"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -62,14 +65,17 @@
         # override the default output from pydantic by calling `to_dict()` of each item in blocks (list)
         _items = []
         if self.blocks:
             for _item in self.blocks:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['blocks'] = _items
+        # override the default output from pydantic by calling `to_dict()` of dsp_job_id
+        if self.dsp_job_id:
+            _dict['dspJobId'] = self.dsp_job_id.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> TunerTrial:
         """Create an instance of TunerTrial from a dict"""
         if obj is None:
             return None
@@ -85,11 +91,13 @@
             "retries": obj.get("retries"),
             "current_epoch": obj.get("currentEpoch"),
             "worker_id": obj.get("workerId"),
             "blocks": [TunerTrialBlocksInner.from_dict(_item) for _item in obj.get("blocks")] if obj.get("blocks") is not None else None,
             "impulse": obj.get("impulse"),
             "experiment": obj.get("experiment"),
             "original_trial_id": obj.get("original_trial_id"),
-            "model": obj.get("model")
+            "model": obj.get("model"),
+            "dsp_job_id": TunerTrialDspJobId.from_dict(obj.get("dspJobId")) if obj.get("dspJobId") is not None else None,
+            "learn_job_id": obj.get("learnJobId")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/tuner_trial_blocks_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/tuner_trial_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_job_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_job_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_add_collaborator_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_bucket_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_create_empty_project_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_create_empty_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_create_project_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_data_campaign_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_data_item_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_data_item_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_dataset_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_dsp_block_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_portal_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_organization_bucket_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,61 +13,65 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
+from edgeimpulse_api.models.verify_organization_bucket_response_all_of_files import VerifyOrganizationBucketResponseAllOfFiles
 
-class UpdateOrganizationPortalResponse(BaseModel):
+class VerifyOrganizationBucketResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    url: StrictStr = Field(..., description="URL to the portal")
-    signed_url: Optional[StrictStr] = Field(None, alias="signedUrl", description="pre-signed upload URL, only set if not using the Edge Impulse hosted bucket.")
-    bucket_bucket: Optional[StrictStr] = Field(None, alias="bucketBucket", description="Only set if not using the Edge Impulse hosted bucket.")
-    __properties = ["success", "error", "url", "signedUrl", "bucketBucket"]
+    files: List[VerifyOrganizationBucketResponseAllOfFiles] = Field(..., description="20 random files from the bucket.")
+    __properties = ["success", "error", "files"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateOrganizationPortalResponse:
-        """Create an instance of UpdateOrganizationPortalResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyOrganizationBucketResponse:
+        """Create an instance of VerifyOrganizationBucketResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in files (list)
+        _items = []
+        if self.files:
+            for _item in self.files:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['files'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateOrganizationPortalResponse:
-        """Create an instance of UpdateOrganizationPortalResponse from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketResponse:
+        """Create an instance of VerifyOrganizationBucketResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UpdateOrganizationPortalResponse.construct(**obj)
+            return VerifyOrganizationBucketResponse.construct(**obj)
 
-        _obj = UpdateOrganizationPortalResponse.construct(**{
+        _obj = VerifyOrganizationBucketResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
-            "url": obj.get("url"),
-            "signed_url": obj.get("signedUrl"),
-            "bucket_bucket": obj.get("bucketBucket")
+            "files": [VerifyOrganizationBucketResponseAllOfFiles.from_dict(_item) for _item in obj.get("files")] if obj.get("files") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_portal_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     object_detection_last_layer: Optional[ObjectDetectionLastLayer] = Field(None, alias="objectDetectionLastLayer")
     implementation_version: Optional[StrictInt] = Field(None, alias="implementationVersion")
     is_public: Optional[StrictBool] = Field(None, alias="isPublic", description="Whether this block is publicly available to Edge Impulse users (if false, then only for members of the owning organization)")
     is_public_for_devices: Optional[List[StrictStr]] = Field(None, alias="isPublicForDevices", description="If `isPublic` is true, the list of devices (from latencyDevices) for which this model can be shown.")
     repository_url: Optional[StrictStr] = Field(None, alias="repositoryUrl", description="URL to the source code of this custom learn block.")
     parameters: Optional[List[Dict[str, Any]]] = Field(None, description="List of parameters, spec'ed according to https://docs.edgeimpulse.com/docs/tips-and-tricks/adding-parameters-to-custom-blocks")
     image_input_scaling: Optional[ImageInputScaling] = Field(None, alias="imageInputScaling")
-    __properties = ["name", "dockerContainer", "description", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "repositoryUrl", "parameters", "imageInputScaling"]
+    ind_requires_gpu: Optional[StrictBool] = Field(None, alias="indRequiresGpu", description="If set, requires this block to be scheduled on GPU.")
+    __properties = ["name", "dockerContainer", "description", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "repositoryUrl", "parameters", "imageInputScaling", "indRequiresGpu"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -78,11 +79,12 @@
             "operates_on": obj.get("operatesOn"),
             "object_detection_last_layer": obj.get("objectDetectionLastLayer"),
             "implementation_version": obj.get("implementationVersion"),
             "is_public": obj.get("isPublic"),
             "is_public_for_devices": obj.get("isPublicForDevices"),
             "repository_url": obj.get("repositoryUrl"),
             "parameters": obj.get("parameters"),
-            "image_input_scaling": obj.get("imageInputScaling")
+            "image_input_scaling": obj.get("imageInputScaling"),
+            "ind_requires_gpu": obj.get("indRequiresGpu")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_organization_transformation_block_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_project_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_project_tags_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_project_tags_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_theme_colors_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_theme_colors_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_theme_logos_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_theme_logos_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_third_party_auth_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_user_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_version_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/upload_asset_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/upload_asset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/upload_asset_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/upload_asset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/upload_readme_image_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/upload_readme_image_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/upload_user_photo_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/upload_user_photo_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/upload_user_photo_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/upload_user_photo_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/user.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/enterprise_trial.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,84 +13,75 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
-from edgeimpulse_api.models.permission import Permission
-from edgeimpulse_api.models.staff_info import StaffInfo
-
-class User(BaseModel):
-    id: StrictInt = ...
-    username: StrictStr = ...
-    name: StrictStr = ...
-    email: StrictStr = ...
-    photo: Optional[StrictStr] = None
-    created: datetime = ...
-    last_seen: Optional[datetime] = Field(None, alias="lastSeen")
-    staff_info: StaffInfo = Field(..., alias="staffInfo")
-    pending: StrictBool = ...
-    last_tos_acceptance_date: Optional[datetime] = Field(None, alias="lastTosAcceptanceDate")
-    job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
-    permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
-    company_name: Optional[StrictStr] = Field(None, alias="companyName")
-    activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated"]
+from typing import Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr
+
+class EnterpriseTrial(BaseModel):
+    id: StrictInt = Field(..., description="Unique identifier of the trial.")
+    user_id: StrictInt = Field(..., alias="userId", description="ID of the user who created the trial.")
+    organization_id: StrictInt = Field(..., alias="organizationId", description="ID of the organization created for the trial.")
+    created: datetime = Field(..., description="Date when the trial was created. Trials start immediately on creation.")
+    expiration_date: datetime = Field(..., alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization.")
+    notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text.")
+    expired_date: Optional[datetime] = Field(..., alias="expiredDate", description="Date when the trial actually expired. This is set when the trial is expired by the system.")
+    deleted_date: Optional[datetime] = Field(..., alias="deletedDate", description="Date when the trial was deleted. This is set when the trial is fully  deleted by the system.")
+    __properties = ["id", "userId", "organizationId", "created", "expirationDate", "notes", "expiredDate", "deletedDate"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> User:
-        """Create an instance of User from a JSON string"""
+    def from_json(cls, json_str: str) -> EnterpriseTrial:
+        """Create an instance of EnterpriseTrial from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of staff_info
-        if self.staff_info:
-            _dict['staffInfo'] = self.staff_info.to_dict()
+        # set to None if expired_date (nullable) is None
+        if self.expired_date is None:
+            _dict['expiredDate'] = None
+
+        # set to None if deleted_date (nullable) is None
+        if self.deleted_date is None:
+            _dict['deletedDate'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> User:
-        """Create an instance of User from a dict"""
+    def from_dict(cls, obj: dict) -> EnterpriseTrial:
+        """Create an instance of EnterpriseTrial from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return User.construct(**obj)
+            return EnterpriseTrial.construct(**obj)
 
-        _obj = User.construct(**{
+        _obj = EnterpriseTrial.construct(**{
             "id": obj.get("id"),
-            "username": obj.get("username"),
-            "name": obj.get("name"),
-            "email": obj.get("email"),
-            "photo": obj.get("photo"),
+            "user_id": obj.get("userId"),
+            "organization_id": obj.get("organizationId"),
             "created": obj.get("created"),
-            "last_seen": obj.get("lastSeen"),
-            "staff_info": StaffInfo.from_dict(obj.get("staffInfo")) if obj.get("staffInfo") is not None else None,
-            "pending": obj.get("pending"),
-            "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
-            "job_title": obj.get("jobTitle"),
-            "permissions": obj.get("permissions"),
-            "company_name": obj.get("companyName"),
-            "activated": obj.get("activated")
+            "expiration_date": obj.get("expirationDate"),
+            "notes": obj.get("notes"),
+            "expired_date": obj.get("expiredDate"),
+            "deleted_date": obj.get("deletedDate")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/user_by_third_party_activation_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/user_by_third_party_activation_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/user_experiment.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/user_experiment.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/user_organization.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_create_user_trial_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,68 +12,58 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
-class UserOrganization(BaseModel):
-    id: StrictInt = ...
-    name: StrictStr = ...
-    logo: Optional[StrictStr] = None
-    is_developer_profile: StrictBool = Field(..., alias="isDeveloperProfile")
-    whitelabel_id: Optional[StrictInt] = Field(..., alias="whitelabelId", description="Unique identifier of the white label this project belongs to, if any.")
-    is_admin: StrictBool = Field(..., alias="isAdmin", description="Whether the user is admin of this organization or not.")
-    __properties = ["id", "name", "logo", "isDeveloperProfile", "whitelabelId", "isAdmin"]
+class AdminCreateUserTrialRequest(BaseModel):
+    organization_name: Optional[StrictStr] = Field(None, alias="organizationName", description="Name of the trial organization. All enterprise features are tied to an organization. This organization will be deleted after the trial ends. If no organization name is provided, the user's name will be used.")
+    expiration_date: datetime = Field(..., alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization.")
+    notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text.")
+    __properties = ["organizationName", "expirationDate", "notes"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserOrganization:
-        """Create an instance of UserOrganization from a JSON string"""
+    def from_json(cls, json_str: str) -> AdminCreateUserTrialRequest:
+        """Create an instance of AdminCreateUserTrialRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if whitelabel_id (nullable) is None
-        if self.whitelabel_id is None:
-            _dict['whitelabelId'] = None
-
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UserOrganization:
-        """Create an instance of UserOrganization from a dict"""
+    def from_dict(cls, obj: dict) -> AdminCreateUserTrialRequest:
+        """Create an instance of AdminCreateUserTrialRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UserOrganization.construct(**obj)
+            return AdminCreateUserTrialRequest.construct(**obj)
 
-        _obj = UserOrganization.construct(**{
-            "id": obj.get("id"),
-            "name": obj.get("name"),
-            "logo": obj.get("logo"),
-            "is_developer_profile": obj.get("isDeveloperProfile"),
-            "whitelabel_id": obj.get("whitelabelId"),
-            "is_admin": obj.get("isAdmin")
+        _obj = AdminCreateUserTrialRequest.construct(**{
+            "organization_name": obj.get("organizationName"),
+            "expiration_date": obj.get("expirationDate"),
+            "notes": obj.get("notes")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_dsp_block_url_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_dsp_block_url_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_dsp_block_url_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_dsp_block_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_organization_bucket_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_organization_bucket_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/admin_get_user_trial_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,65 +13,61 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
-from edgeimpulse_api.models.verify_organization_bucket_response_all_of_files import VerifyOrganizationBucketResponseAllOfFiles
+from edgeimpulse_api.models.enterprise_trial import EnterpriseTrial
 
-class VerifyOrganizationBucketResponse(BaseModel):
+class AdminGetUserTrialResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    files: List[VerifyOrganizationBucketResponseAllOfFiles] = Field(..., description="20 random files from the bucket.")
-    __properties = ["success", "error", "files"]
+    trial: EnterpriseTrial = ...
+    __properties = ["success", "error", "trial"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyOrganizationBucketResponse:
-        """Create an instance of VerifyOrganizationBucketResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> AdminGetUserTrialResponse:
+        """Create an instance of AdminGetUserTrialResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in files (list)
-        _items = []
-        if self.files:
-            for _item in self.files:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['files'] = _items
+        # override the default output from pydantic by calling `to_dict()` of trial
+        if self.trial:
+            _dict['trial'] = self.trial.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketResponse:
-        """Create an instance of VerifyOrganizationBucketResponse from a dict"""
+    def from_dict(cls, obj: dict) -> AdminGetUserTrialResponse:
+        """Create an instance of AdminGetUserTrialResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyOrganizationBucketResponse.construct(**obj)
+            return AdminGetUserTrialResponse.construct(**obj)
 
-        _obj = VerifyOrganizationBucketResponse.construct(**{
+        _obj = AdminGetUserTrialResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
-            "files": [VerifyOrganizationBucketResponseAllOfFiles.from_dict(_item) for _item in obj.get("files")] if obj.get("files") is not None else None
+            "trial": EnterpriseTrial.from_dict(obj.get("trial")) if obj.get("trial") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/verify_reset_password_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/verify_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/whitelabel.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/whitelabel.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from edgeimpulse_api.models.project_type import ProjectType
 from edgeimpulse_api.models.theme import Theme
 from edgeimpulse_api.models.whitelabel_custom_deployment_blocks_inner import WhitelabelCustomDeploymentBlocksInner
 
 class Whitelabel(BaseModel):
     id: StrictInt = ...
     name: StrictStr = ...
     domain: StrictStr = ...
@@ -35,15 +36,16 @@
     all_deployment_targets: Optional[List[StrictStr]] = Field(None, alias="allDeploymentTargets", description="List of all supported deployment targets")
     custom_deployment_blocks: Optional[List[WhitelabelCustomDeploymentBlocksInner]] = Field(None, alias="customDeploymentBlocks", description="List of custom deployment blocks available to this white label")
     deployment_options_order: Optional[List[StrictStr]] = Field(None, alias="deploymentOptionsOrder", description="Optional attribute allowing a whitelabel to customize the order of deployment options in the deployment view, given as an in-order list of deployment options.")
     allow_signup: StrictBool = Field(..., alias="allowSignup")
     allow_free_projects: StrictBool = Field(..., alias="allowFreeProjects")
     expose_public_projects: Optional[StrictBool] = Field(None, alias="exposePublicProjects")
     default_deployment_target: Optional[StrictStr] = Field(None, alias="defaultDeploymentTarget", description="The name of the default deployment target for this white label")
-    __properties = ["id", "name", "domain", "ownerOrganizationId", "themeId", "theme", "identityProviders", "allowPasswordAuth", "deploymentTargets", "allDeploymentTargets", "customDeploymentBlocks", "deploymentOptionsOrder", "allowSignup", "allowFreeProjects", "exposePublicProjects", "defaultDeploymentTarget"]
+    supported_project_types: List[ProjectType] = Field(..., alias="supportedProjectTypes")
+    __properties = ["id", "name", "domain", "ownerOrganizationId", "themeId", "theme", "identityProviders", "allowPasswordAuth", "deploymentTargets", "allDeploymentTargets", "customDeploymentBlocks", "deploymentOptionsOrder", "allowSignup", "allowFreeProjects", "exposePublicProjects", "defaultDeploymentTarget", "supportedProjectTypes"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -101,11 +103,12 @@
             "deployment_targets": obj.get("deploymentTargets"),
             "all_deployment_targets": obj.get("allDeploymentTargets"),
             "custom_deployment_blocks": [WhitelabelCustomDeploymentBlocksInner.from_dict(_item) for _item in obj.get("customDeploymentBlocks")] if obj.get("customDeploymentBlocks") is not None else None,
             "deployment_options_order": obj.get("deploymentOptionsOrder"),
             "allow_signup": obj.get("allowSignup"),
             "allow_free_projects": obj.get("allowFreeProjects"),
             "expose_public_projects": obj.get("exposePublicProjects"),
-            "default_deployment_target": obj.get("defaultDeploymentTarget")
+            "default_deployment_target": obj.get("defaultDeploymentTarget"),
+            "supported_project_types": obj.get("supportedProjectTypes")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/window_settings_response.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/window_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/window_settings_response_all_of.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/window_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/edgeimpulse_api/rest.py` & `edgeimpulse_api-1.25.31/edgeimpulse_api/rest.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.25.16/pyproject.toml` & `edgeimpulse_api-1.25.31/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "edgeimpulse-api"
-version = "1.25.16" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+version = "1.25.31" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 description = "Python bindings for the Edge Impulse API."
 authors = ["EdgeImpulse Inc. <hello@edgeimpulse.com>"]
 license = "Apache-2.0"
 homepage = "https://edgeimpulse.com"
 documentation = "https://docs.edgeimpulse.com/reference/edge-impulse-api/edge-impulse-api"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Embedded Systems"
 ]
 packages = [{include = "edgeimpulse_api"}]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-python_dateutil = ">= 2.5.3"
-urllib3 = ">= 1.25.3"
+python_dateutil = "^2.5.3"
+urllib3 = "^1.25.3"
 pydantic = "^1.10.2"
-aenum = ">= 3.1.11"
+aenum = "^3.1.11"
 
 [tool.poetry.dev-dependencies]
 pytest = ">= 7.1.3"
 pytest-cov = ">= 2.8.1"
 pytest-randomly = ">= 3.12.0"
 sphinx = ">=5.3.0"
 sphinx-markdown-builder = ">=0.5.5"
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `edgeimpulse_api-1.25.16/PKG-INFO` & `edgeimpulse_api-1.25.31/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgeimpulse-api
-Version: 1.25.16
+Version: 1.25.31
 Summary: Python bindings for the Edge Impulse API.
 Home-page: https://edgeimpulse.com
 License: Apache-2.0
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Embedded Systems
-Requires-Dist: aenum (>=3.1.11)
+Requires-Dist: aenum (>=3.1.11,<4.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: python_dateutil (>=2.5.3)
-Requires-Dist: urllib3 (>=1.25.3)
+Requires-Dist: python_dateutil (>=2.5.3,<3.0.0)
+Requires-Dist: urllib3 (>=1.25.3,<2.0.0)
 Project-URL: Documentation, https://docs.edgeimpulse.com/reference/edge-impulse-api/edge-impulse-api
 Description-Content-Type: text/markdown
 
 # Edge Impulse API bindings
 
 This is the official Python API bindings for Edge Impulse. It's designed to make it easier to use the Edge Impulse API from Python.
```

