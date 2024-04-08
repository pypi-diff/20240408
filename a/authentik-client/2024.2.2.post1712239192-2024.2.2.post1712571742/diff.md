# Comparing `tmp/authentik_client-2024.2.2.post1712239192.tar.gz` & `tmp/authentik_client-2024.2.2.post1712571742.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentik_client-2024.2.2.post1712239192.tar", max compression
+gzip compressed data, was "authentik_client-2024.2.2.post1712571742.tar", max compression
```

## Comparing `authentik_client-2024.2.2.post1712239192.tar` & `authentik_client-2024.2.2.post1712571742.tar`

### file list

```diff
@@ -1,580 +1,583 @@
--rw-r--r--   0        0        0   139998 2024-04-04 14:00:05.091852 authentik_client-2024.2.2.post1712239192/README.md
--rw-r--r--   0        0        0    47193 2024-04-04 14:00:05.107852 authentik_client-2024.2.2.post1712239192/authentik_client/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-04 14:00:05.107852 authentik_client-2024.2.2.post1712239192/authentik_client/api/__init__.py
--rw-r--r--   0        0        0    97518 2024-04-04 14:00:04.771847 authentik_client-2024.2.2.post1712239192/authentik_client/api/admin_api.py
--rw-r--r--   0        0        0   700271 2024-04-04 14:00:04.791847 authentik_client-2024.2.2.post1712239192/authentik_client/api/authenticators_api.py
--rw-r--r--   0        0        0   699928 2024-04-04 14:00:04.819847 authentik_client-2024.2.2.post1712239192/authentik_client/api/core_api.py
--rw-r--r--   0        0        0   116805 2024-04-04 14:00:04.831848 authentik_client-2024.2.2.post1712239192/authentik_client/api/crypto_api.py
--rw-r--r--   0        0        0   107946 2024-04-04 14:00:04.843848 authentik_client-2024.2.2.post1712239192/authentik_client/api/enterprise_api.py
--rw-r--r--   0        0        0   408008 2024-04-04 14:00:04.855848 authentik_client-2024.2.2.post1712239192/authentik_client/api/events_api.py
--rw-r--r--   0        0        0   280806 2024-04-04 14:00:04.863848 authentik_client-2024.2.2.post1712239192/authentik_client/api/flows_api.py
--rw-r--r--   0        0        0   101134 2024-04-04 14:00:04.875848 authentik_client-2024.2.2.post1712239192/authentik_client/api/managed_api.py
--rw-r--r--   0        0        0   135649 2024-04-04 14:00:04.879848 authentik_client-2024.2.2.post1712239192/authentik_client/api/oauth2_api.py
--rw-r--r--   0        0        0   413301 2024-04-04 14:00:04.891849 authentik_client-2024.2.2.post1712239192/authentik_client/api/outposts_api.py
--rw-r--r--   0        0        0   725201 2024-04-04 14:00:04.915849 authentik_client-2024.2.2.post1712239192/authentik_client/api/policies_api.py
--rw-r--r--   0        0        0   552586 2024-04-04 14:00:04.935849 authentik_client-2024.2.2.post1712239192/authentik_client/api/propertymappings_api.py
--rw-r--r--   0        0        0   718066 2024-04-04 14:00:04.959850 authentik_client-2024.2.2.post1712239192/authentik_client/api/providers_api.py
--rw-r--r--   0        0        0   150485 2024-04-04 14:00:04.975850 authentik_client-2024.2.2.post1712239192/authentik_client/api/rac_api.py
--rw-r--r--   0        0        0   207550 2024-04-04 14:00:04.983850 authentik_client-2024.2.2.post1712239192/authentik_client/api/rbac_api.py
--rw-r--r--   0        0        0    10391 2024-04-04 14:00:04.991850 authentik_client-2024.2.2.post1712239192/authentik_client/api/root_api.py
--rw-r--r--   0        0        0    11845 2024-04-04 14:00:04.999850 authentik_client-2024.2.2.post1712239192/authentik_client/api/schema_api.py
--rw-r--r--   0        0        0   802117 2024-04-04 14:00:05.015851 authentik_client-2024.2.2.post1712239192/authentik_client/api/sources_api.py
--rw-r--r--   0        0        0  1919636 2024-04-04 14:00:05.063851 authentik_client-2024.2.2.post1712239192/authentik_client/api/stages_api.py
--rw-r--r--   0        0        0   157909 2024-04-04 14:00:05.083852 authentik_client-2024.2.2.post1712239192/authentik_client/api/tenants_api.py
--rw-r--r--   0        0        0    25779 2024-04-04 14:00:05.111852 authentik_client-2024.2.2.post1712239192/authentik_client/api_client.py
--rw-r--r--   0        0        0      652 2024-04-04 14:00:05.111852 authentik_client-2024.2.2.post1712239192/authentik_client/api_response.py
--rw-r--r--   0        0        0    15345 2024-04-04 14:00:05.103852 authentik_client-2024.2.2.post1712239192/authentik_client/configuration.py
--rw-r--r--   0        0        0     5934 2024-04-04 14:00:05.111852 authentik_client-2024.2.2.post1712239192/authentik_client/exceptions.py
--rw-r--r--   0        0        0    45495 2024-04-04 14:00:05.107852 authentik_client-2024.2.2.post1712239192/authentik_client/models/__init__.py
--rw-r--r--   0        0        0     4513 2024-04-04 14:00:01.887801 authentik_client-2024.2.2.post1712239192/authentik_client/models/access_denied_challenge.py
--rw-r--r--   0        0        0     2482 2024-04-04 14:00:01.903802 authentik_client-2024.2.2.post1712239192/authentik_client/models/app.py
--rw-r--r--   0        0        0     4168 2024-04-04 14:00:01.907802 authentik_client-2024.2.2.post1712239192/authentik_client/models/app_enum.py
--rw-r--r--   0        0        0     2702 2024-04-04 14:00:01.919802 authentik_client-2024.2.2.post1712239192/authentik_client/models/apple_challenge_response_request.py
--rw-r--r--   0        0        0     4508 2024-04-04 14:00:01.931802 authentik_client-2024.2.2.post1712239192/authentik_client/models/apple_login_challenge.py
--rw-r--r--   0        0        0     6686 2024-04-04 14:00:01.939802 authentik_client-2024.2.2.post1712239192/authentik_client/models/application.py
--rw-r--r--   0        0        0     4473 2024-04-04 14:00:01.947802 authentik_client-2024.2.2.post1712239192/authentik_client/models/application_request.py
--rw-r--r--   0        0        0      711 2024-04-04 14:00:01.955802 authentik_client-2024.2.2.post1712239192/authentik_client/models/auth_mode_enum.py
--rw-r--r--   0        0        0      709 2024-04-04 14:00:01.959802 authentik_client-2024.2.2.post1712239192/authentik_client/models/auth_type_enum.py
--rw-r--r--   0        0        0     6061 2024-04-04 14:00:01.963802 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticate_web_authn_stage.py
--rw-r--r--   0        0        0     5130 2024-04-04 14:00:01.971803 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticate_web_authn_stage_request.py
--rw-r--r--   0        0        0     4984 2024-04-04 14:00:01.979803 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session.py
--rw-r--r--   0        0        0     3064 2024-04-04 14:00:01.983803 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_asn.py
--rw-r--r--   0        0        0     2826 2024-04-04 14:00:01.991803 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_geo_ip.py
--rw-r--r--   0        0        0     3865 2024-04-04 14:00:01.995803 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_user_agent.py
--rw-r--r--   0        0        0     2646 2024-04-04 14:00:02.003803 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_user_agent_device.py
--rw-r--r--   0        0        0     2792 2024-04-04 14:00:02.007803 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_user_agent_os.py
--rw-r--r--   0        0        0     2725 2024-04-04 14:00:02.015803 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_user_agent_user_agent.py
--rw-r--r--   0        0        0      895 2024-04-04 14:00:02.019803 authentik_client-2024.2.2.post1712239192/authentik_client/models/authentication_enum.py
--rw-r--r--   0        0        0      782 2024-04-04 14:00:02.019803 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_attachment_enum.py
--rw-r--r--   0        0        0     4686 2024-04-04 14:00:02.027804 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_challenge.py
--rw-r--r--   0        0        0     2743 2024-04-04 14:00:02.031804 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_challenge_response_request.py
--rw-r--r--   0        0        0     5327 2024-04-04 14:00:02.047804 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_stage.py
--rw-r--r--   0        0        0     2768 2024-04-04 14:00:02.051804 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_stage_device_import_response.py
--rw-r--r--   0        0        0     2785 2024-04-04 14:00:02.055804 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
--rw-r--r--   0        0        0     4744 2024-04-04 14:00:02.063804 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-04 14:00:02.071804 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_sms_challenge.py
--rw-r--r--   0        0        0     3022 2024-04-04 14:00:02.075804 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_sms_challenge_response_request.py
--rw-r--r--   0        0        0     6409 2024-04-04 14:00:02.083804 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_sms_stage.py
--rw-r--r--   0        0        0     5595 2024-04-04 14:00:02.087804 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4474 2024-04-04 14:00:02.095805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_static_challenge.py
--rw-r--r--   0        0        0     2761 2024-04-04 14:00:02.099805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_static_challenge_response_request.py
--rw-r--r--   0        0        0     5363 2024-04-04 14:00:02.103805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_static_stage.py
--rw-r--r--   0        0        0     4392 2024-04-04 14:00:02.111805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4468 2024-04-04 14:00:02.115805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_totp_challenge.py
--rw-r--r--   0        0        0     2858 2024-04-04 14:00:02.119805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_totp_challenge_response_request.py
--rw-r--r--   0        0        0     5132 2024-04-04 14:00:02.127805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_totp_stage.py
--rw-r--r--   0        0        0     4201 2024-04-04 14:00:02.131805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     5636 2024-04-04 14:00:02.135805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_validate_stage.py
--rw-r--r--   0        0        0     4705 2024-04-04 14:00:02.143805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5717 2024-04-04 14:00:02.147805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_validation_challenge.py
--rw-r--r--   0        0        0     3805 2024-04-04 14:00:02.155805 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_validation_challenge_response_request.py
--rw-r--r--   0        0        0     4499 2024-04-04 14:00:02.159806 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_web_authn_challenge.py
--rw-r--r--   0        0        0     2852 2024-04-04 14:00:02.163806 authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_web_authn_challenge_response_request.py
--rw-r--r--   0        0        0     2718 2024-04-04 14:00:02.167806 authentik_client-2024.2.2.post1712239192/authentik_client/models/auto_submit_challenge_response_request.py
--rw-r--r--   0        0        0     4388 2024-04-04 14:00:02.175806 authentik_client-2024.2.2.post1712239192/authentik_client/models/autosubmit_challenge.py
--rw-r--r--   0        0        0      950 2024-04-04 14:00:02.175806 authentik_client-2024.2.2.post1712239192/authentik_client/models/backends_enum.py
--rw-r--r--   0        0        0      748 2024-04-04 14:00:02.179806 authentik_client-2024.2.2.post1712239192/authentik_client/models/binding_type_enum.py
--rw-r--r--   0        0        0     2995 2024-04-04 14:00:02.183806 authentik_client-2024.2.2.post1712239192/authentik_client/models/blueprint_file.py
--rw-r--r--   0        0        0     4453 2024-04-04 14:00:02.187806 authentik_client-2024.2.2.post1712239192/authentik_client/models/blueprint_instance.py
--rw-r--r--   0        0        0     3208 2024-04-04 14:00:02.191806 authentik_client-2024.2.2.post1712239192/authentik_client/models/blueprint_instance_request.py
--rw-r--r--   0        0        0      836 2024-04-04 14:00:02.195806 authentik_client-2024.2.2.post1712239192/authentik_client/models/blueprint_instance_status_enum.py
--rw-r--r--   0        0        0     6255 2024-04-04 14:00:02.199806 authentik_client-2024.2.2.post1712239192/authentik_client/models/brand.py
--rw-r--r--   0        0        0     6307 2024-04-04 14:00:02.203806 authentik_client-2024.2.2.post1712239192/authentik_client/models/brand_request.py
--rw-r--r--   0        0        0     2501 2024-04-04 14:00:02.207806 authentik_client-2024.2.2.post1712239192/authentik_client/models/cache.py
--rw-r--r--   0        0        0      875 2024-04-04 14:00:02.211806 authentik_client-2024.2.2.post1712239192/authentik_client/models/capabilities_enum.py
--rw-r--r--   0        0        0     4476 2024-04-04 14:00:02.215807 authentik_client-2024.2.2.post1712239192/authentik_client/models/captcha_challenge.py
--rw-r--r--   0        0        0     2797 2024-04-04 14:00:02.219807 authentik_client-2024.2.2.post1712239192/authentik_client/models/captcha_challenge_response_request.py
--rw-r--r--   0        0        0     4438 2024-04-04 14:00:02.223807 authentik_client-2024.2.2.post1712239192/authentik_client/models/captcha_stage.py
--rw-r--r--   0        0        0     3774 2024-04-04 14:00:02.227807 authentik_client-2024.2.2.post1712239192/authentik_client/models/captcha_stage_request.py
--rw-r--r--   0        0        0     2522 2024-04-04 14:00:02.231807 authentik_client-2024.2.2.post1712239192/authentik_client/models/certificate_data.py
--rw-r--r--   0        0        0     2861 2024-04-04 14:00:02.235807 authentik_client-2024.2.2.post1712239192/authentik_client/models/certificate_generation_request.py
--rw-r--r--   0        0        0     6655 2024-04-04 14:00:02.239807 authentik_client-2024.2.2.post1712239192/authentik_client/models/certificate_key_pair.py
--rw-r--r--   0        0        0     2989 2024-04-04 14:00:02.247807 authentik_client-2024.2.2.post1712239192/authentik_client/models/certificate_key_pair_request.py
--rw-r--r--   0        0        0      747 2024-04-04 14:00:02.247807 authentik_client-2024.2.2.post1712239192/authentik_client/models/challenge_choices.py
--rw-r--r--   0        0        0    24236 2024-04-04 14:00:02.255807 authentik_client-2024.2.2.post1712239192/authentik_client/models/challenge_types.py
--rw-r--r--   0        0        0      729 2024-04-04 14:00:02.259807 authentik_client-2024.2.2.post1712239192/authentik_client/models/client_type_enum.py
--rw-r--r--   0        0        0     3539 2024-04-04 14:00:02.263807 authentik_client-2024.2.2.post1712239192/authentik_client/models/config.py
--rw-r--r--   0        0        0     4021 2024-04-04 14:00:02.271807 authentik_client-2024.2.2.post1712239192/authentik_client/models/connection_token.py
--rw-r--r--   0        0        0     2662 2024-04-04 14:00:02.275807 authentik_client-2024.2.2.post1712239192/authentik_client/models/connection_token_request.py
--rw-r--r--   0        0        0     5736 2024-04-04 14:00:02.279807 authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_challenge.py
--rw-r--r--   0        0        0     2838 2024-04-04 14:00:02.283808 authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_challenge_response_request.py
--rw-r--r--   0        0        0     2513 2024-04-04 14:00:02.287808 authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_permission.py
--rw-r--r--   0        0        0     4511 2024-04-04 14:00:02.295808 authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_stage.py
--rw-r--r--   0        0        0      783 2024-04-04 14:00:02.295808 authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_stage_mode_enum.py
--rw-r--r--   0        0        0     3569 2024-04-04 14:00:02.299808 authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_stage_request.py
--rw-r--r--   0        0        0     2891 2024-04-04 14:00:02.307808 authentik_client-2024.2.2.post1712239192/authentik_client/models/contextual_flow_info.py
--rw-r--r--   0        0        0      879 2024-04-04 14:00:02.307808 authentik_client-2024.2.2.post1712239192/authentik_client/models/contextual_flow_info_layout_enum.py
--rw-r--r--   0        0        0     2657 2024-04-04 14:00:02.311808 authentik_client-2024.2.2.post1712239192/authentik_client/models/coordinate.py
--rw-r--r--   0        0        0     4704 2024-04-04 14:00:02.319808 authentik_client-2024.2.2.post1712239192/authentik_client/models/current_brand.py
--rw-r--r--   0        0        0      771 2024-04-04 14:00:02.319808 authentik_client-2024.2.2.post1712239192/authentik_client/models/denied_action_enum.py
--rw-r--r--   0        0        0     4200 2024-04-04 14:00:02.331808 authentik_client-2024.2.2.post1712239192/authentik_client/models/deny_stage.py
--rw-r--r--   0        0        0     3230 2024-04-04 14:00:02.335808 authentik_client-2024.2.2.post1712239192/authentik_client/models/deny_stage_request.py
--rw-r--r--   0        0        0     3522 2024-04-04 14:00:02.339809 authentik_client-2024.2.2.post1712239192/authentik_client/models/device.py
--rw-r--r--   0        0        0     2657 2024-04-04 14:00:02.343809 authentik_client-2024.2.2.post1712239192/authentik_client/models/device_challenge.py
--rw-r--r--   0        0        0     2792 2024-04-04 14:00:02.351809 authentik_client-2024.2.2.post1712239192/authentik_client/models/device_challenge_request.py
--rw-r--r--   0        0        0      780 2024-04-04 14:00:02.351809 authentik_client-2024.2.2.post1712239192/authentik_client/models/device_classes_enum.py
--rw-r--r--   0        0        0     1244 2024-04-04 14:00:02.355809 authentik_client-2024.2.2.post1712239192/authentik_client/models/digest_algorithm_enum.py
--rw-r--r--   0        0        0      695 2024-04-04 14:00:02.359809 authentik_client-2024.2.2.post1712239192/authentik_client/models/digits_enum.py
--rw-r--r--   0        0        0     4969 2024-04-04 14:00:02.363809 authentik_client-2024.2.2.post1712239192/authentik_client/models/docker_service_connection.py
--rw-r--r--   0        0        0     4087 2024-04-04 14:00:02.367809 authentik_client-2024.2.2.post1712239192/authentik_client/models/docker_service_connection_request.py
--rw-r--r--   0        0        0     2847 2024-04-04 14:00:02.371809 authentik_client-2024.2.2.post1712239192/authentik_client/models/domain.py
--rw-r--r--   0        0        0     2746 2024-04-04 14:00:02.375809 authentik_client-2024.2.2.post1712239192/authentik_client/models/domain_request.py
--rw-r--r--   0        0        0     4155 2024-04-04 14:00:02.379809 authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_challenge.py
--rw-r--r--   0        0        0     2681 2024-04-04 14:00:02.383809 authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_challenge_response_request.py
--rw-r--r--   0        0        0     4515 2024-04-04 14:00:02.387809 authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_policy.py
--rw-r--r--   0        0        0     3237 2024-04-04 14:00:02.387809 authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_policy_request.py
--rw-r--r--   0        0        0     4213 2024-04-04 14:00:02.395809 authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_stage.py
--rw-r--r--   0        0        0     3232 2024-04-04 14:00:02.395809 authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_stage_request.py
--rw-r--r--   0        0        0     2720 2024-04-04 14:00:02.399809 authentik_client-2024.2.2.post1712239192/authentik_client/models/duo_device.py
--rw-r--r--   0        0        0     2575 2024-04-04 14:00:02.403809 authentik_client-2024.2.2.post1712239192/authentik_client/models/duo_device_enrollment_status.py
--rw-r--r--   0        0        0     2619 2024-04-04 14:00:02.407810 authentik_client-2024.2.2.post1712239192/authentik_client/models/duo_device_request.py
--rw-r--r--   0        0        0      748 2024-04-04 14:00:02.411810 authentik_client-2024.2.2.post1712239192/authentik_client/models/duo_response_enum.py
--rw-r--r--   0        0        0     4090 2024-04-04 14:00:02.415810 authentik_client-2024.2.2.post1712239192/authentik_client/models/email_challenge.py
--rw-r--r--   0        0        0     2770 2024-04-04 14:00:02.427810 authentik_client-2024.2.2.post1712239192/authentik_client/models/email_challenge_response_request.py
--rw-r--r--   0        0        0     5902 2024-04-04 14:00:02.431810 authentik_client-2024.2.2.post1712239192/authentik_client/models/email_stage.py
--rw-r--r--   0        0        0     5121 2024-04-04 14:00:02.439810 authentik_client-2024.2.2.post1712239192/authentik_client/models/email_stage_request.py
--rw-r--r--   0        0        0     4707 2024-04-04 14:00:02.447810 authentik_client-2024.2.2.post1712239192/authentik_client/models/endpoint.py
--rw-r--r--   0        0        0     3678 2024-04-04 14:00:02.455810 authentik_client-2024.2.2.post1712239192/authentik_client/models/endpoint_request.py
--rw-r--r--   0        0        0     2530 2024-04-04 14:00:02.459810 authentik_client-2024.2.2.post1712239192/authentik_client/models/error_detail.py
--rw-r--r--   0        0        0     3309 2024-04-04 14:00:02.463810 authentik_client-2024.2.2.post1712239192/authentik_client/models/error_reporting_config.py
--rw-r--r--   0        0        0     4129 2024-04-04 14:00:02.471810 authentik_client-2024.2.2.post1712239192/authentik_client/models/event.py
--rw-r--r--   0        0        0     1730 2024-04-04 14:00:02.475811 authentik_client-2024.2.2.post1712239192/authentik_client/models/event_actions.py
--rw-r--r--   0        0        0     6006 2024-04-04 14:00:02.479811 authentik_client-2024.2.2.post1712239192/authentik_client/models/event_matcher_policy.py
--rw-r--r--   0        0        0     4807 2024-04-04 14:00:02.487811 authentik_client-2024.2.2.post1712239192/authentik_client/models/event_matcher_policy_request.py
--rw-r--r--   0        0        0     3990 2024-04-04 14:00:02.491811 authentik_client-2024.2.2.post1712239192/authentik_client/models/event_request.py
--rw-r--r--   0        0        0     2697 2024-04-04 14:00:02.499811 authentik_client-2024.2.2.post1712239192/authentik_client/models/event_top_per_user.py
--rw-r--r--   0        0        0     3715 2024-04-04 14:00:02.503811 authentik_client-2024.2.2.post1712239192/authentik_client/models/expiring_base_grant_model.py
--rw-r--r--   0        0        0     4191 2024-04-04 14:00:02.511811 authentik_client-2024.2.2.post1712239192/authentik_client/models/expression_policy.py
--rw-r--r--   0        0        0     2992 2024-04-04 14:00:02.515811 authentik_client-2024.2.2.post1712239192/authentik_client/models/expression_policy_request.py
--rw-r--r--   0        0        0     4524 2024-04-04 14:00:02.523811 authentik_client-2024.2.2.post1712239192/authentik_client/models/extra_role_object_permission.py
--rw-r--r--   0        0        0     4524 2024-04-04 14:00:02.531812 authentik_client-2024.2.2.post1712239192/authentik_client/models/extra_user_object_permission.py
--rw-r--r--   0        0        0     2519 2024-04-04 14:00:02.535812 authentik_client-2024.2.2.post1712239192/authentik_client/models/file_path_request.py
--rw-r--r--   0        0        0     6047 2024-04-04 14:00:02.543812 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow.py
--rw-r--r--   0        0        0    25850 2024-04-04 14:00:02.547812 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_challenge_response_request.py
--rw-r--r--   0        0        0      934 2024-04-04 14:00:02.551812 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_designation_enum.py
--rw-r--r--   0        0        0     2533 2024-04-04 14:00:02.567812 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_diagram.py
--rw-r--r--   0        0        0     4505 2024-04-04 14:00:02.575812 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_error_challenge.py
--rw-r--r--   0        0        0     3111 2024-04-04 14:00:02.583812 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_import_result.py
--rw-r--r--   0        0        0     3418 2024-04-04 14:00:02.591812 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_inspection.py
--rw-r--r--   0        0        0     3875 2024-04-04 14:00:02.595812 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_inspector_plan.py
--rw-r--r--   0        0        0      837 2024-04-04 14:00:02.599813 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_layout_enum.py
--rw-r--r--   0        0        0     4741 2024-04-04 14:00:02.607813 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_request.py
--rw-r--r--   0        0        0     5223 2024-04-04 14:00:02.615813 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_set.py
--rw-r--r--   0        0        0     4459 2024-04-04 14:00:02.623813 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_set_request.py
--rw-r--r--   0        0        0     4763 2024-04-04 14:00:02.627813 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_stage_binding.py
--rw-r--r--   0        0        0     3983 2024-04-04 14:00:02.635813 authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_stage_binding_request.py
--rw-r--r--   0        0        0     2641 2024-04-04 14:00:02.639813 authentik_client-2024.2.2.post1712239192/authentik_client/models/footer_link.py
--rw-r--r--   0        0        0     2531 2024-04-04 14:00:02.647813 authentik_client-2024.2.2.post1712239192/authentik_client/models/generic_error.py
--rw-r--r--   0        0        0      865 2024-04-04 14:00:02.651813 authentik_client-2024.2.2.post1712239192/authentik_client/models/geoip_binding_enum.py
--rw-r--r--   0        0        0     5216 2024-04-04 14:00:02.655813 authentik_client-2024.2.2.post1712239192/authentik_client/models/group.py
--rw-r--r--   0        0        0     4209 2024-04-04 14:00:02.663813 authentik_client-2024.2.2.post1712239192/authentik_client/models/group_member.py
--rw-r--r--   0        0        0     4006 2024-04-04 14:00:02.671814 authentik_client-2024.2.2.post1712239192/authentik_client/models/group_member_request.py
--rw-r--r--   0        0        0     3347 2024-04-04 14:00:02.679814 authentik_client-2024.2.2.post1712239192/authentik_client/models/group_request.py
--rw-r--r--   0        0        0     6080 2024-04-04 14:00:02.683814 authentik_client-2024.2.2.post1712239192/authentik_client/models/identification_challenge.py
--rw-r--r--   0        0        0     3174 2024-04-04 14:00:02.691814 authentik_client-2024.2.2.post1712239192/authentik_client/models/identification_challenge_response_request.py
--rw-r--r--   0        0        0     7503 2024-04-04 14:00:02.699814 authentik_client-2024.2.2.post1712239192/authentik_client/models/identification_stage.py
--rw-r--r--   0        0        0     6533 2024-04-04 14:00:02.707814 authentik_client-2024.2.2.post1712239192/authentik_client/models/identification_stage_request.py
--rw-r--r--   0        0        0     2438 2024-04-04 14:00:02.711814 authentik_client-2024.2.2.post1712239192/authentik_client/models/install_id.py
--rw-r--r--   0        0        0      771 2024-04-04 14:00:02.715814 authentik_client-2024.2.2.post1712239192/authentik_client/models/intent_enum.py
--rw-r--r--   0        0        0      800 2024-04-04 14:00:02.719814 authentik_client-2024.2.2.post1712239192/authentik_client/models/invalid_response_action_enum.py
--rw-r--r--   0        0        0     4667 2024-04-04 14:00:02.723815 authentik_client-2024.2.2.post1712239192/authentik_client/models/invitation.py
--rw-r--r--   0        0        0     3684 2024-04-04 14:00:02.731815 authentik_client-2024.2.2.post1712239192/authentik_client/models/invitation_request.py
--rw-r--r--   0        0        0     4508 2024-04-04 14:00:02.739815 authentik_client-2024.2.2.post1712239192/authentik_client/models/invitation_stage.py
--rw-r--r--   0        0        0     3527 2024-04-04 14:00:02.747815 authentik_client-2024.2.2.post1712239192/authentik_client/models/invitation_stage_request.py
--rw-r--r--   0        0        0      729 2024-04-04 14:00:02.747815 authentik_client-2024.2.2.post1712239192/authentik_client/models/issuer_mode_enum.py
--rw-r--r--   0        0        0     4386 2024-04-04 14:00:02.755815 authentik_client-2024.2.2.post1712239192/authentik_client/models/kubernetes_service_connection.py
--rw-r--r--   0        0        0     3454 2024-04-04 14:00:02.759815 authentik_client-2024.2.2.post1712239192/authentik_client/models/kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     2811 2024-04-04 14:00:02.767815 authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_debug.py
--rw-r--r--   0        0        0     5765 2024-04-04 14:00:02.775815 authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_outpost_config.py
--rw-r--r--   0        0        0     4378 2024-04-04 14:00:02.779815 authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_property_mapping.py
--rw-r--r--   0        0        0     3478 2024-04-04 14:00:02.783815 authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_property_mapping_request.py
--rw-r--r--   0        0        0     8694 2024-04-04 14:00:02.787815 authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_provider.py
--rw-r--r--   0        0        0     6192 2024-04-04 14:00:02.791816 authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_provider_request.py
--rw-r--r--   0        0        0    11791 2024-04-04 14:00:02.795816 authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_source.py
--rw-r--r--   0        0        0     9542 2024-04-04 14:00:02.799816 authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_source_request.py
--rw-r--r--   0        0        0     3129 2024-04-04 14:00:02.803816 authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_sync_status.py
--rw-r--r--   0        0        0      726 2024-04-04 14:00:02.763815 authentik_client-2024.2.2.post1712239192/authentik_client/models/ldapapi_access_mode.py
--rw-r--r--   0        0        0     3278 2024-04-04 14:00:02.807816 authentik_client-2024.2.2.post1712239192/authentik_client/models/license.py
--rw-r--r--   0        0        0     2897 2024-04-04 14:00:02.811816 authentik_client-2024.2.2.post1712239192/authentik_client/models/license_forecast.py
--rw-r--r--   0        0        0     2509 2024-04-04 14:00:02.815816 authentik_client-2024.2.2.post1712239192/authentik_client/models/license_request.py
--rw-r--r--   0        0        0     3222 2024-04-04 14:00:02.819816 authentik_client-2024.2.2.post1712239192/authentik_client/models/license_summary.py
--rw-r--r--   0        0        0     2411 2024-04-04 14:00:02.819816 authentik_client-2024.2.2.post1712239192/authentik_client/models/link.py
--rw-r--r--   0        0        0     2882 2024-04-04 14:00:02.823816 authentik_client-2024.2.2.post1712239192/authentik_client/models/log_event.py
--rw-r--r--   0        0        0      843 2024-04-04 14:00:02.827816 authentik_client-2024.2.2.post1712239192/authentik_client/models/log_level_enum.py
--rw-r--r--   0        0        0     6520 2024-04-04 14:00:02.831816 authentik_client-2024.2.2.post1712239192/authentik_client/models/login_challenge_types.py
--rw-r--r--   0        0        0     4171 2024-04-04 14:00:02.835816 authentik_client-2024.2.2.post1712239192/authentik_client/models/login_metrics.py
--rw-r--r--   0        0        0     3192 2024-04-04 14:00:02.839816 authentik_client-2024.2.2.post1712239192/authentik_client/models/login_source.py
--rw-r--r--   0        0        0     2513 2024-04-04 14:00:02.843816 authentik_client-2024.2.2.post1712239192/authentik_client/models/metadata.py
--rw-r--r--   0        0        0     7522 2024-04-04 14:00:02.843816 authentik_client-2024.2.2.post1712239192/authentik_client/models/model_enum.py
--rw-r--r--   0        0        0     9828 2024-04-04 14:00:02.847816 authentik_client-2024.2.2.post1712239192/authentik_client/models/model_request.py
--rw-r--r--   0        0        0     1559 2024-04-04 14:00:02.851817 authentik_client-2024.2.2.post1712239192/authentik_client/models/name_id_policy_enum.py
--rw-r--r--   0        0        0      831 2024-04-04 14:00:02.855816 authentik_client-2024.2.2.post1712239192/authentik_client/models/network_binding_enum.py
--rw-r--r--   0        0        0      764 2024-04-04 14:00:02.855816 authentik_client-2024.2.2.post1712239192/authentik_client/models/not_configured_action_enum.py
--rw-r--r--   0        0        0     3479 2024-04-04 14:00:02.859817 authentik_client-2024.2.2.post1712239192/authentik_client/models/notification.py
--rw-r--r--   0        0        0     2858 2024-04-04 14:00:02.863817 authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_request.py
--rw-r--r--   0        0        0     4010 2024-04-04 14:00:02.867817 authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_rule.py
--rw-r--r--   0        0        0     3549 2024-04-04 14:00:02.871817 authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_rule_request.py
--rw-r--r--   0        0        0     3760 2024-04-04 14:00:02.875817 authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_transport.py
--rw-r--r--   0        0        0      818 2024-04-04 14:00:02.875817 authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_transport_mode_enum.py
--rw-r--r--   0        0        0     3500 2024-04-04 14:00:02.879817 authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_transport_request.py
--rw-r--r--   0        0        0     2503 2024-04-04 14:00:02.883817 authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_transport_test.py
--rw-r--r--   0        0        0     2707 2024-04-04 14:00:02.891817 authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_webhook_mapping.py
--rw-r--r--   0        0        0     2717 2024-04-04 14:00:02.895817 authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     8888 2024-04-04 14:00:02.899817 authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth2_provider.py
--rw-r--r--   0        0        0     6654 2024-04-04 14:00:02.903817 authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth2_provider_request.py
--rw-r--r--   0        0        0     3482 2024-04-04 14:00:02.907817 authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth2_provider_setup_urls.py
--rw-r--r--   0        0        0     4164 2024-04-04 14:00:02.911817 authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_device_code_challenge.py
--rw-r--r--   0        0        0     2846 2024-04-04 14:00:02.911817 authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_device_code_challenge_response_request.py
--rw-r--r--   0        0        0     4213 2024-04-04 14:00:02.919818 authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_device_code_finish_challenge.py
--rw-r--r--   0        0        0     2816 2024-04-04 14:00:02.919818 authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
--rw-r--r--   0        0        0    10563 2024-04-04 14:00:02.927818 authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_source.py
--rw-r--r--   0        0        0     8069 2024-04-04 14:00:02.931818 authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_source_request.py
--rw-r--r--   0        0        0     3922 2024-04-04 14:00:02.935818 authentik_client-2024.2.2.post1712239192/authentik_client/models/open_id_connect_configuration.py
--rw-r--r--   0        0        0     5545 2024-04-04 14:00:02.939818 authentik_client-2024.2.2.post1712239192/authentik_client/models/outpost.py
--rw-r--r--   0        0        0     2541 2024-04-04 14:00:02.939818 authentik_client-2024.2.2.post1712239192/authentik_client/models/outpost_default_config.py
--rw-r--r--   0        0        0     3755 2024-04-04 14:00:02.943818 authentik_client-2024.2.2.post1712239192/authentik_client/models/outpost_health.py
--rw-r--r--   0        0        0     4050 2024-04-04 14:00:02.947818 authentik_client-2024.2.2.post1712239192/authentik_client/models/outpost_request.py
--rw-r--r--   0        0        0      752 2024-04-04 14:00:02.951818 authentik_client-2024.2.2.post1712239192/authentik_client/models/outpost_type_enum.py
--rw-r--r--   0        0        0     3322 2024-04-04 14:00:02.951818 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_application_list.py
--rw-r--r--   0        0        0     3437 2024-04-04 14:00:02.955818 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticate_web_authn_stage_list.py
--rw-r--r--   0        0        0     3395 2024-04-04 14:00:02.959818 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticated_session_list.py
--rw-r--r--   0        0        0     3404 2024-04-04 14:00:02.959818 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticator_duo_stage_list.py
--rw-r--r--   0        0        0     3404 2024-04-04 14:00:02.963818 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticator_sms_stage_list.py
--rw-r--r--   0        0        0     3428 2024-04-04 14:00:02.967818 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticator_static_stage_list.py
--rw-r--r--   0        0        0     3412 2024-04-04 14:00:02.971818 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticator_totp_stage_list.py
--rw-r--r--   0        0        0     3444 2024-04-04 14:00:02.975818 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticator_validate_stage_list.py
--rw-r--r--   0        0        0     3371 2024-04-04 14:00:02.975818 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_blueprint_instance_list.py
--rw-r--r--   0        0        0     3274 2024-04-04 14:00:02.979818 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_brand_list.py
--rw-r--r--   0        0        0     3331 2024-04-04 14:00:02.983819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_captcha_stage_list.py
--rw-r--r--   0        0        0     3380 2024-04-04 14:00:02.987819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_certificate_key_pair_list.py
--rw-r--r--   0        0        0     3355 2024-04-04 14:00:02.991819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_connection_token_list.py
--rw-r--r--   0        0        0     3331 2024-04-04 14:00:02.991819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_consent_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-04 14:00:02.995819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_deny_stage_list.py
--rw-r--r--   0        0        0     3420 2024-04-04 14:00:02.999819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_docker_service_connection_list.py
--rw-r--r--   0        0        0     3282 2024-04-04 14:00:03.003819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_domain_list.py
--rw-r--r--   0        0        0     3323 2024-04-04 14:00:03.007819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_dummy_policy_list.py
--rw-r--r--   0        0        0     3315 2024-04-04 14:00:03.011819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_dummy_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-04 14:00:03.015819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_duo_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-04 14:00:03.015819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_email_stage_list.py
--rw-r--r--   0        0        0     3298 2024-04-04 14:00:03.019819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_endpoint_list.py
--rw-r--r--   0        0        0     3274 2024-04-04 14:00:03.023819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_event_list.py
--rw-r--r--   0        0        0     3380 2024-04-04 14:00:03.023819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_event_matcher_policy_list.py
--rw-r--r--   0        0        0     3413 2024-04-04 14:00:03.027819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_expiring_base_grant_model_list.py
--rw-r--r--   0        0        0     3363 2024-04-04 14:00:03.031819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_expression_policy_list.py
--rw-r--r--   0        0        0     3437 2024-04-04 14:00:03.031819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_extra_role_object_permission_list.py
--rw-r--r--   0        0        0     3437 2024-04-04 14:00:03.035819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_extra_user_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-04 14:00:03.039820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_flow_list.py
--rw-r--r--   0        0        0     3364 2024-04-04 14:00:03.039820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_flow_stage_binding_list.py
--rw-r--r--   0        0        0     3274 2024-04-04 14:00:03.043820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_group_list.py
--rw-r--r--   0        0        0     3387 2024-04-04 14:00:03.047819 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_identification_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-04 14:00:03.051820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_invitation_list.py
--rw-r--r--   0        0        0     3355 2024-04-04 14:00:03.055820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_invitation_stage_list.py
--rw-r--r--   0        0        0     3452 2024-04-04 14:00:03.059820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_kubernetes_service_connection_list.py
--rw-r--r--   0        0        0     3372 2024-04-04 14:00:03.063820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_ldap_outpost_config_list.py
--rw-r--r--   0        0        0     3388 2024-04-04 14:00:03.063820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_ldap_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-04 14:00:03.067820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_ldap_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-04 14:00:03.071820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_ldap_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-04 14:00:03.075820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_license_list.py
--rw-r--r--   0        0        0     3330 2024-04-04 14:00:03.079820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_notification_list.py
--rw-r--r--   0        0        0     3363 2024-04-04 14:00:03.083820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_notification_rule_list.py
--rw-r--r--   0        0        0     3403 2024-04-04 14:00:03.083820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_notification_transport_list.py
--rw-r--r--   0        0        0     3444 2024-04-04 14:00:03.087820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_notification_webhook_mapping_list.py
--rw-r--r--   0        0        0     3348 2024-04-04 14:00:03.091820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_o_auth2_provider_list.py
--rw-r--r--   0        0        0     3324 2024-04-04 14:00:03.095820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_o_auth_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-04 14:00:03.099820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_outpost_list.py
--rw-r--r--   0        0        0     3396 2024-04-04 14:00:03.103820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_password_expiry_policy_list.py
--rw-r--r--   0        0        0     3347 2024-04-04 14:00:03.103820 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_password_policy_list.py
--rw-r--r--   0        0        0     3339 2024-04-04 14:00:03.107821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_password_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-04 14:00:03.111821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_permission_list.py
--rw-r--r--   0        0        0     3396 2024-04-04 14:00:03.115821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_plex_source_connection_list.py
--rw-r--r--   0        0        0     3315 2024-04-04 14:00:03.119821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_plex_source_list.py
--rw-r--r--   0        0        0     3339 2024-04-04 14:00:03.123821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_policy_binding_list.py
--rw-r--r--   0        0        0     3282 2024-04-04 14:00:03.127821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_policy_list.py
--rw-r--r--   0        0        0     3282 2024-04-04 14:00:03.127821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_prompt_list.py
--rw-r--r--   0        0        0     3323 2024-04-04 14:00:03.131821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_prompt_stage_list.py
--rw-r--r--   0        0        0     3355 2024-04-04 14:00:03.135821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_property_mapping_list.py
--rw-r--r--   0        0        0     3298 2024-04-04 14:00:03.139821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-04 14:00:03.143821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_proxy_outpost_config_list.py
--rw-r--r--   0        0        0     3339 2024-04-04 14:00:03.147821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_proxy_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-04 14:00:03.147821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_rac_property_mapping_list.py
--rw-r--r--   0        0        0     3323 2024-04-04 14:00:03.151821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_rac_provider_list.py
--rw-r--r--   0        0        0     3388 2024-04-04 14:00:03.155821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_radius_outpost_config_list.py
--rw-r--r--   0        0        0     3347 2024-04-04 14:00:03.159821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_radius_provider_list.py
--rw-r--r--   0        0        0     3314 2024-04-04 14:00:03.163821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_reputation_list.py
--rw-r--r--   0        0        0     3363 2024-04-04 14:00:03.167822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_reputation_policy_list.py
--rw-r--r--   0        0        0     3461 2024-04-04 14:00:03.167822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_role_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-04 14:00:03.171821 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_role_list.py
--rw-r--r--   0        0        0     3388 2024-04-04 14:00:03.179822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_saml_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-04 14:00:03.183822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_saml_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-04 14:00:03.187822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_saml_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-04 14:00:03.191822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_scim_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-04 14:00:03.195822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_scim_provider_list.py
--rw-r--r--   0        0        0     3331 2024-04-04 14:00:03.199822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_scope_mapping_list.py
--rw-r--r--   0        0        0     3371 2024-04-04 14:00:03.203822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_service_connection_list.py
--rw-r--r--   0        0        0     3307 2024-04-04 14:00:03.199822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_sms_device_list.py
--rw-r--r--   0        0        0     3282 2024-04-04 14:00:03.207822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-04 14:00:03.211822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_source_stage_list.py
--rw-r--r--   0        0        0     3274 2024-04-04 14:00:03.215822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_stage_list.py
--rw-r--r--   0        0        0     3331 2024-04-04 14:00:03.219822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_static_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-04 14:00:03.223822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_system_task_list.py
--rw-r--r--   0        0        0     3282 2024-04-04 14:00:03.227822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_tenant_list.py
--rw-r--r--   0        0        0     3274 2024-04-04 14:00:03.231823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_token_list.py
--rw-r--r--   0        0        0     3315 2024-04-04 14:00:03.235823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_token_model_list.py
--rw-r--r--   0        0        0     3315 2024-04-04 14:00:03.223822 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_totp_device_list.py
--rw-r--r--   0        0        0     3461 2024-04-04 14:00:03.239823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3323 2024-04-04 14:00:03.243823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_consent_list.py
--rw-r--r--   0        0        0     3356 2024-04-04 14:00:03.247823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_delete_stage_list.py
--rw-r--r--   0        0        0     3266 2024-04-04 14:00:03.247823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_list.py
--rw-r--r--   0        0        0     3348 2024-04-04 14:00:03.251823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_login_stage_list.py
--rw-r--r--   0        0        0     3356 2024-04-04 14:00:03.255823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_logout_stage_list.py
--rw-r--r--   0        0        0     3438 2024-04-04 14:00:03.259823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_o_auth_source_connection_list.py
--rw-r--r--   0        0        0     3429 2024-04-04 14:00:03.263823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_saml_source_connection_list.py
--rw-r--r--   0        0        0     3396 2024-04-04 14:00:03.263823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_source_connection_list.py
--rw-r--r--   0        0        0     3348 2024-04-04 14:00:03.267823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_write_stage_list.py
--rw-r--r--   0        0        0     3348 2024-04-04 14:00:03.271823 authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_web_authn_device_list.py
--rw-r--r--   0        0        0     3076 2024-04-04 14:00:03.275823 authentik_client-2024.2.2.post1712239192/authentik_client/models/pagination.py
--rw-r--r--   0        0        0     4454 2024-04-04 14:00:03.279823 authentik_client-2024.2.2.post1712239192/authentik_client/models/password_challenge.py
--rw-r--r--   0        0        0     2819 2024-04-04 14:00:03.279823 authentik_client-2024.2.2.post1712239192/authentik_client/models/password_challenge_response_request.py
--rw-r--r--   0        0        0     4377 2024-04-04 14:00:03.283823 authentik_client-2024.2.2.post1712239192/authentik_client/models/password_expiry_policy.py
--rw-r--r--   0        0        0     3099 2024-04-04 14:00:03.287823 authentik_client-2024.2.2.post1712239192/authentik_client/models/password_expiry_policy_request.py
--rw-r--r--   0        0        0     6428 2024-04-04 14:00:03.287823 authentik_client-2024.2.2.post1712239192/authentik_client/models/password_policy.py
--rw-r--r--   0        0        0     5239 2024-04-04 14:00:03.291823 authentik_client-2024.2.2.post1712239192/authentik_client/models/password_policy_request.py
--rw-r--r--   0        0        0     5274 2024-04-04 14:00:03.295823 authentik_client-2024.2.2.post1712239192/authentik_client/models/password_stage.py
--rw-r--r--   0        0        0     4264 2024-04-04 14:00:03.295823 authentik_client-2024.2.2.post1712239192/authentik_client/models/password_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-04 14:00:03.299824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_application_request.py
--rw-r--r--   0        0        0     5168 2024-04-04 14:00:03.303824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticate_web_authn_stage_request.py
--rw-r--r--   0        0        0     4833 2024-04-04 14:00:03.307824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     5701 2024-04-04 14:00:03.311824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4430 2024-04-04 14:00:03.311824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4256 2024-04-04 14:00:03.315824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     4743 2024-04-04 14:00:03.319824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     3246 2024-04-04 14:00:03.323824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_blueprint_instance_request.py
--rw-r--r--   0        0        0     6352 2024-04-04 14:00:03.323824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_brand_request.py
--rw-r--r--   0        0        0     3860 2024-04-04 14:00:03.327824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_captcha_stage_request.py
--rw-r--r--   0        0        0     3051 2024-04-04 14:00:03.331824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_certificate_key_pair_request.py
--rw-r--r--   0        0        0     2717 2024-04-04 14:00:03.331824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_connection_token_request.py
--rw-r--r--   0        0        0     3607 2024-04-04 14:00:03.335824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_consent_stage_request.py
--rw-r--r--   0        0        0     3268 2024-04-04 14:00:03.335824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_deny_stage_request.py
--rw-r--r--   0        0        0     4149 2024-04-04 14:00:03.339824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_docker_service_connection_request.py
--rw-r--r--   0        0        0     2801 2024-04-04 14:00:03.339824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_domain_request.py
--rw-r--r--   0        0        0     3275 2024-04-04 14:00:03.343824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_dummy_policy_request.py
--rw-r--r--   0        0        0     3270 2024-04-04 14:00:03.343824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_dummy_stage_request.py
--rw-r--r--   0        0        0     2674 2024-04-04 14:00:03.347824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_duo_device_request.py
--rw-r--r--   0        0        0     5159 2024-04-04 14:00:03.347824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_email_stage_request.py
--rw-r--r--   0        0        0     3784 2024-04-04 14:00:03.351824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_endpoint_request.py
--rw-r--r--   0        0        0     4845 2024-04-04 14:00:03.355824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_event_matcher_policy_request.py
--rw-r--r--   0        0        0     4045 2024-04-04 14:00:03.355824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_event_request.py
--rw-r--r--   0        0        0     3047 2024-04-04 14:00:03.359825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_expression_policy_request.py
--rw-r--r--   0        0        0     4903 2024-04-04 14:00:03.363824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_flow_request.py
--rw-r--r--   0        0        0     4055 2024-04-04 14:00:03.363824 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_flow_stage_binding_request.py
--rw-r--r--   0        0        0     3385 2024-04-04 14:00:03.367825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_group_request.py
--rw-r--r--   0        0        0     6571 2024-04-04 14:00:03.371825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_identification_stage_request.py
--rw-r--r--   0        0        0     3774 2024-04-04 14:00:03.375825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_invitation_request.py
--rw-r--r--   0        0        0     3565 2024-04-04 14:00:03.375825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_invitation_stage_request.py
--rw-r--r--   0        0        0     3492 2024-04-04 14:00:03.379825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     3550 2024-04-04 14:00:03.383825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_ldap_property_mapping_request.py
--rw-r--r--   0        0        0     6254 2024-04-04 14:00:03.383825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_ldap_provider_request.py
--rw-r--r--   0        0        0     9697 2024-04-04 14:00:03.387825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_ldap_source_request.py
--rw-r--r--   0        0        0     2557 2024-04-04 14:00:03.391825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_license_request.py
--rw-r--r--   0        0        0     2879 2024-04-04 14:00:03.395825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_notification_request.py
--rw-r--r--   0        0        0     3587 2024-04-04 14:00:03.399825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_notification_rule_request.py
--rw-r--r--   0        0        0     3538 2024-04-04 14:00:03.399825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_notification_transport_request.py
--rw-r--r--   0        0        0     2782 2024-04-04 14:00:03.403825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     6716 2024-04-04 14:00:03.407825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_o_auth2_provider_request.py
--rw-r--r--   0        0        0     8241 2024-04-04 14:00:03.407825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_o_auth_source_request.py
--rw-r--r--   0        0        0     4139 2024-04-04 14:00:03.411825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_outpost_request.py
--rw-r--r--   0        0        0     3154 2024-04-04 14:00:03.415825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_password_expiry_policy_request.py
--rw-r--r--   0        0        0     5277 2024-04-04 14:00:03.415825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_password_policy_request.py
--rw-r--r--   0        0        0     4326 2024-04-04 14:00:03.419825 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_password_stage_request.py
--rw-r--r--   0        0        0     2922 2024-04-04 14:00:03.423826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_permission_assign_request.py
--rw-r--r--   0        0        0     2784 2024-04-04 14:00:03.427826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_plex_source_connection_request.py
--rw-r--r--   0        0        0     5905 2024-04-04 14:00:03.431826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_plex_source_request.py
--rw-r--r--   0        0        0     4286 2024-04-04 14:00:03.431826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_policy_binding_request.py
--rw-r--r--   0        0        0     5023 2024-04-04 14:00:03.435826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_prompt_request.py
--rw-r--r--   0        0        0     3406 2024-04-04 14:00:03.439826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_prompt_stage_request.py
--rw-r--r--   0        0        0     6907 2024-04-04 14:00:03.443826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_proxy_provider_request.py
--rw-r--r--   0        0        0     3495 2024-04-04 14:00:03.443826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_rac_property_mapping_request.py
--rw-r--r--   0        0        0     4413 2024-04-04 14:00:03.451826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_rac_provider_request.py
--rw-r--r--   0        0        0     4563 2024-04-04 14:00:03.455826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_radius_provider_request.py
--rw-r--r--   0        0        0     3276 2024-04-04 14:00:03.459826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_reputation_policy_request.py
--rw-r--r--   0        0        0     2565 2024-04-04 14:00:03.459826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_role_request.py
--rw-r--r--   0        0        0     3901 2024-04-04 14:00:03.463826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_saml_property_mapping_request.py
--rw-r--r--   0        0        0     7539 2024-04-04 14:00:03.463826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_saml_provider_request.py
--rw-r--r--   0        0        0     8676 2024-04-04 14:00:03.467826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_saml_source_request.py
--rw-r--r--   0        0        0     3364 2024-04-04 14:00:03.467826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_scim_mapping_request.py
--rw-r--r--   0        0        0     3888 2024-04-04 14:00:03.471826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_scim_provider_request.py
--rw-r--r--   0        0        0     3819 2024-04-04 14:00:03.475826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_scope_mapping_request.py
--rw-r--r--   0        0        0     4590 2024-04-04 14:00:03.479826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_settings_request.py
--rw-r--r--   0        0        0     2674 2024-04-04 14:00:03.475826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_sms_device_request.py
--rw-r--r--   0        0        0     3562 2024-04-04 14:00:03.483826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_source_stage_request.py
--rw-r--r--   0        0        0     2686 2024-04-04 14:00:03.483826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_static_device_request.py
--rw-r--r--   0        0        0     2820 2024-04-04 14:00:03.491827 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_tenant_request.py
--rw-r--r--   0        0        0     4208 2024-04-04 14:00:03.495827 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_token_request.py
--rw-r--r--   0        0        0     2678 2024-04-04 14:00:03.487826 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_totp_device_request.py
--rw-r--r--   0        0        0     3167 2024-04-04 14:00:03.499827 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_delete_stage_request.py
--rw-r--r--   0        0        0     4766 2024-04-04 14:00:03.499827 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_login_stage_request.py
--rw-r--r--   0        0        0     3167 2024-04-04 14:00:03.503827 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_logout_stage_request.py
--rw-r--r--   0        0        0     3109 2024-04-04 14:00:03.507827 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3934 2024-04-04 14:00:03.511827 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_request.py
--rw-r--r--   0        0        0     2733 2024-04-04 14:00:03.515827 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_saml_source_connection_request.py
--rw-r--r--   0        0        0     4450 2024-04-04 14:00:03.519827 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_write_stage_request.py
--rw-r--r--   0        0        0     2625 2024-04-04 14:00:03.519827 authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_web_authn_device_request.py
--rw-r--r--   0        0        0     3548 2024-04-04 14:00:03.523827 authentik_client-2024.2.2.post1712239192/authentik_client/models/permission.py
--rw-r--r--   0        0        0     2884 2024-04-04 14:00:03.527827 authentik_client-2024.2.2.post1712239192/authentik_client/models/permission_assign_request.py
--rw-r--r--   0        0        0     4315 2024-04-04 14:00:03.531827 authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_authentication_challenge.py
--rw-r--r--   0        0        0     2726 2024-04-04 14:00:03.531827 authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_authentication_challenge_response_request.py
--rw-r--r--   0        0        0     7752 2024-04-04 14:00:03.535827 authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_source.py
--rw-r--r--   0        0        0     3265 2024-04-04 14:00:03.539827 authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_source_connection.py
--rw-r--r--   0        0        0     2719 2024-04-04 14:00:03.539827 authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_source_connection_request.py
--rw-r--r--   0        0        0     5760 2024-04-04 14:00:03.543827 authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_source_request.py
--rw-r--r--   0        0        0     2576 2024-04-04 14:00:03.547827 authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_token_redeem_request.py
--rw-r--r--   0        0        0     4055 2024-04-04 14:00:03.551828 authentik_client-2024.2.2.post1712239192/authentik_client/models/policy.py
--rw-r--r--   0        0        0     5643 2024-04-04 14:00:03.551828 authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_binding.py
--rw-r--r--   0        0        0     4231 2024-04-04 14:00:03.555827 authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_binding_request.py
--rw-r--r--   0        0        0      711 2024-04-04 14:00:03.555827 authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_engine_mode.py
--rw-r--r--   0        0        0     2817 2024-04-04 14:00:03.559828 authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_request.py
--rw-r--r--   0        0        0     2583 2024-04-04 14:00:03.563828 authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_test_request.py
--rw-r--r--   0        0        0     3281 2024-04-04 14:00:03.563828 authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_test_result.py
--rw-r--r--   0        0        0     4885 2024-04-04 14:00:03.567828 authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt.py
--rw-r--r--   0        0        0     4649 2024-04-04 14:00:03.571828 authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_challenge.py
--rw-r--r--   0        0        0     3325 2024-04-04 14:00:03.571828 authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_challenge_response_request.py
--rw-r--r--   0        0        0     4927 2024-04-04 14:00:03.575828 authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_request.py
--rw-r--r--   0        0        0     4321 2024-04-04 14:00:03.575828 authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_stage.py
--rw-r--r--   0        0        0     3351 2024-04-04 14:00:03.579828 authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_stage_request.py
--rw-r--r--   0        0        0     1185 2024-04-04 14:00:03.579828 authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_type_enum.py
--rw-r--r--   0        0        0     4264 2024-04-04 14:00:03.583828 authentik_client-2024.2.2.post1712239192/authentik_client/models/property_mapping.py
--rw-r--r--   0        0        0     2610 2024-04-04 14:00:03.587828 authentik_client-2024.2.2.post1712239192/authentik_client/models/property_mapping_preview.py
--rw-r--r--   0        0        0     2744 2024-04-04 14:00:03.587828 authentik_client-2024.2.2.post1712239192/authentik_client/models/property_mapping_test_result.py
--rw-r--r--   0        0        0      715 2024-04-04 14:00:03.591828 authentik_client-2024.2.2.post1712239192/authentik_client/models/protocol_enum.py
--rw-r--r--   0        0        0     5722 2024-04-04 14:00:03.591828 authentik_client-2024.2.2.post1712239192/authentik_client/models/provider.py
--rw-r--r--   0        0        0      713 2024-04-04 14:00:03.595828 authentik_client-2024.2.2.post1712239192/authentik_client/models/provider_enum.py
--rw-r--r--   0        0        0     1314 2024-04-04 14:00:03.595828 authentik_client-2024.2.2.post1712239192/authentik_client/models/provider_model_enum.py
--rw-r--r--   0        0        0     3397 2024-04-04 14:00:03.595828 authentik_client-2024.2.2.post1712239192/authentik_client/models/provider_request.py
--rw-r--r--   0        0        0     1009 2024-04-04 14:00:03.599828 authentik_client-2024.2.2.post1712239192/authentik_client/models/provider_type_enum.py
--rw-r--r--   0        0        0      754 2024-04-04 14:00:03.599828 authentik_client-2024.2.2.post1712239192/authentik_client/models/proxy_mode.py
--rw-r--r--   0        0        0     7819 2024-04-04 14:00:03.599828 authentik_client-2024.2.2.post1712239192/authentik_client/models/proxy_outpost_config.py
--rw-r--r--   0        0        0     9552 2024-04-04 14:00:03.603828 authentik_client-2024.2.2.post1712239192/authentik_client/models/proxy_provider.py
--rw-r--r--   0        0        0     6828 2024-04-04 14:00:03.603828 authentik_client-2024.2.2.post1712239192/authentik_client/models/proxy_provider_request.py
--rw-r--r--   0        0        0     4407 2024-04-04 14:00:03.607828 authentik_client-2024.2.2.post1712239192/authentik_client/models/rac_property_mapping.py
--rw-r--r--   0        0        0     3440 2024-04-04 14:00:03.607828 authentik_client-2024.2.2.post1712239192/authentik_client/models/rac_property_mapping_request.py
--rw-r--r--   0        0        0     6813 2024-04-04 14:00:03.611828 authentik_client-2024.2.2.post1712239192/authentik_client/models/rac_provider.py
--rw-r--r--   0        0        0     4351 2024-04-04 14:00:03.611828 authentik_client-2024.2.2.post1712239192/authentik_client/models/rac_provider_request.py
--rw-r--r--   0        0        0     3833 2024-04-04 14:00:03.615829 authentik_client-2024.2.2.post1712239192/authentik_client/models/radius_outpost_config.py
--rw-r--r--   0        0        0     6924 2024-04-04 14:00:03.615829 authentik_client-2024.2.2.post1712239192/authentik_client/models/radius_provider.py
--rw-r--r--   0        0        0     4501 2024-04-04 14:00:03.619829 authentik_client-2024.2.2.post1712239192/authentik_client/models/radius_provider_request.py
--rw-r--r--   0        0        0     4184 2024-04-04 14:00:03.623829 authentik_client-2024.2.2.post1712239192/authentik_client/models/redirect_challenge.py
--rw-r--r--   0        0        0     3642 2024-04-04 14:00:03.623829 authentik_client-2024.2.2.post1712239192/authentik_client/models/reputation.py
--rw-r--r--   0        0        0     4516 2024-04-04 14:00:03.627829 authentik_client-2024.2.2.post1712239192/authentik_client/models/reputation_policy.py
--rw-r--r--   0        0        0     3238 2024-04-04 14:00:03.627829 authentik_client-2024.2.2.post1712239192/authentik_client/models/reputation_policy_request.py
--rw-r--r--   0        0        0      795 2024-04-04 14:00:03.631829 authentik_client-2024.2.2.post1712239192/authentik_client/models/resident_key_requirement_enum.py
--rw-r--r--   0        0        0     2618 2024-04-04 14:00:03.631829 authentik_client-2024.2.2.post1712239192/authentik_client/models/role.py
--rw-r--r--   0        0        0     3333 2024-04-04 14:00:03.635829 authentik_client-2024.2.2.post1712239192/authentik_client/models/role_assigned_object_permission.py
--rw-r--r--   0        0        0     3293 2024-04-04 14:00:03.639829 authentik_client-2024.2.2.post1712239192/authentik_client/models/role_object_permission.py
--rw-r--r--   0        0        0     2517 2024-04-04 14:00:03.639829 authentik_client-2024.2.2.post1712239192/authentik_client/models/role_request.py
--rw-r--r--   0        0        0     2712 2024-04-04 14:00:03.643829 authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_metadata.py
--rw-r--r--   0        0        0     4718 2024-04-04 14:00:03.647829 authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_property_mapping.py
--rw-r--r--   0        0        0     3829 2024-04-04 14:00:03.651829 authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_property_mapping_request.py
--rw-r--r--   0        0        0    11056 2024-04-04 14:00:03.651829 authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_provider.py
--rw-r--r--   0        0        0     7460 2024-04-04 14:00:03.655829 authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_provider_request.py
--rw-r--r--   0        0        0    10563 2024-04-04 14:00:03.659829 authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_source.py
--rw-r--r--   0        0        0     8507 2024-04-04 14:00:03.663829 authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_source_request.py
--rw-r--r--   0        0        0     4248 2024-04-04 14:00:03.663829 authentik_client-2024.2.2.post1712239192/authentik_client/models/scim_mapping.py
--rw-r--r--   0        0        0     3309 2024-04-04 14:00:03.667829 authentik_client-2024.2.2.post1712239192/authentik_client/models/scim_mapping_request.py
--rw-r--r--   0        0        0     5454 2024-04-04 14:00:03.671829 authentik_client-2024.2.2.post1712239192/authentik_client/models/scim_provider.py
--rw-r--r--   0        0        0     3802 2024-04-04 14:00:03.671829 authentik_client-2024.2.2.post1712239192/authentik_client/models/scim_provider_request.py
--rw-r--r--   0        0        0     3131 2024-04-04 14:00:03.675830 authentik_client-2024.2.2.post1712239192/authentik_client/models/scim_sync_status.py
--rw-r--r--   0        0        0     4629 2024-04-04 14:00:03.683830 authentik_client-2024.2.2.post1712239192/authentik_client/models/scope_mapping.py
--rw-r--r--   0        0        0     3740 2024-04-04 14:00:03.687830 authentik_client-2024.2.2.post1712239192/authentik_client/models/scope_mapping_request.py
--rw-r--r--   0        0        0     2738 2024-04-04 14:00:03.687830 authentik_client-2024.2.2.post1712239192/authentik_client/models/selectable_stage.py
--rw-r--r--   0        0        0     3773 2024-04-04 14:00:03.691830 authentik_client-2024.2.2.post1712239192/authentik_client/models/service_connection.py
--rw-r--r--   0        0        0     2776 2024-04-04 14:00:03.695830 authentik_client-2024.2.2.post1712239192/authentik_client/models/service_connection_request.py
--rw-r--r--   0        0        0     2731 2024-04-04 14:00:03.695830 authentik_client-2024.2.2.post1712239192/authentik_client/models/service_connection_state.py
--rw-r--r--   0        0        0     3178 2024-04-04 14:00:03.699830 authentik_client-2024.2.2.post1712239192/authentik_client/models/session_user.py
--rw-r--r--   0        0        0     4441 2024-04-04 14:00:03.703830 authentik_client-2024.2.2.post1712239192/authentik_client/models/settings.py
--rw-r--r--   0        0        0     4569 2024-04-04 14:00:03.703830 authentik_client-2024.2.2.post1712239192/authentik_client/models/settings_request.py
--rw-r--r--   0        0        0      733 2024-04-04 14:00:03.707830 authentik_client-2024.2.2.post1712239192/authentik_client/models/severity_enum.py
--rw-r--r--   0        0        0     4175 2024-04-04 14:00:03.715830 authentik_client-2024.2.2.post1712239192/authentik_client/models/shell_challenge.py
--rw-r--r--   0        0        0     1492 2024-04-04 14:00:03.715830 authentik_client-2024.2.2.post1712239192/authentik_client/models/signature_algorithm_enum.py
--rw-r--r--   0        0        0     2906 2024-04-04 14:00:03.679829 authentik_client-2024.2.2.post1712239192/authentik_client/models/sms_device.py
--rw-r--r--   0        0        0     2619 2024-04-04 14:00:03.679829 authentik_client-2024.2.2.post1712239192/authentik_client/models/sms_device_request.py
--rw-r--r--   0        0        0     6945 2024-04-04 14:00:03.719830 authentik_client-2024.2.2.post1712239192/authentik_client/models/source.py
--rw-r--r--   0        0        0     4836 2024-04-04 14:00:03.723830 authentik_client-2024.2.2.post1712239192/authentik_client/models/source_request.py
--rw-r--r--   0        0        0     4438 2024-04-04 14:00:03.723830 authentik_client-2024.2.2.post1712239192/authentik_client/models/source_stage.py
--rw-r--r--   0        0        0     3507 2024-04-04 14:00:03.727830 authentik_client-2024.2.2.post1712239192/authentik_client/models/source_stage_request.py
--rw-r--r--   0        0        0     5355 2024-04-04 14:00:03.731830 authentik_client-2024.2.2.post1712239192/authentik_client/models/source_type.py
--rw-r--r--   0        0        0      714 2024-04-04 14:00:03.731830 authentik_client-2024.2.2.post1712239192/authentik_client/models/sp_binding_enum.py
--rw-r--r--   0        0        0     4070 2024-04-04 14:00:03.735830 authentik_client-2024.2.2.post1712239192/authentik_client/models/stage.py
--rw-r--r--   0        0        0     3437 2024-04-04 14:00:03.739830 authentik_client-2024.2.2.post1712239192/authentik_client/models/stage_prompt.py
--rw-r--r--   0        0        0     3089 2024-04-04 14:00:03.739830 authentik_client-2024.2.2.post1712239192/authentik_client/models/stage_request.py
--rw-r--r--   0        0        0     3385 2024-04-04 14:00:03.743831 authentik_client-2024.2.2.post1712239192/authentik_client/models/static_device.py
--rw-r--r--   0        0        0     2631 2024-04-04 14:00:03.747830 authentik_client-2024.2.2.post1712239192/authentik_client/models/static_device_request.py
--rw-r--r--   0        0        0     2546 2024-04-04 14:00:03.747830 authentik_client-2024.2.2.post1712239192/authentik_client/models/static_device_token.py
--rw-r--r--   0        0        0     2581 2024-04-04 14:00:03.751831 authentik_client-2024.2.2.post1712239192/authentik_client/models/static_device_token_request.py
--rw-r--r--   0        0        0      846 2024-04-04 14:00:03.751831 authentik_client-2024.2.2.post1712239192/authentik_client/models/sub_mode_enum.py
--rw-r--r--   0        0        0     4463 2024-04-04 14:00:03.755831 authentik_client-2024.2.2.post1712239192/authentik_client/models/system_info.py
--rw-r--r--   0        0        0     2934 2024-04-04 14:00:03.759831 authentik_client-2024.2.2.post1712239192/authentik_client/models/system_info_runtime.py
--rw-r--r--   0        0        0     4286 2024-04-04 14:00:03.759831 authentik_client-2024.2.2.post1712239192/authentik_client/models/system_task.py
--rw-r--r--   0        0        0      789 2024-04-04 14:00:03.763831 authentik_client-2024.2.2.post1712239192/authentik_client/models/system_task_status_enum.py
--rw-r--r--   0        0        0     2872 2024-04-04 14:00:03.771831 authentik_client-2024.2.2.post1712239192/authentik_client/models/tenant.py
--rw-r--r--   0        0        0     2589 2024-04-04 14:00:03.771831 authentik_client-2024.2.2.post1712239192/authentik_client/models/tenant_admin_group_request_request.py
--rw-r--r--   0        0        0     2705 2024-04-04 14:00:03.775831 authentik_client-2024.2.2.post1712239192/authentik_client/models/tenant_recovery_key_request_request.py
--rw-r--r--   0        0        0     2599 2024-04-04 14:00:03.779831 authentik_client-2024.2.2.post1712239192/authentik_client/models/tenant_recovery_key_response.py
--rw-r--r--   0        0        0     2765 2024-04-04 14:00:03.779831 authentik_client-2024.2.2.post1712239192/authentik_client/models/tenant_request.py
--rw-r--r--   0        0        0     4591 2024-04-04 14:00:03.783831 authentik_client-2024.2.2.post1712239192/authentik_client/models/token.py
--rw-r--r--   0        0        0     3987 2024-04-04 14:00:03.787831 authentik_client-2024.2.2.post1712239192/authentik_client/models/token_model.py
--rw-r--r--   0        0        0     4118 2024-04-04 14:00:03.791831 authentik_client-2024.2.2.post1712239192/authentik_client/models/token_request.py
--rw-r--r--   0        0        0     2521 2024-04-04 14:00:03.795831 authentik_client-2024.2.2.post1712239192/authentik_client/models/token_set_key_request.py
--rw-r--r--   0        0        0     2494 2024-04-04 14:00:03.795831 authentik_client-2024.2.2.post1712239192/authentik_client/models/token_view.py
--rw-r--r--   0        0        0     2724 2024-04-04 14:00:03.763831 authentik_client-2024.2.2.post1712239192/authentik_client/models/totp_device.py
--rw-r--r--   0        0        0     2623 2024-04-04 14:00:03.767831 authentik_client-2024.2.2.post1712239192/authentik_client/models/totp_device_request.py
--rw-r--r--   0        0        0     3389 2024-04-04 14:00:03.799831 authentik_client-2024.2.2.post1712239192/authentik_client/models/transaction_application_request.py
--rw-r--r--   0        0        0     2595 2024-04-04 14:00:03.803831 authentik_client-2024.2.2.post1712239192/authentik_client/models/transaction_application_response.py
--rw-r--r--   0        0        0     2936 2024-04-04 14:00:03.807832 authentik_client-2024.2.2.post1712239192/authentik_client/models/type_create.py
--rw-r--r--   0        0        0      730 2024-04-04 14:00:03.807832 authentik_client-2024.2.2.post1712239192/authentik_client/models/ui_theme_enum.py
--rw-r--r--   0        0        0     2808 2024-04-04 14:00:03.811832 authentik_client-2024.2.2.post1712239192/authentik_client/models/used_by.py
--rw-r--r--   0        0        0      795 2024-04-04 14:00:03.811832 authentik_client-2024.2.2.post1712239192/authentik_client/models/used_by_action_enum.py
--rw-r--r--   0        0        0     5226 2024-04-04 14:00:03.815832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user.py
--rw-r--r--   0        0        0     2458 2024-04-04 14:00:03.819832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_account_request.py
--rw-r--r--   0        0        0     4946 2024-04-04 14:00:03.823832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_assigned_object_permission.py
--rw-r--r--   0        0        0     3617 2024-04-04 14:00:03.823832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_consent.py
--rw-r--r--   0        0        0      811 2024-04-04 14:00:03.827832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_creation_mode_enum.py
--rw-r--r--   0        0        0     4110 2024-04-04 14:00:03.827832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_delete_stage.py
--rw-r--r--   0        0        0     3129 2024-04-04 14:00:03.831832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_delete_stage_request.py
--rw-r--r--   0        0        0      735 2024-04-04 14:00:03.835832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_fields_enum.py
--rw-r--r--   0        0        0     3909 2024-04-04 14:00:03.835832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_group.py
--rw-r--r--   0        0        0     3193 2024-04-04 14:00:03.839832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_group_request.py
--rw-r--r--   0        0        0     4334 2024-04-04 14:00:03.843832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_login_challenge.py
--rw-r--r--   0        0        0     2805 2024-04-04 14:00:03.847832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_login_challenge_response_request.py
--rw-r--r--   0        0        0     5631 2024-04-04 14:00:03.847832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_login_stage.py
--rw-r--r--   0        0        0     4728 2024-04-04 14:00:03.851832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_login_stage_request.py
--rw-r--r--   0        0        0     4110 2024-04-04 14:00:03.855832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_logout_stage.py
--rw-r--r--   0        0        0     3129 2024-04-04 14:00:03.859832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_logout_stage_request.py
--rw-r--r--   0        0        0      853 2024-04-04 14:00:03.859832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_matching_mode_enum.py
--rw-r--r--   0        0        0     4160 2024-04-04 14:00:03.863832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_metrics.py
--rw-r--r--   0        0        0     3188 2024-04-04 14:00:03.863832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_o_auth_source_connection.py
--rw-r--r--   0        0        0     3054 2024-04-04 14:00:03.867833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3293 2024-04-04 14:00:03.871832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_object_permission.py
--rw-r--r--   0        0        0     2557 2024-04-04 14:00:03.871832 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_password_set_request.py
--rw-r--r--   0        0        0     2491 2024-04-04 14:00:03.875833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_path.py
--rw-r--r--   0        0        0     3872 2024-04-04 14:00:03.879833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_request.py
--rw-r--r--   0        0        0     3107 2024-04-04 14:00:03.879833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_saml_source_connection.py
--rw-r--r--   0        0        0     2668 2024-04-04 14:00:03.883833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_saml_source_connection_request.py
--rw-r--r--   0        0        0     5465 2024-04-04 14:00:03.887833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_self.py
--rw-r--r--   0        0        0     2629 2024-04-04 14:00:03.887833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_self_groups.py
--rw-r--r--   0        0        0     3074 2024-04-04 14:00:03.891833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_service_account_request.py
--rw-r--r--   0        0        0     2844 2024-04-04 14:00:03.895833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_service_account_response.py
--rw-r--r--   0        0        0     2866 2024-04-04 14:00:03.895833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_setting.py
--rw-r--r--   0        0        0     3245 2024-04-04 14:00:03.899833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_source_connection.py
--rw-r--r--   0        0        0      817 2024-04-04 14:00:03.899833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_type_enum.py
--rw-r--r--   0        0        0      777 2024-04-04 14:00:03.903833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_verification_enum.py
--rw-r--r--   0        0        0     5382 2024-04-04 14:00:03.907833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_write_stage.py
--rw-r--r--   0        0        0     4412 2024-04-04 14:00:03.907833 authentik_client-2024.2.2.post1712239192/authentik_client/models/user_write_stage_request.py
--rw-r--r--   0        0        0     3197 2024-04-04 14:00:03.911833 authentik_client-2024.2.2.post1712239192/authentik_client/models/validation_error.py
--rw-r--r--   0        0        0     3589 2024-04-04 14:00:03.915833 authentik_client-2024.2.2.post1712239192/authentik_client/models/version.py
--rw-r--r--   0        0        0     2872 2024-04-04 14:00:03.919833 authentik_client-2024.2.2.post1712239192/authentik_client/models/web_authn_device.py
--rw-r--r--   0        0        0     2577 2024-04-04 14:00:03.919833 authentik_client-2024.2.2.post1712239192/authentik_client/models/web_authn_device_request.py
--rw-r--r--   0        0        0     2410 2024-04-04 14:00:03.923833 authentik_client-2024.2.2.post1712239192/authentik_client/models/workers.py
--rw-r--r--   0        0        0        0 2024-04-04 14:00:05.103852 authentik_client-2024.2.2.post1712239192/authentik_client/py.typed
--rw-r--r--   0        0        0     9196 2024-04-04 14:00:05.111852 authentik_client-2024.2.2.post1712239192/authentik_client/rest.py
--rw-r--r--   0        0        0     1936 2024-04-04 14:00:05.099852 authentik_client-2024.2.2.post1712239192/pyproject.toml
--rw-r--r--   0        0        0   140950 1970-01-01 00:00:00.000000 authentik_client-2024.2.2.post1712239192/PKG-INFO
+-rw-r--r--   0        0        0   140605 2024-04-08 10:22:33.843093 authentik_client-2024.2.2.post1712571742/README.md
+-rw-r--r--   0        0        0    47475 2024-04-08 10:22:33.851093 authentik_client-2024.2.2.post1712571742/authentik_client/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-08 10:22:33.855093 authentik_client-2024.2.2.post1712571742/authentik_client/api/__init__.py
+-rw-r--r--   0        0        0    97518 2024-04-08 10:22:33.599094 authentik_client-2024.2.2.post1712571742/authentik_client/api/admin_api.py
+-rw-r--r--   0        0        0   700271 2024-04-08 10:22:33.619094 authentik_client-2024.2.2.post1712571742/authentik_client/api/authenticators_api.py
+-rw-r--r--   0        0        0   699928 2024-04-08 10:22:33.655094 authentik_client-2024.2.2.post1712571742/authentik_client/api/core_api.py
+-rw-r--r--   0        0        0   116805 2024-04-08 10:22:33.671094 authentik_client-2024.2.2.post1712571742/authentik_client/api/crypto_api.py
+-rw-r--r--   0        0        0   107946 2024-04-08 10:22:33.679094 authentik_client-2024.2.2.post1712571742/authentik_client/api/enterprise_api.py
+-rw-r--r--   0        0        0   408008 2024-04-08 10:22:33.691094 authentik_client-2024.2.2.post1712571742/authentik_client/api/events_api.py
+-rw-r--r--   0        0        0   280806 2024-04-08 10:22:33.703094 authentik_client-2024.2.2.post1712571742/authentik_client/api/flows_api.py
+-rw-r--r--   0        0        0   101134 2024-04-08 10:22:33.711094 authentik_client-2024.2.2.post1712571742/authentik_client/api/managed_api.py
+-rw-r--r--   0        0        0   135649 2024-04-08 10:22:33.719094 authentik_client-2024.2.2.post1712571742/authentik_client/api/oauth2_api.py
+-rw-r--r--   0        0        0   413301 2024-04-08 10:22:33.727094 authentik_client-2024.2.2.post1712571742/authentik_client/api/outposts_api.py
+-rw-r--r--   0        0        0   725201 2024-04-08 10:22:33.739094 authentik_client-2024.2.2.post1712571742/authentik_client/api/policies_api.py
+-rw-r--r--   0        0        0   552586 2024-04-08 10:22:33.751093 authentik_client-2024.2.2.post1712571742/authentik_client/api/propertymappings_api.py
+-rw-r--r--   0        0        0   718066 2024-04-08 10:22:33.763094 authentik_client-2024.2.2.post1712571742/authentik_client/api/providers_api.py
+-rw-r--r--   0        0        0   150485 2024-04-08 10:22:33.771093 authentik_client-2024.2.2.post1712571742/authentik_client/api/rac_api.py
+-rw-r--r--   0        0        0   207550 2024-04-08 10:22:33.779093 authentik_client-2024.2.2.post1712571742/authentik_client/api/rbac_api.py
+-rw-r--r--   0        0        0    10391 2024-04-08 10:22:33.783093 authentik_client-2024.2.2.post1712571742/authentik_client/api/root_api.py
+-rw-r--r--   0        0        0    11845 2024-04-08 10:22:33.791093 authentik_client-2024.2.2.post1712571742/authentik_client/api/schema_api.py
+-rw-r--r--   0        0        0   802117 2024-04-08 10:22:33.799093 authentik_client-2024.2.2.post1712571742/authentik_client/api/sources_api.py
+-rw-r--r--   0        0        0  1945986 2024-04-08 10:22:33.823093 authentik_client-2024.2.2.post1712571742/authentik_client/api/stages_api.py
+-rw-r--r--   0        0        0   157909 2024-04-08 10:22:33.835093 authentik_client-2024.2.2.post1712571742/authentik_client/api/tenants_api.py
+-rw-r--r--   0        0        0    25779 2024-04-08 10:22:33.855093 authentik_client-2024.2.2.post1712571742/authentik_client/api_client.py
+-rw-r--r--   0        0        0      652 2024-04-08 10:22:33.855093 authentik_client-2024.2.2.post1712571742/authentik_client/api_response.py
+-rw-r--r--   0        0        0    15345 2024-04-08 10:22:33.851093 authentik_client-2024.2.2.post1712571742/authentik_client/configuration.py
+-rw-r--r--   0        0        0     5934 2024-04-08 10:22:33.855093 authentik_client-2024.2.2.post1712571742/authentik_client/exceptions.py
+-rw-r--r--   0        0        0    45777 2024-04-08 10:22:33.851093 authentik_client-2024.2.2.post1712571742/authentik_client/models/__init__.py
+-rw-r--r--   0        0        0     4513 2024-04-08 10:22:30.991111 authentik_client-2024.2.2.post1712571742/authentik_client/models/access_denied_challenge.py
+-rw-r--r--   0        0        0     2482 2024-04-08 10:22:31.007111 authentik_client-2024.2.2.post1712571742/authentik_client/models/app.py
+-rw-r--r--   0        0        0     4168 2024-04-08 10:22:31.011111 authentik_client-2024.2.2.post1712571742/authentik_client/models/app_enum.py
+-rw-r--r--   0        0        0     2702 2024-04-08 10:22:31.023111 authentik_client-2024.2.2.post1712571742/authentik_client/models/apple_challenge_response_request.py
+-rw-r--r--   0        0        0     4508 2024-04-08 10:22:31.035111 authentik_client-2024.2.2.post1712571742/authentik_client/models/apple_login_challenge.py
+-rw-r--r--   0        0        0     6686 2024-04-08 10:22:31.043111 authentik_client-2024.2.2.post1712571742/authentik_client/models/application.py
+-rw-r--r--   0        0        0     4473 2024-04-08 10:22:31.051111 authentik_client-2024.2.2.post1712571742/authentik_client/models/application_request.py
+-rw-r--r--   0        0        0      711 2024-04-08 10:22:31.055111 authentik_client-2024.2.2.post1712571742/authentik_client/models/auth_mode_enum.py
+-rw-r--r--   0        0        0      709 2024-04-08 10:22:31.059111 authentik_client-2024.2.2.post1712571742/authentik_client/models/auth_type_enum.py
+-rw-r--r--   0        0        0     4984 2024-04-08 10:22:31.067111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session.py
+-rw-r--r--   0        0        0     3064 2024-04-08 10:22:31.071111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_asn.py
+-rw-r--r--   0        0        0     2826 2024-04-08 10:22:31.075111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_geo_ip.py
+-rw-r--r--   0        0        0     3865 2024-04-08 10:22:31.083111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent.py
+-rw-r--r--   0        0        0     2646 2024-04-08 10:22:31.087111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_device.py
+-rw-r--r--   0        0        0     2792 2024-04-08 10:22:31.095111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_os.py
+-rw-r--r--   0        0        0     2725 2024-04-08 10:22:31.099110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_user_agent.py
+-rw-r--r--   0        0        0      895 2024-04-08 10:22:31.103111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authentication_enum.py
+-rw-r--r--   0        0        0      782 2024-04-08 10:22:31.103111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_attachment_enum.py
+-rw-r--r--   0        0        0     4686 2024-04-08 10:22:31.111111 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_challenge.py
+-rw-r--r--   0        0        0     2743 2024-04-08 10:22:31.115110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_challenge_response_request.py
+-rw-r--r--   0        0        0     5327 2024-04-08 10:22:31.123110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage.py
+-rw-r--r--   0        0        0     2768 2024-04-08 10:22:31.127110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_device_import_response.py
+-rw-r--r--   0        0        0     2785 2024-04-08 10:22:31.135110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
+-rw-r--r--   0        0        0     4744 2024-04-08 10:22:31.139110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-08 10:22:31.143110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_challenge.py
+-rw-r--r--   0        0        0     3022 2024-04-08 10:22:31.151110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_challenge_response_request.py
+-rw-r--r--   0        0        0     6409 2024-04-08 10:22:31.155110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_stage.py
+-rw-r--r--   0        0        0     5595 2024-04-08 10:22:31.163110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4474 2024-04-08 10:22:31.167110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_challenge.py
+-rw-r--r--   0        0        0     2761 2024-04-08 10:22:31.175110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_challenge_response_request.py
+-rw-r--r--   0        0        0     5363 2024-04-08 10:22:31.179110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_stage.py
+-rw-r--r--   0        0        0     4392 2024-04-08 10:22:31.183110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4468 2024-04-08 10:22:31.191110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_challenge.py
+-rw-r--r--   0        0        0     2858 2024-04-08 10:22:31.195110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_challenge_response_request.py
+-rw-r--r--   0        0        0     5132 2024-04-08 10:22:31.199110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_stage.py
+-rw-r--r--   0        0        0     4201 2024-04-08 10:22:31.207110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     5636 2024-04-08 10:22:31.211110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validate_stage.py
+-rw-r--r--   0        0        0     4705 2024-04-08 10:22:31.215110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5717 2024-04-08 10:22:31.223110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validation_challenge.py
+-rw-r--r--   0        0        0     3805 2024-04-08 10:22:31.227110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validation_challenge_response_request.py
+-rw-r--r--   0        0        0     4499 2024-04-08 10:22:31.231110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_challenge.py
+-rw-r--r--   0        0        0     2852 2024-04-08 10:22:31.239110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_challenge_response_request.py
+-rw-r--r--   0        0        0     7081 2024-04-08 10:22:31.243110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_stage.py
+-rw-r--r--   0        0        0     5302 2024-04-08 10:22:31.247110 authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     2718 2024-04-08 10:22:31.251110 authentik_client-2024.2.2.post1712571742/authentik_client/models/auto_submit_challenge_response_request.py
+-rw-r--r--   0        0        0     4388 2024-04-08 10:22:31.259110 authentik_client-2024.2.2.post1712571742/authentik_client/models/autosubmit_challenge.py
+-rw-r--r--   0        0        0      950 2024-04-08 10:22:31.263110 authentik_client-2024.2.2.post1712571742/authentik_client/models/backends_enum.py
+-rw-r--r--   0        0        0      748 2024-04-08 10:22:31.263110 authentik_client-2024.2.2.post1712571742/authentik_client/models/binding_type_enum.py
+-rw-r--r--   0        0        0     2995 2024-04-08 10:22:31.267109 authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_file.py
+-rw-r--r--   0        0        0     4453 2024-04-08 10:22:31.271109 authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance.py
+-rw-r--r--   0        0        0     3208 2024-04-08 10:22:31.279109 authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance_request.py
+-rw-r--r--   0        0        0      836 2024-04-08 10:22:31.279109 authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance_status_enum.py
+-rw-r--r--   0        0        0     6255 2024-04-08 10:22:31.283109 authentik_client-2024.2.2.post1712571742/authentik_client/models/brand.py
+-rw-r--r--   0        0        0     6307 2024-04-08 10:22:31.291109 authentik_client-2024.2.2.post1712571742/authentik_client/models/brand_request.py
+-rw-r--r--   0        0        0     2501 2024-04-08 10:22:31.295109 authentik_client-2024.2.2.post1712571742/authentik_client/models/cache.py
+-rw-r--r--   0        0        0      875 2024-04-08 10:22:31.299109 authentik_client-2024.2.2.post1712571742/authentik_client/models/capabilities_enum.py
+-rw-r--r--   0        0        0     4476 2024-04-08 10:22:31.303109 authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_challenge.py
+-rw-r--r--   0        0        0     2797 2024-04-08 10:22:31.307109 authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_challenge_response_request.py
+-rw-r--r--   0        0        0     4438 2024-04-08 10:22:31.311109 authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_stage.py
+-rw-r--r--   0        0        0     3774 2024-04-08 10:22:31.315109 authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_stage_request.py
+-rw-r--r--   0        0        0     2522 2024-04-08 10:22:31.319109 authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_data.py
+-rw-r--r--   0        0        0     2861 2024-04-08 10:22:31.323109 authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_generation_request.py
+-rw-r--r--   0        0        0     6655 2024-04-08 10:22:31.327109 authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_key_pair.py
+-rw-r--r--   0        0        0     2989 2024-04-08 10:22:31.331109 authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_key_pair_request.py
+-rw-r--r--   0        0        0      747 2024-04-08 10:22:31.335109 authentik_client-2024.2.2.post1712571742/authentik_client/models/challenge_choices.py
+-rw-r--r--   0        0        0    24236 2024-04-08 10:22:31.343109 authentik_client-2024.2.2.post1712571742/authentik_client/models/challenge_types.py
+-rw-r--r--   0        0        0      729 2024-04-08 10:22:31.347109 authentik_client-2024.2.2.post1712571742/authentik_client/models/client_type_enum.py
+-rw-r--r--   0        0        0     3539 2024-04-08 10:22:31.359109 authentik_client-2024.2.2.post1712571742/authentik_client/models/config.py
+-rw-r--r--   0        0        0     4021 2024-04-08 10:22:31.363109 authentik_client-2024.2.2.post1712571742/authentik_client/models/connection_token.py
+-rw-r--r--   0        0        0     2662 2024-04-08 10:22:31.367109 authentik_client-2024.2.2.post1712571742/authentik_client/models/connection_token_request.py
+-rw-r--r--   0        0        0     5736 2024-04-08 10:22:31.375109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_challenge.py
+-rw-r--r--   0        0        0     2838 2024-04-08 10:22:31.379109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_challenge_response_request.py
+-rw-r--r--   0        0        0     2513 2024-04-08 10:22:31.383109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_permission.py
+-rw-r--r--   0        0        0     4511 2024-04-08 10:22:31.387109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage.py
+-rw-r--r--   0        0        0      783 2024-04-08 10:22:31.391109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage_mode_enum.py
+-rw-r--r--   0        0        0     3569 2024-04-08 10:22:31.395109 authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage_request.py
+-rw-r--r--   0        0        0     2891 2024-04-08 10:22:31.399109 authentik_client-2024.2.2.post1712571742/authentik_client/models/contextual_flow_info.py
+-rw-r--r--   0        0        0      879 2024-04-08 10:22:31.403109 authentik_client-2024.2.2.post1712571742/authentik_client/models/contextual_flow_info_layout_enum.py
+-rw-r--r--   0        0        0     2657 2024-04-08 10:22:31.407109 authentik_client-2024.2.2.post1712571742/authentik_client/models/coordinate.py
+-rw-r--r--   0        0        0     4704 2024-04-08 10:22:31.411109 authentik_client-2024.2.2.post1712571742/authentik_client/models/current_brand.py
+-rw-r--r--   0        0        0      771 2024-04-08 10:22:31.415109 authentik_client-2024.2.2.post1712571742/authentik_client/models/denied_action_enum.py
+-rw-r--r--   0        0        0     4200 2024-04-08 10:22:31.419108 authentik_client-2024.2.2.post1712571742/authentik_client/models/deny_stage.py
+-rw-r--r--   0        0        0     3230 2024-04-08 10:22:31.423108 authentik_client-2024.2.2.post1712571742/authentik_client/models/deny_stage_request.py
+-rw-r--r--   0        0        0     3522 2024-04-08 10:22:31.431108 authentik_client-2024.2.2.post1712571742/authentik_client/models/device.py
+-rw-r--r--   0        0        0     2657 2024-04-08 10:22:31.435109 authentik_client-2024.2.2.post1712571742/authentik_client/models/device_challenge.py
+-rw-r--r--   0        0        0     2792 2024-04-08 10:22:31.439108 authentik_client-2024.2.2.post1712571742/authentik_client/models/device_challenge_request.py
+-rw-r--r--   0        0        0      780 2024-04-08 10:22:31.443108 authentik_client-2024.2.2.post1712571742/authentik_client/models/device_classes_enum.py
+-rw-r--r--   0        0        0     1244 2024-04-08 10:22:31.447108 authentik_client-2024.2.2.post1712571742/authentik_client/models/digest_algorithm_enum.py
+-rw-r--r--   0        0        0      695 2024-04-08 10:22:31.447108 authentik_client-2024.2.2.post1712571742/authentik_client/models/digits_enum.py
+-rw-r--r--   0        0        0     4969 2024-04-08 10:22:31.451108 authentik_client-2024.2.2.post1712571742/authentik_client/models/docker_service_connection.py
+-rw-r--r--   0        0        0     4087 2024-04-08 10:22:31.455108 authentik_client-2024.2.2.post1712571742/authentik_client/models/docker_service_connection_request.py
+-rw-r--r--   0        0        0     2847 2024-04-08 10:22:31.459108 authentik_client-2024.2.2.post1712571742/authentik_client/models/domain.py
+-rw-r--r--   0        0        0     2746 2024-04-08 10:22:31.467108 authentik_client-2024.2.2.post1712571742/authentik_client/models/domain_request.py
+-rw-r--r--   0        0        0     4155 2024-04-08 10:22:31.471108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_challenge.py
+-rw-r--r--   0        0        0     2681 2024-04-08 10:22:31.475108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_challenge_response_request.py
+-rw-r--r--   0        0        0     4515 2024-04-08 10:22:31.483108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_policy.py
+-rw-r--r--   0        0        0     3237 2024-04-08 10:22:31.487108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_policy_request.py
+-rw-r--r--   0        0        0     4213 2024-04-08 10:22:31.491108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_stage.py
+-rw-r--r--   0        0        0     3232 2024-04-08 10:22:31.495108 authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_stage_request.py
+-rw-r--r--   0        0        0     2720 2024-04-08 10:22:31.499108 authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device.py
+-rw-r--r--   0        0        0     2575 2024-04-08 10:22:31.503108 authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device_enrollment_status.py
+-rw-r--r--   0        0        0     2619 2024-04-08 10:22:31.507108 authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device_request.py
+-rw-r--r--   0        0        0      748 2024-04-08 10:22:31.511108 authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_response_enum.py
+-rw-r--r--   0        0        0     4090 2024-04-08 10:22:31.515108 authentik_client-2024.2.2.post1712571742/authentik_client/models/email_challenge.py
+-rw-r--r--   0        0        0     2770 2024-04-08 10:22:31.523108 authentik_client-2024.2.2.post1712571742/authentik_client/models/email_challenge_response_request.py
+-rw-r--r--   0        0        0     5902 2024-04-08 10:22:31.531108 authentik_client-2024.2.2.post1712571742/authentik_client/models/email_stage.py
+-rw-r--r--   0        0        0     5121 2024-04-08 10:22:31.535108 authentik_client-2024.2.2.post1712571742/authentik_client/models/email_stage_request.py
+-rw-r--r--   0        0        0     4707 2024-04-08 10:22:31.543108 authentik_client-2024.2.2.post1712571742/authentik_client/models/endpoint.py
+-rw-r--r--   0        0        0     3678 2024-04-08 10:22:31.547108 authentik_client-2024.2.2.post1712571742/authentik_client/models/endpoint_request.py
+-rw-r--r--   0        0        0     2530 2024-04-08 10:22:31.551108 authentik_client-2024.2.2.post1712571742/authentik_client/models/error_detail.py
+-rw-r--r--   0        0        0     3309 2024-04-08 10:22:31.555108 authentik_client-2024.2.2.post1712571742/authentik_client/models/error_reporting_config.py
+-rw-r--r--   0        0        0     4129 2024-04-08 10:22:31.559108 authentik_client-2024.2.2.post1712571742/authentik_client/models/event.py
+-rw-r--r--   0        0        0     1730 2024-04-08 10:22:31.563108 authentik_client-2024.2.2.post1712571742/authentik_client/models/event_actions.py
+-rw-r--r--   0        0        0     6006 2024-04-08 10:22:31.567108 authentik_client-2024.2.2.post1712571742/authentik_client/models/event_matcher_policy.py
+-rw-r--r--   0        0        0     4807 2024-04-08 10:22:31.575107 authentik_client-2024.2.2.post1712571742/authentik_client/models/event_matcher_policy_request.py
+-rw-r--r--   0        0        0     3990 2024-04-08 10:22:31.579107 authentik_client-2024.2.2.post1712571742/authentik_client/models/event_request.py
+-rw-r--r--   0        0        0     2697 2024-04-08 10:22:31.583108 authentik_client-2024.2.2.post1712571742/authentik_client/models/event_top_per_user.py
+-rw-r--r--   0        0        0     3715 2024-04-08 10:22:31.591107 authentik_client-2024.2.2.post1712571742/authentik_client/models/expiring_base_grant_model.py
+-rw-r--r--   0        0        0     4191 2024-04-08 10:22:31.595107 authentik_client-2024.2.2.post1712571742/authentik_client/models/expression_policy.py
+-rw-r--r--   0        0        0     2992 2024-04-08 10:22:31.603107 authentik_client-2024.2.2.post1712571742/authentik_client/models/expression_policy_request.py
+-rw-r--r--   0        0        0     4524 2024-04-08 10:22:31.603107 authentik_client-2024.2.2.post1712571742/authentik_client/models/extra_role_object_permission.py
+-rw-r--r--   0        0        0     4524 2024-04-08 10:22:31.607107 authentik_client-2024.2.2.post1712571742/authentik_client/models/extra_user_object_permission.py
+-rw-r--r--   0        0        0     2519 2024-04-08 10:22:31.611107 authentik_client-2024.2.2.post1712571742/authentik_client/models/file_path_request.py
+-rw-r--r--   0        0        0     6047 2024-04-08 10:22:31.615107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow.py
+-rw-r--r--   0        0        0    25850 2024-04-08 10:22:31.623107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_challenge_response_request.py
+-rw-r--r--   0        0        0      934 2024-04-08 10:22:31.623107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_designation_enum.py
+-rw-r--r--   0        0        0     2533 2024-04-08 10:22:31.627107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_diagram.py
+-rw-r--r--   0        0        0     4505 2024-04-08 10:22:31.631107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_error_challenge.py
+-rw-r--r--   0        0        0     3111 2024-04-08 10:22:31.635107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_import_result.py
+-rw-r--r--   0        0        0     3418 2024-04-08 10:22:31.639107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_inspection.py
+-rw-r--r--   0        0        0     3875 2024-04-08 10:22:31.643107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_inspector_plan.py
+-rw-r--r--   0        0        0      837 2024-04-08 10:22:31.647107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_layout_enum.py
+-rw-r--r--   0        0        0     4741 2024-04-08 10:22:31.651107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_request.py
+-rw-r--r--   0        0        0     5223 2024-04-08 10:22:31.655107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_set.py
+-rw-r--r--   0        0        0     4459 2024-04-08 10:22:31.659107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_set_request.py
+-rw-r--r--   0        0        0     4763 2024-04-08 10:22:31.663107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_stage_binding.py
+-rw-r--r--   0        0        0     3983 2024-04-08 10:22:31.667107 authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_stage_binding_request.py
+-rw-r--r--   0        0        0     2641 2024-04-08 10:22:31.667107 authentik_client-2024.2.2.post1712571742/authentik_client/models/footer_link.py
+-rw-r--r--   0        0        0     2531 2024-04-08 10:22:31.671107 authentik_client-2024.2.2.post1712571742/authentik_client/models/generic_error.py
+-rw-r--r--   0        0        0      865 2024-04-08 10:22:31.671107 authentik_client-2024.2.2.post1712571742/authentik_client/models/geoip_binding_enum.py
+-rw-r--r--   0        0        0     5216 2024-04-08 10:22:31.675107 authentik_client-2024.2.2.post1712571742/authentik_client/models/group.py
+-rw-r--r--   0        0        0     4209 2024-04-08 10:22:31.679107 authentik_client-2024.2.2.post1712571742/authentik_client/models/group_member.py
+-rw-r--r--   0        0        0     4006 2024-04-08 10:22:31.683107 authentik_client-2024.2.2.post1712571742/authentik_client/models/group_member_request.py
+-rw-r--r--   0        0        0     3347 2024-04-08 10:22:31.687107 authentik_client-2024.2.2.post1712571742/authentik_client/models/group_request.py
+-rw-r--r--   0        0        0     6080 2024-04-08 10:22:31.691107 authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_challenge.py
+-rw-r--r--   0        0        0     3174 2024-04-08 10:22:31.695107 authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_challenge_response_request.py
+-rw-r--r--   0        0        0     7503 2024-04-08 10:22:31.699107 authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_stage.py
+-rw-r--r--   0        0        0     6533 2024-04-08 10:22:31.703107 authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_stage_request.py
+-rw-r--r--   0        0        0     2438 2024-04-08 10:22:31.707107 authentik_client-2024.2.2.post1712571742/authentik_client/models/install_id.py
+-rw-r--r--   0        0        0      771 2024-04-08 10:22:31.707107 authentik_client-2024.2.2.post1712571742/authentik_client/models/intent_enum.py
+-rw-r--r--   0        0        0      800 2024-04-08 10:22:31.711107 authentik_client-2024.2.2.post1712571742/authentik_client/models/invalid_response_action_enum.py
+-rw-r--r--   0        0        0     4667 2024-04-08 10:22:31.715107 authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation.py
+-rw-r--r--   0        0        0     3684 2024-04-08 10:22:31.719107 authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_request.py
+-rw-r--r--   0        0        0     4508 2024-04-08 10:22:31.719107 authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_stage.py
+-rw-r--r--   0        0        0     3527 2024-04-08 10:22:31.723106 authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_stage_request.py
+-rw-r--r--   0        0        0      729 2024-04-08 10:22:31.727106 authentik_client-2024.2.2.post1712571742/authentik_client/models/issuer_mode_enum.py
+-rw-r--r--   0        0        0     4386 2024-04-08 10:22:31.727106 authentik_client-2024.2.2.post1712571742/authentik_client/models/kubernetes_service_connection.py
+-rw-r--r--   0        0        0     3454 2024-04-08 10:22:31.731107 authentik_client-2024.2.2.post1712571742/authentik_client/models/kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     2811 2024-04-08 10:22:31.735107 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_debug.py
+-rw-r--r--   0        0        0     5765 2024-04-08 10:22:31.739107 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_outpost_config.py
+-rw-r--r--   0        0        0     4378 2024-04-08 10:22:31.739107 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_property_mapping.py
+-rw-r--r--   0        0        0     3478 2024-04-08 10:22:31.743106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     8694 2024-04-08 10:22:31.747106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_provider.py
+-rw-r--r--   0        0        0     6192 2024-04-08 10:22:31.747106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_provider_request.py
+-rw-r--r--   0        0        0    11791 2024-04-08 10:22:31.751106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_source.py
+-rw-r--r--   0        0        0     9542 2024-04-08 10:22:31.755106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_source_request.py
+-rw-r--r--   0        0        0     3129 2024-04-08 10:22:31.759106 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_sync_status.py
+-rw-r--r--   0        0        0      726 2024-04-08 10:22:31.731107 authentik_client-2024.2.2.post1712571742/authentik_client/models/ldapapi_access_mode.py
+-rw-r--r--   0        0        0     3278 2024-04-08 10:22:31.763106 authentik_client-2024.2.2.post1712571742/authentik_client/models/license.py
+-rw-r--r--   0        0        0     2897 2024-04-08 10:22:31.767106 authentik_client-2024.2.2.post1712571742/authentik_client/models/license_forecast.py
+-rw-r--r--   0        0        0     2509 2024-04-08 10:22:31.775106 authentik_client-2024.2.2.post1712571742/authentik_client/models/license_request.py
+-rw-r--r--   0        0        0     3222 2024-04-08 10:22:31.779106 authentik_client-2024.2.2.post1712571742/authentik_client/models/license_summary.py
+-rw-r--r--   0        0        0     2411 2024-04-08 10:22:31.779106 authentik_client-2024.2.2.post1712571742/authentik_client/models/link.py
+-rw-r--r--   0        0        0     2882 2024-04-08 10:22:31.787106 authentik_client-2024.2.2.post1712571742/authentik_client/models/log_event.py
+-rw-r--r--   0        0        0      843 2024-04-08 10:22:31.787106 authentik_client-2024.2.2.post1712571742/authentik_client/models/log_level_enum.py
+-rw-r--r--   0        0        0     6520 2024-04-08 10:22:31.795106 authentik_client-2024.2.2.post1712571742/authentik_client/models/login_challenge_types.py
+-rw-r--r--   0        0        0     4171 2024-04-08 10:22:31.799106 authentik_client-2024.2.2.post1712571742/authentik_client/models/login_metrics.py
+-rw-r--r--   0        0        0     3192 2024-04-08 10:22:31.803106 authentik_client-2024.2.2.post1712571742/authentik_client/models/login_source.py
+-rw-r--r--   0        0        0     2513 2024-04-08 10:22:31.811106 authentik_client-2024.2.2.post1712571742/authentik_client/models/metadata.py
+-rw-r--r--   0        0        0     7524 2024-04-08 10:22:31.815106 authentik_client-2024.2.2.post1712571742/authentik_client/models/model_enum.py
+-rw-r--r--   0        0        0     9828 2024-04-08 10:22:31.819106 authentik_client-2024.2.2.post1712571742/authentik_client/models/model_request.py
+-rw-r--r--   0        0        0     1559 2024-04-08 10:22:31.823106 authentik_client-2024.2.2.post1712571742/authentik_client/models/name_id_policy_enum.py
+-rw-r--r--   0        0        0      831 2024-04-08 10:22:31.823106 authentik_client-2024.2.2.post1712571742/authentik_client/models/network_binding_enum.py
+-rw-r--r--   0        0        0      764 2024-04-08 10:22:31.827106 authentik_client-2024.2.2.post1712571742/authentik_client/models/not_configured_action_enum.py
+-rw-r--r--   0        0        0     3479 2024-04-08 10:22:31.827106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification.py
+-rw-r--r--   0        0        0     2858 2024-04-08 10:22:31.831106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_request.py
+-rw-r--r--   0        0        0     4010 2024-04-08 10:22:31.835106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_rule.py
+-rw-r--r--   0        0        0     3549 2024-04-08 10:22:31.839106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_rule_request.py
+-rw-r--r--   0        0        0     3760 2024-04-08 10:22:31.839106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport.py
+-rw-r--r--   0        0        0      818 2024-04-08 10:22:31.843106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_mode_enum.py
+-rw-r--r--   0        0        0     3500 2024-04-08 10:22:31.843106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_request.py
+-rw-r--r--   0        0        0     2503 2024-04-08 10:22:31.847106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_test.py
+-rw-r--r--   0        0        0     2707 2024-04-08 10:22:31.851106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_webhook_mapping.py
+-rw-r--r--   0        0        0     2717 2024-04-08 10:22:31.855106 authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     8888 2024-04-08 10:22:31.859106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider.py
+-rw-r--r--   0        0        0     6654 2024-04-08 10:22:31.863106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider_request.py
+-rw-r--r--   0        0        0     3482 2024-04-08 10:22:31.867106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider_setup_urls.py
+-rw-r--r--   0        0        0     4164 2024-04-08 10:22:31.871106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_challenge.py
+-rw-r--r--   0        0        0     2846 2024-04-08 10:22:31.875106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_challenge_response_request.py
+-rw-r--r--   0        0        0     4213 2024-04-08 10:22:31.879106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_finish_challenge.py
+-rw-r--r--   0        0        0     2816 2024-04-08 10:22:31.879106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
+-rw-r--r--   0        0        0    10563 2024-04-08 10:22:31.883106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_source.py
+-rw-r--r--   0        0        0     8069 2024-04-08 10:22:31.887106 authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_source_request.py
+-rw-r--r--   0        0        0     3922 2024-04-08 10:22:31.891106 authentik_client-2024.2.2.post1712571742/authentik_client/models/open_id_connect_configuration.py
+-rw-r--r--   0        0        0     5545 2024-04-08 10:22:31.895105 authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost.py
+-rw-r--r--   0        0        0     2541 2024-04-08 10:22:31.899105 authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_default_config.py
+-rw-r--r--   0        0        0     3755 2024-04-08 10:22:31.899105 authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_health.py
+-rw-r--r--   0        0        0     4050 2024-04-08 10:22:31.903105 authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_request.py
+-rw-r--r--   0        0        0      752 2024-04-08 10:22:31.907105 authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_type_enum.py
+-rw-r--r--   0        0        0     3322 2024-04-08 10:22:31.907105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_application_list.py
+-rw-r--r--   0        0        0     3395 2024-04-08 10:22:31.911105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticated_session_list.py
+-rw-r--r--   0        0        0     3404 2024-04-08 10:22:31.915105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_duo_stage_list.py
+-rw-r--r--   0        0        0     3404 2024-04-08 10:22:31.919105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_sms_stage_list.py
+-rw-r--r--   0        0        0     3428 2024-04-08 10:22:31.923105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_static_stage_list.py
+-rw-r--r--   0        0        0     3412 2024-04-08 10:22:31.923105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_totp_stage_list.py
+-rw-r--r--   0        0        0     3444 2024-04-08 10:22:31.927105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_validate_stage_list.py
+-rw-r--r--   0        0        0     3445 2024-04-08 10:22:31.931105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
+-rw-r--r--   0        0        0     3371 2024-04-08 10:22:31.935105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_blueprint_instance_list.py
+-rw-r--r--   0        0        0     3274 2024-04-08 10:22:31.935105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_brand_list.py
+-rw-r--r--   0        0        0     3331 2024-04-08 10:22:31.939105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_captcha_stage_list.py
+-rw-r--r--   0        0        0     3380 2024-04-08 10:22:31.943105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_certificate_key_pair_list.py
+-rw-r--r--   0        0        0     3355 2024-04-08 10:22:31.947105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_connection_token_list.py
+-rw-r--r--   0        0        0     3331 2024-04-08 10:22:31.947105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_consent_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-08 10:22:31.951105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_deny_stage_list.py
+-rw-r--r--   0        0        0     3420 2024-04-08 10:22:31.955105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_docker_service_connection_list.py
+-rw-r--r--   0        0        0     3282 2024-04-08 10:22:31.959105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_domain_list.py
+-rw-r--r--   0        0        0     3323 2024-04-08 10:22:31.963105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_dummy_policy_list.py
+-rw-r--r--   0        0        0     3315 2024-04-08 10:22:31.967105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_dummy_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-08 10:22:31.967105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_duo_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-08 10:22:31.971105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_email_stage_list.py
+-rw-r--r--   0        0        0     3298 2024-04-08 10:22:31.975105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_endpoint_list.py
+-rw-r--r--   0        0        0     3274 2024-04-08 10:22:31.979105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_event_list.py
+-rw-r--r--   0        0        0     3380 2024-04-08 10:22:31.979105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_event_matcher_policy_list.py
+-rw-r--r--   0        0        0     3413 2024-04-08 10:22:31.983105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_expiring_base_grant_model_list.py
+-rw-r--r--   0        0        0     3363 2024-04-08 10:22:31.987105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_expression_policy_list.py
+-rw-r--r--   0        0        0     3437 2024-04-08 10:22:31.987105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_extra_role_object_permission_list.py
+-rw-r--r--   0        0        0     3437 2024-04-08 10:22:31.991105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_extra_user_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-08 10:22:31.995105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_flow_list.py
+-rw-r--r--   0        0        0     3364 2024-04-08 10:22:31.995105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_flow_stage_binding_list.py
+-rw-r--r--   0        0        0     3274 2024-04-08 10:22:31.999105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_group_list.py
+-rw-r--r--   0        0        0     3387 2024-04-08 10:22:32.003105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_identification_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-08 10:22:32.007105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_invitation_list.py
+-rw-r--r--   0        0        0     3355 2024-04-08 10:22:32.007105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_invitation_stage_list.py
+-rw-r--r--   0        0        0     3452 2024-04-08 10:22:32.011105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_kubernetes_service_connection_list.py
+-rw-r--r--   0        0        0     3372 2024-04-08 10:22:32.015105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_outpost_config_list.py
+-rw-r--r--   0        0        0     3388 2024-04-08 10:22:32.015105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-08 10:22:32.019105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.023105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-08 10:22:32.023105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_license_list.py
+-rw-r--r--   0        0        0     3330 2024-04-08 10:22:32.027105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_list.py
+-rw-r--r--   0        0        0     3363 2024-04-08 10:22:32.031105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_rule_list.py
+-rw-r--r--   0        0        0     3403 2024-04-08 10:22:32.035105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_transport_list.py
+-rw-r--r--   0        0        0     3444 2024-04-08 10:22:32.039105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_webhook_mapping_list.py
+-rw-r--r--   0        0        0     3348 2024-04-08 10:22:32.039105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_o_auth2_provider_list.py
+-rw-r--r--   0        0        0     3324 2024-04-08 10:22:32.043105 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_o_auth_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-08 10:22:32.047104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_outpost_list.py
+-rw-r--r--   0        0        0     3396 2024-04-08 10:22:32.051104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_expiry_policy_list.py
+-rw-r--r--   0        0        0     3347 2024-04-08 10:22:32.055104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_policy_list.py
+-rw-r--r--   0        0        0     3339 2024-04-08 10:22:32.059104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-08 10:22:32.059104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_permission_list.py
+-rw-r--r--   0        0        0     3396 2024-04-08 10:22:32.063104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_plex_source_connection_list.py
+-rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.067104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_plex_source_list.py
+-rw-r--r--   0        0        0     3339 2024-04-08 10:22:32.071104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_policy_binding_list.py
+-rw-r--r--   0        0        0     3282 2024-04-08 10:22:32.075104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_policy_list.py
+-rw-r--r--   0        0        0     3282 2024-04-08 10:22:32.075104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_prompt_list.py
+-rw-r--r--   0        0        0     3323 2024-04-08 10:22:32.079104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_prompt_stage_list.py
+-rw-r--r--   0        0        0     3355 2024-04-08 10:22:32.083104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_property_mapping_list.py
+-rw-r--r--   0        0        0     3298 2024-04-08 10:22:32.083104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-08 10:22:32.087104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_proxy_outpost_config_list.py
+-rw-r--r--   0        0        0     3339 2024-04-08 10:22:32.087104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_proxy_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-08 10:22:32.091104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_rac_property_mapping_list.py
+-rw-r--r--   0        0        0     3323 2024-04-08 10:22:32.091104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_rac_provider_list.py
+-rw-r--r--   0        0        0     3388 2024-04-08 10:22:32.095104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_radius_outpost_config_list.py
+-rw-r--r--   0        0        0     3347 2024-04-08 10:22:32.099104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_radius_provider_list.py
+-rw-r--r--   0        0        0     3314 2024-04-08 10:22:32.099104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_reputation_list.py
+-rw-r--r--   0        0        0     3363 2024-04-08 10:22:32.103104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_reputation_policy_list.py
+-rw-r--r--   0        0        0     3461 2024-04-08 10:22:32.103104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_role_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-08 10:22:32.107104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_role_list.py
+-rw-r--r--   0        0        0     3388 2024-04-08 10:22:32.111104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-08 10:22:32.111104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.115104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-08 10:22:32.115104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scim_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-08 10:22:32.119104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scim_provider_list.py
+-rw-r--r--   0        0        0     3331 2024-04-08 10:22:32.123104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scope_mapping_list.py
+-rw-r--r--   0        0        0     3371 2024-04-08 10:22:32.123104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_service_connection_list.py
+-rw-r--r--   0        0        0     3307 2024-04-08 10:22:32.119104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_sms_device_list.py
+-rw-r--r--   0        0        0     3282 2024-04-08 10:22:32.127104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-08 10:22:32.127104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_source_stage_list.py
+-rw-r--r--   0        0        0     3274 2024-04-08 10:22:32.131104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_stage_list.py
+-rw-r--r--   0        0        0     3331 2024-04-08 10:22:32.135104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_static_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.135104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_system_task_list.py
+-rw-r--r--   0        0        0     3282 2024-04-08 10:22:32.143104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_tenant_list.py
+-rw-r--r--   0        0        0     3274 2024-04-08 10:22:32.147104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_token_list.py
+-rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.147104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_token_model_list.py
+-rw-r--r--   0        0        0     3315 2024-04-08 10:22:32.139104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_totp_device_list.py
+-rw-r--r--   0        0        0     3461 2024-04-08 10:22:32.151104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3323 2024-04-08 10:22:32.151104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_consent_list.py
+-rw-r--r--   0        0        0     3356 2024-04-08 10:22:32.155104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_delete_stage_list.py
+-rw-r--r--   0        0        0     3266 2024-04-08 10:22:32.155104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_list.py
+-rw-r--r--   0        0        0     3348 2024-04-08 10:22:32.159104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_login_stage_list.py
+-rw-r--r--   0        0        0     3356 2024-04-08 10:22:32.159104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_logout_stage_list.py
+-rw-r--r--   0        0        0     3438 2024-04-08 10:22:32.163104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_o_auth_source_connection_list.py
+-rw-r--r--   0        0        0     3429 2024-04-08 10:22:32.163104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_saml_source_connection_list.py
+-rw-r--r--   0        0        0     3396 2024-04-08 10:22:32.167104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_source_connection_list.py
+-rw-r--r--   0        0        0     3348 2024-04-08 10:22:32.171104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_write_stage_list.py
+-rw-r--r--   0        0        0     3348 2024-04-08 10:22:32.171104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_web_authn_device_list.py
+-rw-r--r--   0        0        0     3381 2024-04-08 10:22:32.175104 authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_web_authn_device_type_list.py
+-rw-r--r--   0        0        0     3076 2024-04-08 10:22:32.175104 authentik_client-2024.2.2.post1712571742/authentik_client/models/pagination.py
+-rw-r--r--   0        0        0     4454 2024-04-08 10:22:32.179104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_challenge.py
+-rw-r--r--   0        0        0     2819 2024-04-08 10:22:32.179104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_challenge_response_request.py
+-rw-r--r--   0        0        0     4377 2024-04-08 10:22:32.183104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_expiry_policy.py
+-rw-r--r--   0        0        0     3099 2024-04-08 10:22:32.183104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_expiry_policy_request.py
+-rw-r--r--   0        0        0     6428 2024-04-08 10:22:32.187104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_policy.py
+-rw-r--r--   0        0        0     5239 2024-04-08 10:22:32.187104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_policy_request.py
+-rw-r--r--   0        0        0     5274 2024-04-08 10:22:32.191104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_stage.py
+-rw-r--r--   0        0        0     4264 2024-04-08 10:22:32.195104 authentik_client-2024.2.2.post1712571742/authentik_client/models/password_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-08 10:22:32.195104 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_application_request.py
+-rw-r--r--   0        0        0     4833 2024-04-08 10:22:32.199103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     5701 2024-04-08 10:22:32.199103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4430 2024-04-08 10:22:32.203103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4256 2024-04-08 10:22:32.207104 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     4743 2024-04-08 10:22:32.207104 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5340 2024-04-08 10:22:32.211104 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     3246 2024-04-08 10:22:32.211104 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_blueprint_instance_request.py
+-rw-r--r--   0        0        0     6352 2024-04-08 10:22:32.215103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_brand_request.py
+-rw-r--r--   0        0        0     3860 2024-04-08 10:22:32.219103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_captcha_stage_request.py
+-rw-r--r--   0        0        0     3051 2024-04-08 10:22:32.219103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_certificate_key_pair_request.py
+-rw-r--r--   0        0        0     2717 2024-04-08 10:22:32.223103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_connection_token_request.py
+-rw-r--r--   0        0        0     3607 2024-04-08 10:22:32.223103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_consent_stage_request.py
+-rw-r--r--   0        0        0     3268 2024-04-08 10:22:32.227103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_deny_stage_request.py
+-rw-r--r--   0        0        0     4149 2024-04-08 10:22:32.227103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_docker_service_connection_request.py
+-rw-r--r--   0        0        0     2801 2024-04-08 10:22:32.231103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_domain_request.py
+-rw-r--r--   0        0        0     3275 2024-04-08 10:22:32.231103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_dummy_policy_request.py
+-rw-r--r--   0        0        0     3270 2024-04-08 10:22:32.235103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_dummy_stage_request.py
+-rw-r--r--   0        0        0     2674 2024-04-08 10:22:32.235103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_duo_device_request.py
+-rw-r--r--   0        0        0     5159 2024-04-08 10:22:32.239103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_email_stage_request.py
+-rw-r--r--   0        0        0     3784 2024-04-08 10:22:32.239103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_endpoint_request.py
+-rw-r--r--   0        0        0     4845 2024-04-08 10:22:32.243103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_event_matcher_policy_request.py
+-rw-r--r--   0        0        0     4045 2024-04-08 10:22:32.243103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_event_request.py
+-rw-r--r--   0        0        0     3047 2024-04-08 10:22:32.247103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_expression_policy_request.py
+-rw-r--r--   0        0        0     4903 2024-04-08 10:22:32.251103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_flow_request.py
+-rw-r--r--   0        0        0     4055 2024-04-08 10:22:32.251103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_flow_stage_binding_request.py
+-rw-r--r--   0        0        0     3385 2024-04-08 10:22:32.255103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_group_request.py
+-rw-r--r--   0        0        0     6571 2024-04-08 10:22:32.259103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_identification_stage_request.py
+-rw-r--r--   0        0        0     3774 2024-04-08 10:22:32.263103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_invitation_request.py
+-rw-r--r--   0        0        0     3565 2024-04-08 10:22:32.267103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_invitation_stage_request.py
+-rw-r--r--   0        0        0     3492 2024-04-08 10:22:32.267103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     3550 2024-04-08 10:22:32.271103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     6254 2024-04-08 10:22:32.275103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_provider_request.py
+-rw-r--r--   0        0        0     9697 2024-04-08 10:22:32.275103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_source_request.py
+-rw-r--r--   0        0        0     2557 2024-04-08 10:22:32.279103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_license_request.py
+-rw-r--r--   0        0        0     2879 2024-04-08 10:22:32.279103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_request.py
+-rw-r--r--   0        0        0     3587 2024-04-08 10:22:32.283103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_rule_request.py
+-rw-r--r--   0        0        0     3538 2024-04-08 10:22:32.283103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_transport_request.py
+-rw-r--r--   0        0        0     2782 2024-04-08 10:22:32.287103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     6716 2024-04-08 10:22:32.291103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_o_auth2_provider_request.py
+-rw-r--r--   0        0        0     8241 2024-04-08 10:22:32.291103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_o_auth_source_request.py
+-rw-r--r--   0        0        0     4139 2024-04-08 10:22:32.295103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_outpost_request.py
+-rw-r--r--   0        0        0     3154 2024-04-08 10:22:32.295103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_expiry_policy_request.py
+-rw-r--r--   0        0        0     5277 2024-04-08 10:22:32.299103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_policy_request.py
+-rw-r--r--   0        0        0     4326 2024-04-08 10:22:32.303103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_stage_request.py
+-rw-r--r--   0        0        0     2922 2024-04-08 10:22:32.303103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_permission_assign_request.py
+-rw-r--r--   0        0        0     2784 2024-04-08 10:22:32.307103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_plex_source_connection_request.py
+-rw-r--r--   0        0        0     5905 2024-04-08 10:22:32.311103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_plex_source_request.py
+-rw-r--r--   0        0        0     4286 2024-04-08 10:22:32.315103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_policy_binding_request.py
+-rw-r--r--   0        0        0     5023 2024-04-08 10:22:32.315103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_prompt_request.py
+-rw-r--r--   0        0        0     3406 2024-04-08 10:22:32.319103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_prompt_stage_request.py
+-rw-r--r--   0        0        0     6907 2024-04-08 10:22:32.323103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_proxy_provider_request.py
+-rw-r--r--   0        0        0     3495 2024-04-08 10:22:32.323103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_rac_property_mapping_request.py
+-rw-r--r--   0        0        0     4413 2024-04-08 10:22:32.327103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_rac_provider_request.py
+-rw-r--r--   0        0        0     4563 2024-04-08 10:22:32.331103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_radius_provider_request.py
+-rw-r--r--   0        0        0     3276 2024-04-08 10:22:32.331103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_reputation_policy_request.py
+-rw-r--r--   0        0        0     2565 2024-04-08 10:22:32.335103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_role_request.py
+-rw-r--r--   0        0        0     3901 2024-04-08 10:22:32.339103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_property_mapping_request.py
+-rw-r--r--   0        0        0     7539 2024-04-08 10:22:32.339103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_provider_request.py
+-rw-r--r--   0        0        0     8676 2024-04-08 10:22:32.343103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_source_request.py
+-rw-r--r--   0        0        0     3364 2024-04-08 10:22:32.347102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scim_mapping_request.py
+-rw-r--r--   0        0        0     3888 2024-04-08 10:22:32.347102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scim_provider_request.py
+-rw-r--r--   0        0        0     3819 2024-04-08 10:22:32.355103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scope_mapping_request.py
+-rw-r--r--   0        0        0     4590 2024-04-08 10:22:32.355103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_settings_request.py
+-rw-r--r--   0        0        0     2674 2024-04-08 10:22:32.351102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_sms_device_request.py
+-rw-r--r--   0        0        0     3562 2024-04-08 10:22:32.359103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_source_stage_request.py
+-rw-r--r--   0        0        0     2686 2024-04-08 10:22:32.359103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_static_device_request.py
+-rw-r--r--   0        0        0     2820 2024-04-08 10:22:32.367102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_tenant_request.py
+-rw-r--r--   0        0        0     4208 2024-04-08 10:22:32.367102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_token_request.py
+-rw-r--r--   0        0        0     2678 2024-04-08 10:22:32.363103 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_totp_device_request.py
+-rw-r--r--   0        0        0     3167 2024-04-08 10:22:32.371102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_delete_stage_request.py
+-rw-r--r--   0        0        0     4766 2024-04-08 10:22:32.371102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_login_stage_request.py
+-rw-r--r--   0        0        0     3167 2024-04-08 10:22:32.375102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_logout_stage_request.py
+-rw-r--r--   0        0        0     3109 2024-04-08 10:22:32.379102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3934 2024-04-08 10:22:32.379102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_request.py
+-rw-r--r--   0        0        0     2733 2024-04-08 10:22:32.383102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     4450 2024-04-08 10:22:32.383102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_write_stage_request.py
+-rw-r--r--   0        0        0     2625 2024-04-08 10:22:32.387102 authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_web_authn_device_request.py
+-rw-r--r--   0        0        0     3548 2024-04-08 10:22:32.387102 authentik_client-2024.2.2.post1712571742/authentik_client/models/permission.py
+-rw-r--r--   0        0        0     2884 2024-04-08 10:22:32.391102 authentik_client-2024.2.2.post1712571742/authentik_client/models/permission_assign_request.py
+-rw-r--r--   0        0        0     4315 2024-04-08 10:22:32.395102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_authentication_challenge.py
+-rw-r--r--   0        0        0     2726 2024-04-08 10:22:32.395102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_authentication_challenge_response_request.py
+-rw-r--r--   0        0        0     7752 2024-04-08 10:22:32.399102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source.py
+-rw-r--r--   0        0        0     3265 2024-04-08 10:22:32.403102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_connection.py
+-rw-r--r--   0        0        0     2719 2024-04-08 10:22:32.403102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_connection_request.py
+-rw-r--r--   0        0        0     5760 2024-04-08 10:22:32.407102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_request.py
+-rw-r--r--   0        0        0     2576 2024-04-08 10:22:32.411102 authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_token_redeem_request.py
+-rw-r--r--   0        0        0     4055 2024-04-08 10:22:32.415102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy.py
+-rw-r--r--   0        0        0     5643 2024-04-08 10:22:32.415102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_binding.py
+-rw-r--r--   0        0        0     4231 2024-04-08 10:22:32.419102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_binding_request.py
+-rw-r--r--   0        0        0      711 2024-04-08 10:22:32.419102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_engine_mode.py
+-rw-r--r--   0        0        0     2817 2024-04-08 10:22:32.423102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_request.py
+-rw-r--r--   0        0        0     2583 2024-04-08 10:22:32.427102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_test_request.py
+-rw-r--r--   0        0        0     3281 2024-04-08 10:22:32.427102 authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_test_result.py
+-rw-r--r--   0        0        0     4885 2024-04-08 10:22:32.431102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt.py
+-rw-r--r--   0        0        0     4649 2024-04-08 10:22:32.435102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_challenge.py
+-rw-r--r--   0        0        0     3325 2024-04-08 10:22:32.435102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_challenge_response_request.py
+-rw-r--r--   0        0        0     4927 2024-04-08 10:22:32.439102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_request.py
+-rw-r--r--   0        0        0     4321 2024-04-08 10:22:32.439102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_stage.py
+-rw-r--r--   0        0        0     3351 2024-04-08 10:22:32.443102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_stage_request.py
+-rw-r--r--   0        0        0     1185 2024-04-08 10:22:32.443102 authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_type_enum.py
+-rw-r--r--   0        0        0     4264 2024-04-08 10:22:32.443102 authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping.py
+-rw-r--r--   0        0        0     2610 2024-04-08 10:22:32.447102 authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping_preview.py
+-rw-r--r--   0        0        0     2744 2024-04-08 10:22:32.447102 authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping_test_result.py
+-rw-r--r--   0        0        0      715 2024-04-08 10:22:32.451102 authentik_client-2024.2.2.post1712571742/authentik_client/models/protocol_enum.py
+-rw-r--r--   0        0        0     5722 2024-04-08 10:22:32.451102 authentik_client-2024.2.2.post1712571742/authentik_client/models/provider.py
+-rw-r--r--   0        0        0      713 2024-04-08 10:22:32.455102 authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_enum.py
+-rw-r--r--   0        0        0     1314 2024-04-08 10:22:32.455102 authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_model_enum.py
+-rw-r--r--   0        0        0     3397 2024-04-08 10:22:32.455102 authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_request.py
+-rw-r--r--   0        0        0     1009 2024-04-08 10:22:32.455102 authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_type_enum.py
+-rw-r--r--   0        0        0      754 2024-04-08 10:22:32.459102 authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_mode.py
+-rw-r--r--   0        0        0     7819 2024-04-08 10:22:32.459102 authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_outpost_config.py
+-rw-r--r--   0        0        0     9552 2024-04-08 10:22:32.463102 authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_provider.py
+-rw-r--r--   0        0        0     6828 2024-04-08 10:22:32.463102 authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_provider_request.py
+-rw-r--r--   0        0        0     4407 2024-04-08 10:22:32.463102 authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_property_mapping.py
+-rw-r--r--   0        0        0     3440 2024-04-08 10:22:32.467102 authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_property_mapping_request.py
+-rw-r--r--   0        0        0     6813 2024-04-08 10:22:32.467102 authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_provider.py
+-rw-r--r--   0        0        0     4351 2024-04-08 10:22:32.471102 authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_provider_request.py
+-rw-r--r--   0        0        0     3833 2024-04-08 10:22:32.471102 authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_outpost_config.py
+-rw-r--r--   0        0        0     6924 2024-04-08 10:22:32.475102 authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_provider.py
+-rw-r--r--   0        0        0     4501 2024-04-08 10:22:32.475102 authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_provider_request.py
+-rw-r--r--   0        0        0     4184 2024-04-08 10:22:32.479102 authentik_client-2024.2.2.post1712571742/authentik_client/models/redirect_challenge.py
+-rw-r--r--   0        0        0     3642 2024-04-08 10:22:32.483102 authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation.py
+-rw-r--r--   0        0        0     4516 2024-04-08 10:22:32.483102 authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation_policy.py
+-rw-r--r--   0        0        0     3238 2024-04-08 10:22:32.487102 authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation_policy_request.py
+-rw-r--r--   0        0        0      795 2024-04-08 10:22:32.487102 authentik_client-2024.2.2.post1712571742/authentik_client/models/resident_key_requirement_enum.py
+-rw-r--r--   0        0        0     2618 2024-04-08 10:22:32.487102 authentik_client-2024.2.2.post1712571742/authentik_client/models/role.py
+-rw-r--r--   0        0        0     3333 2024-04-08 10:22:32.491102 authentik_client-2024.2.2.post1712571742/authentik_client/models/role_assigned_object_permission.py
+-rw-r--r--   0        0        0     3293 2024-04-08 10:22:32.491102 authentik_client-2024.2.2.post1712571742/authentik_client/models/role_object_permission.py
+-rw-r--r--   0        0        0     2517 2024-04-08 10:22:32.495102 authentik_client-2024.2.2.post1712571742/authentik_client/models/role_request.py
+-rw-r--r--   0        0        0     2712 2024-04-08 10:22:32.495102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_metadata.py
+-rw-r--r--   0        0        0     4718 2024-04-08 10:22:32.503102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_property_mapping.py
+-rw-r--r--   0        0        0     3829 2024-04-08 10:22:32.503102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_property_mapping_request.py
+-rw-r--r--   0        0        0    11056 2024-04-08 10:22:32.507102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_provider.py
+-rw-r--r--   0        0        0     7460 2024-04-08 10:22:32.511102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_provider_request.py
+-rw-r--r--   0        0        0    10563 2024-04-08 10:22:32.511102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_source.py
+-rw-r--r--   0        0        0     8507 2024-04-08 10:22:32.515102 authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_source_request.py
+-rw-r--r--   0        0        0     4248 2024-04-08 10:22:32.519101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_mapping.py
+-rw-r--r--   0        0        0     3309 2024-04-08 10:22:32.523101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_mapping_request.py
+-rw-r--r--   0        0        0     5454 2024-04-08 10:22:32.523101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_provider.py
+-rw-r--r--   0        0        0     3802 2024-04-08 10:22:32.527101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_provider_request.py
+-rw-r--r--   0        0        0     3131 2024-04-08 10:22:32.531101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_sync_status.py
+-rw-r--r--   0        0        0     4629 2024-04-08 10:22:32.535101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scope_mapping.py
+-rw-r--r--   0        0        0     3740 2024-04-08 10:22:32.539101 authentik_client-2024.2.2.post1712571742/authentik_client/models/scope_mapping_request.py
+-rw-r--r--   0        0        0     2738 2024-04-08 10:22:32.543101 authentik_client-2024.2.2.post1712571742/authentik_client/models/selectable_stage.py
+-rw-r--r--   0        0        0     3773 2024-04-08 10:22:32.543101 authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection.py
+-rw-r--r--   0        0        0     2776 2024-04-08 10:22:32.547101 authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection_request.py
+-rw-r--r--   0        0        0     2731 2024-04-08 10:22:32.551101 authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection_state.py
+-rw-r--r--   0        0        0     3178 2024-04-08 10:22:32.551101 authentik_client-2024.2.2.post1712571742/authentik_client/models/session_user.py
+-rw-r--r--   0        0        0     4441 2024-04-08 10:22:32.555101 authentik_client-2024.2.2.post1712571742/authentik_client/models/settings.py
+-rw-r--r--   0        0        0     4569 2024-04-08 10:22:32.559101 authentik_client-2024.2.2.post1712571742/authentik_client/models/settings_request.py
+-rw-r--r--   0        0        0      733 2024-04-08 10:22:32.559101 authentik_client-2024.2.2.post1712571742/authentik_client/models/severity_enum.py
+-rw-r--r--   0        0        0     4175 2024-04-08 10:22:32.563101 authentik_client-2024.2.2.post1712571742/authentik_client/models/shell_challenge.py
+-rw-r--r--   0        0        0     1492 2024-04-08 10:22:32.563101 authentik_client-2024.2.2.post1712571742/authentik_client/models/signature_algorithm_enum.py
+-rw-r--r--   0        0        0     2906 2024-04-08 10:22:32.531101 authentik_client-2024.2.2.post1712571742/authentik_client/models/sms_device.py
+-rw-r--r--   0        0        0     2619 2024-04-08 10:22:32.535101 authentik_client-2024.2.2.post1712571742/authentik_client/models/sms_device_request.py
+-rw-r--r--   0        0        0     6945 2024-04-08 10:22:32.567101 authentik_client-2024.2.2.post1712571742/authentik_client/models/source.py
+-rw-r--r--   0        0        0     4836 2024-04-08 10:22:32.571101 authentik_client-2024.2.2.post1712571742/authentik_client/models/source_request.py
+-rw-r--r--   0        0        0     4438 2024-04-08 10:22:32.575101 authentik_client-2024.2.2.post1712571742/authentik_client/models/source_stage.py
+-rw-r--r--   0        0        0     3507 2024-04-08 10:22:32.579101 authentik_client-2024.2.2.post1712571742/authentik_client/models/source_stage_request.py
+-rw-r--r--   0        0        0     5355 2024-04-08 10:22:32.579101 authentik_client-2024.2.2.post1712571742/authentik_client/models/source_type.py
+-rw-r--r--   0        0        0      714 2024-04-08 10:22:32.583101 authentik_client-2024.2.2.post1712571742/authentik_client/models/sp_binding_enum.py
+-rw-r--r--   0        0        0     4070 2024-04-08 10:22:32.583101 authentik_client-2024.2.2.post1712571742/authentik_client/models/stage.py
+-rw-r--r--   0        0        0     3437 2024-04-08 10:22:32.587101 authentik_client-2024.2.2.post1712571742/authentik_client/models/stage_prompt.py
+-rw-r--r--   0        0        0     3089 2024-04-08 10:22:32.591101 authentik_client-2024.2.2.post1712571742/authentik_client/models/stage_request.py
+-rw-r--r--   0        0        0     3385 2024-04-08 10:22:32.591101 authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device.py
+-rw-r--r--   0        0        0     2631 2024-04-08 10:22:32.595101 authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_request.py
+-rw-r--r--   0        0        0     2546 2024-04-08 10:22:32.599101 authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_token.py
+-rw-r--r--   0        0        0     2581 2024-04-08 10:22:32.603101 authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_token_request.py
+-rw-r--r--   0        0        0      846 2024-04-08 10:22:32.603101 authentik_client-2024.2.2.post1712571742/authentik_client/models/sub_mode_enum.py
+-rw-r--r--   0        0        0     4463 2024-04-08 10:22:32.607101 authentik_client-2024.2.2.post1712571742/authentik_client/models/system_info.py
+-rw-r--r--   0        0        0     2934 2024-04-08 10:22:32.607101 authentik_client-2024.2.2.post1712571742/authentik_client/models/system_info_runtime.py
+-rw-r--r--   0        0        0     4286 2024-04-08 10:22:32.611101 authentik_client-2024.2.2.post1712571742/authentik_client/models/system_task.py
+-rw-r--r--   0        0        0      789 2024-04-08 10:22:32.611101 authentik_client-2024.2.2.post1712571742/authentik_client/models/system_task_status_enum.py
+-rw-r--r--   0        0        0     2872 2024-04-08 10:22:32.619101 authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant.py
+-rw-r--r--   0        0        0     2589 2024-04-08 10:22:32.623101 authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_admin_group_request_request.py
+-rw-r--r--   0        0        0     2705 2024-04-08 10:22:32.627101 authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_recovery_key_request_request.py
+-rw-r--r--   0        0        0     2599 2024-04-08 10:22:32.631101 authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_recovery_key_response.py
+-rw-r--r--   0        0        0     2765 2024-04-08 10:22:32.631101 authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_request.py
+-rw-r--r--   0        0        0     4591 2024-04-08 10:22:32.635101 authentik_client-2024.2.2.post1712571742/authentik_client/models/token.py
+-rw-r--r--   0        0        0     3987 2024-04-08 10:22:32.639101 authentik_client-2024.2.2.post1712571742/authentik_client/models/token_model.py
+-rw-r--r--   0        0        0     4118 2024-04-08 10:22:32.643101 authentik_client-2024.2.2.post1712571742/authentik_client/models/token_request.py
+-rw-r--r--   0        0        0     2521 2024-04-08 10:22:32.643101 authentik_client-2024.2.2.post1712571742/authentik_client/models/token_set_key_request.py
+-rw-r--r--   0        0        0     2494 2024-04-08 10:22:32.647101 authentik_client-2024.2.2.post1712571742/authentik_client/models/token_view.py
+-rw-r--r--   0        0        0     2724 2024-04-08 10:22:32.615101 authentik_client-2024.2.2.post1712571742/authentik_client/models/totp_device.py
+-rw-r--r--   0        0        0     2623 2024-04-08 10:22:32.619101 authentik_client-2024.2.2.post1712571742/authentik_client/models/totp_device_request.py
+-rw-r--r--   0        0        0     3389 2024-04-08 10:22:32.651101 authentik_client-2024.2.2.post1712571742/authentik_client/models/transaction_application_request.py
+-rw-r--r--   0        0        0     2595 2024-04-08 10:22:32.651101 authentik_client-2024.2.2.post1712571742/authentik_client/models/transaction_application_response.py
+-rw-r--r--   0        0        0     2936 2024-04-08 10:22:32.655101 authentik_client-2024.2.2.post1712571742/authentik_client/models/type_create.py
+-rw-r--r--   0        0        0      730 2024-04-08 10:22:32.655101 authentik_client-2024.2.2.post1712571742/authentik_client/models/ui_theme_enum.py
+-rw-r--r--   0        0        0     2808 2024-04-08 10:22:32.659101 authentik_client-2024.2.2.post1712571742/authentik_client/models/used_by.py
+-rw-r--r--   0        0        0      795 2024-04-08 10:22:32.659101 authentik_client-2024.2.2.post1712571742/authentik_client/models/used_by_action_enum.py
+-rw-r--r--   0        0        0     5226 2024-04-08 10:22:32.663101 authentik_client-2024.2.2.post1712571742/authentik_client/models/user.py
+-rw-r--r--   0        0        0     2458 2024-04-08 10:22:32.667101 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_account_request.py
+-rw-r--r--   0        0        0     4946 2024-04-08 10:22:32.671100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_assigned_object_permission.py
+-rw-r--r--   0        0        0     3617 2024-04-08 10:22:32.675100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_consent.py
+-rw-r--r--   0        0        0      811 2024-04-08 10:22:32.675100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_creation_mode_enum.py
+-rw-r--r--   0        0        0     4110 2024-04-08 10:22:32.679100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_delete_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-08 10:22:32.683100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_delete_stage_request.py
+-rw-r--r--   0        0        0      735 2024-04-08 10:22:32.683100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_fields_enum.py
+-rw-r--r--   0        0        0     3909 2024-04-08 10:22:32.687101 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_group.py
+-rw-r--r--   0        0        0     3193 2024-04-08 10:22:32.687101 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_group_request.py
+-rw-r--r--   0        0        0     4334 2024-04-08 10:22:32.691100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_challenge.py
+-rw-r--r--   0        0        0     2805 2024-04-08 10:22:32.695100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_challenge_response_request.py
+-rw-r--r--   0        0        0     5631 2024-04-08 10:22:32.699100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_stage.py
+-rw-r--r--   0        0        0     4728 2024-04-08 10:22:32.703100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_stage_request.py
+-rw-r--r--   0        0        0     4110 2024-04-08 10:22:32.703100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_logout_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-08 10:22:32.707100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_logout_stage_request.py
+-rw-r--r--   0        0        0      853 2024-04-08 10:22:32.711100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_matching_mode_enum.py
+-rw-r--r--   0        0        0     4160 2024-04-08 10:22:32.711100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_metrics.py
+-rw-r--r--   0        0        0     3188 2024-04-08 10:22:32.715100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_o_auth_source_connection.py
+-rw-r--r--   0        0        0     3054 2024-04-08 10:22:32.715100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3293 2024-04-08 10:22:32.719100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_object_permission.py
+-rw-r--r--   0        0        0     2557 2024-04-08 10:22:32.719100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_password_set_request.py
+-rw-r--r--   0        0        0     2491 2024-04-08 10:22:32.723100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_path.py
+-rw-r--r--   0        0        0     3872 2024-04-08 10:22:32.723100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_request.py
+-rw-r--r--   0        0        0     3107 2024-04-08 10:22:32.727100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_saml_source_connection.py
+-rw-r--r--   0        0        0     2668 2024-04-08 10:22:32.727100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     5465 2024-04-08 10:22:32.731100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_self.py
+-rw-r--r--   0        0        0     2629 2024-04-08 10:22:32.731100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_self_groups.py
+-rw-r--r--   0        0        0     3074 2024-04-08 10:22:32.731100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_service_account_request.py
+-rw-r--r--   0        0        0     2844 2024-04-08 10:22:32.735100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_service_account_response.py
+-rw-r--r--   0        0        0     2866 2024-04-08 10:22:32.735100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_setting.py
+-rw-r--r--   0        0        0     3245 2024-04-08 10:22:32.739100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_source_connection.py
+-rw-r--r--   0        0        0      817 2024-04-08 10:22:32.739100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_type_enum.py
+-rw-r--r--   0        0        0      777 2024-04-08 10:22:32.739100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_verification_enum.py
+-rw-r--r--   0        0        0     5382 2024-04-08 10:22:32.743100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_write_stage.py
+-rw-r--r--   0        0        0     4412 2024-04-08 10:22:32.743100 authentik_client-2024.2.2.post1712571742/authentik_client/models/user_write_stage_request.py
+-rw-r--r--   0        0        0     3197 2024-04-08 10:22:32.747100 authentik_client-2024.2.2.post1712571742/authentik_client/models/validation_error.py
+-rw-r--r--   0        0        0     3589 2024-04-08 10:22:32.751100 authentik_client-2024.2.2.post1712571742/authentik_client/models/version.py
+-rw-r--r--   0        0        0     3630 2024-04-08 10:22:32.751100 authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device.py
+-rw-r--r--   0        0        0     2577 2024-04-08 10:22:32.755100 authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device_request.py
+-rw-r--r--   0        0        0     2562 2024-04-08 10:22:32.755100 authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device_type.py
+-rw-r--r--   0        0        0     2669 2024-04-08 10:22:32.759100 authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device_type_request.py
+-rw-r--r--   0        0        0     2410 2024-04-08 10:22:32.759100 authentik_client-2024.2.2.post1712571742/authentik_client/models/workers.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:22:33.847093 authentik_client-2024.2.2.post1712571742/authentik_client/py.typed
+-rw-r--r--   0        0        0     9196 2024-04-08 10:22:33.855093 authentik_client-2024.2.2.post1712571742/authentik_client/rest.py
+-rw-r--r--   0        0        0     1936 2024-04-08 10:22:33.847093 authentik_client-2024.2.2.post1712571742/pyproject.toml
+-rw-r--r--   0        0        0   141557 1970-01-01 00:00:00.000000 authentik_client-2024.2.2.post1712571742/PKG-INFO
```

### Comparing `authentik_client-2024.2.2.post1712239192/README.md` & `authentik_client-2024.2.2.post1712571742/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.2.2
-- Package version: 2024.2.2-1712239192
+- Package version: 2024.2.2-1712571742
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -675,14 +675,16 @@
 *StagesApi* | [**stages_authenticator_validate_list**](docs/StagesApi.md#stages_authenticator_validate_list) | **GET** /stages/authenticator/validate/ | 
 *StagesApi* | [**stages_authenticator_validate_partial_update**](docs/StagesApi.md#stages_authenticator_validate_partial_update) | **PATCH** /stages/authenticator/validate/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_validate_retrieve**](docs/StagesApi.md#stages_authenticator_validate_retrieve) | **GET** /stages/authenticator/validate/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_validate_update**](docs/StagesApi.md#stages_authenticator_validate_update) | **PUT** /stages/authenticator/validate/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_validate_used_by_list**](docs/StagesApi.md#stages_authenticator_validate_used_by_list) | **GET** /stages/authenticator/validate/{stage_uuid}/used_by/ | 
 *StagesApi* | [**stages_authenticator_webauthn_create**](docs/StagesApi.md#stages_authenticator_webauthn_create) | **POST** /stages/authenticator/webauthn/ | 
 *StagesApi* | [**stages_authenticator_webauthn_destroy**](docs/StagesApi.md#stages_authenticator_webauthn_destroy) | **DELETE** /stages/authenticator/webauthn/{stage_uuid}/ | 
+*StagesApi* | [**stages_authenticator_webauthn_device_types_list**](docs/StagesApi.md#stages_authenticator_webauthn_device_types_list) | **GET** /stages/authenticator/webauthn_device_types/ | 
+*StagesApi* | [**stages_authenticator_webauthn_device_types_retrieve**](docs/StagesApi.md#stages_authenticator_webauthn_device_types_retrieve) | **GET** /stages/authenticator/webauthn_device_types/{aaguid}/ | 
 *StagesApi* | [**stages_authenticator_webauthn_list**](docs/StagesApi.md#stages_authenticator_webauthn_list) | **GET** /stages/authenticator/webauthn/ | 
 *StagesApi* | [**stages_authenticator_webauthn_partial_update**](docs/StagesApi.md#stages_authenticator_webauthn_partial_update) | **PATCH** /stages/authenticator/webauthn/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_webauthn_retrieve**](docs/StagesApi.md#stages_authenticator_webauthn_retrieve) | **GET** /stages/authenticator/webauthn/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_webauthn_update**](docs/StagesApi.md#stages_authenticator_webauthn_update) | **PUT** /stages/authenticator/webauthn/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_webauthn_used_by_list**](docs/StagesApi.md#stages_authenticator_webauthn_used_by_list) | **GET** /stages/authenticator/webauthn/{stage_uuid}/used_by/ | 
 *StagesApi* | [**stages_captcha_create**](docs/StagesApi.md#stages_captcha_create) | **POST** /stages/captcha/ | 
 *StagesApi* | [**stages_captcha_destroy**](docs/StagesApi.md#stages_captcha_destroy) | **DELETE** /stages/captcha/{stage_uuid}/ | 
@@ -821,16 +823,14 @@
  - [AppEnum](docs/AppEnum.md)
  - [AppleChallengeResponseRequest](docs/AppleChallengeResponseRequest.md)
  - [AppleLoginChallenge](docs/AppleLoginChallenge.md)
  - [Application](docs/Application.md)
  - [ApplicationRequest](docs/ApplicationRequest.md)
  - [AuthModeEnum](docs/AuthModeEnum.md)
  - [AuthTypeEnum](docs/AuthTypeEnum.md)
- - [AuthenticateWebAuthnStage](docs/AuthenticateWebAuthnStage.md)
- - [AuthenticateWebAuthnStageRequest](docs/AuthenticateWebAuthnStageRequest.md)
  - [AuthenticatedSession](docs/AuthenticatedSession.md)
  - [AuthenticatedSessionAsn](docs/AuthenticatedSessionAsn.md)
  - [AuthenticatedSessionGeoIp](docs/AuthenticatedSessionGeoIp.md)
  - [AuthenticatedSessionUserAgent](docs/AuthenticatedSessionUserAgent.md)
  - [AuthenticatedSessionUserAgentDevice](docs/AuthenticatedSessionUserAgentDevice.md)
  - [AuthenticatedSessionUserAgentOs](docs/AuthenticatedSessionUserAgentOs.md)
  - [AuthenticatedSessionUserAgentUserAgent](docs/AuthenticatedSessionUserAgentUserAgent.md)
@@ -856,14 +856,16 @@
  - [AuthenticatorTOTPStageRequest](docs/AuthenticatorTOTPStageRequest.md)
  - [AuthenticatorValidateStage](docs/AuthenticatorValidateStage.md)
  - [AuthenticatorValidateStageRequest](docs/AuthenticatorValidateStageRequest.md)
  - [AuthenticatorValidationChallenge](docs/AuthenticatorValidationChallenge.md)
  - [AuthenticatorValidationChallengeResponseRequest](docs/AuthenticatorValidationChallengeResponseRequest.md)
  - [AuthenticatorWebAuthnChallenge](docs/AuthenticatorWebAuthnChallenge.md)
  - [AuthenticatorWebAuthnChallengeResponseRequest](docs/AuthenticatorWebAuthnChallengeResponseRequest.md)
+ - [AuthenticatorWebAuthnStage](docs/AuthenticatorWebAuthnStage.md)
+ - [AuthenticatorWebAuthnStageRequest](docs/AuthenticatorWebAuthnStageRequest.md)
  - [AutoSubmitChallengeResponseRequest](docs/AutoSubmitChallengeResponseRequest.md)
  - [AutosubmitChallenge](docs/AutosubmitChallenge.md)
  - [BackendsEnum](docs/BackendsEnum.md)
  - [BindingTypeEnum](docs/BindingTypeEnum.md)
  - [BlueprintFile](docs/BlueprintFile.md)
  - [BlueprintInstance](docs/BlueprintInstance.md)
  - [BlueprintInstanceRequest](docs/BlueprintInstanceRequest.md)
@@ -1022,21 +1024,21 @@
  - [OpenIDConnectConfiguration](docs/OpenIDConnectConfiguration.md)
  - [Outpost](docs/Outpost.md)
  - [OutpostDefaultConfig](docs/OutpostDefaultConfig.md)
  - [OutpostHealth](docs/OutpostHealth.md)
  - [OutpostRequest](docs/OutpostRequest.md)
  - [OutpostTypeEnum](docs/OutpostTypeEnum.md)
  - [PaginatedApplicationList](docs/PaginatedApplicationList.md)
- - [PaginatedAuthenticateWebAuthnStageList](docs/PaginatedAuthenticateWebAuthnStageList.md)
  - [PaginatedAuthenticatedSessionList](docs/PaginatedAuthenticatedSessionList.md)
  - [PaginatedAuthenticatorDuoStageList](docs/PaginatedAuthenticatorDuoStageList.md)
  - [PaginatedAuthenticatorSMSStageList](docs/PaginatedAuthenticatorSMSStageList.md)
  - [PaginatedAuthenticatorStaticStageList](docs/PaginatedAuthenticatorStaticStageList.md)
  - [PaginatedAuthenticatorTOTPStageList](docs/PaginatedAuthenticatorTOTPStageList.md)
  - [PaginatedAuthenticatorValidateStageList](docs/PaginatedAuthenticatorValidateStageList.md)
+ - [PaginatedAuthenticatorWebAuthnStageList](docs/PaginatedAuthenticatorWebAuthnStageList.md)
  - [PaginatedBlueprintInstanceList](docs/PaginatedBlueprintInstanceList.md)
  - [PaginatedBrandList](docs/PaginatedBrandList.md)
  - [PaginatedCaptchaStageList](docs/PaginatedCaptchaStageList.md)
  - [PaginatedCertificateKeyPairList](docs/PaginatedCertificateKeyPairList.md)
  - [PaginatedConnectionTokenList](docs/PaginatedConnectionTokenList.md)
  - [PaginatedConsentStageList](docs/PaginatedConsentStageList.md)
  - [PaginatedDenyStageList](docs/PaginatedDenyStageList.md)
@@ -1118,30 +1120,31 @@
  - [PaginatedUserLoginStageList](docs/PaginatedUserLoginStageList.md)
  - [PaginatedUserLogoutStageList](docs/PaginatedUserLogoutStageList.md)
  - [PaginatedUserOAuthSourceConnectionList](docs/PaginatedUserOAuthSourceConnectionList.md)
  - [PaginatedUserSAMLSourceConnectionList](docs/PaginatedUserSAMLSourceConnectionList.md)
  - [PaginatedUserSourceConnectionList](docs/PaginatedUserSourceConnectionList.md)
  - [PaginatedUserWriteStageList](docs/PaginatedUserWriteStageList.md)
  - [PaginatedWebAuthnDeviceList](docs/PaginatedWebAuthnDeviceList.md)
+ - [PaginatedWebAuthnDeviceTypeList](docs/PaginatedWebAuthnDeviceTypeList.md)
  - [Pagination](docs/Pagination.md)
  - [PasswordChallenge](docs/PasswordChallenge.md)
  - [PasswordChallengeResponseRequest](docs/PasswordChallengeResponseRequest.md)
  - [PasswordExpiryPolicy](docs/PasswordExpiryPolicy.md)
  - [PasswordExpiryPolicyRequest](docs/PasswordExpiryPolicyRequest.md)
  - [PasswordPolicy](docs/PasswordPolicy.md)
  - [PasswordPolicyRequest](docs/PasswordPolicyRequest.md)
  - [PasswordStage](docs/PasswordStage.md)
  - [PasswordStageRequest](docs/PasswordStageRequest.md)
  - [PatchedApplicationRequest](docs/PatchedApplicationRequest.md)
- - [PatchedAuthenticateWebAuthnStageRequest](docs/PatchedAuthenticateWebAuthnStageRequest.md)
  - [PatchedAuthenticatorDuoStageRequest](docs/PatchedAuthenticatorDuoStageRequest.md)
  - [PatchedAuthenticatorSMSStageRequest](docs/PatchedAuthenticatorSMSStageRequest.md)
  - [PatchedAuthenticatorStaticStageRequest](docs/PatchedAuthenticatorStaticStageRequest.md)
  - [PatchedAuthenticatorTOTPStageRequest](docs/PatchedAuthenticatorTOTPStageRequest.md)
  - [PatchedAuthenticatorValidateStageRequest](docs/PatchedAuthenticatorValidateStageRequest.md)
+ - [PatchedAuthenticatorWebAuthnStageRequest](docs/PatchedAuthenticatorWebAuthnStageRequest.md)
  - [PatchedBlueprintInstanceRequest](docs/PatchedBlueprintInstanceRequest.md)
  - [PatchedBrandRequest](docs/PatchedBrandRequest.md)
  - [PatchedCaptchaStageRequest](docs/PatchedCaptchaStageRequest.md)
  - [PatchedCertificateKeyPairRequest](docs/PatchedCertificateKeyPairRequest.md)
  - [PatchedConnectionTokenRequest](docs/PatchedConnectionTokenRequest.md)
  - [PatchedConsentStageRequest](docs/PatchedConsentStageRequest.md)
  - [PatchedDenyStageRequest](docs/PatchedDenyStageRequest.md)
@@ -1359,14 +1362,16 @@
  - [UserVerificationEnum](docs/UserVerificationEnum.md)
  - [UserWriteStage](docs/UserWriteStage.md)
  - [UserWriteStageRequest](docs/UserWriteStageRequest.md)
  - [ValidationError](docs/ValidationError.md)
  - [Version](docs/Version.md)
  - [WebAuthnDevice](docs/WebAuthnDevice.md)
  - [WebAuthnDeviceRequest](docs/WebAuthnDeviceRequest.md)
+ - [WebAuthnDeviceType](docs/WebAuthnDeviceType.md)
+ - [WebAuthnDeviceTypeRequest](docs/WebAuthnDeviceTypeRequest.md)
  - [Workers](docs/Workers.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/__init__.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2024.2.2-1712239192"
+__version__ = "2024.2.2-1712571742"
 
 # import apis into sdk package
 from authentik_client.api.admin_api import AdminApi
 from authentik_client.api.authenticators_api import AuthenticatorsApi
 from authentik_client.api.core_api import CoreApi
 from authentik_client.api.crypto_api import CryptoApi
 from authentik_client.api.enterprise_api import EnterpriseApi
@@ -56,16 +56,14 @@
 from authentik_client.models.app_enum import AppEnum
 from authentik_client.models.apple_challenge_response_request import AppleChallengeResponseRequest
 from authentik_client.models.apple_login_challenge import AppleLoginChallenge
 from authentik_client.models.application import Application
 from authentik_client.models.application_request import ApplicationRequest
 from authentik_client.models.auth_mode_enum import AuthModeEnum
 from authentik_client.models.auth_type_enum import AuthTypeEnum
-from authentik_client.models.authenticate_web_authn_stage import AuthenticateWebAuthnStage
-from authentik_client.models.authenticate_web_authn_stage_request import AuthenticateWebAuthnStageRequest
 from authentik_client.models.authenticated_session import AuthenticatedSession
 from authentik_client.models.authenticated_session_asn import AuthenticatedSessionAsn
 from authentik_client.models.authenticated_session_geo_ip import AuthenticatedSessionGeoIp
 from authentik_client.models.authenticated_session_user_agent import AuthenticatedSessionUserAgent
 from authentik_client.models.authenticated_session_user_agent_device import AuthenticatedSessionUserAgentDevice
 from authentik_client.models.authenticated_session_user_agent_os import AuthenticatedSessionUserAgentOs
 from authentik_client.models.authenticated_session_user_agent_user_agent import AuthenticatedSessionUserAgentUserAgent
@@ -91,14 +89,16 @@
 from authentik_client.models.authenticator_totp_stage_request import AuthenticatorTOTPStageRequest
 from authentik_client.models.authenticator_validate_stage import AuthenticatorValidateStage
 from authentik_client.models.authenticator_validate_stage_request import AuthenticatorValidateStageRequest
 from authentik_client.models.authenticator_validation_challenge import AuthenticatorValidationChallenge
 from authentik_client.models.authenticator_validation_challenge_response_request import AuthenticatorValidationChallengeResponseRequest
 from authentik_client.models.authenticator_web_authn_challenge import AuthenticatorWebAuthnChallenge
 from authentik_client.models.authenticator_web_authn_challenge_response_request import AuthenticatorWebAuthnChallengeResponseRequest
+from authentik_client.models.authenticator_web_authn_stage import AuthenticatorWebAuthnStage
+from authentik_client.models.authenticator_web_authn_stage_request import AuthenticatorWebAuthnStageRequest
 from authentik_client.models.auto_submit_challenge_response_request import AutoSubmitChallengeResponseRequest
 from authentik_client.models.autosubmit_challenge import AutosubmitChallenge
 from authentik_client.models.backends_enum import BackendsEnum
 from authentik_client.models.binding_type_enum import BindingTypeEnum
 from authentik_client.models.blueprint_file import BlueprintFile
 from authentik_client.models.blueprint_instance import BlueprintInstance
 from authentik_client.models.blueprint_instance_request import BlueprintInstanceRequest
@@ -257,21 +257,21 @@
 from authentik_client.models.open_id_connect_configuration import OpenIDConnectConfiguration
 from authentik_client.models.outpost import Outpost
 from authentik_client.models.outpost_default_config import OutpostDefaultConfig
 from authentik_client.models.outpost_health import OutpostHealth
 from authentik_client.models.outpost_request import OutpostRequest
 from authentik_client.models.outpost_type_enum import OutpostTypeEnum
 from authentik_client.models.paginated_application_list import PaginatedApplicationList
-from authentik_client.models.paginated_authenticate_web_authn_stage_list import PaginatedAuthenticateWebAuthnStageList
 from authentik_client.models.paginated_authenticated_session_list import PaginatedAuthenticatedSessionList
 from authentik_client.models.paginated_authenticator_duo_stage_list import PaginatedAuthenticatorDuoStageList
 from authentik_client.models.paginated_authenticator_sms_stage_list import PaginatedAuthenticatorSMSStageList
 from authentik_client.models.paginated_authenticator_static_stage_list import PaginatedAuthenticatorStaticStageList
 from authentik_client.models.paginated_authenticator_totp_stage_list import PaginatedAuthenticatorTOTPStageList
 from authentik_client.models.paginated_authenticator_validate_stage_list import PaginatedAuthenticatorValidateStageList
+from authentik_client.models.paginated_authenticator_web_authn_stage_list import PaginatedAuthenticatorWebAuthnStageList
 from authentik_client.models.paginated_blueprint_instance_list import PaginatedBlueprintInstanceList
 from authentik_client.models.paginated_brand_list import PaginatedBrandList
 from authentik_client.models.paginated_captcha_stage_list import PaginatedCaptchaStageList
 from authentik_client.models.paginated_certificate_key_pair_list import PaginatedCertificateKeyPairList
 from authentik_client.models.paginated_connection_token_list import PaginatedConnectionTokenList
 from authentik_client.models.paginated_consent_stage_list import PaginatedConsentStageList
 from authentik_client.models.paginated_deny_stage_list import PaginatedDenyStageList
@@ -353,30 +353,31 @@
 from authentik_client.models.paginated_user_login_stage_list import PaginatedUserLoginStageList
 from authentik_client.models.paginated_user_logout_stage_list import PaginatedUserLogoutStageList
 from authentik_client.models.paginated_user_o_auth_source_connection_list import PaginatedUserOAuthSourceConnectionList
 from authentik_client.models.paginated_user_saml_source_connection_list import PaginatedUserSAMLSourceConnectionList
 from authentik_client.models.paginated_user_source_connection_list import PaginatedUserSourceConnectionList
 from authentik_client.models.paginated_user_write_stage_list import PaginatedUserWriteStageList
 from authentik_client.models.paginated_web_authn_device_list import PaginatedWebAuthnDeviceList
+from authentik_client.models.paginated_web_authn_device_type_list import PaginatedWebAuthnDeviceTypeList
 from authentik_client.models.pagination import Pagination
 from authentik_client.models.password_challenge import PasswordChallenge
 from authentik_client.models.password_challenge_response_request import PasswordChallengeResponseRequest
 from authentik_client.models.password_expiry_policy import PasswordExpiryPolicy
 from authentik_client.models.password_expiry_policy_request import PasswordExpiryPolicyRequest
 from authentik_client.models.password_policy import PasswordPolicy
 from authentik_client.models.password_policy_request import PasswordPolicyRequest
 from authentik_client.models.password_stage import PasswordStage
 from authentik_client.models.password_stage_request import PasswordStageRequest
 from authentik_client.models.patched_application_request import PatchedApplicationRequest
-from authentik_client.models.patched_authenticate_web_authn_stage_request import PatchedAuthenticateWebAuthnStageRequest
 from authentik_client.models.patched_authenticator_duo_stage_request import PatchedAuthenticatorDuoStageRequest
 from authentik_client.models.patched_authenticator_sms_stage_request import PatchedAuthenticatorSMSStageRequest
 from authentik_client.models.patched_authenticator_static_stage_request import PatchedAuthenticatorStaticStageRequest
 from authentik_client.models.patched_authenticator_totp_stage_request import PatchedAuthenticatorTOTPStageRequest
 from authentik_client.models.patched_authenticator_validate_stage_request import PatchedAuthenticatorValidateStageRequest
+from authentik_client.models.patched_authenticator_web_authn_stage_request import PatchedAuthenticatorWebAuthnStageRequest
 from authentik_client.models.patched_blueprint_instance_request import PatchedBlueprintInstanceRequest
 from authentik_client.models.patched_brand_request import PatchedBrandRequest
 from authentik_client.models.patched_captcha_stage_request import PatchedCaptchaStageRequest
 from authentik_client.models.patched_certificate_key_pair_request import PatchedCertificateKeyPairRequest
 from authentik_client.models.patched_connection_token_request import PatchedConnectionTokenRequest
 from authentik_client.models.patched_consent_stage_request import PatchedConsentStageRequest
 from authentik_client.models.patched_deny_stage_request import PatchedDenyStageRequest
@@ -594,8 +595,10 @@
 from authentik_client.models.user_verification_enum import UserVerificationEnum
 from authentik_client.models.user_write_stage import UserWriteStage
 from authentik_client.models.user_write_stage_request import UserWriteStageRequest
 from authentik_client.models.validation_error import ValidationError
 from authentik_client.models.version import Version
 from authentik_client.models.web_authn_device import WebAuthnDevice
 from authentik_client.models.web_authn_device_request import WebAuthnDeviceRequest
+from authentik_client.models.web_authn_device_type import WebAuthnDeviceType
+from authentik_client.models.web_authn_device_type_request import WebAuthnDeviceTypeRequest
 from authentik_client.models.workers import Workers
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/__init__.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/admin_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/authenticators_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/authenticators_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/core_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/crypto_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/crypto_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/enterprise_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/enterprise_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/events_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/flows_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/flows_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/managed_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/managed_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/oauth2_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/oauth2_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/outposts_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/outposts_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/policies_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/propertymappings_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/propertymappings_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/providers_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/providers_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/rac_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/rac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/rbac_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/rbac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/root_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/root_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/schema_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/sources_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/sources_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/stages_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/stages_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from datetime import datetime
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
 from typing import List, Optional
 from typing_extensions import Annotated
-from authentik_client.models.authenticate_web_authn_stage import AuthenticateWebAuthnStage
-from authentik_client.models.authenticate_web_authn_stage_request import AuthenticateWebAuthnStageRequest
 from authentik_client.models.authenticator_duo_stage import AuthenticatorDuoStage
 from authentik_client.models.authenticator_duo_stage_device_import_response import AuthenticatorDuoStageDeviceImportResponse
 from authentik_client.models.authenticator_duo_stage_manual_device_import_request import AuthenticatorDuoStageManualDeviceImportRequest
 from authentik_client.models.authenticator_duo_stage_request import AuthenticatorDuoStageRequest
 from authentik_client.models.authenticator_sms_stage import AuthenticatorSMSStage
 from authentik_client.models.authenticator_sms_stage_request import AuthenticatorSMSStageRequest
 from authentik_client.models.authenticator_static_stage import AuthenticatorStaticStage
 from authentik_client.models.authenticator_static_stage_request import AuthenticatorStaticStageRequest
 from authentik_client.models.authenticator_totp_stage import AuthenticatorTOTPStage
 from authentik_client.models.authenticator_totp_stage_request import AuthenticatorTOTPStageRequest
 from authentik_client.models.authenticator_validate_stage import AuthenticatorValidateStage
 from authentik_client.models.authenticator_validate_stage_request import AuthenticatorValidateStageRequest
+from authentik_client.models.authenticator_web_authn_stage import AuthenticatorWebAuthnStage
+from authentik_client.models.authenticator_web_authn_stage_request import AuthenticatorWebAuthnStageRequest
 from authentik_client.models.captcha_stage import CaptchaStage
 from authentik_client.models.captcha_stage_request import CaptchaStageRequest
 from authentik_client.models.consent_stage import ConsentStage
 from authentik_client.models.consent_stage_request import ConsentStageRequest
 from authentik_client.models.deny_stage import DenyStage
 from authentik_client.models.deny_stage_request import DenyStageRequest
 from authentik_client.models.dummy_stage import DummyStage
@@ -48,20 +48,20 @@
 from authentik_client.models.email_stage_request import EmailStageRequest
 from authentik_client.models.identification_stage import IdentificationStage
 from authentik_client.models.identification_stage_request import IdentificationStageRequest
 from authentik_client.models.invitation import Invitation
 from authentik_client.models.invitation_request import InvitationRequest
 from authentik_client.models.invitation_stage import InvitationStage
 from authentik_client.models.invitation_stage_request import InvitationStageRequest
-from authentik_client.models.paginated_authenticate_web_authn_stage_list import PaginatedAuthenticateWebAuthnStageList
 from authentik_client.models.paginated_authenticator_duo_stage_list import PaginatedAuthenticatorDuoStageList
 from authentik_client.models.paginated_authenticator_sms_stage_list import PaginatedAuthenticatorSMSStageList
 from authentik_client.models.paginated_authenticator_static_stage_list import PaginatedAuthenticatorStaticStageList
 from authentik_client.models.paginated_authenticator_totp_stage_list import PaginatedAuthenticatorTOTPStageList
 from authentik_client.models.paginated_authenticator_validate_stage_list import PaginatedAuthenticatorValidateStageList
+from authentik_client.models.paginated_authenticator_web_authn_stage_list import PaginatedAuthenticatorWebAuthnStageList
 from authentik_client.models.paginated_captcha_stage_list import PaginatedCaptchaStageList
 from authentik_client.models.paginated_consent_stage_list import PaginatedConsentStageList
 from authentik_client.models.paginated_deny_stage_list import PaginatedDenyStageList
 from authentik_client.models.paginated_dummy_stage_list import PaginatedDummyStageList
 from authentik_client.models.paginated_email_stage_list import PaginatedEmailStageList
 from authentik_client.models.paginated_identification_stage_list import PaginatedIdentificationStageList
 from authentik_client.models.paginated_invitation_list import PaginatedInvitationList
@@ -71,22 +71,23 @@
 from authentik_client.models.paginated_prompt_stage_list import PaginatedPromptStageList
 from authentik_client.models.paginated_source_stage_list import PaginatedSourceStageList
 from authentik_client.models.paginated_stage_list import PaginatedStageList
 from authentik_client.models.paginated_user_delete_stage_list import PaginatedUserDeleteStageList
 from authentik_client.models.paginated_user_login_stage_list import PaginatedUserLoginStageList
 from authentik_client.models.paginated_user_logout_stage_list import PaginatedUserLogoutStageList
 from authentik_client.models.paginated_user_write_stage_list import PaginatedUserWriteStageList
+from authentik_client.models.paginated_web_authn_device_type_list import PaginatedWebAuthnDeviceTypeList
 from authentik_client.models.password_stage import PasswordStage
 from authentik_client.models.password_stage_request import PasswordStageRequest
-from authentik_client.models.patched_authenticate_web_authn_stage_request import PatchedAuthenticateWebAuthnStageRequest
 from authentik_client.models.patched_authenticator_duo_stage_request import PatchedAuthenticatorDuoStageRequest
 from authentik_client.models.patched_authenticator_sms_stage_request import PatchedAuthenticatorSMSStageRequest
 from authentik_client.models.patched_authenticator_static_stage_request import PatchedAuthenticatorStaticStageRequest
 from authentik_client.models.patched_authenticator_totp_stage_request import PatchedAuthenticatorTOTPStageRequest
 from authentik_client.models.patched_authenticator_validate_stage_request import PatchedAuthenticatorValidateStageRequest
+from authentik_client.models.patched_authenticator_web_authn_stage_request import PatchedAuthenticatorWebAuthnStageRequest
 from authentik_client.models.patched_captcha_stage_request import PatchedCaptchaStageRequest
 from authentik_client.models.patched_consent_stage_request import PatchedConsentStageRequest
 from authentik_client.models.patched_deny_stage_request import PatchedDenyStageRequest
 from authentik_client.models.patched_dummy_stage_request import PatchedDummyStageRequest
 from authentik_client.models.patched_email_stage_request import PatchedEmailStageRequest
 from authentik_client.models.patched_identification_stage_request import PatchedIdentificationStageRequest
 from authentik_client.models.patched_invitation_request import PatchedInvitationRequest
@@ -114,14 +115,15 @@
 from authentik_client.models.user_login_stage import UserLoginStage
 from authentik_client.models.user_login_stage_request import UserLoginStageRequest
 from authentik_client.models.user_logout_stage import UserLogoutStage
 from authentik_client.models.user_logout_stage_request import UserLogoutStageRequest
 from authentik_client.models.user_setting import UserSetting
 from authentik_client.models.user_write_stage import UserWriteStage
 from authentik_client.models.user_write_stage_request import UserWriteStageRequest
+from authentik_client.models.web_authn_device_type import WebAuthnDeviceType
 
 from authentik_client.api_client import ApiClient, RequestSerialized
 from authentik_client.api_response import ApiResponse
 from authentik_client.rest import RESTResponseType
 
 
 class StagesApi:
@@ -12941,34 +12943,34 @@
 
 
 
 
     @validate_call
     def stages_authenticator_webauthn_create(
         self,
-        authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest,
+        authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> AuthenticateWebAuthnStage:
+    ) -> AuthenticatorWebAuthnStage:
         """stages_authenticator_webauthn_create
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
-        :param authenticate_web_authn_stage_request: (required)
-        :type authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest
+        :param authenticator_web_authn_stage_request: (required)
+        :type authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -12984,23 +12986,23 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_create_serialize(
-            authenticate_web_authn_stage_request=authenticate_web_authn_stage_request,
+            authenticator_web_authn_stage_request=authenticator_web_authn_stage_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "AuthenticateWebAuthnStage",
+            '201': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -13010,34 +13012,34 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def stages_authenticator_webauthn_create_with_http_info(
         self,
-        authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest,
+        authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[AuthenticateWebAuthnStage]:
+    ) -> ApiResponse[AuthenticatorWebAuthnStage]:
         """stages_authenticator_webauthn_create
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
-        :param authenticate_web_authn_stage_request: (required)
-        :type authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest
+        :param authenticator_web_authn_stage_request: (required)
+        :type authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -13053,23 +13055,23 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_create_serialize(
-            authenticate_web_authn_stage_request=authenticate_web_authn_stage_request,
+            authenticator_web_authn_stage_request=authenticator_web_authn_stage_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "AuthenticateWebAuthnStage",
+            '201': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -13079,15 +13081,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def stages_authenticator_webauthn_create_without_preload_content(
         self,
-        authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest,
+        authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -13095,18 +13097,18 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """stages_authenticator_webauthn_create
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
-        :param authenticate_web_authn_stage_request: (required)
-        :type authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest
+        :param authenticator_web_authn_stage_request: (required)
+        :type authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -13122,36 +13124,36 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_create_serialize(
-            authenticate_web_authn_stage_request=authenticate_web_authn_stage_request,
+            authenticator_web_authn_stage_request=authenticator_web_authn_stage_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "AuthenticateWebAuthnStage",
+            '201': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _stages_authenticator_webauthn_create_serialize(
         self,
-        authenticate_web_authn_stage_request,
+        authenticator_web_authn_stage_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -13167,16 +13169,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if authenticate_web_authn_stage_request is not None:
-            _body_params = authenticate_web_authn_stage_request
+        if authenticator_web_authn_stage_request is not None:
+            _body_params = authenticator_web_authn_stage_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -13234,15 +13236,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
         """stages_authenticator_webauthn_destroy
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -13303,15 +13305,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
         """stages_authenticator_webauthn_destroy
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -13372,15 +13374,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """stages_authenticator_webauthn_destroy
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -13480,18 +13482,651 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def stages_authenticator_webauthn_device_types_list(
+        self,
+        aaguid: Optional[StrictStr] = None,
+        description: Optional[StrictStr] = None,
+        icon: Optional[StrictStr] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
+        search: Annotated[Optional[StrictStr], Field(description="A search term.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> PaginatedWebAuthnDeviceTypeList:
+        """stages_authenticator_webauthn_device_types_list
+
+        WebAuthnDeviceType Viewset
+
+        :param aaguid:
+        :type aaguid: str
+        :param description:
+        :type description: str
+        :param icon:
+        :type icon: str
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
+        :param search: A search term.
+        :type search: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._stages_authenticator_webauthn_device_types_list_serialize(
+            aaguid=aaguid,
+            description=description,
+            icon=icon,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
+            search=search,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PaginatedWebAuthnDeviceTypeList",
+            '400': "ValidationError",
+            '403': "GenericError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def stages_authenticator_webauthn_device_types_list_with_http_info(
+        self,
+        aaguid: Optional[StrictStr] = None,
+        description: Optional[StrictStr] = None,
+        icon: Optional[StrictStr] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
+        search: Annotated[Optional[StrictStr], Field(description="A search term.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[PaginatedWebAuthnDeviceTypeList]:
+        """stages_authenticator_webauthn_device_types_list
+
+        WebAuthnDeviceType Viewset
+
+        :param aaguid:
+        :type aaguid: str
+        :param description:
+        :type description: str
+        :param icon:
+        :type icon: str
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
+        :param search: A search term.
+        :type search: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._stages_authenticator_webauthn_device_types_list_serialize(
+            aaguid=aaguid,
+            description=description,
+            icon=icon,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
+            search=search,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PaginatedWebAuthnDeviceTypeList",
+            '400': "ValidationError",
+            '403': "GenericError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def stages_authenticator_webauthn_device_types_list_without_preload_content(
+        self,
+        aaguid: Optional[StrictStr] = None,
+        description: Optional[StrictStr] = None,
+        icon: Optional[StrictStr] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
+        search: Annotated[Optional[StrictStr], Field(description="A search term.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """stages_authenticator_webauthn_device_types_list
+
+        WebAuthnDeviceType Viewset
+
+        :param aaguid:
+        :type aaguid: str
+        :param description:
+        :type description: str
+        :param icon:
+        :type icon: str
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
+        :param search: A search term.
+        :type search: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._stages_authenticator_webauthn_device_types_list_serialize(
+            aaguid=aaguid,
+            description=description,
+            icon=icon,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
+            search=search,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PaginatedWebAuthnDeviceTypeList",
+            '400': "ValidationError",
+            '403': "GenericError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _stages_authenticator_webauthn_device_types_list_serialize(
+        self,
+        aaguid,
+        description,
+        icon,
+        ordering,
+        page,
+        page_size,
+        search,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if aaguid is not None:
+            
+            _query_params.append(('aaguid', aaguid))
+            
+        if description is not None:
+            
+            _query_params.append(('description', description))
+            
+        if icon is not None:
+            
+            _query_params.append(('icon', icon))
+            
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
+        if search is not None:
+            
+            _query_params.append(('search', search))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'authentik'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/stages/authenticator/webauthn_device_types/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def stages_authenticator_webauthn_device_types_retrieve(
+        self,
+        aaguid: Annotated[StrictStr, Field(description="A UUID string identifying this WebAuthn Device type.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> WebAuthnDeviceType:
+        """stages_authenticator_webauthn_device_types_retrieve
+
+        WebAuthnDeviceType Viewset
+
+        :param aaguid: A UUID string identifying this WebAuthn Device type. (required)
+        :type aaguid: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._stages_authenticator_webauthn_device_types_retrieve_serialize(
+            aaguid=aaguid,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "WebAuthnDeviceType",
+            '400': "ValidationError",
+            '403': "GenericError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def stages_authenticator_webauthn_device_types_retrieve_with_http_info(
+        self,
+        aaguid: Annotated[StrictStr, Field(description="A UUID string identifying this WebAuthn Device type.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[WebAuthnDeviceType]:
+        """stages_authenticator_webauthn_device_types_retrieve
+
+        WebAuthnDeviceType Viewset
+
+        :param aaguid: A UUID string identifying this WebAuthn Device type. (required)
+        :type aaguid: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._stages_authenticator_webauthn_device_types_retrieve_serialize(
+            aaguid=aaguid,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "WebAuthnDeviceType",
+            '400': "ValidationError",
+            '403': "GenericError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def stages_authenticator_webauthn_device_types_retrieve_without_preload_content(
+        self,
+        aaguid: Annotated[StrictStr, Field(description="A UUID string identifying this WebAuthn Device type.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """stages_authenticator_webauthn_device_types_retrieve
+
+        WebAuthnDeviceType Viewset
+
+        :param aaguid: A UUID string identifying this WebAuthn Device type. (required)
+        :type aaguid: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._stages_authenticator_webauthn_device_types_retrieve_serialize(
+            aaguid=aaguid,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "WebAuthnDeviceType",
+            '400': "ValidationError",
+            '403': "GenericError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _stages_authenticator_webauthn_device_types_retrieve_serialize(
+        self,
+        aaguid,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if aaguid is not None:
+            _path_params['aaguid'] = aaguid
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'authentik'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/stages/authenticator/webauthn_device_types/{aaguid}/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def stages_authenticator_webauthn_list(
         self,
         authenticator_attachment: Optional[StrictStr] = None,
         configure_flow: Optional[StrictStr] = None,
+        device_type_restrictions: Optional[List[StrictStr]] = None,
         friendly_name: Optional[StrictStr] = None,
         name: Optional[StrictStr] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         resident_key_requirement: Optional[StrictStr] = None,
         search: Annotated[Optional[StrictStr], Field(description="A search term.")] = None,
@@ -13505,23 +14140,25 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> PaginatedAuthenticateWebAuthnStageList:
+    ) -> PaginatedAuthenticatorWebAuthnStageList:
         """stages_authenticator_webauthn_list
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param authenticator_attachment:
         :type authenticator_attachment: str
         :param configure_flow:
         :type configure_flow: str
+        :param device_type_restrictions:
+        :type device_type_restrictions: List[str]
         :param friendly_name:
         :type friendly_name: str
         :param name:
         :type name: str
         :param ordering: Which field to use when ordering the results.
         :type ordering: str
         :param page: A page number within the paginated result set.
@@ -13557,14 +14194,15 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_list_serialize(
             authenticator_attachment=authenticator_attachment,
             configure_flow=configure_flow,
+            device_type_restrictions=device_type_restrictions,
             friendly_name=friendly_name,
             name=name,
             ordering=ordering,
             page=page,
             page_size=page_size,
             resident_key_requirement=resident_key_requirement,
             search=search,
@@ -13573,15 +14211,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedAuthenticateWebAuthnStageList",
+            '200': "PaginatedAuthenticatorWebAuthnStageList",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -13593,14 +14231,15 @@
 
 
     @validate_call
     def stages_authenticator_webauthn_list_with_http_info(
         self,
         authenticator_attachment: Optional[StrictStr] = None,
         configure_flow: Optional[StrictStr] = None,
+        device_type_restrictions: Optional[List[StrictStr]] = None,
         friendly_name: Optional[StrictStr] = None,
         name: Optional[StrictStr] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         resident_key_requirement: Optional[StrictStr] = None,
         search: Annotated[Optional[StrictStr], Field(description="A search term.")] = None,
@@ -13614,23 +14253,25 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[PaginatedAuthenticateWebAuthnStageList]:
+    ) -> ApiResponse[PaginatedAuthenticatorWebAuthnStageList]:
         """stages_authenticator_webauthn_list
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param authenticator_attachment:
         :type authenticator_attachment: str
         :param configure_flow:
         :type configure_flow: str
+        :param device_type_restrictions:
+        :type device_type_restrictions: List[str]
         :param friendly_name:
         :type friendly_name: str
         :param name:
         :type name: str
         :param ordering: Which field to use when ordering the results.
         :type ordering: str
         :param page: A page number within the paginated result set.
@@ -13666,14 +14307,15 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_list_serialize(
             authenticator_attachment=authenticator_attachment,
             configure_flow=configure_flow,
+            device_type_restrictions=device_type_restrictions,
             friendly_name=friendly_name,
             name=name,
             ordering=ordering,
             page=page,
             page_size=page_size,
             resident_key_requirement=resident_key_requirement,
             search=search,
@@ -13682,15 +14324,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedAuthenticateWebAuthnStageList",
+            '200': "PaginatedAuthenticatorWebAuthnStageList",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -13702,14 +14344,15 @@
 
 
     @validate_call
     def stages_authenticator_webauthn_list_without_preload_content(
         self,
         authenticator_attachment: Optional[StrictStr] = None,
         configure_flow: Optional[StrictStr] = None,
+        device_type_restrictions: Optional[List[StrictStr]] = None,
         friendly_name: Optional[StrictStr] = None,
         name: Optional[StrictStr] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         resident_key_requirement: Optional[StrictStr] = None,
         search: Annotated[Optional[StrictStr], Field(description="A search term.")] = None,
@@ -13726,20 +14369,22 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """stages_authenticator_webauthn_list
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param authenticator_attachment:
         :type authenticator_attachment: str
         :param configure_flow:
         :type configure_flow: str
+        :param device_type_restrictions:
+        :type device_type_restrictions: List[str]
         :param friendly_name:
         :type friendly_name: str
         :param name:
         :type name: str
         :param ordering: Which field to use when ordering the results.
         :type ordering: str
         :param page: A page number within the paginated result set.
@@ -13775,14 +14420,15 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_list_serialize(
             authenticator_attachment=authenticator_attachment,
             configure_flow=configure_flow,
+            device_type_restrictions=device_type_restrictions,
             friendly_name=friendly_name,
             name=name,
             ordering=ordering,
             page=page,
             page_size=page_size,
             resident_key_requirement=resident_key_requirement,
             search=search,
@@ -13791,29 +14437,30 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedAuthenticateWebAuthnStageList",
+            '200': "PaginatedAuthenticatorWebAuthnStageList",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _stages_authenticator_webauthn_list_serialize(
         self,
         authenticator_attachment,
         configure_flow,
+        device_type_restrictions,
         friendly_name,
         name,
         ordering,
         page,
         page_size,
         resident_key_requirement,
         search,
@@ -13824,14 +14471,15 @@
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
+            'device_type_restrictions': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
@@ -13843,14 +14491,18 @@
             
             _query_params.append(('authenticator_attachment', authenticator_attachment))
             
         if configure_flow is not None:
             
             _query_params.append(('configure_flow', configure_flow))
             
+        if device_type_restrictions is not None:
+            
+            _query_params.append(('device_type_restrictions', device_type_restrictions))
+            
         if friendly_name is not None:
             
             _query_params.append(('friendly_name', friendly_name))
             
         if name is not None:
             
             _query_params.append(('name', name))
@@ -13919,36 +14571,36 @@
 
 
 
     @validate_call
     def stages_authenticator_webauthn_partial_update(
         self,
         stage_uuid: Annotated[StrictStr, Field(description="A UUID string identifying this WebAuthn Authenticator Setup Stage.")],
-        patched_authenticate_web_authn_stage_request: Optional[PatchedAuthenticateWebAuthnStageRequest] = None,
+        patched_authenticator_web_authn_stage_request: Optional[PatchedAuthenticatorWebAuthnStageRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> AuthenticateWebAuthnStage:
+    ) -> AuthenticatorWebAuthnStage:
         """stages_authenticator_webauthn_partial_update
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
-        :param patched_authenticate_web_authn_stage_request:
-        :type patched_authenticate_web_authn_stage_request: PatchedAuthenticateWebAuthnStageRequest
+        :param patched_authenticator_web_authn_stage_request:
+        :type patched_authenticator_web_authn_stage_request: PatchedAuthenticatorWebAuthnStageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -13965,23 +14617,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_partial_update_serialize(
             stage_uuid=stage_uuid,
-            patched_authenticate_web_authn_stage_request=patched_authenticate_web_authn_stage_request,
+            patched_authenticator_web_authn_stage_request=patched_authenticator_web_authn_stage_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AuthenticateWebAuthnStage",
+            '200': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -13992,36 +14644,36 @@
         ).data
 
 
     @validate_call
     def stages_authenticator_webauthn_partial_update_with_http_info(
         self,
         stage_uuid: Annotated[StrictStr, Field(description="A UUID string identifying this WebAuthn Authenticator Setup Stage.")],
-        patched_authenticate_web_authn_stage_request: Optional[PatchedAuthenticateWebAuthnStageRequest] = None,
+        patched_authenticator_web_authn_stage_request: Optional[PatchedAuthenticatorWebAuthnStageRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[AuthenticateWebAuthnStage]:
+    ) -> ApiResponse[AuthenticatorWebAuthnStage]:
         """stages_authenticator_webauthn_partial_update
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
-        :param patched_authenticate_web_authn_stage_request:
-        :type patched_authenticate_web_authn_stage_request: PatchedAuthenticateWebAuthnStageRequest
+        :param patched_authenticator_web_authn_stage_request:
+        :type patched_authenticator_web_authn_stage_request: PatchedAuthenticatorWebAuthnStageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -14038,23 +14690,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_partial_update_serialize(
             stage_uuid=stage_uuid,
-            patched_authenticate_web_authn_stage_request=patched_authenticate_web_authn_stage_request,
+            patched_authenticator_web_authn_stage_request=patched_authenticator_web_authn_stage_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AuthenticateWebAuthnStage",
+            '200': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -14065,15 +14717,15 @@
         )
 
 
     @validate_call
     def stages_authenticator_webauthn_partial_update_without_preload_content(
         self,
         stage_uuid: Annotated[StrictStr, Field(description="A UUID string identifying this WebAuthn Authenticator Setup Stage.")],
-        patched_authenticate_web_authn_stage_request: Optional[PatchedAuthenticateWebAuthnStageRequest] = None,
+        patched_authenticator_web_authn_stage_request: Optional[PatchedAuthenticatorWebAuthnStageRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -14081,20 +14733,20 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """stages_authenticator_webauthn_partial_update
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
-        :param patched_authenticate_web_authn_stage_request:
-        :type patched_authenticate_web_authn_stage_request: PatchedAuthenticateWebAuthnStageRequest
+        :param patched_authenticator_web_authn_stage_request:
+        :type patched_authenticator_web_authn_stage_request: PatchedAuthenticatorWebAuthnStageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -14111,37 +14763,37 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_partial_update_serialize(
             stage_uuid=stage_uuid,
-            patched_authenticate_web_authn_stage_request=patched_authenticate_web_authn_stage_request,
+            patched_authenticator_web_authn_stage_request=patched_authenticator_web_authn_stage_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AuthenticateWebAuthnStage",
+            '200': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _stages_authenticator_webauthn_partial_update_serialize(
         self,
         stage_uuid,
-        patched_authenticate_web_authn_stage_request,
+        patched_authenticator_web_authn_stage_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -14159,16 +14811,16 @@
         # process the path parameters
         if stage_uuid is not None:
             _path_params['stage_uuid'] = stage_uuid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if patched_authenticate_web_authn_stage_request is not None:
-            _body_params = patched_authenticate_web_authn_stage_request
+        if patched_authenticator_web_authn_stage_request is not None:
+            _body_params = patched_authenticator_web_authn_stage_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -14223,18 +14875,18 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> AuthenticateWebAuthnStage:
+    ) -> AuthenticatorWebAuthnStage:
         """stages_authenticator_webauthn_retrieve
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -14261,15 +14913,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AuthenticateWebAuthnStage",
+            '200': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -14292,18 +14944,18 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[AuthenticateWebAuthnStage]:
+    ) -> ApiResponse[AuthenticatorWebAuthnStage]:
         """stages_authenticator_webauthn_retrieve
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -14330,15 +14982,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AuthenticateWebAuthnStage",
+            '200': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -14364,15 +15016,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """stages_authenticator_webauthn_retrieve
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -14399,15 +15051,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AuthenticateWebAuthnStage",
+            '200': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -14475,36 +15127,36 @@
 
 
 
     @validate_call
     def stages_authenticator_webauthn_update(
         self,
         stage_uuid: Annotated[StrictStr, Field(description="A UUID string identifying this WebAuthn Authenticator Setup Stage.")],
-        authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest,
+        authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> AuthenticateWebAuthnStage:
+    ) -> AuthenticatorWebAuthnStage:
         """stages_authenticator_webauthn_update
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
-        :param authenticate_web_authn_stage_request: (required)
-        :type authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest
+        :param authenticator_web_authn_stage_request: (required)
+        :type authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -14521,23 +15173,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_update_serialize(
             stage_uuid=stage_uuid,
-            authenticate_web_authn_stage_request=authenticate_web_authn_stage_request,
+            authenticator_web_authn_stage_request=authenticator_web_authn_stage_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AuthenticateWebAuthnStage",
+            '200': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -14548,36 +15200,36 @@
         ).data
 
 
     @validate_call
     def stages_authenticator_webauthn_update_with_http_info(
         self,
         stage_uuid: Annotated[StrictStr, Field(description="A UUID string identifying this WebAuthn Authenticator Setup Stage.")],
-        authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest,
+        authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[AuthenticateWebAuthnStage]:
+    ) -> ApiResponse[AuthenticatorWebAuthnStage]:
         """stages_authenticator_webauthn_update
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
-        :param authenticate_web_authn_stage_request: (required)
-        :type authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest
+        :param authenticator_web_authn_stage_request: (required)
+        :type authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -14594,23 +15246,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_update_serialize(
             stage_uuid=stage_uuid,
-            authenticate_web_authn_stage_request=authenticate_web_authn_stage_request,
+            authenticator_web_authn_stage_request=authenticator_web_authn_stage_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AuthenticateWebAuthnStage",
+            '200': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -14621,15 +15273,15 @@
         )
 
 
     @validate_call
     def stages_authenticator_webauthn_update_without_preload_content(
         self,
         stage_uuid: Annotated[StrictStr, Field(description="A UUID string identifying this WebAuthn Authenticator Setup Stage.")],
-        authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest,
+        authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -14637,20 +15289,20 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """stages_authenticator_webauthn_update
 
-        AuthenticateWebAuthnStage Viewset
+        AuthenticatorWebAuthnStage Viewset
 
         :param stage_uuid: A UUID string identifying this WebAuthn Authenticator Setup Stage. (required)
         :type stage_uuid: str
-        :param authenticate_web_authn_stage_request: (required)
-        :type authenticate_web_authn_stage_request: AuthenticateWebAuthnStageRequest
+        :param authenticator_web_authn_stage_request: (required)
+        :type authenticator_web_authn_stage_request: AuthenticatorWebAuthnStageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -14667,37 +15319,37 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._stages_authenticator_webauthn_update_serialize(
             stage_uuid=stage_uuid,
-            authenticate_web_authn_stage_request=authenticate_web_authn_stage_request,
+            authenticator_web_authn_stage_request=authenticator_web_authn_stage_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AuthenticateWebAuthnStage",
+            '200': "AuthenticatorWebAuthnStage",
             '400': "ValidationError",
             '403': "GenericError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _stages_authenticator_webauthn_update_serialize(
         self,
         stage_uuid,
-        authenticate_web_authn_stage_request,
+        authenticator_web_authn_stage_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -14715,16 +15367,16 @@
         # process the path parameters
         if stage_uuid is not None:
             _path_params['stage_uuid'] = stage_uuid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if authenticate_web_authn_stage_request is not None:
-            _body_params = authenticate_web_authn_stage_request
+        if authenticator_web_authn_stage_request is not None:
+            _body_params = authenticator_web_authn_stage_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api/tenants_api.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api/tenants_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api_client.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.2.2-1712239192/python'
+        self.user_agent = 'OpenAPI-Generator/2024.2.2-1712571742/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/api_response.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/api_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/configuration.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2024.2.2\n"\
-               "SDK Package Version: 2024.2.2-1712239192".\
+               "SDK Package Version: 2024.2.2-1712571742".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/exceptions.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/__init__.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 from authentik_client.models.app_enum import AppEnum
 from authentik_client.models.apple_challenge_response_request import AppleChallengeResponseRequest
 from authentik_client.models.apple_login_challenge import AppleLoginChallenge
 from authentik_client.models.application import Application
 from authentik_client.models.application_request import ApplicationRequest
 from authentik_client.models.auth_mode_enum import AuthModeEnum
 from authentik_client.models.auth_type_enum import AuthTypeEnum
-from authentik_client.models.authenticate_web_authn_stage import AuthenticateWebAuthnStage
-from authentik_client.models.authenticate_web_authn_stage_request import AuthenticateWebAuthnStageRequest
 from authentik_client.models.authenticated_session import AuthenticatedSession
 from authentik_client.models.authenticated_session_asn import AuthenticatedSessionAsn
 from authentik_client.models.authenticated_session_geo_ip import AuthenticatedSessionGeoIp
 from authentik_client.models.authenticated_session_user_agent import AuthenticatedSessionUserAgent
 from authentik_client.models.authenticated_session_user_agent_device import AuthenticatedSessionUserAgentDevice
 from authentik_client.models.authenticated_session_user_agent_os import AuthenticatedSessionUserAgentOs
 from authentik_client.models.authenticated_session_user_agent_user_agent import AuthenticatedSessionUserAgentUserAgent
@@ -55,14 +53,16 @@
 from authentik_client.models.authenticator_totp_stage_request import AuthenticatorTOTPStageRequest
 from authentik_client.models.authenticator_validate_stage import AuthenticatorValidateStage
 from authentik_client.models.authenticator_validate_stage_request import AuthenticatorValidateStageRequest
 from authentik_client.models.authenticator_validation_challenge import AuthenticatorValidationChallenge
 from authentik_client.models.authenticator_validation_challenge_response_request import AuthenticatorValidationChallengeResponseRequest
 from authentik_client.models.authenticator_web_authn_challenge import AuthenticatorWebAuthnChallenge
 from authentik_client.models.authenticator_web_authn_challenge_response_request import AuthenticatorWebAuthnChallengeResponseRequest
+from authentik_client.models.authenticator_web_authn_stage import AuthenticatorWebAuthnStage
+from authentik_client.models.authenticator_web_authn_stage_request import AuthenticatorWebAuthnStageRequest
 from authentik_client.models.auto_submit_challenge_response_request import AutoSubmitChallengeResponseRequest
 from authentik_client.models.autosubmit_challenge import AutosubmitChallenge
 from authentik_client.models.backends_enum import BackendsEnum
 from authentik_client.models.binding_type_enum import BindingTypeEnum
 from authentik_client.models.blueprint_file import BlueprintFile
 from authentik_client.models.blueprint_instance import BlueprintInstance
 from authentik_client.models.blueprint_instance_request import BlueprintInstanceRequest
@@ -221,21 +221,21 @@
 from authentik_client.models.open_id_connect_configuration import OpenIDConnectConfiguration
 from authentik_client.models.outpost import Outpost
 from authentik_client.models.outpost_default_config import OutpostDefaultConfig
 from authentik_client.models.outpost_health import OutpostHealth
 from authentik_client.models.outpost_request import OutpostRequest
 from authentik_client.models.outpost_type_enum import OutpostTypeEnum
 from authentik_client.models.paginated_application_list import PaginatedApplicationList
-from authentik_client.models.paginated_authenticate_web_authn_stage_list import PaginatedAuthenticateWebAuthnStageList
 from authentik_client.models.paginated_authenticated_session_list import PaginatedAuthenticatedSessionList
 from authentik_client.models.paginated_authenticator_duo_stage_list import PaginatedAuthenticatorDuoStageList
 from authentik_client.models.paginated_authenticator_sms_stage_list import PaginatedAuthenticatorSMSStageList
 from authentik_client.models.paginated_authenticator_static_stage_list import PaginatedAuthenticatorStaticStageList
 from authentik_client.models.paginated_authenticator_totp_stage_list import PaginatedAuthenticatorTOTPStageList
 from authentik_client.models.paginated_authenticator_validate_stage_list import PaginatedAuthenticatorValidateStageList
+from authentik_client.models.paginated_authenticator_web_authn_stage_list import PaginatedAuthenticatorWebAuthnStageList
 from authentik_client.models.paginated_blueprint_instance_list import PaginatedBlueprintInstanceList
 from authentik_client.models.paginated_brand_list import PaginatedBrandList
 from authentik_client.models.paginated_captcha_stage_list import PaginatedCaptchaStageList
 from authentik_client.models.paginated_certificate_key_pair_list import PaginatedCertificateKeyPairList
 from authentik_client.models.paginated_connection_token_list import PaginatedConnectionTokenList
 from authentik_client.models.paginated_consent_stage_list import PaginatedConsentStageList
 from authentik_client.models.paginated_deny_stage_list import PaginatedDenyStageList
@@ -317,30 +317,31 @@
 from authentik_client.models.paginated_user_login_stage_list import PaginatedUserLoginStageList
 from authentik_client.models.paginated_user_logout_stage_list import PaginatedUserLogoutStageList
 from authentik_client.models.paginated_user_o_auth_source_connection_list import PaginatedUserOAuthSourceConnectionList
 from authentik_client.models.paginated_user_saml_source_connection_list import PaginatedUserSAMLSourceConnectionList
 from authentik_client.models.paginated_user_source_connection_list import PaginatedUserSourceConnectionList
 from authentik_client.models.paginated_user_write_stage_list import PaginatedUserWriteStageList
 from authentik_client.models.paginated_web_authn_device_list import PaginatedWebAuthnDeviceList
+from authentik_client.models.paginated_web_authn_device_type_list import PaginatedWebAuthnDeviceTypeList
 from authentik_client.models.pagination import Pagination
 from authentik_client.models.password_challenge import PasswordChallenge
 from authentik_client.models.password_challenge_response_request import PasswordChallengeResponseRequest
 from authentik_client.models.password_expiry_policy import PasswordExpiryPolicy
 from authentik_client.models.password_expiry_policy_request import PasswordExpiryPolicyRequest
 from authentik_client.models.password_policy import PasswordPolicy
 from authentik_client.models.password_policy_request import PasswordPolicyRequest
 from authentik_client.models.password_stage import PasswordStage
 from authentik_client.models.password_stage_request import PasswordStageRequest
 from authentik_client.models.patched_application_request import PatchedApplicationRequest
-from authentik_client.models.patched_authenticate_web_authn_stage_request import PatchedAuthenticateWebAuthnStageRequest
 from authentik_client.models.patched_authenticator_duo_stage_request import PatchedAuthenticatorDuoStageRequest
 from authentik_client.models.patched_authenticator_sms_stage_request import PatchedAuthenticatorSMSStageRequest
 from authentik_client.models.patched_authenticator_static_stage_request import PatchedAuthenticatorStaticStageRequest
 from authentik_client.models.patched_authenticator_totp_stage_request import PatchedAuthenticatorTOTPStageRequest
 from authentik_client.models.patched_authenticator_validate_stage_request import PatchedAuthenticatorValidateStageRequest
+from authentik_client.models.patched_authenticator_web_authn_stage_request import PatchedAuthenticatorWebAuthnStageRequest
 from authentik_client.models.patched_blueprint_instance_request import PatchedBlueprintInstanceRequest
 from authentik_client.models.patched_brand_request import PatchedBrandRequest
 from authentik_client.models.patched_captcha_stage_request import PatchedCaptchaStageRequest
 from authentik_client.models.patched_certificate_key_pair_request import PatchedCertificateKeyPairRequest
 from authentik_client.models.patched_connection_token_request import PatchedConnectionTokenRequest
 from authentik_client.models.patched_consent_stage_request import PatchedConsentStageRequest
 from authentik_client.models.patched_deny_stage_request import PatchedDenyStageRequest
@@ -558,8 +559,10 @@
 from authentik_client.models.user_verification_enum import UserVerificationEnum
 from authentik_client.models.user_write_stage import UserWriteStage
 from authentik_client.models.user_write_stage_request import UserWriteStageRequest
 from authentik_client.models.validation_error import ValidationError
 from authentik_client.models.version import Version
 from authentik_client.models.web_authn_device import WebAuthnDevice
 from authentik_client.models.web_authn_device_request import WebAuthnDeviceRequest
+from authentik_client.models.web_authn_device_type import WebAuthnDeviceType
+from authentik_client.models.web_authn_device_type_request import WebAuthnDeviceTypeRequest
 from authentik_client.models.workers import Workers
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/access_denied_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/access_denied_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/app.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/app.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/app_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/app_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/apple_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/apple_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/apple_login_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/apple_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/application.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/application.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/application_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/auth_mode_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/auth_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/auth_type_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/auth_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticate_web_authn_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,38 +16,35 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from authentik_client.models.authenticator_attachment_enum import AuthenticatorAttachmentEnum
 from authentik_client.models.flow_set import FlowSet
-from authentik_client.models.resident_key_requirement_enum import ResidentKeyRequirementEnum
-from authentik_client.models.user_verification_enum import UserVerificationEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AuthenticateWebAuthnStage(BaseModel):
+class AuthenticatorDuoStage(BaseModel):
     """
-    AuthenticateWebAuthnStage Serializer
+    AuthenticatorDuoStage Serializer
     """ # noqa: E501
     pk: StrictStr
     name: StrictStr
     component: StrictStr = Field(description="Get object type so that we know how to edit the object")
     verbose_name: StrictStr = Field(description="Return object's verbose_name")
     verbose_name_plural: StrictStr = Field(description="Return object's plural verbose_name")
     meta_model_name: StrictStr = Field(description="Return internal model name")
     flow_set: Optional[List[FlowSet]] = None
     configure_flow: Optional[StrictStr] = Field(default=None, description="Flow used by an authenticated user to configure this Stage. If empty, user will not be able to configure this stage.")
     friendly_name: Optional[StrictStr] = None
-    user_verification: Optional[UserVerificationEnum] = None
-    authenticator_attachment: Optional[AuthenticatorAttachmentEnum] = None
-    resident_key_requirement: Optional[ResidentKeyRequirementEnum] = None
-    __properties: ClassVar[List[str]] = ["pk", "name", "component", "verbose_name", "verbose_name_plural", "meta_model_name", "flow_set", "configure_flow", "friendly_name", "user_verification", "authenticator_attachment", "resident_key_requirement"]
+    client_id: StrictStr
+    api_hostname: StrictStr
+    admin_integration_key: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["pk", "name", "component", "verbose_name", "verbose_name_plural", "meta_model_name", "flow_set", "configure_flow", "friendly_name", "client_id", "api_hostname", "admin_integration_key"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -59,15 +56,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AuthenticateWebAuthnStage from a JSON string"""
+        """Create an instance of AuthenticatorDuoStage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -107,24 +104,19 @@
             _dict['configure_flow'] = None
 
         # set to None if friendly_name (nullable) is None
         # and model_fields_set contains the field
         if self.friendly_name is None and "friendly_name" in self.model_fields_set:
             _dict['friendly_name'] = None
 
-        # set to None if authenticator_attachment (nullable) is None
-        # and model_fields_set contains the field
-        if self.authenticator_attachment is None and "authenticator_attachment" in self.model_fields_set:
-            _dict['authenticator_attachment'] = None
-
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AuthenticateWebAuthnStage from a dict"""
+        """Create an instance of AuthenticatorDuoStage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
@@ -133,14 +125,14 @@
             "component": obj.get("component"),
             "verbose_name": obj.get("verbose_name"),
             "verbose_name_plural": obj.get("verbose_name_plural"),
             "meta_model_name": obj.get("meta_model_name"),
             "flow_set": [FlowSet.from_dict(_item) for _item in obj["flow_set"]] if obj.get("flow_set") is not None else None,
             "configure_flow": obj.get("configure_flow"),
             "friendly_name": obj.get("friendly_name"),
-            "user_verification": obj.get("user_verification"),
-            "authenticator_attachment": obj.get("authenticator_attachment"),
-            "resident_key_requirement": obj.get("resident_key_requirement")
+            "client_id": obj.get("client_id"),
+            "api_hostname": obj.get("api_hostname"),
+            "admin_integration_key": obj.get("admin_integration_key")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticate_web_authn_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_stage_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,27 @@
 from authentik_client.models.authenticator_attachment_enum import AuthenticatorAttachmentEnum
 from authentik_client.models.flow_set_request import FlowSetRequest
 from authentik_client.models.resident_key_requirement_enum import ResidentKeyRequirementEnum
 from authentik_client.models.user_verification_enum import UserVerificationEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AuthenticateWebAuthnStageRequest(BaseModel):
+class AuthenticatorWebAuthnStageRequest(BaseModel):
     """
-    AuthenticateWebAuthnStage Serializer
+    AuthenticatorWebAuthnStage Serializer
     """ # noqa: E501
     name: Annotated[str, Field(min_length=1, strict=True)]
     flow_set: Optional[List[FlowSetRequest]] = None
     configure_flow: Optional[StrictStr] = Field(default=None, description="Flow used by an authenticated user to configure this Stage. If empty, user will not be able to configure this stage.")
     friendly_name: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
     user_verification: Optional[UserVerificationEnum] = None
     authenticator_attachment: Optional[AuthenticatorAttachmentEnum] = None
     resident_key_requirement: Optional[ResidentKeyRequirementEnum] = None
-    __properties: ClassVar[List[str]] = ["name", "flow_set", "configure_flow", "friendly_name", "user_verification", "authenticator_attachment", "resident_key_requirement"]
+    device_type_restrictions: Optional[List[StrictStr]] = None
+    __properties: ClassVar[List[str]] = ["name", "flow_set", "configure_flow", "friendly_name", "user_verification", "authenticator_attachment", "resident_key_requirement", "device_type_restrictions"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -55,15 +56,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AuthenticateWebAuthnStageRequest from a JSON string"""
+        """Create an instance of AuthenticatorWebAuthnStageRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -102,26 +103,27 @@
         if self.authenticator_attachment is None and "authenticator_attachment" in self.model_fields_set:
             _dict['authenticator_attachment'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AuthenticateWebAuthnStageRequest from a dict"""
+        """Create an instance of AuthenticatorWebAuthnStageRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
             "flow_set": [FlowSetRequest.from_dict(_item) for _item in obj["flow_set"]] if obj.get("flow_set") is not None else None,
             "configure_flow": obj.get("configure_flow"),
             "friendly_name": obj.get("friendly_name"),
             "user_verification": obj.get("user_verification"),
             "authenticator_attachment": obj.get("authenticator_attachment"),
-            "resident_key_requirement": obj.get("resident_key_requirement")
+            "resident_key_requirement": obj.get("resident_key_requirement"),
+            "device_type_restrictions": obj.get("device_type_restrictions")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_asn.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_asn.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_geo_ip.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_geo_ip.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_user_agent.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_user_agent_device.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_user_agent_os.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_os.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticated_session_user_agent_user_agent.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticated_session_user_agent_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authentication_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authentication_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_attachment_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_attachment_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_stage.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,35 +16,34 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from authentik_client.models.digits_enum import DigitsEnum
 from authentik_client.models.flow_set import FlowSet
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AuthenticatorDuoStage(BaseModel):
+class AuthenticatorTOTPStage(BaseModel):
     """
-    AuthenticatorDuoStage Serializer
+    AuthenticatorTOTPStage Serializer
     """ # noqa: E501
     pk: StrictStr
     name: StrictStr
     component: StrictStr = Field(description="Get object type so that we know how to edit the object")
     verbose_name: StrictStr = Field(description="Return object's verbose_name")
     verbose_name_plural: StrictStr = Field(description="Return object's plural verbose_name")
     meta_model_name: StrictStr = Field(description="Return internal model name")
     flow_set: Optional[List[FlowSet]] = None
     configure_flow: Optional[StrictStr] = Field(default=None, description="Flow used by an authenticated user to configure this Stage. If empty, user will not be able to configure this stage.")
     friendly_name: Optional[StrictStr] = None
-    client_id: StrictStr
-    api_hostname: StrictStr
-    admin_integration_key: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["pk", "name", "component", "verbose_name", "verbose_name_plural", "meta_model_name", "flow_set", "configure_flow", "friendly_name", "client_id", "api_hostname", "admin_integration_key"]
+    digits: DigitsEnum
+    __properties: ClassVar[List[str]] = ["pk", "name", "component", "verbose_name", "verbose_name_plural", "meta_model_name", "flow_set", "configure_flow", "friendly_name", "digits"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -56,15 +55,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AuthenticatorDuoStage from a JSON string"""
+        """Create an instance of AuthenticatorTOTPStage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -108,15 +107,15 @@
         if self.friendly_name is None and "friendly_name" in self.model_fields_set:
             _dict['friendly_name'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AuthenticatorDuoStage from a dict"""
+        """Create an instance of AuthenticatorTOTPStage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
@@ -125,14 +124,12 @@
             "component": obj.get("component"),
             "verbose_name": obj.get("verbose_name"),
             "verbose_name_plural": obj.get("verbose_name_plural"),
             "meta_model_name": obj.get("meta_model_name"),
             "flow_set": [FlowSet.from_dict(_item) for _item in obj["flow_set"]] if obj.get("flow_set") is not None else None,
             "configure_flow": obj.get("configure_flow"),
             "friendly_name": obj.get("friendly_name"),
-            "client_id": obj.get("client_id"),
-            "api_hostname": obj.get("api_hostname"),
-            "admin_integration_key": obj.get("admin_integration_key")
+            "digits": obj.get("digits")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_stage_device_import_response.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_device_import_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_duo_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_sms_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_sms_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_sms_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_sms_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_static_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_static_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_static_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_static_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_totp_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_totp_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_totp_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_stage.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,34 +16,35 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from authentik_client.models.digits_enum import DigitsEnum
+from typing_extensions import Annotated
+from authentik_client.models.backends_enum import BackendsEnum
 from authentik_client.models.flow_set import FlowSet
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AuthenticatorTOTPStage(BaseModel):
+class PasswordStage(BaseModel):
     """
-    AuthenticatorTOTPStage Serializer
+    PasswordStage Serializer
     """ # noqa: E501
     pk: StrictStr
     name: StrictStr
     component: StrictStr = Field(description="Get object type so that we know how to edit the object")
     verbose_name: StrictStr = Field(description="Return object's verbose_name")
     verbose_name_plural: StrictStr = Field(description="Return object's plural verbose_name")
     meta_model_name: StrictStr = Field(description="Return internal model name")
     flow_set: Optional[List[FlowSet]] = None
+    backends: List[BackendsEnum] = Field(description="Selection of backends to test the password against.")
     configure_flow: Optional[StrictStr] = Field(default=None, description="Flow used by an authenticated user to configure this Stage. If empty, user will not be able to configure this stage.")
-    friendly_name: Optional[StrictStr] = None
-    digits: DigitsEnum
-    __properties: ClassVar[List[str]] = ["pk", "name", "component", "verbose_name", "verbose_name_plural", "meta_model_name", "flow_set", "configure_flow", "friendly_name", "digits"]
+    failed_attempts_before_cancel: Optional[Annotated[int, Field(le=2147483647, strict=True, ge=-2147483648)]] = Field(default=None, description="How many attempts a user has before the flow is canceled. To lock the user out, use a reputation policy and a user_write stage.")
+    __properties: ClassVar[List[str]] = ["pk", "name", "component", "verbose_name", "verbose_name_plural", "meta_model_name", "flow_set", "backends", "configure_flow", "failed_attempts_before_cancel"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -55,15 +56,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AuthenticatorTOTPStage from a JSON string"""
+        """Create an instance of PasswordStage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -98,38 +99,33 @@
                     _items.append(_item.to_dict())
             _dict['flow_set'] = _items
         # set to None if configure_flow (nullable) is None
         # and model_fields_set contains the field
         if self.configure_flow is None and "configure_flow" in self.model_fields_set:
             _dict['configure_flow'] = None
 
-        # set to None if friendly_name (nullable) is None
-        # and model_fields_set contains the field
-        if self.friendly_name is None and "friendly_name" in self.model_fields_set:
-            _dict['friendly_name'] = None
-
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AuthenticatorTOTPStage from a dict"""
+        """Create an instance of PasswordStage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pk": obj.get("pk"),
             "name": obj.get("name"),
             "component": obj.get("component"),
             "verbose_name": obj.get("verbose_name"),
             "verbose_name_plural": obj.get("verbose_name_plural"),
             "meta_model_name": obj.get("meta_model_name"),
             "flow_set": [FlowSet.from_dict(_item) for _item in obj["flow_set"]] if obj.get("flow_set") is not None else None,
+            "backends": obj.get("backends"),
             "configure_flow": obj.get("configure_flow"),
-            "friendly_name": obj.get("friendly_name"),
-            "digits": obj.get("digits")
+            "failed_attempts_before_cancel": obj.get("failed_attempts_before_cancel")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_totp_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_validate_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validate_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_validate_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_validation_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validation_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_validation_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_validation_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_web_authn_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/authenticator_web_authn_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/authenticator_web_authn_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/auto_submit_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/auto_submit_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/autosubmit_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/autosubmit_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/backends_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/backends_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/binding_type_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/binding_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/blueprint_file.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_file.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/blueprint_instance.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/blueprint_instance_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/blueprint_instance_status_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/blueprint_instance_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/brand.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/brand_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/cache.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/cache.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/capabilities_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/capabilities_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/captcha_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/captcha_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/captcha_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/captcha_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/certificate_data.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_data.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/certificate_generation_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_generation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/certificate_key_pair.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_key_pair.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/certificate_key_pair_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/challenge_choices.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/challenge_choices.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/challenge_types.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/client_type_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/client_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/config.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/connection_token.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/connection_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/connection_token_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_permission.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_stage_mode_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/consent_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/contextual_flow_info.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/contextual_flow_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/contextual_flow_info_layout_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/contextual_flow_info_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/coordinate.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/coordinate.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/current_brand.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/current_brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/denied_action_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/denied_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/deny_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/deny_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/deny_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/device.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/device_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/device_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/device_challenge_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/device_challenge_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/device_classes_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/device_classes_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/digest_algorithm_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/digest_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/digits_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/digits_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/docker_service_connection.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/docker_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/docker_service_connection_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/domain.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/domain.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/domain_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_policy.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/dummy_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/duo_device.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/duo_device_enrollment_status.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device_enrollment_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/duo_device_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/duo_response_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/duo_response_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/email_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/email_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/email_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/email_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/email_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/email_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/email_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/endpoint.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/endpoint_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/error_detail.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/error_reporting_config.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/error_reporting_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/event.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/event_actions.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/event_actions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/event_matcher_policy.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/event_matcher_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/event_matcher_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/event_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/event_top_per_user.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/event_top_per_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/expiring_base_grant_model.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/expiring_base_grant_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/expression_policy.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/expression_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/expression_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/extra_role_object_permission.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/extra_role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/extra_user_object_permission.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/extra_user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/file_path_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/file_path_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_designation_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_designation_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_diagram.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_diagram.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_error_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_error_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_import_result.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_import_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_inspection.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_inspection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_inspector_plan.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_inspector_plan.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_layout_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_set.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_set.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_set_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_stage_binding.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_stage_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/flow_stage_binding_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/footer_link.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/footer_link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/generic_error.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/generic_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/geoip_binding_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/geoip_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/group.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/group_member.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/group_member_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/group_member_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/group_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/identification_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/identification_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/identification_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/identification_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/install_id.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/install_id.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/intent_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/intent_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/invalid_response_action_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/invalid_response_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/invitation.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/invitation_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/invitation_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/invitation_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/issuer_mode_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/issuer_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/kubernetes_service_connection.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/kubernetes_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/kubernetes_service_connection_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_debug.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_debug.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_outpost_config.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_property_mapping.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_property_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_provider.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_source.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_source_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/ldap_sync_status.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldap_sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/ldapapi_access_mode.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/ldapapi_access_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/license.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/license.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/license_forecast.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/license_forecast.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/license_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/license_summary.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/license_summary.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/link.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/log_event.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/log_event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/log_level_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/log_level_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/login_challenge_types.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/login_challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/login_metrics.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/login_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/login_source.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/login_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/metadata.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/model_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/model_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     AUTHENTIK_STAGES_AUTHENTICATOR_SMS_DOT_AUTHENTICATORSMSSTAGE = 'authentik_stages_authenticator_sms.authenticatorsmsstage'
     AUTHENTIK_STAGES_AUTHENTICATOR_SMS_DOT_SMSDEVICE = 'authentik_stages_authenticator_sms.smsdevice'
     AUTHENTIK_STAGES_AUTHENTICATOR_STATIC_DOT_AUTHENTICATORSTATICSTAGE = 'authentik_stages_authenticator_static.authenticatorstaticstage'
     AUTHENTIK_STAGES_AUTHENTICATOR_STATIC_DOT_STATICDEVICE = 'authentik_stages_authenticator_static.staticdevice'
     AUTHENTIK_STAGES_AUTHENTICATOR_TOTP_DOT_AUTHENTICATORTOTPSTAGE = 'authentik_stages_authenticator_totp.authenticatortotpstage'
     AUTHENTIK_STAGES_AUTHENTICATOR_TOTP_DOT_TOTPDEVICE = 'authentik_stages_authenticator_totp.totpdevice'
     AUTHENTIK_STAGES_AUTHENTICATOR_VALIDATE_DOT_AUTHENTICATORVALIDATESTAGE = 'authentik_stages_authenticator_validate.authenticatorvalidatestage'
-    AUTHENTIK_STAGES_AUTHENTICATOR_WEBAUTHN_DOT_AUTHENTICATEWEBAUTHNSTAGE = 'authentik_stages_authenticator_webauthn.authenticatewebauthnstage'
+    AUTHENTIK_STAGES_AUTHENTICATOR_WEBAUTHN_DOT_AUTHENTICATORWEBAUTHNSTAGE = 'authentik_stages_authenticator_webauthn.authenticatorwebauthnstage'
     AUTHENTIK_STAGES_AUTHENTICATOR_WEBAUTHN_DOT_WEBAUTHNDEVICE = 'authentik_stages_authenticator_webauthn.webauthndevice'
     AUTHENTIK_STAGES_CAPTCHA_DOT_CAPTCHASTAGE = 'authentik_stages_captcha.captchastage'
     AUTHENTIK_STAGES_CONSENT_DOT_CONSENTSTAGE = 'authentik_stages_consent.consentstage'
     AUTHENTIK_STAGES_CONSENT_DOT_USERCONSENT = 'authentik_stages_consent.userconsent'
     AUTHENTIK_STAGES_DENY_DOT_DENYSTAGE = 'authentik_stages_deny.denystage'
     AUTHENTIK_STAGES_DUMMY_DOT_DUMMYSTAGE = 'authentik_stages_dummy.dummystage'
     AUTHENTIK_STAGES_EMAIL_DOT_EMAILSTAGE = 'authentik_stages_email.emailstage'
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/model_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/model_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/name_id_policy_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/name_id_policy_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/network_binding_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/network_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/not_configured_action_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/not_configured_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/notification.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_rule.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_rule.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_rule_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_transport.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_transport_mode_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_transport_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_transport_test.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_transport_test.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_webhook_mapping.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_webhook_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/notification_webhook_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth2_provider.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth2_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth2_provider_setup_urls.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth2_provider_setup_urls.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_device_code_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_device_code_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_device_code_finish_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_finish_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_source.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/o_auth_source_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/open_id_connect_configuration.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/open_id_connect_configuration.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/outpost.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/outpost_default_config.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_default_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/outpost_health.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_health.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/outpost_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/outpost_type_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/outpost_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_application_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticate_web_authn_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_web_authn_stage_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from authentik_client.models.authenticate_web_authn_stage import AuthenticateWebAuthnStage
+from authentik_client.models.authenticator_web_authn_stage import AuthenticatorWebAuthnStage
 from authentik_client.models.pagination import Pagination
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedAuthenticateWebAuthnStageList(BaseModel):
+class PaginatedAuthenticatorWebAuthnStageList(BaseModel):
     """
-    PaginatedAuthenticateWebAuthnStageList
+    PaginatedAuthenticatorWebAuthnStageList
     """ # noqa: E501
     pagination: Pagination
-    results: List[AuthenticateWebAuthnStage]
+    results: List[AuthenticatorWebAuthnStage]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedAuthenticateWebAuthnStageList from a JSON string"""
+        """Create an instance of PaginatedAuthenticatorWebAuthnStageList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedAuthenticateWebAuthnStageList from a dict"""
+        """Create an instance of PaginatedAuthenticatorWebAuthnStageList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [AuthenticateWebAuthnStage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [AuthenticatorWebAuthnStage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticated_session_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticated_session_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticator_duo_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_duo_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticator_sms_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_sms_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticator_static_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_static_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticator_totp_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_totp_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_authenticator_validate_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_authenticator_validate_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_blueprint_instance_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_blueprint_instance_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_brand_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_brand_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_captcha_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_captcha_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_certificate_key_pair_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_certificate_key_pair_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_connection_token_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_connection_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_consent_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_consent_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_deny_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_deny_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_docker_service_connection_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_docker_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_domain_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_domain_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_dummy_policy_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_dummy_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_dummy_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_dummy_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_duo_device_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_duo_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_email_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_email_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_endpoint_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_endpoint_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_event_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_event_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_event_matcher_policy_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_event_matcher_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_expiring_base_grant_model_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_expiring_base_grant_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_expression_policy_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_expression_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_extra_role_object_permission_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_extra_role_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_extra_user_object_permission_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_extra_user_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_flow_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_flow_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_flow_stage_binding_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_flow_stage_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_group_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_identification_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_identification_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_invitation_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_invitation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_invitation_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_invitation_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_kubernetes_service_connection_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_kubernetes_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_ldap_outpost_config_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_ldap_property_mapping_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_ldap_provider_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_ldap_source_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_ldap_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_license_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_license_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_notification_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_notification_rule_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_rule_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_notification_transport_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_transport_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_notification_webhook_mapping_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_notification_webhook_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_o_auth2_provider_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_o_auth2_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_o_auth_source_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_o_auth_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_outpost_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_outpost_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_password_expiry_policy_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_expiry_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_password_policy_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_password_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_password_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_permission_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_plex_source_connection_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_plex_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_plex_source_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_plex_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_policy_binding_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_policy_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_policy_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_prompt_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_prompt_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_prompt_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_prompt_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_property_mapping_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_provider_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_proxy_outpost_config_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_proxy_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_proxy_provider_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_proxy_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_rac_property_mapping_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_rac_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_rac_provider_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_rac_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_radius_outpost_config_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_radius_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_radius_provider_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_radius_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_reputation_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_reputation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_reputation_policy_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_reputation_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_role_assigned_object_permission_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_role_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_role_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_role_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_saml_property_mapping_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_saml_provider_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_saml_source_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_saml_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_scim_mapping_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scim_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_scim_provider_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scim_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_scope_mapping_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_scope_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_service_connection_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_sms_device_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_sms_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_source_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_source_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_source_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_static_device_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_static_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_system_task_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_system_task_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_tenant_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_tenant_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_token_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_token_model_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_token_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_totp_device_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_totp_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_assigned_object_permission_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_consent_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_consent_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_delete_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_delete_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_login_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_login_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_logout_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_logout_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_o_auth_source_connection_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_o_auth_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_saml_source_connection_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_saml_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_source_connection_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_user_write_stage_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_user_write_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/paginated_web_authn_device_list.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_web_authn_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/pagination.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/pagination.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/password_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/password_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/password_expiry_policy.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_expiry_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/password_expiry_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/password_policy.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/password_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/password_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,37 +14,40 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from authentik_client.models.backends_enum import BackendsEnum
-from authentik_client.models.flow_set import FlowSet
+from authentik_client.models.prompt_type_enum import PromptTypeEnum
+from authentik_client.models.stage import Stage
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PasswordStage(BaseModel):
+class Prompt(BaseModel):
     """
-    PasswordStage Serializer
+    Prompt Serializer
     """ # noqa: E501
     pk: StrictStr
     name: StrictStr
-    component: StrictStr = Field(description="Get object type so that we know how to edit the object")
-    verbose_name: StrictStr = Field(description="Return object's verbose_name")
-    verbose_name_plural: StrictStr = Field(description="Return object's plural verbose_name")
-    meta_model_name: StrictStr = Field(description="Return internal model name")
-    flow_set: Optional[List[FlowSet]] = None
-    backends: List[BackendsEnum] = Field(description="Selection of backends to test the password against.")
-    configure_flow: Optional[StrictStr] = Field(default=None, description="Flow used by an authenticated user to configure this Stage. If empty, user will not be able to configure this stage.")
-    failed_attempts_before_cancel: Optional[Annotated[int, Field(le=2147483647, strict=True, ge=-2147483648)]] = Field(default=None, description="How many attempts a user has before the flow is canceled. To lock the user out, use a reputation policy and a user_write stage.")
-    __properties: ClassVar[List[str]] = ["pk", "name", "component", "verbose_name", "verbose_name_plural", "meta_model_name", "flow_set", "backends", "configure_flow", "failed_attempts_before_cancel"]
+    field_key: StrictStr = Field(description="Name of the form field, also used to store the value")
+    label: StrictStr
+    type: PromptTypeEnum
+    required: Optional[StrictBool] = None
+    placeholder: Optional[StrictStr] = Field(default=None, description="Optionally provide a short hint that describes the expected input value. When creating a fixed choice field, enable interpreting as expression and return a list to return multiple choices.")
+    initial_value: Optional[StrictStr] = Field(default=None, description="Optionally pre-fill the input with an initial value. When creating a fixed choice field, enable interpreting as expression and return a list to return multiple default choices.")
+    order: Optional[Annotated[int, Field(le=2147483647, strict=True, ge=-2147483648)]] = None
+    promptstage_set: Optional[List[Stage]] = None
+    sub_text: Optional[StrictStr] = None
+    placeholder_expression: Optional[StrictBool] = None
+    initial_value_expression: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["pk", "name", "field_key", "label", "type", "required", "placeholder", "initial_value", "order", "promptstage_set", "sub_text", "placeholder_expression", "initial_value_expression"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -56,76 +59,66 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PasswordStage from a JSON string"""
+        """Create an instance of Prompt from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
             "pk",
-            "component",
-            "verbose_name",
-            "verbose_name_plural",
-            "meta_model_name",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in flow_set (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in promptstage_set (list)
         _items = []
-        if self.flow_set:
-            for _item in self.flow_set:
+        if self.promptstage_set:
+            for _item in self.promptstage_set:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['flow_set'] = _items
-        # set to None if configure_flow (nullable) is None
-        # and model_fields_set contains the field
-        if self.configure_flow is None and "configure_flow" in self.model_fields_set:
-            _dict['configure_flow'] = None
-
+            _dict['promptstage_set'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PasswordStage from a dict"""
+        """Create an instance of Prompt from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pk": obj.get("pk"),
             "name": obj.get("name"),
-            "component": obj.get("component"),
-            "verbose_name": obj.get("verbose_name"),
-            "verbose_name_plural": obj.get("verbose_name_plural"),
-            "meta_model_name": obj.get("meta_model_name"),
-            "flow_set": [FlowSet.from_dict(_item) for _item in obj["flow_set"]] if obj.get("flow_set") is not None else None,
-            "backends": obj.get("backends"),
-            "configure_flow": obj.get("configure_flow"),
-            "failed_attempts_before_cancel": obj.get("failed_attempts_before_cancel")
+            "field_key": obj.get("field_key"),
+            "label": obj.get("label"),
+            "type": obj.get("type"),
+            "required": obj.get("required"),
+            "placeholder": obj.get("placeholder"),
+            "initial_value": obj.get("initial_value"),
+            "order": obj.get("order"),
+            "promptstage_set": [Stage.from_dict(_item) for _item in obj["promptstage_set"]] if obj.get("promptstage_set") is not None else None,
+            "sub_text": obj.get("sub_text"),
+            "placeholder_expression": obj.get("placeholder_expression"),
+            "initial_value_expression": obj.get("initial_value_expression")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/password_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_application_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticate_web_authn_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_web_authn_stage_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,26 +24,27 @@
 from authentik_client.models.authenticator_attachment_enum import AuthenticatorAttachmentEnum
 from authentik_client.models.flow_set_request import FlowSetRequest
 from authentik_client.models.resident_key_requirement_enum import ResidentKeyRequirementEnum
 from authentik_client.models.user_verification_enum import UserVerificationEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PatchedAuthenticateWebAuthnStageRequest(BaseModel):
+class PatchedAuthenticatorWebAuthnStageRequest(BaseModel):
     """
-    AuthenticateWebAuthnStage Serializer
+    AuthenticatorWebAuthnStage Serializer
     """ # noqa: E501
     name: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
     flow_set: Optional[List[FlowSetRequest]] = None
     configure_flow: Optional[StrictStr] = Field(default=None, description="Flow used by an authenticated user to configure this Stage. If empty, user will not be able to configure this stage.")
     friendly_name: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
     user_verification: Optional[UserVerificationEnum] = None
     authenticator_attachment: Optional[AuthenticatorAttachmentEnum] = None
     resident_key_requirement: Optional[ResidentKeyRequirementEnum] = None
-    __properties: ClassVar[List[str]] = ["name", "flow_set", "configure_flow", "friendly_name", "user_verification", "authenticator_attachment", "resident_key_requirement"]
+    device_type_restrictions: Optional[List[StrictStr]] = None
+    __properties: ClassVar[List[str]] = ["name", "flow_set", "configure_flow", "friendly_name", "user_verification", "authenticator_attachment", "resident_key_requirement", "device_type_restrictions"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -55,15 +56,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PatchedAuthenticateWebAuthnStageRequest from a JSON string"""
+        """Create an instance of PatchedAuthenticatorWebAuthnStageRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -102,26 +103,27 @@
         if self.authenticator_attachment is None and "authenticator_attachment" in self.model_fields_set:
             _dict['authenticator_attachment'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PatchedAuthenticateWebAuthnStageRequest from a dict"""
+        """Create an instance of PatchedAuthenticatorWebAuthnStageRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
             "flow_set": [FlowSetRequest.from_dict(_item) for _item in obj["flow_set"]] if obj.get("flow_set") is not None else None,
             "configure_flow": obj.get("configure_flow"),
             "friendly_name": obj.get("friendly_name"),
             "user_verification": obj.get("user_verification"),
             "authenticator_attachment": obj.get("authenticator_attachment"),
-            "resident_key_requirement": obj.get("resident_key_requirement")
+            "resident_key_requirement": obj.get("resident_key_requirement"),
+            "device_type_restrictions": obj.get("device_type_restrictions")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticator_duo_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticator_sms_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticator_static_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticator_totp_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_authenticator_validate_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_blueprint_instance_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_brand_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_captcha_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_certificate_key_pair_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_connection_token_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_consent_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_deny_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_docker_service_connection_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_domain_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_dummy_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_dummy_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_duo_device_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_email_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_endpoint_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_event_matcher_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_event_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_expression_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_flow_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_flow_stage_binding_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_group_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_identification_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_invitation_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_invitation_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_kubernetes_service_connection_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_ldap_property_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_ldap_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_ldap_source_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_license_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_notification_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_notification_rule_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_notification_transport_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_notification_webhook_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_o_auth2_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_o_auth_source_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_outpost_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_password_expiry_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_password_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_password_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_permission_assign_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_plex_source_connection_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_plex_source_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_policy_binding_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_prompt_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_prompt_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_proxy_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_rac_property_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_rac_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_radius_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_reputation_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_role_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_saml_property_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_saml_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_saml_source_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_scim_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_scim_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_scope_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_settings_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_sms_device_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_source_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_static_device_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_tenant_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_token_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_totp_device_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_delete_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_login_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_logout_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_o_auth_source_connection_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_saml_source_connection_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_user_write_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/patched_web_authn_device_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/patched_web_authn_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/permission.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/permission_assign_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_authentication_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_authentication_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_authentication_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_authentication_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_source.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_source_connection.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_source_connection_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_source_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/plex_token_redeem_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/plex_token_redeem_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/policy.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_binding.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_binding_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_engine_mode.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_engine_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_test_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_test_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/policy_test_result.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/policy_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,36 +18,35 @@
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from authentik_client.models.prompt_type_enum import PromptTypeEnum
-from authentik_client.models.stage import Stage
+from authentik_client.models.stage_request import StageRequest
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Prompt(BaseModel):
+class PromptRequest(BaseModel):
     """
     Prompt Serializer
     """ # noqa: E501
-    pk: StrictStr
-    name: StrictStr
-    field_key: StrictStr = Field(description="Name of the form field, also used to store the value")
-    label: StrictStr
+    name: Annotated[str, Field(min_length=1, strict=True)]
+    field_key: Annotated[str, Field(min_length=1, strict=True)] = Field(description="Name of the form field, also used to store the value")
+    label: Annotated[str, Field(min_length=1, strict=True)]
     type: PromptTypeEnum
     required: Optional[StrictBool] = None
     placeholder: Optional[StrictStr] = Field(default=None, description="Optionally provide a short hint that describes the expected input value. When creating a fixed choice field, enable interpreting as expression and return a list to return multiple choices.")
     initial_value: Optional[StrictStr] = Field(default=None, description="Optionally pre-fill the input with an initial value. When creating a fixed choice field, enable interpreting as expression and return a list to return multiple default choices.")
     order: Optional[Annotated[int, Field(le=2147483647, strict=True, ge=-2147483648)]] = None
-    promptstage_set: Optional[List[Stage]] = None
+    promptstage_set: Optional[List[StageRequest]] = None
     sub_text: Optional[StrictStr] = None
     placeholder_expression: Optional[StrictBool] = None
     initial_value_expression: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["pk", "name", "field_key", "label", "type", "required", "placeholder", "initial_value", "order", "promptstage_set", "sub_text", "placeholder_expression", "initial_value_expression"]
+    __properties: ClassVar[List[str]] = ["name", "field_key", "label", "type", "required", "placeholder", "initial_value", "order", "promptstage_set", "sub_text", "placeholder_expression", "initial_value_expression"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -59,30 +58,28 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Prompt from a JSON string"""
+        """Create an instance of PromptRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "pk",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
@@ -93,32 +90,31 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['promptstage_set'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Prompt from a dict"""
+        """Create an instance of PromptRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "pk": obj.get("pk"),
             "name": obj.get("name"),
             "field_key": obj.get("field_key"),
             "label": obj.get("label"),
             "type": obj.get("type"),
             "required": obj.get("required"),
             "placeholder": obj.get("placeholder"),
             "initial_value": obj.get("initial_value"),
             "order": obj.get("order"),
-            "promptstage_set": [Stage.from_dict(_item) for _item in obj["promptstage_set"]] if obj.get("promptstage_set") is not None else None,
+            "promptstage_set": [StageRequest.from_dict(_item) for _item in obj["promptstage_set"]] if obj.get("promptstage_set") is not None else None,
             "sub_text": obj.get("sub_text"),
             "placeholder_expression": obj.get("placeholder_expression"),
             "initial_value_expression": obj.get("initial_value_expression")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/source_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,39 +14,42 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from authentik_client.models.prompt_type_enum import PromptTypeEnum
-from authentik_client.models.stage_request import StageRequest
+from authentik_client.models.policy_engine_mode import PolicyEngineMode
+from authentik_client.models.user_matching_mode_enum import UserMatchingModeEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PromptRequest(BaseModel):
+class SourceRequest(BaseModel):
     """
-    Prompt Serializer
+    Source Serializer
     """ # noqa: E501
-    name: Annotated[str, Field(min_length=1, strict=True)]
-    field_key: Annotated[str, Field(min_length=1, strict=True)] = Field(description="Name of the form field, also used to store the value")
-    label: Annotated[str, Field(min_length=1, strict=True)]
-    type: PromptTypeEnum
-    required: Optional[StrictBool] = None
-    placeholder: Optional[StrictStr] = Field(default=None, description="Optionally provide a short hint that describes the expected input value. When creating a fixed choice field, enable interpreting as expression and return a list to return multiple choices.")
-    initial_value: Optional[StrictStr] = Field(default=None, description="Optionally pre-fill the input with an initial value. When creating a fixed choice field, enable interpreting as expression and return a list to return multiple default choices.")
-    order: Optional[Annotated[int, Field(le=2147483647, strict=True, ge=-2147483648)]] = None
-    promptstage_set: Optional[List[StageRequest]] = None
-    sub_text: Optional[StrictStr] = None
-    placeholder_expression: Optional[StrictBool] = None
-    initial_value_expression: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["name", "field_key", "label", "type", "required", "placeholder", "initial_value", "order", "promptstage_set", "sub_text", "placeholder_expression", "initial_value_expression"]
+    name: Annotated[str, Field(min_length=1, strict=True)] = Field(description="Source's display Name.")
+    slug: Annotated[str, Field(min_length=1, strict=True, max_length=50)] = Field(description="Internal source name, used in URLs.")
+    enabled: Optional[StrictBool] = None
+    authentication_flow: Optional[StrictStr] = Field(default=None, description="Flow to use when authenticating existing users.")
+    enrollment_flow: Optional[StrictStr] = Field(default=None, description="Flow to use when enrolling new users.")
+    policy_engine_mode: Optional[PolicyEngineMode] = None
+    user_matching_mode: Optional[UserMatchingModeEnum] = Field(default=None, description="How the source determines if an existing user should be authenticated or a new user enrolled.")
+    user_path_template: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
+    __properties: ClassVar[List[str]] = ["name", "slug", "enabled", "authentication_flow", "enrollment_flow", "policy_engine_mode", "user_matching_mode", "user_path_template"]
+
+    @field_validator('slug')
+    def slug_validate_regular_expression(cls, value):
+        """Validates the regular expression"""
+        if not re.match(r"^[-a-zA-Z0-9_]+$", value):
+            raise ValueError(r"must validate the regular expression /^[-a-zA-Z0-9_]+$/")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -58,15 +61,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PromptRequest from a JSON string"""
+        """Create an instance of SourceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,42 +82,41 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in promptstage_set (list)
-        _items = []
-        if self.promptstage_set:
-            for _item in self.promptstage_set:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['promptstage_set'] = _items
+        # set to None if authentication_flow (nullable) is None
+        # and model_fields_set contains the field
+        if self.authentication_flow is None and "authentication_flow" in self.model_fields_set:
+            _dict['authentication_flow'] = None
+
+        # set to None if enrollment_flow (nullable) is None
+        # and model_fields_set contains the field
+        if self.enrollment_flow is None and "enrollment_flow" in self.model_fields_set:
+            _dict['enrollment_flow'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PromptRequest from a dict"""
+        """Create an instance of SourceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
-            "field_key": obj.get("field_key"),
-            "label": obj.get("label"),
-            "type": obj.get("type"),
-            "required": obj.get("required"),
-            "placeholder": obj.get("placeholder"),
-            "initial_value": obj.get("initial_value"),
-            "order": obj.get("order"),
-            "promptstage_set": [StageRequest.from_dict(_item) for _item in obj["promptstage_set"]] if obj.get("promptstage_set") is not None else None,
-            "sub_text": obj.get("sub_text"),
-            "placeholder_expression": obj.get("placeholder_expression"),
-            "initial_value_expression": obj.get("initial_value_expression")
+            "slug": obj.get("slug"),
+            "enabled": obj.get("enabled"),
+            "authentication_flow": obj.get("authentication_flow"),
+            "enrollment_flow": obj.get("enrollment_flow"),
+            "policy_engine_mode": obj.get("policy_engine_mode"),
+            "user_matching_mode": obj.get("user_matching_mode"),
+            "user_path_template": obj.get("user_path_template")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/prompt_type_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/prompt_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/property_mapping.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/property_mapping_preview.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping_preview.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/property_mapping_test_result.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/property_mapping_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/protocol_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/protocol_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/provider.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/provider_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/provider_model_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/provider_type_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/provider_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/proxy_mode.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/proxy_outpost_config.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/proxy_provider.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/proxy_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/rac_property_mapping.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/rac_property_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/rac_provider.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/rac_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/radius_outpost_config.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/radius_provider.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/radius_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/redirect_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/redirect_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/reputation.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/reputation_policy.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/reputation_policy_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/resident_key_requirement_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/resident_key_requirement_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/role.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/role.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/role_assigned_object_permission.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/role_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/role_object_permission.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/role_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_metadata.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_property_mapping.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_property_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_provider.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_source.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/saml_source_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/scim_mapping.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/scim_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/scim_provider.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/scim_provider_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/scim_sync_status.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/scim_sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/scope_mapping.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/scope_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/scope_mapping_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/selectable_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/selectable_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/service_connection.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/service_connection_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/service_connection_state.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/service_connection_state.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/session_user.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/session_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/settings.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/settings.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/settings_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/severity_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/severity_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/shell_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/shell_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/signature_algorithm_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/signature_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/sms_device.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/sms_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/sms_device_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/source.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/source_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_write_stage_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,42 +14,35 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from authentik_client.models.policy_engine_mode import PolicyEngineMode
-from authentik_client.models.user_matching_mode_enum import UserMatchingModeEnum
+from authentik_client.models.flow_set_request import FlowSetRequest
+from authentik_client.models.user_creation_mode_enum import UserCreationModeEnum
+from authentik_client.models.user_type_enum import UserTypeEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SourceRequest(BaseModel):
+class UserWriteStageRequest(BaseModel):
     """
-    Source Serializer
+    UserWriteStage Serializer
     """ # noqa: E501
-    name: Annotated[str, Field(min_length=1, strict=True)] = Field(description="Source's display Name.")
-    slug: Annotated[str, Field(min_length=1, strict=True, max_length=50)] = Field(description="Internal source name, used in URLs.")
-    enabled: Optional[StrictBool] = None
-    authentication_flow: Optional[StrictStr] = Field(default=None, description="Flow to use when authenticating existing users.")
-    enrollment_flow: Optional[StrictStr] = Field(default=None, description="Flow to use when enrolling new users.")
-    policy_engine_mode: Optional[PolicyEngineMode] = None
-    user_matching_mode: Optional[UserMatchingModeEnum] = Field(default=None, description="How the source determines if an existing user should be authenticated or a new user enrolled.")
-    user_path_template: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
-    __properties: ClassVar[List[str]] = ["name", "slug", "enabled", "authentication_flow", "enrollment_flow", "policy_engine_mode", "user_matching_mode", "user_path_template"]
-
-    @field_validator('slug')
-    def slug_validate_regular_expression(cls, value):
-        """Validates the regular expression"""
-        if not re.match(r"^[-a-zA-Z0-9_]+$", value):
-            raise ValueError(r"must validate the regular expression /^[-a-zA-Z0-9_]+$/")
-        return value
+    name: Annotated[str, Field(min_length=1, strict=True)]
+    flow_set: Optional[List[FlowSetRequest]] = None
+    user_creation_mode: Optional[UserCreationModeEnum] = None
+    create_users_as_inactive: Optional[StrictBool] = Field(default=None, description="When set, newly created users are inactive and cannot login.")
+    create_users_group: Optional[StrictStr] = Field(default=None, description="Optionally add newly created users to this group.")
+    user_type: Optional[UserTypeEnum] = None
+    user_path_template: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["name", "flow_set", "user_creation_mode", "create_users_as_inactive", "create_users_group", "user_type", "user_path_template"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -61,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SourceRequest from a JSON string"""
+        """Create an instance of UserWriteStageRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,41 +75,42 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if authentication_flow (nullable) is None
+        # override the default output from pydantic by calling `to_dict()` of each item in flow_set (list)
+        _items = []
+        if self.flow_set:
+            for _item in self.flow_set:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['flow_set'] = _items
+        # set to None if create_users_group (nullable) is None
         # and model_fields_set contains the field
-        if self.authentication_flow is None and "authentication_flow" in self.model_fields_set:
-            _dict['authentication_flow'] = None
-
-        # set to None if enrollment_flow (nullable) is None
-        # and model_fields_set contains the field
-        if self.enrollment_flow is None and "enrollment_flow" in self.model_fields_set:
-            _dict['enrollment_flow'] = None
+        if self.create_users_group is None and "create_users_group" in self.model_fields_set:
+            _dict['create_users_group'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SourceRequest from a dict"""
+        """Create an instance of UserWriteStageRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
-            "slug": obj.get("slug"),
-            "enabled": obj.get("enabled"),
-            "authentication_flow": obj.get("authentication_flow"),
-            "enrollment_flow": obj.get("enrollment_flow"),
-            "policy_engine_mode": obj.get("policy_engine_mode"),
-            "user_matching_mode": obj.get("user_matching_mode"),
+            "flow_set": [FlowSetRequest.from_dict(_item) for _item in obj["flow_set"]] if obj.get("flow_set") is not None else None,
+            "user_creation_mode": obj.get("user_creation_mode"),
+            "create_users_as_inactive": obj.get("create_users_as_inactive"),
+            "create_users_group": obj.get("create_users_group"),
+            "user_type": obj.get("user_type"),
             "user_path_template": obj.get("user_path_template")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/source_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/source_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/source_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/source_type.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/source_type.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/sp_binding_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/sp_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/stage_prompt.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/stage_prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/static_device.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/static_device_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/static_device_token.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/static_device_token_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/static_device_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/sub_mode_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/sub_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/system_info.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/system_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/system_info_runtime.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/system_info_runtime.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/system_task.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/system_task.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/system_task_status_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/system_task_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/tenant.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/tenant_admin_group_request_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_admin_group_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/tenant_recovery_key_request_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_recovery_key_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/tenant_recovery_key_response.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_recovery_key_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/tenant_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/token.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/token_model.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/token_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/token_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/token_set_key_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/token_set_key_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/token_view.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/token_view.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/totp_device.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/totp_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/totp_device_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/transaction_application_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/transaction_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/transaction_application_response.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/transaction_application_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/type_create.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/type_create.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/ui_theme_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/ui_theme_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/used_by.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/used_by.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/used_by_action_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/used_by_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_account_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_account_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_assigned_object_permission.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_consent.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_consent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_creation_mode_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_creation_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_delete_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_delete_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_delete_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_fields_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_fields_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_group.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_group_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_login_challenge.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_login_challenge_response_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_login_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_login_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_logout_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_logout_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_logout_stage_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_matching_mode_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_matching_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_metrics.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_o_auth_source_connection.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_o_auth_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_o_auth_source_connection_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_object_permission.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_password_set_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_password_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_path.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_path.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_saml_source_connection.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_saml_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_saml_source_connection_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_self.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_self.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_self_groups.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_self_groups.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_service_account_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_service_account_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_service_account_response.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_service_account_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_setting.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_setting.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_source_connection.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_type_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_verification_enum.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_verification_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/user_write_stage.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/user_write_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/validation_error.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/version.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/version.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/web_authn_device.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/workers.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,29 +14,25 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, ConfigDict, Field, StrictInt
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List
-from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class WebAuthnDevice(BaseModel):
+class Workers(BaseModel):
     """
-    Serializer for WebAuthn authenticator devices
+    Workers
     """ # noqa: E501
-    pk: StrictInt
-    name: Annotated[str, Field(strict=True, max_length=200)]
-    created_on: datetime
-    __properties: ClassVar[List[str]] = ["pk", "name", "created_on"]
+    count: StrictInt
+    __properties: ClassVar[List[str]] = ["count"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -48,51 +44,45 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of WebAuthnDevice from a JSON string"""
+        """Create an instance of Workers from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "pk",
-            "created_on",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of WebAuthnDevice from a dict"""
+        """Create an instance of Workers from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "pk": obj.get("pk"),
-            "name": obj.get("name"),
-            "created_on": obj.get("created_on")
+            "count": obj.get("count")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/web_authn_device_request.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/web_authn_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/models/workers.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/models/paginated_web_authn_device_type_list.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,25 +14,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
+from authentik_client.models.pagination import Pagination
+from authentik_client.models.web_authn_device_type import WebAuthnDeviceType
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Workers(BaseModel):
+class PaginatedWebAuthnDeviceTypeList(BaseModel):
     """
-    Workers
+    PaginatedWebAuthnDeviceTypeList
     """ # noqa: E501
-    count: StrictInt
-    __properties: ClassVar[List[str]] = ["count"]
+    pagination: Pagination
+    results: List[WebAuthnDeviceType]
+    __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Workers from a JSON string"""
+        """Create an instance of PaginatedWebAuthnDeviceTypeList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,24 +68,35 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of pagination
+        if self.pagination:
+            _dict['pagination'] = self.pagination.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in results (list)
+        _items = []
+        if self.results:
+            for _item in self.results:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Workers from a dict"""
+        """Create an instance of PaginatedWebAuthnDeviceTypeList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "count": obj.get("count")
+            "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
+            "results": [WebAuthnDeviceType.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712239192/authentik_client/rest.py` & `authentik_client-2024.2.2.post1712571742/authentik_client/rest.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712239192/pyproject.toml` & `authentik_client-2024.2.2.post1712571742/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "authentik_client"
-version = "2024.2.2-1712239192"
+version = "2024.2.2-1712571742"
 description = "authentik"
 authors = ["authentik Team <hello@goauthentik.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/goauthentik/authentik"
 keywords = ["OpenAPI", "OpenAPI-Generator", "authentik"]
 include = ["authentik_client/py.typed"]
```

### Comparing `authentik_client-2024.2.2.post1712239192/PKG-INFO` & `authentik_client-2024.2.2.post1712571742/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentik_client
-Version: 2024.2.2.post1712239192
+Version: 2024.2.2.post1712571742
 Summary: authentik
 Home-page: https://github.com/goauthentik/authentik
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,authentik
 Author: authentik Team
 Author-email: hello@goauthentik.io
 Requires-Python: >=3.7,<4.0
@@ -25,15 +25,15 @@
 
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.2.2
-- Package version: 2024.2.2-1712239192
+- Package version: 2024.2.2-1712571742
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -700,14 +700,16 @@
 *StagesApi* | [**stages_authenticator_validate_list**](docs/StagesApi.md#stages_authenticator_validate_list) | **GET** /stages/authenticator/validate/ | 
 *StagesApi* | [**stages_authenticator_validate_partial_update**](docs/StagesApi.md#stages_authenticator_validate_partial_update) | **PATCH** /stages/authenticator/validate/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_validate_retrieve**](docs/StagesApi.md#stages_authenticator_validate_retrieve) | **GET** /stages/authenticator/validate/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_validate_update**](docs/StagesApi.md#stages_authenticator_validate_update) | **PUT** /stages/authenticator/validate/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_validate_used_by_list**](docs/StagesApi.md#stages_authenticator_validate_used_by_list) | **GET** /stages/authenticator/validate/{stage_uuid}/used_by/ | 
 *StagesApi* | [**stages_authenticator_webauthn_create**](docs/StagesApi.md#stages_authenticator_webauthn_create) | **POST** /stages/authenticator/webauthn/ | 
 *StagesApi* | [**stages_authenticator_webauthn_destroy**](docs/StagesApi.md#stages_authenticator_webauthn_destroy) | **DELETE** /stages/authenticator/webauthn/{stage_uuid}/ | 
+*StagesApi* | [**stages_authenticator_webauthn_device_types_list**](docs/StagesApi.md#stages_authenticator_webauthn_device_types_list) | **GET** /stages/authenticator/webauthn_device_types/ | 
+*StagesApi* | [**stages_authenticator_webauthn_device_types_retrieve**](docs/StagesApi.md#stages_authenticator_webauthn_device_types_retrieve) | **GET** /stages/authenticator/webauthn_device_types/{aaguid}/ | 
 *StagesApi* | [**stages_authenticator_webauthn_list**](docs/StagesApi.md#stages_authenticator_webauthn_list) | **GET** /stages/authenticator/webauthn/ | 
 *StagesApi* | [**stages_authenticator_webauthn_partial_update**](docs/StagesApi.md#stages_authenticator_webauthn_partial_update) | **PATCH** /stages/authenticator/webauthn/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_webauthn_retrieve**](docs/StagesApi.md#stages_authenticator_webauthn_retrieve) | **GET** /stages/authenticator/webauthn/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_webauthn_update**](docs/StagesApi.md#stages_authenticator_webauthn_update) | **PUT** /stages/authenticator/webauthn/{stage_uuid}/ | 
 *StagesApi* | [**stages_authenticator_webauthn_used_by_list**](docs/StagesApi.md#stages_authenticator_webauthn_used_by_list) | **GET** /stages/authenticator/webauthn/{stage_uuid}/used_by/ | 
 *StagesApi* | [**stages_captcha_create**](docs/StagesApi.md#stages_captcha_create) | **POST** /stages/captcha/ | 
 *StagesApi* | [**stages_captcha_destroy**](docs/StagesApi.md#stages_captcha_destroy) | **DELETE** /stages/captcha/{stage_uuid}/ | 
@@ -846,16 +848,14 @@
  - [AppEnum](docs/AppEnum.md)
  - [AppleChallengeResponseRequest](docs/AppleChallengeResponseRequest.md)
  - [AppleLoginChallenge](docs/AppleLoginChallenge.md)
  - [Application](docs/Application.md)
  - [ApplicationRequest](docs/ApplicationRequest.md)
  - [AuthModeEnum](docs/AuthModeEnum.md)
  - [AuthTypeEnum](docs/AuthTypeEnum.md)
- - [AuthenticateWebAuthnStage](docs/AuthenticateWebAuthnStage.md)
- - [AuthenticateWebAuthnStageRequest](docs/AuthenticateWebAuthnStageRequest.md)
  - [AuthenticatedSession](docs/AuthenticatedSession.md)
  - [AuthenticatedSessionAsn](docs/AuthenticatedSessionAsn.md)
  - [AuthenticatedSessionGeoIp](docs/AuthenticatedSessionGeoIp.md)
  - [AuthenticatedSessionUserAgent](docs/AuthenticatedSessionUserAgent.md)
  - [AuthenticatedSessionUserAgentDevice](docs/AuthenticatedSessionUserAgentDevice.md)
  - [AuthenticatedSessionUserAgentOs](docs/AuthenticatedSessionUserAgentOs.md)
  - [AuthenticatedSessionUserAgentUserAgent](docs/AuthenticatedSessionUserAgentUserAgent.md)
@@ -881,14 +881,16 @@
  - [AuthenticatorTOTPStageRequest](docs/AuthenticatorTOTPStageRequest.md)
  - [AuthenticatorValidateStage](docs/AuthenticatorValidateStage.md)
  - [AuthenticatorValidateStageRequest](docs/AuthenticatorValidateStageRequest.md)
  - [AuthenticatorValidationChallenge](docs/AuthenticatorValidationChallenge.md)
  - [AuthenticatorValidationChallengeResponseRequest](docs/AuthenticatorValidationChallengeResponseRequest.md)
  - [AuthenticatorWebAuthnChallenge](docs/AuthenticatorWebAuthnChallenge.md)
  - [AuthenticatorWebAuthnChallengeResponseRequest](docs/AuthenticatorWebAuthnChallengeResponseRequest.md)
+ - [AuthenticatorWebAuthnStage](docs/AuthenticatorWebAuthnStage.md)
+ - [AuthenticatorWebAuthnStageRequest](docs/AuthenticatorWebAuthnStageRequest.md)
  - [AutoSubmitChallengeResponseRequest](docs/AutoSubmitChallengeResponseRequest.md)
  - [AutosubmitChallenge](docs/AutosubmitChallenge.md)
  - [BackendsEnum](docs/BackendsEnum.md)
  - [BindingTypeEnum](docs/BindingTypeEnum.md)
  - [BlueprintFile](docs/BlueprintFile.md)
  - [BlueprintInstance](docs/BlueprintInstance.md)
  - [BlueprintInstanceRequest](docs/BlueprintInstanceRequest.md)
@@ -1047,21 +1049,21 @@
  - [OpenIDConnectConfiguration](docs/OpenIDConnectConfiguration.md)
  - [Outpost](docs/Outpost.md)
  - [OutpostDefaultConfig](docs/OutpostDefaultConfig.md)
  - [OutpostHealth](docs/OutpostHealth.md)
  - [OutpostRequest](docs/OutpostRequest.md)
  - [OutpostTypeEnum](docs/OutpostTypeEnum.md)
  - [PaginatedApplicationList](docs/PaginatedApplicationList.md)
- - [PaginatedAuthenticateWebAuthnStageList](docs/PaginatedAuthenticateWebAuthnStageList.md)
  - [PaginatedAuthenticatedSessionList](docs/PaginatedAuthenticatedSessionList.md)
  - [PaginatedAuthenticatorDuoStageList](docs/PaginatedAuthenticatorDuoStageList.md)
  - [PaginatedAuthenticatorSMSStageList](docs/PaginatedAuthenticatorSMSStageList.md)
  - [PaginatedAuthenticatorStaticStageList](docs/PaginatedAuthenticatorStaticStageList.md)
  - [PaginatedAuthenticatorTOTPStageList](docs/PaginatedAuthenticatorTOTPStageList.md)
  - [PaginatedAuthenticatorValidateStageList](docs/PaginatedAuthenticatorValidateStageList.md)
+ - [PaginatedAuthenticatorWebAuthnStageList](docs/PaginatedAuthenticatorWebAuthnStageList.md)
  - [PaginatedBlueprintInstanceList](docs/PaginatedBlueprintInstanceList.md)
  - [PaginatedBrandList](docs/PaginatedBrandList.md)
  - [PaginatedCaptchaStageList](docs/PaginatedCaptchaStageList.md)
  - [PaginatedCertificateKeyPairList](docs/PaginatedCertificateKeyPairList.md)
  - [PaginatedConnectionTokenList](docs/PaginatedConnectionTokenList.md)
  - [PaginatedConsentStageList](docs/PaginatedConsentStageList.md)
  - [PaginatedDenyStageList](docs/PaginatedDenyStageList.md)
@@ -1143,30 +1145,31 @@
  - [PaginatedUserLoginStageList](docs/PaginatedUserLoginStageList.md)
  - [PaginatedUserLogoutStageList](docs/PaginatedUserLogoutStageList.md)
  - [PaginatedUserOAuthSourceConnectionList](docs/PaginatedUserOAuthSourceConnectionList.md)
  - [PaginatedUserSAMLSourceConnectionList](docs/PaginatedUserSAMLSourceConnectionList.md)
  - [PaginatedUserSourceConnectionList](docs/PaginatedUserSourceConnectionList.md)
  - [PaginatedUserWriteStageList](docs/PaginatedUserWriteStageList.md)
  - [PaginatedWebAuthnDeviceList](docs/PaginatedWebAuthnDeviceList.md)
+ - [PaginatedWebAuthnDeviceTypeList](docs/PaginatedWebAuthnDeviceTypeList.md)
  - [Pagination](docs/Pagination.md)
  - [PasswordChallenge](docs/PasswordChallenge.md)
  - [PasswordChallengeResponseRequest](docs/PasswordChallengeResponseRequest.md)
  - [PasswordExpiryPolicy](docs/PasswordExpiryPolicy.md)
  - [PasswordExpiryPolicyRequest](docs/PasswordExpiryPolicyRequest.md)
  - [PasswordPolicy](docs/PasswordPolicy.md)
  - [PasswordPolicyRequest](docs/PasswordPolicyRequest.md)
  - [PasswordStage](docs/PasswordStage.md)
  - [PasswordStageRequest](docs/PasswordStageRequest.md)
  - [PatchedApplicationRequest](docs/PatchedApplicationRequest.md)
- - [PatchedAuthenticateWebAuthnStageRequest](docs/PatchedAuthenticateWebAuthnStageRequest.md)
  - [PatchedAuthenticatorDuoStageRequest](docs/PatchedAuthenticatorDuoStageRequest.md)
  - [PatchedAuthenticatorSMSStageRequest](docs/PatchedAuthenticatorSMSStageRequest.md)
  - [PatchedAuthenticatorStaticStageRequest](docs/PatchedAuthenticatorStaticStageRequest.md)
  - [PatchedAuthenticatorTOTPStageRequest](docs/PatchedAuthenticatorTOTPStageRequest.md)
  - [PatchedAuthenticatorValidateStageRequest](docs/PatchedAuthenticatorValidateStageRequest.md)
+ - [PatchedAuthenticatorWebAuthnStageRequest](docs/PatchedAuthenticatorWebAuthnStageRequest.md)
  - [PatchedBlueprintInstanceRequest](docs/PatchedBlueprintInstanceRequest.md)
  - [PatchedBrandRequest](docs/PatchedBrandRequest.md)
  - [PatchedCaptchaStageRequest](docs/PatchedCaptchaStageRequest.md)
  - [PatchedCertificateKeyPairRequest](docs/PatchedCertificateKeyPairRequest.md)
  - [PatchedConnectionTokenRequest](docs/PatchedConnectionTokenRequest.md)
  - [PatchedConsentStageRequest](docs/PatchedConsentStageRequest.md)
  - [PatchedDenyStageRequest](docs/PatchedDenyStageRequest.md)
@@ -1384,14 +1387,16 @@
  - [UserVerificationEnum](docs/UserVerificationEnum.md)
  - [UserWriteStage](docs/UserWriteStage.md)
  - [UserWriteStageRequest](docs/UserWriteStageRequest.md)
  - [ValidationError](docs/ValidationError.md)
  - [Version](docs/Version.md)
  - [WebAuthnDevice](docs/WebAuthnDevice.md)
  - [WebAuthnDeviceRequest](docs/WebAuthnDeviceRequest.md)
+ - [WebAuthnDeviceType](docs/WebAuthnDeviceType.md)
+ - [WebAuthnDeviceTypeRequest](docs/WebAuthnDeviceTypeRequest.md)
  - [Workers](docs/Workers.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
```

