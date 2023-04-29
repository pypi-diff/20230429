# Comparing `tmp/ory-kratos-client-0.9.0a2.tar.gz` & `tmp/ory-kratos-client-0.9.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ory-kratos-client-0.9.0a2.tar", last modified: Tue Mar 22 10:27:43 2022, max compression
+gzip compressed data, was "dist/ory-kratos-client-0.9.0a3.tar", last modified: Fri Mar 25 10:10:36 2022, max compression
```

## Comparing `ory-kratos-client-0.9.0a2.tar` & `ory-kratos-client-0.9.0a3.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/
--rw-r--r--   0 root         (0) root         (0)      751 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18033 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/
--rw-r--r--   0 root         (0) root         (0)     1160 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/api/
--rw-r--r--   0 root         (0) root         (0)      222 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15336 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/api/metadata_api.py
--rw-r--r--   0 root         (0) root         (0)   236910 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/api/v0alpha2_api.py
--rw-r--r--   0 root         (0) root         (0)    38028 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/apis/
--rw-r--r--   0 root         (0) root         (0)      533 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17503 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5449 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/
--rw-r--r--   0 root         (0) root         (0)      348 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15500 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_body.py
--rw-r--r--   0 root         (0) root         (0)    11940 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_import_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)    12663 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_import_credentials_oidc_config.py
--rw-r--r--   0 root         (0) root         (0)    12201 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_import_credentials_oidc_provider.py
--rw-r--r--   0 root         (0) root         (0)    11980 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_import_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)    12149 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_import_credentials_password_config.py
--rw-r--r--   0 root         (0) root         (0)    12265 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_self_service_recovery_link_body.py
--rw-r--r--   0 root         (0) root         (0)    12422 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_identity_import_credentials.py
--rw-r--r--   0 root         (0) root         (0)    13025 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_update_identity_body.py
--rw-r--r--   0 root         (0) root         (0)    13723 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/authenticator_assurance_level.py
--rw-r--r--   0 root         (0) root         (0)    14235 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/error_authenticator_assurance_level_not_satisfied.py
--rw-r--r--   0 root         (0) root         (0)    13691 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/generic_error.py
--rw-r--r--   0 root         (0) root         (0)    11600 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/health_not_ready_status.py
--rw-r--r--   0 root         (0) root         (0)    11474 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/health_status.py
--rw-r--r--   0 root         (0) root         (0)    16264 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity.py
--rw-r--r--   0 root         (0) root         (0)    13512 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_credentials.py
--rw-r--r--   0 root         (0) root         (0)    11802 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)    12429 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_credentials_oidc_provider.py
--rw-r--r--   0 root         (0) root         (0)    11616 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)    12257 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_credentials_type.py
--rw-r--r--   0 root         (0) root         (0)    11837 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_list.py
--rw-r--r--   0 root         (0) root         (0)    11920 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_schema.py
--rw-r--r--   0 root         (0) root         (0)    12005 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)    12129 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_state.py
--rw-r--r--   0 root         (0) root         (0)    11509 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/inline_response200.py
--rw-r--r--   0 root         (0) root         (0)    11547 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/inline_response2001.py
--rw-r--r--   0 root         (0) root         (0)    11643 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/inline_response503.py
--rw-r--r--   0 root         (0) root         (0)    11647 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/json_error.py
--rw-r--r--   0 root         (0) root         (0)    14378 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/needs_privileged_session_error.py
--rw-r--r--   0 root         (0) root         (0)    12135 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/pagination.py
--rw-r--r--   0 root         (0) root         (0)    12475 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/recovery_address.py
--rw-r--r--   0 root         (0) root         (0)    11500 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/revoked_sessions.py
--rw-r--r--   0 root         (0) root         (0)    14304 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_browser_location_change_required_error.py
--rw-r--r--   0 root         (0) root         (0)    12479 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_error.py
--rw-r--r--   0 root         (0) root         (0)    14687 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_flow_expired_error.py
--rw-r--r--   0 root         (0) root         (0)    15720 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_login_flow.py
--rw-r--r--   0 root         (0) root         (0)    12062 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_logout_url.py
--rw-r--r--   0 root         (0) root         (0)    14713 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_recovery_flow.py
--rw-r--r--   0 root         (0) root         (0)    13232 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_recovery_flow_state.py
--rw-r--r--   0 root         (0) root         (0)    12065 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_recovery_link.py
--rw-r--r--   0 root         (0) root         (0)    14255 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_registration_flow.py
--rw-r--r--   0 root         (0) root         (0)    15039 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_settings_flow.py
--rw-r--r--   0 root         (0) root         (0)    13490 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_settings_flow_state.py
--rw-r--r--   0 root         (0) root         (0)    14625 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_verification_flow.py
--rw-r--r--   0 root         (0) root         (0)    13260 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_verification_flow_state.py
--rw-r--r--   0 root         (0) root         (0)    14648 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/session.py
--rw-r--r--   0 root         (0) root         (0)    12524 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/session_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)    12342 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/session_authentication_methods.py
--rw-r--r--   0 root         (0) root         (0)    11485 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/session_device.py
--rw-r--r--   0 root         (0) root         (0)    11825 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/session_list.py
--rw-r--r--   0 root         (0) root         (0)    12654 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/settings_profile_form_config.py
--rw-r--r--   0 root         (0) root         (0)    12365 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_flow_with_web_authn_registration_method.py
--rw-r--r--   0 root         (0) root         (0)    19610 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    12445 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_with_lookup_secret_method_body.py
--rw-r--r--   0 root         (0) root         (0)    12774 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_with_oidc_method_body.py
--rw-r--r--   0 root         (0) root         (0)    13319 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_with_password_method_body.py
--rw-r--r--   0 root         (0) root         (0)    12333 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_with_totp_method_body.py
--rw-r--r--   0 root         (0) root         (0)    13112 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_with_web_authn_method_body.py
--rw-r--r--   0 root         (0) root         (0)    11740 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_logout_flow_without_browser_body.py
--rw-r--r--   0 root         (0) root         (0)    15140 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_recovery_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    12672 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_recovery_flow_with_link_method_body.py
--rw-r--r--   0 root         (0) root         (0)    17694 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_registration_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    12695 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_registration_flow_with_oidc_method_body.py
--rw-r--r--   0 root         (0) root         (0)    12757 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_registration_flow_with_password_method_body.py
--rw-r--r--   0 root         (0) root         (0)    13541 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_registration_flow_with_web_authn_method_body.py
--rw-r--r--   0 root         (0) root         (0)    22487 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    13481 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_lookup_method_body.py
--rw-r--r--   0 root         (0) root         (0)    13097 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_oidc_method_body.py
--rw-r--r--   0 root         (0) root         (0)    12293 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_password_method_body.py
--rw-r--r--   0 root         (0) root         (0)    12582 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_profile_method_body.py
--rw-r--r--   0 root         (0) root         (0)    12816 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_totp_method_body.py
--rw-r--r--   0 root         (0) root         (0)    13480 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_web_authn_method_body.py
--rw-r--r--   0 root         (0) root         (0)    15198 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_verification_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    12698 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_verification_flow_with_link_method_body.py
--rw-r--r--   0 root         (0) root         (0)    12421 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/successful_self_service_login_without_browser.py
--rw-r--r--   0 root         (0) root         (0)    12934 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/successful_self_service_registration_without_browser.py
--rw-r--r--   0 root         (0) root         (0)    12612 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_container.py
--rw-r--r--   0 root         (0) root         (0)    12767 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node.py
--rw-r--r--   0 root         (0) root         (0)    12383 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_anchor_attributes.py
--rw-r--r--   0 root         (0) root         (0)    20551 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_attributes.py
--rw-r--r--   0 root         (0) root         (0)    12476 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_image_attributes.py
--rw-r--r--   0 root         (0) root         (0)    13942 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_input_attributes.py
--rw-r--r--   0 root         (0) root         (0)    11560 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_meta.py
--rw-r--r--   0 root         (0) root         (0)    14081 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_script_attributes.py
--rw-r--r--   0 root         (0) root         (0)    12080 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_text_attributes.py
--rw-r--r--   0 root         (0) root         (0)    11805 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_nodes.py
--rw-r--r--   0 root         (0) root         (0)    12383 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_text.py
--rw-r--r--   0 root         (0) root         (0)    11805 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_texts.py
--rw-r--r--   0 root         (0) root         (0)    13658 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/verifiable_identity_address.py
--rw-r--r--   0 root         (0) root         (0)    11470 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model/version.py
--rw-r--r--   0 root         (0) root         (0)    82466 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/models/
--rw-r--r--   0 root         (0) root         (0)     9267 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14576 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/ory_kratos_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/ory_kratos_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      751 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/ory_kratos_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10278 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/ory_kratos_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/ory_kratos_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/ory_kratos_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/ory_kratos_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1829 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 10:27:43.000000 ory-kratos-client-0.9.0a2/test/
--rw-r--r--   0 root         (0) root         (0)     1771 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_admin_create_identity_body.py
--rw-r--r--   0 root         (0) root         (0)     1578 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_admin_create_identity_import_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)     1890 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_admin_create_identity_import_credentials_oidc_config.py
--rw-r--r--   0 root         (0) root         (0)     1390 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_admin_create_identity_import_credentials_oidc_provider.py
--rw-r--r--   0 root         (0) root         (0)     1622 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_admin_create_identity_import_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)     1404 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_admin_create_identity_import_credentials_password_config.py
--rw-r--r--   0 root         (0) root         (0)     1320 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_admin_create_self_service_recovery_link_body.py
--rw-r--r--   0 root         (0) root         (0)     1717 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_admin_identity_import_credentials.py
--rw-r--r--   0 root         (0) root         (0)     1320 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_admin_update_identity_body.py
--rw-r--r--   0 root         (0) root         (0)     1239 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_authenticator_assurance_level.py
--rw-r--r--   0 root         (0) root         (0)     1361 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_error_authenticator_assurance_level_not_satisfied.py
--rw-r--r--   0 root         (0) root         (0)     1133 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_generic_error.py
--rw-r--r--   0 root         (0) root         (0)     1191 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_health_not_ready_status.py
--rw-r--r--   0 root         (0) root         (0)     1133 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_health_status.py
--rw-r--r--   0 root         (0) root         (0)     1617 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_identity.py
--rw-r--r--   0 root         (0) root         (0)     1331 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_identity_credentials.py
--rw-r--r--   0 root         (0) root         (0)     1393 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_identity_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)     1268 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_identity_credentials_oidc_provider.py
--rw-r--r--   0 root         (0) root         (0)     1239 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_identity_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)     1211 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_identity_credentials_type.py
--rw-r--r--   0 root         (0) root         (0)     1220 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_identity_list.py
--rw-r--r--   0 root         (0) root         (0)     1147 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_identity_schema.py
--rw-r--r--   0 root         (0) root         (0)     1266 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)     1140 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_identity_state.py
--rw-r--r--   0 root         (0) root         (0)     1168 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_inline_response200.py
--rw-r--r--   0 root         (0) root         (0)     1175 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_inline_response2001.py
--rw-r--r--   0 root         (0) root         (0)     1168 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_inline_response503.py
--rw-r--r--   0 root         (0) root         (0)     1216 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_json_error.py
--rw-r--r--   0 root         (0) root         (0)     1397 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)     1240 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_needs_privileged_session_error.py
--rw-r--r--   0 root         (0) root         (0)     1118 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_pagination.py
--rw-r--r--   0 root         (0) root         (0)     1154 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_recovery_address.py
--rw-r--r--   0 root         (0) root         (0)     1154 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_revoked_sessions.py
--rw-r--r--   0 root         (0) root         (0)     1369 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_browser_location_change_required_error.py
--rw-r--r--   0 root         (0) root         (0)     1162 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_error.py
--rw-r--r--   0 root         (0) root         (0)     1241 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_flow_expired_error.py
--rw-r--r--   0 root         (0) root         (0)     1605 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_login_flow.py
--rw-r--r--   0 root         (0) root         (0)     1191 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_logout_url.py
--rw-r--r--   0 root         (0) root         (0)     1483 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_recovery_flow.py
--rw-r--r--   0 root         (0) root         (0)     1248 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_recovery_flow_state.py
--rw-r--r--   0 root         (0) root         (0)     1212 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_recovery_link.py
--rw-r--r--   0 root         (0) root         (0)     1489 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_registration_flow.py
--rw-r--r--   0 root         (0) root         (0)     1570 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_settings_flow.py
--rw-r--r--   0 root         (0) root         (0)     1248 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_settings_flow_state.py
--rw-r--r--   0 root         (0) root         (0)     1527 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_verification_flow.py
--rw-r--r--   0 root         (0) root         (0)     1276 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_self_service_verification_flow_state.py
--rw-r--r--   0 root         (0) root         (0)     1518 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_session.py
--rw-r--r--   0 root         (0) root         (0)     1404 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_session_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     1411 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_session_authentication_methods.py
--rw-r--r--   0 root         (0) root         (0)     1140 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_session_device.py
--rw-r--r--   0 root         (0) root         (0)     1209 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_session_list.py
--rw-r--r--   0 root         (0) root         (0)     1394 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_settings_profile_form_config.py
--rw-r--r--   0 root         (0) root         (0)     1413 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_flow_with_web_authn_registration_method.py
--rw-r--r--   0 root         (0) root         (0)     2524 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1421 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_with_lookup_secret_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1364 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_with_oidc_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1392 2022-03-22 10:24:33.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_with_password_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1364 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_with_totp_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1393 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_with_web_authn_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1370 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_logout_flow_without_browser_body.py
--rw-r--r--   0 root         (0) root         (0)     1535 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_recovery_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1385 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_recovery_flow_with_link_method_body.py
--rw-r--r--   0 root         (0) root         (0)     2146 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_registration_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1413 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_registration_flow_with_oidc_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1441 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_registration_flow_with_password_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1442 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_registration_flow_with_web_authn_method_body.py
--rw-r--r--   0 root         (0) root         (0)     2843 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1399 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_lookup_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1385 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_oidc_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1413 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_password_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1406 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_profile_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1385 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_totp_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1414 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_web_authn_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1579 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_verification_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1413 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_submit_self_service_verification_flow_with_link_method_body.py
--rw-r--r--   0 root         (0) root         (0)     1416 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_successful_self_service_login_without_browser.py
--rw-r--r--   0 root         (0) root         (0)     1552 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_successful_self_service_registration_without_browser.py
--rw-r--r--   0 root         (0) root         (0)     1294 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_container.py
--rw-r--r--   0 root         (0) root         (0)     1393 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_node.py
--rw-r--r--   0 root         (0) root         (0)     1285 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_node_anchor_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1956 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_node_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1198 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_node_image_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1278 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_node_input_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1200 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_node_meta.py
--rw-r--r--   0 root         (0) root         (0)     1205 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_node_script_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1271 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_node_text_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1178 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_nodes.py
--rw-r--r--   0 root         (0) root         (0)     1091 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_text.py
--rw-r--r--   0 root         (0) root         (0)     1178 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_ui_texts.py
--rw-r--r--   0 root         (0) root         (0)     8904 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_v0alpha2_api.py
--rw-r--r--   0 root         (0) root         (0)     1225 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_verifiable_identity_address.py
--rw-r--r--   0 root         (0) root         (0)     1097 2022-03-22 10:24:34.000000 ory-kratos-client-0.9.0a2/test/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/
+-rw-r--r--   0 root         (0) root         (0)      751 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18033 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/
+-rw-r--r--   0 root         (0) root         (0)     1160 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/api/
+-rw-r--r--   0 root         (0) root         (0)      222 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15336 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/api/metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)   236947 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/api/v0alpha2_api.py
+-rw-r--r--   0 root         (0) root         (0)    38028 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      533 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17503 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5449 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/
+-rw-r--r--   0 root         (0) root         (0)      348 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15500 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)    11940 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_import_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)    12663 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_import_credentials_oidc_config.py
+-rw-r--r--   0 root         (0) root         (0)    12201 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_import_credentials_oidc_provider.py
+-rw-r--r--   0 root         (0) root         (0)    11980 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_import_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)    12149 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_import_credentials_password_config.py
+-rw-r--r--   0 root         (0) root         (0)    12265 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_self_service_recovery_link_body.py
+-rw-r--r--   0 root         (0) root         (0)    12422 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_identity_import_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    13025 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_update_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)    13723 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/authenticator_assurance_level.py
+-rw-r--r--   0 root         (0) root         (0)    14235 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/error_authenticator_assurance_level_not_satisfied.py
+-rw-r--r--   0 root         (0) root         (0)    13691 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/generic_error.py
+-rw-r--r--   0 root         (0) root         (0)    11600 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/health_not_ready_status.py
+-rw-r--r--   0 root         (0) root         (0)    11474 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/health_status.py
+-rw-r--r--   0 root         (0) root         (0)    16264 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity.py
+-rw-r--r--   0 root         (0) root         (0)    13512 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    11802 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_credentials_oidc_provider.py
+-rw-r--r--   0 root         (0) root         (0)    11616 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)    12257 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_credentials_type.py
+-rw-r--r--   0 root         (0) root         (0)    11837 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_list.py
+-rw-r--r--   0 root         (0) root         (0)    11920 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_schema.py
+-rw-r--r--   0 root         (0) root         (0)    12005 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)    12129 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_state.py
+-rw-r--r--   0 root         (0) root         (0)    11509 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/inline_response200.py
+-rw-r--r--   0 root         (0) root         (0)    11547 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/inline_response2001.py
+-rw-r--r--   0 root         (0) root         (0)    11643 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/inline_response503.py
+-rw-r--r--   0 root         (0) root         (0)    11647 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/json_error.py
+-rw-r--r--   0 root         (0) root         (0)    14378 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/needs_privileged_session_error.py
+-rw-r--r--   0 root         (0) root         (0)    12135 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/pagination.py
+-rw-r--r--   0 root         (0) root         (0)    12475 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/recovery_address.py
+-rw-r--r--   0 root         (0) root         (0)    11500 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/revoked_sessions.py
+-rw-r--r--   0 root         (0) root         (0)    14304 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_browser_location_change_required_error.py
+-rw-r--r--   0 root         (0) root         (0)    12479 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_error.py
+-rw-r--r--   0 root         (0) root         (0)    14687 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_flow_expired_error.py
+-rw-r--r--   0 root         (0) root         (0)    15720 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_login_flow.py
+-rw-r--r--   0 root         (0) root         (0)    12062 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_logout_url.py
+-rw-r--r--   0 root         (0) root         (0)    14713 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_recovery_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13232 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_recovery_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)    12065 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_recovery_link.py
+-rw-r--r--   0 root         (0) root         (0)    14255 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_registration_flow.py
+-rw-r--r--   0 root         (0) root         (0)    15039 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_settings_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13490 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_settings_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)    14625 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_verification_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13260 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_verification_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)    14648 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/session.py
+-rw-r--r--   0 root         (0) root         (0)    12524 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/session_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)    12342 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/session_authentication_methods.py
+-rw-r--r--   0 root         (0) root         (0)    11485 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/session_device.py
+-rw-r--r--   0 root         (0) root         (0)    11825 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/session_list.py
+-rw-r--r--   0 root         (0) root         (0)    12654 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/settings_profile_form_config.py
+-rw-r--r--   0 root         (0) root         (0)    12365 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_flow_with_web_authn_registration_method.py
+-rw-r--r--   0 root         (0) root         (0)    19610 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    12445 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_with_lookup_secret_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    12774 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_with_oidc_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    13319 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_with_password_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    12333 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_with_totp_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    13112 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_with_web_authn_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    11740 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_logout_flow_without_browser_body.py
+-rw-r--r--   0 root         (0) root         (0)    15140 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_recovery_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    12672 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_recovery_flow_with_link_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    17694 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_registration_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    12695 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_registration_flow_with_oidc_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    12757 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_registration_flow_with_password_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    13541 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_registration_flow_with_web_authn_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    22487 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    13481 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_lookup_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    13097 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_oidc_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    12293 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_password_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    12582 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_profile_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    12816 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_totp_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    13480 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_web_authn_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    15198 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_verification_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    12698 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_verification_flow_with_link_method_body.py
+-rw-r--r--   0 root         (0) root         (0)    12421 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/successful_self_service_login_without_browser.py
+-rw-r--r--   0 root         (0) root         (0)    12934 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/successful_self_service_registration_without_browser.py
+-rw-r--r--   0 root         (0) root         (0)    12612 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_container.py
+-rw-r--r--   0 root         (0) root         (0)    12767 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node.py
+-rw-r--r--   0 root         (0) root         (0)    12383 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_anchor_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    20551 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    12476 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_image_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    13942 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_input_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    11560 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_meta.py
+-rw-r--r--   0 root         (0) root         (0)    14081 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_script_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    12080 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_text_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    11805 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_nodes.py
+-rw-r--r--   0 root         (0) root         (0)    12383 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_text.py
+-rw-r--r--   0 root         (0) root         (0)    11805 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_texts.py
+-rw-r--r--   0 root         (0) root         (0)    13658 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/verifiable_identity_address.py
+-rw-r--r--   0 root         (0) root         (0)    11470 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model/version.py
+-rw-r--r--   0 root         (0) root         (0)    82466 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/models/
+-rw-r--r--   0 root         (0) root         (0)     9267 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14576 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/ory_kratos_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/ory_kratos_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      751 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/ory_kratos_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10278 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/ory_kratos_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/ory_kratos_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/ory_kratos_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/ory_kratos_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1829 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 10:10:36.000000 ory-kratos-client-0.9.0a3/test/
+-rw-r--r--   0 root         (0) root         (0)     1771 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_admin_create_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_admin_create_identity_import_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_admin_create_identity_import_credentials_oidc_config.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_admin_create_identity_import_credentials_oidc_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_admin_create_identity_import_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_admin_create_identity_import_credentials_password_config.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_admin_create_self_service_recovery_link_body.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_admin_identity_import_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_admin_update_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_authenticator_assurance_level.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_error_authenticator_assurance_level_not_satisfied.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_generic_error.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_health_not_ready_status.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_health_status.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_identity_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_identity_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_identity_credentials_oidc_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_identity_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_identity_credentials_type.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_identity_list.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_identity_schema.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_identity_state.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_inline_response200.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_inline_response2001.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_inline_response503.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_json_error.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/test/test_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_needs_privileged_session_error.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_pagination.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_recovery_address.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_revoked_sessions.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_browser_location_change_required_error.py
+-rw-r--r--   0 root         (0) root         (0)     1162 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_error.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_flow_expired_error.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_login_flow.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_logout_url.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_recovery_flow.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_recovery_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_recovery_link.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_registration_flow.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_settings_flow.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_settings_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_verification_flow.py
+-rw-r--r--   0 root         (0) root         (0)     1276 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_self_service_verification_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_session.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_session_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_session_authentication_methods.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_session_device.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_session_list.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_settings_profile_form_config.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_flow_with_web_authn_registration_method.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_with_lookup_secret_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_with_oidc_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1392 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_with_password_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_with_totp_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_with_web_authn_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_logout_flow_without_browser_body.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_recovery_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_recovery_flow_with_link_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_registration_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_registration_flow_with_oidc_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_registration_flow_with_password_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_registration_flow_with_web_authn_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_lookup_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_oidc_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_password_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_profile_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_totp_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_web_authn_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_verification_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_submit_self_service_verification_flow_with_link_method_body.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_successful_self_service_login_without_browser.py
+-rw-r--r--   0 root         (0) root         (0)     1552 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_successful_self_service_registration_without_browser.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_container.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_node.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_node_anchor_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_node_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_node_image_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_node_input_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_node_meta.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_node_script_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1271 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_node_text_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_text.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_ui_texts.py
+-rw-r--r--   0 root         (0) root         (0)     8904 2022-03-25 10:07:22.000000 ory-kratos-client-0.9.0a3/test/test_v0alpha2_api.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_verifiable_identity_address.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2022-03-25 10:07:21.000000 ory-kratos-client-0.9.0a3/test/test_version.py
```

### Comparing `ory-kratos-client-0.9.0a2/PKG-INFO` & `ory-kratos-client-0.9.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ory-kratos-client
-Version: 0.9.0a2
+Version: 0.9.0a3
 Summary: Ory Kratos API
 Home-page: https://github.com/ory/sdk
 Author: OpenAPI Generator community
 Author-email: hi@ory.sh
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Ory Kratos API
 Platform: UNKNOWN
```

### Comparing `ory-kratos-client-0.9.0a2/README.md` & `ory-kratos-client-0.9.0a3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 while administrative APIs should never be exposed without prior authorization. To protect
 the administative API port you should use something like Nginx, Ory Oathkeeper, or any other
 technology capable of authorizing incoming requests.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: v0.9.0-alpha.2
-- Package version: v0.9.0-alpha.2
+- API version: v0.9.0-alpha.3
+- Package version: v0.9.0-alpha.3
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >=3.6
 
 ## Installation & Usage
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/__init__.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # flake8: noqa
 
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "v0.9.0-alpha.2"
+__version__ = "v0.9.0-alpha.3"
 
 # import ApiClient
 from ory_kratos_client.api_client import ApiClient
 
 # import Configuration
 from ory_kratos_client.configuration import Configuration
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/api/metadata_api.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/api/metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/api/v0alpha2_api.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/api/v0alpha2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -4513,15 +4513,15 @@
     def submit_self_service_login_flow(
         self,
         flow,
         **kwargs
     ):
         """Submit a Login Flow  # noqa: E501
 
-        :::info  This endpoint is EXPERIMENTAL and subject to potential breaking changes in the future.  :::  Use this endpoint to complete a login flow. This endpoint behaves differently for API and browser flows.  API flows expect `application/json` to be sent in the body and responds with HTTP 200 and a application/json body with the session token on success; HTTP 303 redirect to a fresh login flow if the original flow expired with the appropriate error messages set; HTTP 400 on form validation errors.  Browser flows expect a Content-Type of `application/x-www-form-urlencoded` or `application/json` to be sent in the body and respond with a HTTP 303 redirect to the post/after login URL or the `return_to` value if it was set and if the login succeeded; a HTTP 303 redirect to the login UI URL with the flow ID containing the validation errors otherwise.  Browser flows with an accept header of `application/json` will not redirect but instead respond with HTTP 200 and a application/json body with the signed in identity and a `Set-Cookie` header on success; HTTP 303 redirect to a fresh login flow if the original flow expired with the appropriate error messages set; HTTP 400 on form validation errors.  If this endpoint is called with `Accept: application/json` in the header, the response contains the flow without a redirect. In the case of an error, the `error.id` of the JSON response body can be one of:  `session_already_available`: The user is already signed in. `security_csrf_violation`: Unable to fetch the flow because a CSRF violation occurred. `security_identity_mismatch`: The requested `?return_to` address is not allowed to be used. Adjust this in the configuration! `browser_location_change_required`: Usually sent when an AJAX request indicates that the browser needs to open a specific URL. Most likely used in Social Sign In flows.  More information can be found at [Ory Kratos User Login](https://www.ory.sh/docs/kratos/self-service/flows/user-login) and [User Registration Documentation](https://www.ory.sh/docs/kratos/self-service/flows/user-registration).  # noqa: E501
+        :::info  This endpoint is EXPERIMENTAL and subject to potential breaking changes in the future.  :::  Use this endpoint to complete a login flow. This endpoint behaves differently for API and browser flows.  API flows expect `application/json` to be sent in the body and responds with HTTP 200 and a application/json body with the session token on success; HTTP 410 if the original flow expired with the appropriate error messages set and optionally a `use_flow_id` parameter in the body; HTTP 400 on form validation errors.  Browser flows expect a Content-Type of `application/x-www-form-urlencoded` or `application/json` to be sent in the body and respond with a HTTP 303 redirect to the post/after login URL or the `return_to` value if it was set and if the login succeeded; a HTTP 303 redirect to the login UI URL with the flow ID containing the validation errors otherwise.  Browser flows with an accept header of `application/json` will not redirect but instead respond with HTTP 200 and a application/json body with the signed in identity and a `Set-Cookie` header on success; HTTP 303 redirect to a fresh login flow if the original flow expired with the appropriate error messages set; HTTP 400 on form validation errors.  If this endpoint is called with `Accept: application/json` in the header, the response contains the flow without a redirect. In the case of an error, the `error.id` of the JSON response body can be one of:  `session_already_available`: The user is already signed in. `security_csrf_violation`: Unable to fetch the flow because a CSRF violation occurred. `security_identity_mismatch`: The requested `?return_to` address is not allowed to be used. Adjust this in the configuration! `browser_location_change_required`: Usually sent when an AJAX request indicates that the browser needs to open a specific URL. Most likely used in Social Sign In flows.  More information can be found at [Ory Kratos User Login](https://www.ory.sh/docs/kratos/self-service/flows/user-login) and [User Registration Documentation](https://www.ory.sh/docs/kratos/self-service/flows/user-registration).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.submit_self_service_login_flow(flow, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4826,15 +4826,15 @@
     def submit_self_service_registration_flow(
         self,
         flow,
         **kwargs
     ):
         """Submit a Registration Flow  # noqa: E501
 
-        Use this endpoint to complete a registration flow by sending an identity's traits and password. This endpoint behaves differently for API and browser flows.  API flows expect `application/json` to be sent in the body and respond with HTTP 200 and a application/json body with the created identity success - if the session hook is configured the `session` and `session_token` will also be included; HTTP 303 redirect to a fresh registration flow if the original flow expired with the appropriate error messages set; HTTP 400 on form validation errors.  Browser flows expect a Content-Type of `application/x-www-form-urlencoded` or `application/json` to be sent in the body and respond with a HTTP 303 redirect to the post/after registration URL or the `return_to` value if it was set and if the registration succeeded; a HTTP 303 redirect to the registration UI URL with the flow ID containing the validation errors otherwise.  Browser flows with an accept header of `application/json` will not redirect but instead respond with HTTP 200 and a application/json body with the signed in identity and a `Set-Cookie` header on success; HTTP 303 redirect to a fresh login flow if the original flow expired with the appropriate error messages set; HTTP 400 on form validation errors.  If this endpoint is called with `Accept: application/json` in the header, the response contains the flow without a redirect. In the case of an error, the `error.id` of the JSON response body can be one of:  `session_already_available`: The user is already signed in. `security_csrf_violation`: Unable to fetch the flow because a CSRF violation occurred. `security_identity_mismatch`: The requested `?return_to` address is not allowed to be used. Adjust this in the configuration! `browser_location_change_required`: Usually sent when an AJAX request indicates that the browser needs to open a specific URL. Most likely used in Social Sign In flows.  More information can be found at [Ory Kratos User Login](https://www.ory.sh/docs/kratos/self-service/flows/user-login) and [User Registration Documentation](https://www.ory.sh/docs/kratos/self-service/flows/user-registration).  # noqa: E501
+        Use this endpoint to complete a registration flow by sending an identity's traits and password. This endpoint behaves differently for API and browser flows.  API flows expect `application/json` to be sent in the body and respond with HTTP 200 and a application/json body with the created identity success - if the session hook is configured the `session` and `session_token` will also be included; HTTP 410 if the original flow expired with the appropriate error messages set and optionally a `use_flow_id` parameter in the body; HTTP 400 on form validation errors.  Browser flows expect a Content-Type of `application/x-www-form-urlencoded` or `application/json` to be sent in the body and respond with a HTTP 303 redirect to the post/after registration URL or the `return_to` value if it was set and if the registration succeeded; a HTTP 303 redirect to the registration UI URL with the flow ID containing the validation errors otherwise.  Browser flows with an accept header of `application/json` will not redirect but instead respond with HTTP 200 and a application/json body with the signed in identity and a `Set-Cookie` header on success; HTTP 303 redirect to a fresh login flow if the original flow expired with the appropriate error messages set; HTTP 400 on form validation errors.  If this endpoint is called with `Accept: application/json` in the header, the response contains the flow without a redirect. In the case of an error, the `error.id` of the JSON response body can be one of:  `session_already_available`: The user is already signed in. `security_csrf_violation`: Unable to fetch the flow because a CSRF violation occurred. `security_identity_mismatch`: The requested `?return_to` address is not allowed to be used. Adjust this in the configuration! `browser_location_change_required`: Usually sent when an AJAX request indicates that the browser needs to open a specific URL. Most likely used in Social Sign In flows.  More information can be found at [Ory Kratos User Login](https://www.ory.sh/docs/kratos/self-service/flows/user-login) and [User Registration Documentation](https://www.ory.sh/docs/kratos/self-service/flows/user-registration).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.submit_self_service_registration_flow(flow, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/api_client.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/v0.9.0-alpha.2/python'
+        self.user_agent = 'OpenAPI-Generator/v0.9.0-alpha.3/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/apis/__init__.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/configuration.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -405,16 +405,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: v0.9.0-alpha.2\n"\
-               "SDK Package Version: v0.9.0-alpha.2".\
+               "Version of the API: v0.9.0-alpha.3\n"\
+               "SDK Package Version: v0.9.0-alpha.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/exceptions.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_import_credentials_oidc.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_import_credentials_oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_import_credentials_oidc_config.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_import_credentials_oidc_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_import_credentials_oidc_provider.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_import_credentials_oidc_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_import_credentials_password.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_import_credentials_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_identity_import_credentials_password_config.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_identity_import_credentials_password_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_create_self_service_recovery_link_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_create_self_service_recovery_link_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_identity_import_credentials.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_identity_import_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/admin_update_identity_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/admin_update_identity_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/authenticator_assurance_level.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/authenticator_assurance_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/error_authenticator_assurance_level_not_satisfied.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/error_authenticator_assurance_level_not_satisfied.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/generic_error.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/generic_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/health_not_ready_status.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/health_not_ready_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/health_status.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/health_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_credentials.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_credentials_oidc.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_credentials_oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_credentials_oidc_provider.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_credentials_oidc_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_credentials_password.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_credentials_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_credentials_type.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_credentials_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_list.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_schema.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_schemas.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/identity_state.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/identity_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/inline_response200.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/inline_response200.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/inline_response2001.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/inline_response2001.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/inline_response503.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/inline_response503.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/json_error.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/json_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/needs_privileged_session_error.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/needs_privileged_session_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/pagination.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/recovery_address.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/recovery_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/revoked_sessions.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/revoked_sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_browser_location_change_required_error.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_browser_location_change_required_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_error.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_flow_expired_error.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_flow_expired_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_login_flow.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_login_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_logout_url.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_logout_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_recovery_flow.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_recovery_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_recovery_flow_state.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_recovery_flow_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_recovery_link.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_recovery_link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_registration_flow.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_registration_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_settings_flow.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_settings_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_settings_flow_state.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_settings_flow_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_verification_flow.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_verification_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/self_service_verification_flow_state.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/self_service_verification_flow_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/session.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/session_authentication_method.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/session_authentication_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/session_authentication_methods.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/session_authentication_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/session_device.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/session_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/session_list.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/session_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/settings_profile_form_config.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/settings_profile_form_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_flow_with_web_authn_registration_method.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_flow_with_web_authn_registration_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_with_lookup_secret_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_with_lookup_secret_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_with_oidc_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_with_oidc_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_with_password_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_with_password_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_with_totp_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_with_totp_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_login_flow_with_web_authn_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_login_flow_with_web_authn_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_logout_flow_without_browser_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_logout_flow_without_browser_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_recovery_flow_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_recovery_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_recovery_flow_with_link_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_recovery_flow_with_link_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_registration_flow_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_registration_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_registration_flow_with_oidc_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_registration_flow_with_oidc_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_registration_flow_with_password_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_registration_flow_with_password_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_registration_flow_with_web_authn_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_registration_flow_with_web_authn_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_lookup_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_lookup_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_oidc_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_oidc_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_password_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_password_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_profile_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_profile_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_totp_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_totp_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_settings_flow_with_web_authn_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_settings_flow_with_web_authn_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_verification_flow_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_verification_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/submit_self_service_verification_flow_with_link_method_body.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/submit_self_service_verification_flow_with_link_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/successful_self_service_login_without_browser.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/successful_self_service_login_without_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/successful_self_service_registration_without_browser.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/successful_self_service_registration_without_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_container.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_anchor_attributes.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_anchor_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_attributes.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_image_attributes.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_image_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_input_attributes.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_input_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_meta.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_script_attributes.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_script_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_node_text_attributes.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_node_text_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_nodes.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_text.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/ui_texts.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/ui_texts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/verifiable_identity_address.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/verifiable_identity_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model/version.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/model_utils.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/models/__init__.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client/rest.py` & `ory-kratos-client-0.9.0a3/ory_kratos_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client.egg-info/PKG-INFO` & `ory-kratos-client-0.9.0a3/ory_kratos_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ory-kratos-client
-Version: 0.9.0a2
+Version: 0.9.0a3
 Summary: Ory Kratos API
 Home-page: https://github.com/ory/sdk
 Author: OpenAPI Generator community
 Author-email: hi@ory.sh
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Ory Kratos API
 Platform: UNKNOWN
```

### Comparing `ory-kratos-client-0.9.0a2/ory_kratos_client.egg-info/SOURCES.txt` & `ory-kratos-client-0.9.0a3/ory_kratos_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ory-kratos-client-0.9.0a2/setup.py` & `ory-kratos-client-0.9.0a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ory-kratos-client"
-VERSION = "v0.9.0-alpha.2"
+VERSION = "v0.9.0-alpha.3"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_admin_create_identity_body.py` & `ory-kratos-client-0.9.0a3/test/test_admin_create_identity_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_admin_create_identity_import_credentials_oidc.py` & `ory-kratos-client-0.9.0a3/test/test_admin_create_identity_import_credentials_oidc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_admin_create_identity_import_credentials_oidc_config.py` & `ory-kratos-client-0.9.0a3/test/test_admin_create_identity_import_credentials_oidc_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_admin_create_identity_import_credentials_oidc_provider.py` & `ory-kratos-client-0.9.0a3/test/test_admin_create_identity_import_credentials_oidc_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_admin_create_identity_import_credentials_password.py` & `ory-kratos-client-0.9.0a3/test/test_admin_create_identity_import_credentials_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_admin_create_identity_import_credentials_password_config.py` & `ory-kratos-client-0.9.0a3/test/test_admin_create_identity_import_credentials_password_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_admin_create_self_service_recovery_link_body.py` & `ory-kratos-client-0.9.0a3/test/test_admin_create_self_service_recovery_link_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_admin_identity_import_credentials.py` & `ory-kratos-client-0.9.0a3/test/test_admin_identity_import_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_admin_update_identity_body.py` & `ory-kratos-client-0.9.0a3/test/test_admin_update_identity_body.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_authenticator_assurance_level.py` & `ory-kratos-client-0.9.0a3/test/test_authenticator_assurance_level.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_error_authenticator_assurance_level_not_satisfied.py` & `ory-kratos-client-0.9.0a3/test/test_error_authenticator_assurance_level_not_satisfied.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_generic_error.py` & `ory-kratos-client-0.9.0a3/test/test_generic_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_health_not_ready_status.py` & `ory-kratos-client-0.9.0a3/test/test_health_not_ready_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_health_status.py` & `ory-kratos-client-0.9.0a3/test/test_health_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_identity.py` & `ory-kratos-client-0.9.0a3/test/test_identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_identity_credentials.py` & `ory-kratos-client-0.9.0a3/test/test_identity_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_identity_credentials_oidc.py` & `ory-kratos-client-0.9.0a3/test/test_identity_credentials_oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_identity_credentials_oidc_provider.py` & `ory-kratos-client-0.9.0a3/test/test_identity_credentials_oidc_provider.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_identity_credentials_password.py` & `ory-kratos-client-0.9.0a3/test/test_identity_credentials_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_identity_credentials_type.py` & `ory-kratos-client-0.9.0a3/test/test_identity_credentials_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_identity_list.py` & `ory-kratos-client-0.9.0a3/test/test_identity_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_identity_schema.py` & `ory-kratos-client-0.9.0a3/test/test_identity_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_identity_schemas.py` & `ory-kratos-client-0.9.0a3/test/test_identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_identity_state.py` & `ory-kratos-client-0.9.0a3/test/test_identity_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_inline_response200.py` & `ory-kratos-client-0.9.0a3/test/test_inline_response200.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_inline_response2001.py` & `ory-kratos-client-0.9.0a3/test/test_inline_response2001.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_inline_response503.py` & `ory-kratos-client-0.9.0a3/test/test_inline_response503.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_json_error.py` & `ory-kratos-client-0.9.0a3/test/test_json_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_metadata_api.py` & `ory-kratos-client-0.9.0a3/test/test_metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_needs_privileged_session_error.py` & `ory-kratos-client-0.9.0a3/test/test_needs_privileged_session_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_pagination.py` & `ory-kratos-client-0.9.0a3/test/test_pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_recovery_address.py` & `ory-kratos-client-0.9.0a3/test/test_recovery_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_revoked_sessions.py` & `ory-kratos-client-0.9.0a3/test/test_revoked_sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_browser_location_change_required_error.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_browser_location_change_required_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_error.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_flow_expired_error.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_flow_expired_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_login_flow.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_login_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_logout_url.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_logout_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_recovery_flow.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_recovery_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_recovery_flow_state.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_recovery_flow_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_recovery_link.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_recovery_link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_registration_flow.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_registration_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_settings_flow.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_settings_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_settings_flow_state.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_settings_flow_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_verification_flow.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_verification_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_self_service_verification_flow_state.py` & `ory-kratos-client-0.9.0a3/test/test_self_service_verification_flow_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_session.py` & `ory-kratos-client-0.9.0a3/test/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_session_authentication_method.py` & `ory-kratos-client-0.9.0a3/test/test_session_authentication_method.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_session_authentication_methods.py` & `ory-kratos-client-0.9.0a3/test/test_session_authentication_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_session_device.py` & `ory-kratos-client-0.9.0a3/test/test_session_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_session_list.py` & `ory-kratos-client-0.9.0a3/test/test_session_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_settings_profile_form_config.py` & `ory-kratos-client-0.9.0a3/test/test_settings_profile_form_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_flow_with_web_authn_registration_method.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_flow_with_web_authn_registration_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_with_lookup_secret_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_with_lookup_secret_method_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_with_oidc_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_with_oidc_method_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_with_password_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_with_password_method_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_with_totp_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_with_totp_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_login_flow_with_web_authn_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_login_flow_with_web_authn_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_logout_flow_without_browser_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_logout_flow_without_browser_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_recovery_flow_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_recovery_flow_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_recovery_flow_with_link_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_recovery_flow_with_link_method_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_registration_flow_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_registration_flow_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_registration_flow_with_oidc_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_registration_flow_with_oidc_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_registration_flow_with_password_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_registration_flow_with_password_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_registration_flow_with_web_authn_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_registration_flow_with_web_authn_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_lookup_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_lookup_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_oidc_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_oidc_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_password_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_password_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_profile_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_profile_method_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_totp_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_totp_method_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_settings_flow_with_web_authn_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_settings_flow_with_web_authn_method_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_verification_flow_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_verification_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_submit_self_service_verification_flow_with_link_method_body.py` & `ory-kratos-client-0.9.0a3/test/test_submit_self_service_verification_flow_with_link_method_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_successful_self_service_login_without_browser.py` & `ory-kratos-client-0.9.0a3/test/test_successful_self_service_login_without_browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_successful_self_service_registration_without_browser.py` & `ory-kratos-client-0.9.0a3/test/test_successful_self_service_registration_without_browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_container.py` & `ory-kratos-client-0.9.0a3/test/test_ui_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_node.py` & `ory-kratos-client-0.9.0a3/test/test_ui_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_node_anchor_attributes.py` & `ory-kratos-client-0.9.0a3/test/test_ui_node_anchor_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_node_attributes.py` & `ory-kratos-client-0.9.0a3/test/test_ui_node_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_node_image_attributes.py` & `ory-kratos-client-0.9.0a3/test/test_ui_node_image_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_node_input_attributes.py` & `ory-kratos-client-0.9.0a3/test/test_ui_node_input_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_node_meta.py` & `ory-kratos-client-0.9.0a3/test/test_ui_node_meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_node_script_attributes.py` & `ory-kratos-client-0.9.0a3/test/test_ui_node_script_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_node_text_attributes.py` & `ory-kratos-client-0.9.0a3/test/test_ui_node_text_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_nodes.py` & `ory-kratos-client-0.9.0a3/test/test_ui_nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_text.py` & `ory-kratos-client-0.9.0a3/test/test_ui_text.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_ui_texts.py` & `ory-kratos-client-0.9.0a3/test/test_ui_texts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_v0alpha2_api.py` & `ory-kratos-client-0.9.0a3/test/test_v0alpha2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_verifiable_identity_address.py` & `ory-kratos-client-0.9.0a3/test/test_verifiable_identity_address.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-kratos-client-0.9.0a2/test/test_version.py` & `ory-kratos-client-0.9.0a3/test/test_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Kratos API
 
     Documentation for all public and administrative Ory Kratos APIs. Public and administrative APIs are exposed on different ports. Public APIs can face the public internet without any protection while administrative APIs should never be exposed without prior authorization. To protect the administative API port you should use something like Nginx, Ory Oathkeeper, or any other technology capable of authorizing incoming requests.   # noqa: E501
 
-    The version of the OpenAPI document: v0.9.0-alpha.2
+    The version of the OpenAPI document: v0.9.0-alpha.3
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

