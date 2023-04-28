# Comparing `tmp/pyspnego-0.8.0.tar.gz` & `tmp/pyspnego-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspnego-0.8.0.tar", last modified: Thu Feb 16 20:19:21 2023, max compression
+gzip compressed data, was "pyspnego-0.9.0.tar", last modified: Fri Apr 28 22:32:32 2023, max compression
```

## Comparing `pyspnego-0.8.0.tar` & `pyspnego-0.9.0.tar`

### file list

```diff
@@ -1,143 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.306394 pyspnego-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-02-16 20:19:12.000000 pyspnego-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-16 20:19:12.000000 pyspnego-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-16 20:19:12.000000 pyspnego-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-02-16 20:19:21.306394 pyspnego-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-02-16 20:19:12.000000 pyspnego-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.294394 pyspnego-0.8.0/build_helpers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2768 2023-02-16 20:19:12.000000 pyspnego-0.8.0/build_helpers/lib.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-02-16 20:19:12.000000 pyspnego-0.8.0/build_helpers/run-ci.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-02-16 20:19:12.000000 pyspnego-0.8.0/build_helpers/run-container.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-02-16 20:19:12.000000 pyspnego-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-16 20:19:12.000000 pyspnego-0.8.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 20:19:21.306394 pyspnego-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-02-16 20:19:12.000000 pyspnego-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.290394 pyspnego-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.294394 pyspnego-0.8.0/src/pyspnego.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-02-16 20:19:21.000000 pyspnego-0.8.0/src/pyspnego.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-02-16 20:19:21.000000 pyspnego-0.8.0/src/pyspnego.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 20:19:21.000000 pyspnego-0.8.0/src/pyspnego.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-16 20:19:21.000000 pyspnego-0.8.0/src/pyspnego.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-16 20:19:21.000000 pyspnego-0.8.0/src/pyspnego.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-16 20:19:21.000000 pyspnego-0.8.0/src/pyspnego.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.298394 pyspnego-0.8.0/src/spnego/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33393 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)    33191 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    25805 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_credssp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_credssp_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    23536 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_gss.py
--rw-r--r--   0 runner    (1001) docker     (123)    56199 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_kerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_negotiate.py
--rw-r--r--   0 runner    (1001) docker     (123)    31171 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_ntlm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.298394 pyspnego-0.8.0/src/spnego/_ntlm_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_ntlm_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19800 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_ntlm_raw/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    21201 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_ntlm_raw/des.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_ntlm_raw/md4.py
--rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_ntlm_raw/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_ntlm_raw/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    19451 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_spnego.py
--rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_sspi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.298394 pyspnego-0.8.0/src/spnego/_sspi_raw/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_sspi_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_sspi_raw/security.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_sspi_raw/sspi.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_sspi_raw/sspi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25416 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_sspi_raw/sspi.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_sspi_raw/text.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_sspi_raw/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_sspi_raw/text.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_sspi_raw/windows.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    32305 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_tls_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/channel_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15133 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/gss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/iov.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/negotiate.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/ntlm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/sspi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-02-16 20:19:12.000000 pyspnego-0.8.0/src/spnego/tls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.302394 pyspnego-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.302394 pyspnego-0.8.0/tests/_ntlm_raw/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/_ntlm_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/_ntlm_raw/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/_ntlm_raw/test_des.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/_ntlm_raw/test_md4.py
--rw-r--r--   0 runner    (1001) docker     (123)    46406 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/_ntlm_raw/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/_ntlm_raw/test_security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.302394 pyspnego-0.8.0/tests/_sspi_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/_sspi_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/_sspi_raw/test_sspi.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/_sspi_raw/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.306394 pyspnego-0.8.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/credssp_ts_credential_password
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/credssp_ts_credential_remote_guard_empty_supplemental
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/credssp_ts_credential_remote_guard_multiple
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/credssp_ts_credential_remote_guard_no_supplemental
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/credssp_ts_credential_smart_card
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/credssp_ts_credential_smart_card_full
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/credssp_ts_remote_guard_ms_example
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/credssp_ts_request
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/initial_context_token_krb_ap_rep
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/initial_context_token_krb_ap_req
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/initial_context_token_neg_token_init
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/initial_context_token_neg_token_init2
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/krb_as_rep
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/krb_as_req
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/krb_error
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/krb_tgs_rep
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/krb_tgs_req
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/neg_token_resp
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/ntlm_authenticate
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/ntlm_authenticate_no_sign_seal
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/ntlm_challenge
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/ntlm_negotiate
--rw-r--r--   0 runner    (1001) docker     (123)    42066 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/pyspnego.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/tls1.0_client_hello
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/tls1.0_server_hello
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/tls1.1_client_hello
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/tls1.1_server_hello
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/tls1.2_client_hello
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/tls1.2_client_key_exchange
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/tls1.2_server_hello
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/tls1.3_client_hello
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/data/tls1.3_server_hello
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.306394 pyspnego-0.8.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/integration/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/integration/Vagrantfile
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/integration/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/integration/inventory.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/integration/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:19:21.306394 pyspnego-0.8.0/tests/integration/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/integration/templates/generate_cert.sh.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/integration/templates/krb5.conf.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)    35053 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/integration/templates/test_integration.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/integration/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)    66243 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_channel_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_credssp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_credssp_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_gss.py
--rw-r--r--   0 runner    (1001) docker     (123)    29749 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_kerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)    58560 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_negotiate.py
--rw-r--r--   0 runner    (1001) docker     (123)    20715 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_ntlm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_spnego.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_sspi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-02-16 20:19:12.000000 pyspnego-0.8.0/tests/test_tls_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.927079 pyspnego-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-04-28 22:32:25.000000 pyspnego-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 22:32:25.000000 pyspnego-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 22:32:25.000000 pyspnego-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-28 22:32:32.927079 pyspnego-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-28 22:32:25.000000 pyspnego-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.907079 pyspnego-0.9.0/build_helpers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2768 2023-04-28 22:32:25.000000 pyspnego-0.9.0/build_helpers/lib.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-04-28 22:32:25.000000 pyspnego-0.9.0/build_helpers/run-ci.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-04-28 22:32:25.000000 pyspnego-0.9.0/build_helpers/run-container.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-28 22:32:25.000000 pyspnego-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-28 22:32:25.000000 pyspnego-0.9.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:32:32.927079 pyspnego-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-28 22:32:25.000000 pyspnego-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.903079 pyspnego-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.907079 pyspnego-0.9.0/src/pyspnego.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.911079 pyspnego-0.9.0/src/spnego/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33434 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34578 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26302 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_credssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_credssp_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24467 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_gss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56199 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_kerberos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18885 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_negotiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36954 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.911079 pyspnego-0.9.0/src/spnego/_ntlm_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19800 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21201 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/md4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19451 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_spnego.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18586 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.915079 pyspnego-0.9.0/src/spnego/_sspi_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/security.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25487 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/text.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/text.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/windows.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32305 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_tls_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/channel_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/gss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/iov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/negotiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/ntlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/sspi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/tls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.915079 pyspnego-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.919079 pyspnego-0.9.0/tests/_ntlm_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/test_md4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46406 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/test_security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.919079 pyspnego-0.9.0/tests/_sspi_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_sspi_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_sspi_raw/test_sspi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_sspi_raw/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.923079 pyspnego-0.9.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_password
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_remote_guard_empty_supplemental
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_remote_guard_multiple
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_remote_guard_no_supplemental
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_smart_card
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_smart_card_full
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_remote_guard_ms_example
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_request
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/initial_context_token_krb_ap_rep
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/initial_context_token_krb_ap_req
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/initial_context_token_neg_token_init
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/initial_context_token_neg_token_init2
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/krb_as_rep
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/krb_as_req
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/krb_error
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/krb_tgs_rep
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/krb_tgs_req
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/neg_token_resp
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/ntlm_authenticate
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/ntlm_authenticate_no_sign_seal
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/ntlm_challenge
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/ntlm_negotiate
+-rw-r--r--   0 runner    (1001) docker     (123)    42066 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/pyspnego.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.0_client_hello
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.0_server_hello
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.1_client_hello
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.1_server_hello
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.2_client_hello
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.2_client_key_exchange
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.2_server_hello
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.3_client_hello
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.3_server_hello
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.923079 pyspnego-0.9.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/Vagrantfile
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/inventory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.923079 pyspnego-0.9.0/tests/integration/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/templates/generate_cert.sh.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/templates/krb5.conf.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)    60904 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/templates/test_integration.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66365 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_auth_dce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_channel_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_credssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_credssp_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_gss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29749 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_kerberos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58565 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_negotiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30784 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_ntlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_spnego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_sspi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_tls_struct.py
```

### Comparing `pyspnego-0.8.0/CHANGELOG.md` & `pyspnego-0.9.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,42 @@
 # Changelog
 
+## 0.9.0 - 2023-04-29
+
+* Added the `spnego.ContextReq.dce_style` flag to enable DCE authentication mode
+  * This is used in protocols like RPC/DCE
+* The value for `spnego.iov.BufferType.sign_only` on SSPI has changed from representing `SECBUFFER_MECHLIST` to `SECBUFFER_READONLY_WITH_CHECKSUM`
+  * This is to better match what `sign_only` means when using it with GSSAPI
+  * It is needed to support RPC encryption and signature headers on SSPI
+  * The use of `SECBUFFER_MECHLIST` is not seen in any examples in the wild and is most likely an internal flag
+* Added the IOV buffer type `spnego.iov.BufferType.data_readonly`
+  * For SSPI this corresponds to `SECBUFFER_DATA | SECBUFFER_READONLY`
+  * For GSSAPI this corresponds to `GSS_IOV_BUFFER_TYPE_EMPTY`
+  * As GSSAPI has no actual equivalent to this the empty buffer type is used which in testing results in compatible buffers
+  * This is used for DCE/RPC wrapping when the PDU header and sec trailer are not signed but are included in the wrap_iov buffers.
+* Added limited support for `wrap_iov` and `unwrap_iov` in the Python NTLM context provider.
+  * This currently only supports `spnego.iov.BufferType.header`, `spnego.iov.BufferType.data`, `spnego.iov.BufferType.sign_only`, `spnego.iov.BufferType.data_readonly`, and `spnego.iov.BufferType.stream`
+  * `header`
+    * `wrap_iov`: Used to place the resulting signature in the buffer
+    * `unwrap_iov`: Used as the signature source for validation
+  * `data`
+    * `wrap_iov`: Data to be encrypted/sealed
+    * `unwrap_iov`: Data to be decrypted/unsealed
+  * `sign_only`
+    * `wrap_iov`: Data to be included in the signature/header generation
+    * `unwrap_iov`: Data to be included in the signature/header verification
+  * `data_readonly` is treated the same as `sign_only`
+  * `stream`
+    * `wrap_iov`: Not supported
+    * `unwrap_iov`: Contains the full value to decrypt with the headers in the beginning, must be coupled with a subsequent data buffer of the type `data` to place the decrypted value into
+  * The behaviour used here is modelled as closely as possible to how `SSPI` works but not all the permutations have been tested.
+  * The header/signature will be generated from the `data`, `sign_only`, `data_readonly` values concat together in the order they are provided.
+* Added the `query_message_sizes()` function on a context to retrieve the important message sizes
+  * Currently this only contains the size of the message `header`, also known as the signature or security trailer
+
 ## 0.8.0 - 2023-02-17
 
 * Added the `spnego.ContextReq.no_integrity` flag to disable integrity/confidentiality on Kerberos/Negotiate contexts
   * This is used by authentication contexts that need to disable integrity/confidentiality explicitly
   * An example would be the LDAP SASL `GSS-SPNEGO` where the context flags control the SSF flags
 * Added optional kwargs to `step()` on a security context `channel_bindings`
   * This can be used to supply the channel bindings when performing a context step rather than when creating the context
```

### Comparing `pyspnego-0.8.0/LICENSE` & `pyspnego-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/PKG-INFO` & `pyspnego-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspnego
-Version: 0.8.0
+Version: 0.9.0
 Summary: Windows Negotiate Authentication Client and Server
 Author-email: Jordan Borean <jborean93@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Jordan Borean, Red Hat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyspnego-0.8.0/README.md` & `pyspnego-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/build_helpers/lib.sh` & `pyspnego-0.9.0/build_helpers/lib.sh`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/build_helpers/run-container.sh` & `pyspnego-0.9.0/build_helpers/run-container.sh`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/pyproject.toml` & `pyspnego-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/setup.py` & `pyspnego-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/pyspnego.egg-info/PKG-INFO` & `pyspnego-0.9.0/src/pyspnego.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspnego
-Version: 0.8.0
+Version: 0.9.0
 Summary: Windows Negotiate Authentication Client and Server
 Author-email: Jordan Borean <jborean93@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Jordan Borean, Red Hat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyspnego-0.8.0/src/pyspnego.egg-info/SOURCES.txt` & `pyspnego-0.9.0/src/pyspnego.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 src/spnego/_sspi_raw/text.pyi
 src/spnego/_sspi_raw/text.pyx
 src/spnego/_sspi_raw/windows.pxd
 tests/__init__.py
 tests/conftest.py
 tests/test_asn1.py
 tests/test_auth.py
+tests/test_auth_dce.py
 tests/test_channel_bindings.py
 tests/test_context.py
 tests/test_credssp.py
 tests/test_credssp_structures.py
 tests/test_deprecation.py
 tests/test_exceptions.py
 tests/test_gss.py
```

### Comparing `pyspnego-0.8.0/src/spnego/__init__.py` & `pyspnego-0.9.0/src/spnego/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/__main__.py` & `pyspnego-0.9.0/src/spnego/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,24 +58,30 @@
     TlsProtocolVersion,
     TlsPskKeyExchangeMode,
     TlsServerNameType,
     TlsSignatureScheme,
     TlsSupportedGroup,
 )
 
+HAS_ARGCOMPLETE = False
 try:
     import argcomplete
+
+    HAS_ARGCOMPLETE = True
 except ImportError:  # pragma: nocover
-    argcomplete = None
+    pass
+
 
-yaml: typing.Optional[typing.Any]
+HAS_YAML = False
 try:
     from ruamel import yaml
+
+    HAS_YAML = True
 except ImportError:  # pragma: nocover
-    yaml = None
+    pass
 
 
 def _parse_ntlm_version(
     version: typing.Optional[Version],
 ) -> typing.Optional[typing.Dict[str, typing.Union[int, str]]]:
     if not version:
         return None
@@ -696,16 +702,16 @@
 
     token_info: typing.Union[typing.List, typing.Dict]
     if re.match(b"[\x00|\x14|\x15|\x16|\x17]\x03[\x01|\x02|\x03]", b_data):
         token_info = parse_tls_token(b_data)
     else:
         token_info = parse_token(b_data, secret=parsed_args.secret, encoding=parsed_args.encoding)
 
-    if parsed_args.output_format == "yaml":
-        y = yaml.YAML()  # type: ignore
+    if parsed_args.output_format == "yaml" and HAS_YAML:
+        y = yaml.YAML()
         y.default_flow_style = False
         y.dump(token_info, sys.stdout)
     else:
         print(json.dumps(token_info, indent=4))
 
 
 def parse_args(args: typing.List[str]) -> argparse.Namespace:
@@ -751,20 +757,20 @@
         dest="secret",
         default=None,
         help="Optional info that is the secret information for a protocol that can be used to decrypt encrypted "
         "fields and/or derive the unique session key in the exchange. This is currently only supported by NTLM "
         "tokens to generate the session key.",
     )
 
-    if argcomplete:
+    if HAS_ARGCOMPLETE:
         argcomplete.autocomplete(parser)
 
     parsed_args = parser.parse_args(args)
 
-    if parsed_args.output_format == "yaml" and not yaml:
+    if parsed_args.output_format == "yaml" and not HAS_YAML:
         raise ValueError("Cannot output as yaml as ruamel.yaml is not installed.")
 
     return parsed_args
 
 
 def parse_token(
     b_data: bytes,
```

### Comparing `pyspnego-0.8.0/src/spnego/_asn1.py` & `pyspnego-0.9.0/src/spnego/_asn1.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_context.py` & `pyspnego-0.9.0/src/spnego/_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright: (c) 2020, Jordan Borean (@jborean93) <jborean93@gmail.com>
 # MIT License (see LICENSE or https://opensource.org/licenses/MIT)
 
 import abc
+import dataclasses
 import enum
 import typing
 import warnings
 
 from spnego._credential import Credential
 from spnego._text import to_text
 from spnego.channel_bindings import GssChannelBindings
@@ -108,25 +109,47 @@
     """Result of the `unwrap_iov()` function."""
 
     buffers: typing.Tuple[IOVResBuffer, ...]  #: The unwrapped IOV buffers.
     encrypted: bool  #: Whether the input buffers were encrypted (True) or not (False)
     qop: int  #: The Quality of Protection used for the encrypted buffers.
 
 
+@dataclasses.dataclass(frozen=True)
+class SecPkgContextSizes:
+    """Sizes of important structures used for messages.
+
+    This dataclass exposes the sizes of important structures used in message
+    support functions like wrap, wrap_iov, sign, etc. Use
+    :meth:`ContextReq.query_message_sizes` to retrieve this value for an
+    authenticated context.
+
+    Currently only ``header`` is exposed but other sizes may be added in the
+    future if needed.
+
+    Attributes:
+        header: The size of the header/signature of a wrapped token. This
+            corresponds to cbSecurityTrailer in SecPkgContext_Sizes in SSPI and
+            the size of the allocated GSS_IOV_BUFFER_TYPE_HEADER IOV buffer.
+    """
+
+    header: int
+
+
 class ContextReq(enum.IntFlag):
     none = 0x00000000
 
     # GSSAPI|SSPI flags
     delegate = 0x00000001
     mutual_auth = 0x00000002
     replay_detect = 0x00000004
     sequence_detect = 0x00000008
     confidentiality = 0x00000010
     integrity = 0x00000020
     # anonymous = 0x00000040  # TODO: Add support for anonymous auth.
+    dce_style = 0x00001000
     identify = 0x00002000
     # Requires newer python-gssapi version to support https://github.com/pythongssapi/python-gssapi/pull/218
     delegate_policy = 0x00080000
 
     # Special flag that disables integrity/confidentiality on Kerberos/Negotiate
     # This should not be set with integrity or confidentiality.
     no_integrity = 0x10000000
@@ -404,14 +427,30 @@
 
         Returns:
             ContextProxy: The new security context.
         """
         pass  # pragma: no cover
 
     @abc.abstractmethod
+    def query_message_sizes(self) -> SecPkgContextSizes:
+        """Gets the important structure sizes for message functions.
+
+        Will get the important sizes for the various message functions used by
+        the current authentication context. This must only be called once the
+        context has been authenticated.
+
+        Returns:
+            SecPkgContextSizes: The sizes for the current context.
+
+        Raises:
+            NoContextError: The security context is not ready to be queried.
+        """
+        pass  # pragma: no cover
+
+    @abc.abstractmethod
     def step(
         self,
         in_token: typing.Optional[bytes] = None,
         *,
         channel_bindings: typing.Optional[GssChannelBindings] = None,
     ) -> typing.Optional[bytes]:
         """Performs a negotiation step.
```

### Comparing `pyspnego-0.8.0/src/spnego/_credential.py` & `pyspnego-0.9.0/src/spnego/_credential.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_credssp.py` & `pyspnego-0.9.0/src/spnego/_credssp.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import spnego
 from spnego._context import (
     IOV,
     ContextProxy,
     ContextReq,
     IOVUnwrapResult,
     IOVWrapResult,
+    SecPkgContextSizes,
     UnwrapResult,
     WinRMWrapResult,
     WrapResult,
     split_username,
 )
 from spnego._credential import Credential, Password, unify_credentials
 from spnego._credssp_structures import (
@@ -36,14 +37,15 @@
 from spnego.exceptions import (
     BadBindingsError,
     ErrorCode,
     FeatureMissingError,
     InvalidTokenError,
     NativeError,
     NegotiateOptions,
+    NoContextError,
     OperationNotAvailableError,
     SpnegoError,
 )
 from spnego.tls import (
     CredSSPTLSContext,
     default_tls_context,
     generate_tls_certificate,
@@ -592,14 +594,23 @@
 
         elif name == "protocol_version" and self._selected_version is not None:
             return self._selected_version
 
         else:
             return default
 
+    def query_message_sizes(self) -> SecPkgContextSizes:
+        if not self._tls_object or not self.complete:
+            raise NoContextError(context_msg="Cannot get message sizes until context has been established")
+
+        cipher_negotiated, tls_protocol, _ = self._tls_object.cipher()  # type: ignore[misc]
+        trailer_length = _tls_trailer_length(0, tls_protocol, cipher_negotiated)
+
+        return SecPkgContextSizes(header=trailer_length)
+
     @_wrap_ssl_error("Invalid TLS state when wrapping data")
     def wrap(self, data: bytes, encrypt: bool = True, qop: typing.Optional[int] = None) -> WrapResult:
         self._tls_object.write(data)
         return WrapResult(data=self._out_buff.read(), encrypted=True)
 
     def wrap_iov(
         self,
```

### Comparing `pyspnego-0.8.0/src/spnego/_credssp_structures.py` & `pyspnego-0.9.0/src/spnego/_credssp_structures.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_gss.py` & `pyspnego-0.9.0/src/spnego/_gss.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from spnego._context import (
     IOV,
     ContextProxy,
     ContextReq,
     GSSMech,
     IOVUnwrapResult,
     IOVWrapResult,
+    SecPkgContextSizes,
     UnwrapResult,
     WinRMWrapResult,
     WrapResult,
     wrap_system_error,
 )
 from spnego._credential import (
     Credential,
@@ -55,15 +56,15 @@
 
 
 HAS_IOV = True
 GSSAPI_IOV_IMP_ERR = None
 try:
     from gssapi.raw import IOV as GSSIOV
     from gssapi.raw import IOVBuffer as GSSIOVBuffer
-    from gssapi.raw import IOVBufferType, unwrap_iov, wrap_iov
+    from gssapi.raw import IOVBufferType, unwrap_iov, wrap_iov, wrap_iov_length
 except ImportError as err:
     GSSAPI_IOV_IMP_ERR = sys.exc_info()
     HAS_IOV = False
     log.debug("Python gssapi IOV extension not available: %s" % str(GSSAPI_IOV_IMP_ERR[1]))
 
 _GSS_C_INQ_SSPI_SESSION_KEY = "1.2.840.113554.1.2.2.5.5"
 
@@ -440,14 +441,27 @@
                 raise
 
         if not self._is_wrapped:
             log.debug("GSSAPI step output: %s", base64.b64encode(out_token or b"").decode())
 
         return out_token
 
+    @wrap_system_error(NativeError, "Getting context sizes")
+    def query_message_sizes(self) -> SecPkgContextSizes:
+        if not self._context:
+            raise NoContextError(context_msg="Cannot get message sizes until context has been established")
+
+        iov = GSSIOV(
+            IOVBufferType.header,
+            b"",
+            std_layout=False,
+        )
+        wrap_iov_length(self._context, iov)
+        return SecPkgContextSizes(header=len(iov[0].value or b""))
+
     @wrap_system_error(NativeError, "Wrapping data")
     def wrap(self, data: bytes, encrypt: bool = True, qop: typing.Optional[int] = None) -> WrapResult:
         if not self._context:
             raise NoContextError(context_msg="Cannot wrap until context has been established")
         res = gssapi.raw.wrap(self._context, data, confidential=encrypt, qop=qop)
 
         return WrapResult(data=res.message, encrypted=res.encrypted)
@@ -540,14 +554,15 @@
         attr_map = [
             (ContextReq.delegate, "delegate_to_peer"),
             (ContextReq.mutual_auth, "mutual_authentication"),
             (ContextReq.replay_detect, "replay_detection"),
             (ContextReq.sequence_detect, "out_of_sequence_detection"),
             (ContextReq.confidentiality, "confidentiality"),
             (ContextReq.integrity, "integrity"),
+            (ContextReq.dce_style, "dce_style"),
             # Only present when the DCE extensions are installed.
             (ContextReq.identify, "identify"),
             # Only present with newer versions of python-gssapi https://github.com/pythongssapi/python-gssapi/pull/218.
             (ContextReq.delegate_policy, "ok_as_delegate"),
         ]
         attrs = []
         for spnego_flag, gssapi_name in attr_map:
@@ -567,8 +582,15 @@
         elif isinstance(buffer.data, int):
             # This shouldn't really occur on GSSAPI but is here to mirror what SSPI does.
             buffer_data = b"\x00" * buffer.data
         else:
             auto_alloc = [BufferType.header, BufferType.padding, BufferType.trailer]
             buffer_alloc = buffer.type in auto_alloc
 
-        return GSSIOVBuffer(IOVBufferType(buffer.type), buffer_alloc, buffer_data)
+        buffer_type = buffer.type
+        if buffer.type == BufferType.data_readonly:
+            # GSSAPI doesn't have the SSPI equivalent of SECBUFFER_READONLY.
+            # the GSS_IOV_BUFFER_TYPE_EMPTY seems to produce the same behaviour
+            # so that's going to be used instead.
+            buffer_type = BufferType.empty
+
+        return GSSIOVBuffer(IOVBufferType(buffer_type), buffer_alloc, buffer_data)
```

### Comparing `pyspnego-0.8.0/src/spnego/_kerberos.py` & `pyspnego-0.9.0/src/spnego/_kerberos.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_negotiate.py` & `pyspnego-0.9.0/src/spnego/_negotiate.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from spnego._context import (
     IOV,
     ContextProxy,
     ContextReq,
     GSSMech,
     IOVUnwrapResult,
     IOVWrapResult,
+    SecPkgContextSizes,
     UnwrapResult,
     WinRMWrapResult,
     WrapResult,
 )
 from spnego._credential import Credential, unify_credentials
 from spnego._gss import GSSAPIProxy
 from spnego._spnego import (
@@ -25,15 +26,20 @@
     NegTokenInit,
     NegTokenResp,
     pack_mech_type_list,
     unpack_token,
 )
 from spnego._sspi import SSPIProxy
 from spnego.channel_bindings import GssChannelBindings
-from spnego.exceptions import BadMechanismError, InvalidTokenError, NegotiateOptions
+from spnego.exceptions import (
+    BadMechanismError,
+    InvalidTokenError,
+    NegotiateOptions,
+    NoContextError,
+)
 
 log = logging.getLogger(__name__)
 
 
 class NegotiateProxy(ContextProxy):
     """A context wrapper for a Python managed SPNEGO context.
 
@@ -69,15 +75,16 @@
         self.__chosen_mech: typing.Optional[GSSMech] = None
         self._mech_list: typing.List[str] = []
 
         self._init_sent = False
         self._mech_sent = False
         self._mic_sent = False
         self._mic_recv = False
-        self._mic_required = False
+        # DCE will always send a MIC token, even for Kerberos.
+        self._mic_required = bool(self.context_req & ContextReq.dce_style)
 
     @classmethod
     def available_protocols(cls, options: typing.Optional[NegotiateOptions] = None) -> typing.List[str]:
         # We always support Negotiate and NTLM as we have our builtin NTLM backend and only support kerberos if gssapi
         # is present.
         protocols = ["ntlm", "negotiate"]
 
@@ -342,14 +349,20 @@
 
             final_token = NegTokenResp(
                 neg_state=state, supported_mech=supported_mech, response_token=out_token, mech_list_mic=out_mic
             ).pack()
 
         return final_token
 
+    def query_message_sizes(self) -> SecPkgContextSizes:
+        if not self.complete:
+            raise NoContextError(context_msg="Cannot get message sizes until context has been established")
+
+        return self._context.query_message_sizes()
+
     def wrap(self, data: bytes, encrypt: bool = True, qop: typing.Optional[int] = None) -> WrapResult:
         return self._context.wrap(data, encrypt=encrypt, qop=qop)
 
     def wrap_iov(
         self,
         iov: typing.Iterable[IOV],
         encrypt: bool = True,
```

### Comparing `pyspnego-0.8.0/src/spnego/_ntlm.py` & `pyspnego-0.9.0/src/spnego/_ntlm.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from spnego._context import (
     IOV,
     ContextProxy,
     ContextReq,
     IOVUnwrapResult,
     IOVWrapResult,
+    SecPkgContextSizes,
     UnwrapResult,
     WinRMWrapResult,
     WrapResult,
     split_username,
 )
 from spnego._credential import (
     Credential,
@@ -61,14 +62,15 @@
     InvalidTokenError,
     NegotiateOptions,
     NoContextError,
     OperationNotAvailableError,
     SpnegoError,
     UnsupportedQop,
 )
+from spnego.iov import BufferType, IOVResBuffer
 
 log = logging.getLogger(__name__)
 
 
 def _get_credential_file() -> typing.Optional[str]:
     """Get the path to the NTLM credential store.
 
@@ -322,15 +324,15 @@
 
     @classmethod
     def available_protocols(cls, options: typing.Optional[NegotiateOptions] = None) -> typing.List[str]:
         return ["ntlm"]
 
     @classmethod
     def iov_available(cls) -> bool:
-        return False
+        return True
 
     @property
     def client_principal(self) -> typing.Optional[str]:
         if self.usage == "accept" and self.complete and self._credential:
             domain_part = self._credential.domain + "\\" if self._credential.domain else ""
             return "%s%s" % (domain_part, self._credential.username)
 
@@ -388,14 +390,17 @@
         if self._complete:
             # Clear out any temp data we still have stored.
             self._temp_negotiate = None
             self._temp_challenge = None
 
             in_usage = "accept" if self.usage == "initiate" else "initiate"
             session_key = self._session_key or b""
+            # if tmp_key := os.environ.get("TESTING", None):
+            #     session_key = self._session_key = base64.b16decode(tmp_key)
+
             self._sign_key_out = signkey(self._context_attr, session_key, self.usage)
             self._sign_key_in = signkey(self._context_attr, session_key, in_usage)
 
             # Found a vague reference in MS-NLMP that states if NTLMv2 authentication was not used then only 1 key is
             # used for sealing. This seems to reference when NTLMSSP_NEGOTIATE_EXTENDED_SESSION_SECURITY is not set and
             # not NTLMv2 messages itself.
             # https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-nlmp/d1c86e81-eb66-47fd-8a6f-970050121347
@@ -612,14 +617,20 @@
 
             if actual_mic != expected_mic:
                 raise InvalidTokenError(context_msg="Invalid MIC in NTLM authentication message")
 
         self._context_attr = auth.flags
         self._complete = True
 
+    def query_message_sizes(self) -> SecPkgContextSizes:
+        if not self.complete:
+            raise NoContextError(context_msg="Cannot get message sizes until context has been established")
+
+        return SecPkgContextSizes(header=16)
+
     def wrap(self, data: bytes, encrypt: bool = True, qop: typing.Optional[int] = None) -> WrapResult:
         if qop:
             raise UnsupportedQop(context_msg="Unsupported QoP value %s specified for NTLM" % qop)
 
         if self.context_attr & ContextReq.integrity == 0 and self.context_attr & ContextReq.confidentiality == 0:
             raise OperationNotAvailableError(context_msg="NTLM wrap without integrity or confidentiality")
 
@@ -638,18 +649,81 @@
 
     def wrap_iov(
         self,
         iov: typing.Iterable[IOV],
         encrypt: bool = True,
         qop: typing.Optional[int] = None,
     ) -> IOVWrapResult:
-        # While this technically works on SSPI by passing multiple data buffers we can achieve the same thing with
-        # wrap. Because this context proxy is meant to replicate gss-ntlmssp which doesn't support IOV in NTLM we just
-        # fail here.
-        raise OperationNotAvailableError(context_msg="NTLM does not offer IOV wrapping")
+        if qop:
+            raise UnsupportedQop(context_msg="Unsupported QoP value %s specified for NTLM" % qop)
+
+        if self.context_attr & ContextReq.integrity == 0 and self.context_attr & ContextReq.confidentiality == 0:
+            raise OperationNotAvailableError(context_msg="NTLM wrap without integrity or confidentiality")
+
+        if not self._handle_out or self._sign_key_out is None:
+            raise NoContextError(context_msg="Cannot wrap until context has been established")
+
+        header_idx = -1
+        data_idx = -1
+        signature_input = []
+        buffers = self._build_iov_list(iov, lambda b: b)
+        res: typing.List[IOVResBuffer] = []
+
+        for idx, buffer in enumerate(buffers):
+            data: bytes
+            if buffer.type == BufferType.header:
+                if header_idx != -1:
+                    raise InvalidTokenError(context_msg="wrap_iov must only be used with 1 header IOV buffer.")
+                header_idx = idx
+                data = b""
+
+            elif buffer.type == BufferType.data:
+                if data_idx != -1:
+                    raise InvalidTokenError(context_msg="wrap_iov must only be used with 1 data IOV buffer.")
+
+                if not isinstance(buffer.data, bytes):
+                    raise InvalidTokenError(context_msg=f"wrap_iov IOV data buffer at [{idx}] must be bytes")
+
+                data_idx = idx
+                data = buffer.data
+                signature_input.append(data)
+
+            elif buffer.type in [BufferType.sign_only, BufferType.data_readonly]:
+                if not isinstance(buffer.data, bytes):
+                    raise InvalidTokenError(
+                        context_msg=f"wrap_iov IOV {buffer.type.name} buffer at [{idx}] must be bytes"
+                    )
+
+                data = buffer.data
+                signature_input.append(data)
+
+            else:
+                raise InvalidTokenError(context_msg=f"wrap_iov unsupported IOV buffer type {buffer.type.name}")
+
+            res.append(IOVResBuffer(buffer.type, data))
+
+        if header_idx == -1:
+            raise InvalidTokenError(context_msg="wrap_iov no IOV header buffer present")
+
+        if data_idx == -1:
+            raise InvalidTokenError(context_msg="wrap_iov no IOV data buffer present")
+
+        enc_msg, signature = seal(
+            self._context_attr,
+            self._handle_out,
+            self._sign_key_out,
+            self._seq_num_out,
+            res[data_idx][1] or b"",
+            to_sign=b"".join(signature_input),
+        )
+
+        res[header_idx] = IOVResBuffer(BufferType.header, signature)
+        res[data_idx] = IOVResBuffer(BufferType.data, enc_msg)
+
+        return IOVWrapResult(tuple(res), encrypted=True)
 
     def wrap_winrm(self, data: bytes) -> WinRMWrapResult:
         enc_data = self.wrap(data).data
         return WinRMWrapResult(header=enc_data[:16], data=enc_data[16:], padding_length=0)
 
     def unwrap(self, data: bytes) -> UnwrapResult:
         if not self._handle_in:
@@ -661,15 +735,92 @@
 
         return UnwrapResult(data=msg, encrypted=True, qop=0)
 
     def unwrap_iov(
         self,
         iov: typing.Iterable[IOV],
     ) -> IOVUnwrapResult:
-        raise OperationNotAvailableError(context_msg="NTLM does not offer IOV wrapping")
+        if self.context_attr & ContextReq.integrity == 0 and self.context_attr & ContextReq.confidentiality == 0:
+            raise OperationNotAvailableError(context_msg="NTLM unwrap without integrity or confidentiality")
+
+        if not self._handle_in or self._sign_key_in is None:
+            raise NoContextError(context_msg="Cannot unwrap until context has been established")
+
+        buffers = self._build_iov_list(iov, lambda b: b)
+
+        # Check if it's a stream + data set of buffers and just call unwrap.
+        if (
+            len(buffers) == 2
+            and buffers[0].type == BufferType.stream
+            and buffers[1].type == BufferType.data
+            and isinstance(buffers[0].data, bytes)
+        ):
+            unwrap_res = self.unwrap(buffers[0].data)
+
+            return IOVUnwrapResult(
+                (
+                    IOVResBuffer(BufferType.stream, buffers[0].data),
+                    IOVResBuffer(BufferType.data, unwrap_res.data),
+                ),
+                encrypted=unwrap_res.encrypted,
+                qop=unwrap_res.qop,
+            )
+
+        header_idx = -1
+        data_idx = -1
+        data_sig_idx = -1
+        signature_input: typing.List[bytes] = []
+
+        res: typing.List[IOVResBuffer] = []
+
+        for idx, buffer in enumerate(buffers):
+            data: bytes
+
+            if not isinstance(buffer.data, bytes):
+                raise InvalidTokenError(
+                    context_msg=f"unwrap_iov IOV {buffer.type.name} buffer at [{idx}] must be bytes"
+                )
+
+            data = buffer.data
+
+            if buffer.type == BufferType.header:
+                if header_idx != -1:
+                    raise InvalidTokenError(context_msg="unwrap_iov must only be used with 1 header IOV buffer.")
+
+                header_idx = idx
+
+            elif buffer.type == BufferType.data:
+                if data_idx != -1:
+                    raise InvalidTokenError(context_msg="unwrap_iov must only be used with 1 data IOV buffer.")
+
+                data_idx = idx
+                data_sig_idx = len(signature_input)
+                signature_input.append(b"")  # Replaced after decryption
+
+            elif buffer.type in [BufferType.sign_only, BufferType.data_readonly]:
+                signature_input.append(data)
+
+            else:
+                raise InvalidTokenError(context_msg=f"unwrap_iov unsupported IOV buffer type {buffer.type.name}")
+
+            res.append(IOVResBuffer(buffer.type, data))
+
+        if header_idx == -1:
+            raise InvalidTokenError(context_msg="unwrap_iov no IOV header buffer present")
+
+        if data_idx == -1:
+            raise InvalidTokenError(context_msg="unwrap_iov no IOV data buffer present")
+
+        dec = self._handle_in.update(res[data_idx].data or b"")
+        res[data_idx] = IOVResBuffer(BufferType.data, dec)
+        signature_input[data_sig_idx] = dec
+
+        self.verify(b"".join(signature_input), res[header_idx].data or b"")
+
+        return IOVUnwrapResult(tuple(res), encrypted=True, qop=0)
 
     def unwrap_winrm(self, header: bytes, data: bytes) -> bytes:
         if not self._handle_in:
             raise NoContextError(context_msg="Cannot unwrap until context has been established")
 
         msg = self._handle_in.update(data)
         self.verify(msg, header)
```

### Comparing `pyspnego-0.8.0/src/spnego/_ntlm_raw/crypto.py` & `pyspnego-0.9.0/src/spnego/_ntlm_raw/crypto.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_ntlm_raw/des.py` & `pyspnego-0.9.0/src/spnego/_ntlm_raw/des.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_ntlm_raw/md4.py` & `pyspnego-0.9.0/src/spnego/_ntlm_raw/md4.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_ntlm_raw/messages.py` & `pyspnego-0.9.0/src/spnego/_ntlm_raw/messages.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_ntlm_raw/security.py` & `pyspnego-0.9.0/src/spnego/_ntlm_raw/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 import typing
 
 from spnego._ntlm_raw.crypto import RC4Handle, crc32, hmac_md5, rc4
 from spnego._ntlm_raw.messages import NegotiateFlags
 from spnego.exceptions import OperationNotAvailableError
 
 
-def seal(flags: int, handle: RC4Handle, signing_key: bytes, seq_num: int, b_data: bytes) -> typing.Tuple[bytes, bytes]:
+def seal(
+    flags: int,
+    handle: RC4Handle,
+    signing_key: bytes,
+    seq_num: int,
+    b_data: bytes,
+    *,
+    to_sign: typing.Optional[bytes] = None,
+) -> typing.Tuple[bytes, bytes]:
     """Create a sealed NTLM message.
 
     Creates a sealed NTLM message as documented at `NTLM Message Confidentiality`_.
 
     Args:
         flags: The negotiated flags between the initiator and acceptor.
         handle: The RC4 handle for the negotiated context.
@@ -24,15 +32,15 @@
     Returns:
         Tuple[bytes, bytes]: The sealed message bytes and the message signature.
 
     .. _NTLM Message Confidentiality:
         https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-nlmp/115f9c7d-bc30-4262-ae96-254555c14ea6
     """
     seal_msg = rc4(handle, b_data)
-    signature = sign(flags, handle, signing_key, seq_num, b_data)
+    signature = sign(flags, handle, signing_key, seq_num, to_sign if to_sign else b_data)
     return seal_msg, signature
 
 
 def sign(
     flags: int,
     handle: RC4Handle,
     signing_key: bytes,
```

### Comparing `pyspnego-0.8.0/src/spnego/_spnego.py` & `pyspnego-0.9.0/src/spnego/_spnego.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_sspi.py` & `pyspnego-0.9.0/src/spnego/_sspi.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,24 +8,30 @@
 
 from spnego._context import (
     IOV,
     ContextProxy,
     ContextReq,
     IOVUnwrapResult,
     IOVWrapResult,
+    SecPkgContextSizes,
     UnwrapResult,
     WinRMWrapResult,
     WrapResult,
     split_username,
     wrap_system_error,
 )
 from spnego._credential import Credential, CredentialCache, Password, unify_credentials
 from spnego._text import to_text
 from spnego.channel_bindings import GssChannelBindings
-from spnego.exceptions import InvalidCredentialError, NegotiateOptions, SpnegoError
+from spnego.exceptions import (
+    InvalidCredentialError,
+    NegotiateOptions,
+    NoContextError,
+    SpnegoError,
+)
 from spnego.exceptions import WinError as NativeError
 from spnego.iov import BufferType, IOVBuffer, IOVResBuffer
 
 log = logging.getLogger(__name__)
 
 HAS_SSPI = True
 SSPI_IMP_ERR = None
@@ -69,15 +75,21 @@
         return []
 
 
 def _create_iov_result(iov: "SecBufferDesc") -> typing.Tuple[IOVResBuffer, ...]:
     """Converts SSPI IOV buffer to generic IOVBuffer result."""
     buffers = []
     for i in iov:
-        buffer_entry = IOVResBuffer(type=BufferType(i.buffer_type), data=i.buffer)
+        buffer_type = i.buffer_type
+        if i.buffer_type & SecBufferType.readonly_with_checksum:
+            buffer_type = BufferType.sign_only
+        elif i.buffer_type & SecBufferType.readonly:
+            buffer_type = BufferType.data_readonly
+
+        buffer_entry = IOVResBuffer(type=BufferType(buffer_type), data=i.buffer)
         buffers.append(buffer_entry)
 
     return tuple(buffers)
 
 
 def _get_sspi_credential(
     principal: typing.Optional[str],
@@ -280,14 +292,20 @@
             self._security_trailer = attr_sizes.security_trailer
 
         if not self._is_wrapped:
             log.debug("SSPI step output: %s", base64.b64encode(out_token or b"").decode())
 
         return out_token
 
+    def query_message_sizes(self) -> SecPkgContextSizes:
+        if not self._security_trailer:
+            raise NoContextError(context_msg="Cannot get message sizes until context has been established")
+
+        return SecPkgContextSizes(header=self._security_trailer)
+
     def wrap(self, data: bytes, encrypt: bool = True, qop: typing.Optional[int] = None) -> WrapResult:
         res = self.wrap_iov([BufferType.header, data, BufferType.padding], encrypt=encrypt, qop=qop)
         return WrapResult(data=b"".join([r.data for r in res.buffers if r.data]), encrypted=res.encrypted)
 
     @wrap_system_error(NativeError, "Wrapping IOV buffer")
     def wrap_iov(
         self,
@@ -381,14 +399,15 @@
             (ContextReq.delegate, "delegate"),
             (ContextReq.delegate_policy, "delegate"),
             (ContextReq.mutual_auth, "mutual_auth"),
             (ContextReq.replay_detect, "replay_detect"),
             (ContextReq.sequence_detect, "sequence_detect"),
             (ContextReq.confidentiality, "confidentiality"),
             (ContextReq.integrity, "integrity"),
+            (ContextReq.dce_style, "use_dce_style"),
             (ContextReq.identify, "identify"),
         ]
         if self.usage == "initiate":
             attr_map.append((ContextReq.no_integrity, "no_integrity"))
 
         attrs = []
         for spnego_flag, gssapi_name in attr_map:
@@ -425,15 +444,23 @@
                 if buffer.type not in auto_alloc_size:
                     raise ValueError(
                         "Cannot auto allocate buffer of type %s.%s" % (type(buffer.type).__name__, buffer.type.name)
                     )
 
                 data = bytearray(auto_alloc_size[buffer.type])
 
-        return (buffer.type, data)
+        # This buffer types need manual mapping from the generic value to the
+        # one understood by SSPI.
+        buffer_type = int(buffer.type)
+        if buffer_type == BufferType.sign_only:
+            buffer_type = SecBufferType.data | SecBufferType.readonly_with_checksum
+        elif buffer_type == BufferType.data_readonly:
+            buffer_type = SecBufferType.data | SecBufferType.readonly
+
+        return (buffer_type, data)
 
     def _get_native_bindings(self, channel_bindings: GssChannelBindings) -> bytearray:
         """Gets the raw byte value of the SEC_CHANNEL_BINDINGS structure."""
         b_bindings = bytearray()
         b_bindings_data = bytearray()
 
         def _pack_binding(name: str, b_bindings: bytearray, b_bindings_data: bytearray) -> None:
```

### Comparing `pyspnego-0.8.0/src/spnego/_sspi_raw/__init__.py` & `pyspnego-0.9.0/src/spnego/_sspi_raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_sspi_raw/security.pxd` & `pyspnego-0.9.0/src/spnego/_sspi_raw/security.pxd`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_sspi_raw/sspi.pxd` & `pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pxd`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_sspi_raw/sspi.pyi` & `pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     identify: int = ...
     manual_cred_validation: int = ...
     mutual_auth: int = ...
     no_integrity: int = ...
     replay_detect: int = ...
     sequence_detect: int = ...
     stream: int = ...
+    use_dce_style: int = ...
     use_session_key: int = ...
     use_supplied_creds: int = ...
 
 class CredentialUse:
     inbound: int = ...
     outbound: int = ...
     both: int = ...
```

### Comparing `pyspnego-0.8.0/src/spnego/_sspi_raw/sspi.pyx` & `pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     ISC_REQ_INTEGRITY,
     ISC_REQ_MANUAL_CRED_VALIDATION,
     ISC_REQ_MUTUAL_AUTH,
     ISC_REQ_NO_INTEGRITY,
     ISC_REQ_REPLAY_DETECT,
     ISC_REQ_SEQUENCE_DETECT,
     ISC_REQ_STREAM,
+    ISC_REQ_USE_DCE_STYLE,
     ISC_REQ_USE_SESSION_KEY,
     ISC_REQ_USE_SUPPLIED_CREDS,
     ISC_RET_DELEGATE,
     ISC_RET_MUTUAL_AUTH,
     ISC_RET_REPLAY_DETECT,
     ISC_RET_SEQUENCE_DETECT,
     ISC_RET_CONFIDENTIALITY,
@@ -242,14 +243,15 @@
     identify = ISC_REQ_IDENTIFY
     manual_cred_validation = ISC_REQ_MANUAL_CRED_VALIDATION
     mutual_auth = ISC_REQ_MUTUAL_AUTH
     no_integrity = ISC_REQ_NO_INTEGRITY
     replay_detect = ISC_REQ_REPLAY_DETECT
     sequence_detect = ISC_REQ_SEQUENCE_DETECT
     stream = ISC_REQ_STREAM
+    use_dce_style = ISC_REQ_USE_DCE_STYLE
     use_session_key = ISC_REQ_USE_SESSION_KEY
     use_supplied_creds = ISC_REQ_USE_SUPPLIED_CREDS
 
 
 class CredentialUse:
     inbound = SECPKG_CRED_INBOUND
     outbound = SECPKG_CRED_OUTBOUND
```

### Comparing `pyspnego-0.8.0/src/spnego/_sspi_raw/text.pyx` & `pyspnego-0.9.0/src/spnego/_sspi_raw/text.pyx`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_sspi_raw/windows.pxd` & `pyspnego-0.9.0/src/spnego/_sspi_raw/windows.pxd`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_text.py` & `pyspnego-0.9.0/src/spnego/_text.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/_tls_struct.py` & `pyspnego-0.9.0/src/spnego/_tls_struct.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/auth.py` & `pyspnego-0.9.0/src/spnego/auth.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/channel_bindings.py` & `pyspnego-0.9.0/src/spnego/channel_bindings.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/src/spnego/exceptions.py` & `pyspnego-0.9.0/src/spnego/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,16 @@
         return self.args[0]
 
     @property
     def message(self) -> str:
         msg = {
             NegotiateOptions.negotiate_kerberos: "The Python gssapi library is not installed so Kerberos cannot be "
             "negotiated.",
-            NegotiateOptions.wrapping_iov: "The system is missing the GSSAPI IOV extension headers or NTLM or CredSSP "
-            "is being requested, cannot utilize wrap_iov and unwrap_iov",
+            NegotiateOptions.wrapping_iov: "The system is missing the GSSAPI IOV extension headers or CredSSP is "
+            "being requested, cannot utilize wrap_iov and unwrap_iov",
             NegotiateOptions.wrapping_winrm: "The system is missing the GSSAPI IOV extension headers required for "
             "WinRM encryption with Kerberos.",
             NegotiateOptions.session_key: "The protocol selected does not support getting the session key.",
         }.get(self.feature_id, "Unknown option flag: %d" % self.feature_id)
 
         return msg
```

### Comparing `pyspnego-0.8.0/src/spnego/iov.py` & `pyspnego-0.9.0/src/spnego/iov.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,22 @@
     empty = 0  # SECBUFFER_EMPTY | GSS_IOV_BUFFER_TYPE_EMPTY
     data = 1  # SECBUFFER_DATA | GSS_IOV_BUFFER_TYPE_DATA
     header = 2  # SECBUFFER_TOKEN | GSS_IOV_BUFFER_TYPE_HEADER
     pkg_params = 3  # SECBUFFER_PKG_PARAMS | GSS_IOV_BUFFER_TYPE_MECH_PARAMS
     trailer = 7  # SECBUFFER_STREAM_HEADER | GSS_IOV_BUFFER_TYPE_TRAILER
     padding = 9  # SECBUFFER_PADDING | GSS_IOV_BUFFER_TYPE_PADDING
     stream = 10  # SECBUFFER_STREAM | GSS_IOV_BUFFER_TYPE_STREAM
-    sign_only = 11  # SECBUFFER_MECHLIST | GSS_IOV_BUFFER_TYPE_SIGN_ONLY
+    sign_only = 11  # (SECBUFFER_DATA | SECBUFFER_READONLY_WITH_CHECKSUM) | GSS_IOV_BUFFER_TYPE_SIGN_ONLY
     mic_token = 12  # SECBUFFER_MECHLIST_SIGNATURE | GSS_IOV_BUFFER_TYPE_MIC_TOKEN
 
+    # This doesn't have an equivalent in GSSAPI but is mapped internally to
+    # the SSPI data + readonly buffer. Luckily GSSAPI seems to treat an empty
+    # buffer as the same as SSPI so that will be used there.
+    data_readonly = 4096  # (SECBUFFER_DATA | SECBUFFER_READONLY) | GSS_IOV_BUFFER_TYPE_EMPTY
+
 
 class IOVBuffer(typing.NamedTuple):
     """A buffer to pass as a list to :meth:`wrap_iov()`.
 
     Defines the buffer inside a list that is passed to :meth:`wrap_iov()`. A list of these buffers are also returned in
     the `IOVUnwrapResult` under the `buffers` attribute.
```

### Comparing `pyspnego-0.8.0/src/spnego/tls.py` & `pyspnego-0.9.0/src/spnego/tls.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/_ntlm_raw/__init__.py` & `pyspnego-0.9.0/tests/_ntlm_raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/_ntlm_raw/test_crypto.py` & `pyspnego-0.9.0/tests/_ntlm_raw/test_crypto.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/_ntlm_raw/test_des.py` & `pyspnego-0.9.0/tests/_ntlm_raw/test_des.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/_ntlm_raw/test_md4.py` & `pyspnego-0.9.0/tests/_ntlm_raw/test_md4.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/_ntlm_raw/test_messages.py` & `pyspnego-0.9.0/tests/_ntlm_raw/test_messages.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/_ntlm_raw/test_security.py` & `pyspnego-0.9.0/tests/_ntlm_raw/test_security.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/_sspi_raw/test_sspi.py` & `pyspnego-0.9.0/tests/_sspi_raw/test_sspi.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/_sspi_raw/test_text.py` & `pyspnego-0.9.0/tests/_sspi_raw/test_text.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/conftest.py` & `pyspnego-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/credssp_ts_remote_guard_ms_example` & `pyspnego-0.9.0/tests/data/credssp_ts_remote_guard_ms_example`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/initial_context_token_krb_ap_req` & `pyspnego-0.9.0/tests/data/initial_context_token_krb_ap_req`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/initial_context_token_neg_token_init` & `pyspnego-0.9.0/tests/data/initial_context_token_neg_token_init`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/krb_as_rep` & `pyspnego-0.9.0/tests/data/krb_as_rep`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/krb_tgs_rep` & `pyspnego-0.9.0/tests/data/krb_tgs_rep`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/krb_tgs_req` & `pyspnego-0.9.0/tests/data/krb_tgs_req`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/pyspnego.ps1` & `pyspnego-0.9.0/tests/data/pyspnego.ps1`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/test_context.py` & `pyspnego-0.9.0/tests/data/test_context.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/tls1.0_server_hello` & `pyspnego-0.9.0/tests/data/tls1.0_server_hello`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/tls1.1_server_hello` & `pyspnego-0.9.0/tests/data/tls1.1_server_hello`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/tls1.2_server_hello` & `pyspnego-0.9.0/tests/data/tls1.2_server_hello`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/data/tls1.3_server_hello` & `pyspnego-0.9.0/tests/data/tls1.3_server_hello`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/integration/README.md` & `pyspnego-0.9.0/tests/integration/README.md`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/integration/Vagrantfile` & `pyspnego-0.9.0/tests/integration/Vagrantfile`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/integration/inventory.yml` & `pyspnego-0.9.0/tests/integration/inventory.yml`

 * *Files 8% similar despite different names*

```diff
@@ -32,35 +32,35 @@
         python_venv_path: C:\temp\venv
         krb_provider: SSPI
 
     linux:
       children:
         linux_children:
           hosts:
-            CENTOS8-MIT:
+            ROCKY9-MIT:
               ansible_host: 192.168.65.13
-              vagrant_box: centos/stream8
+              vagrant_box: generic/rocky9
               krb_packages:
               - krb5-devel
               - krb5-workstation
               krb_provider: MIT
-            CENTOS8-HEIMDAL:
+            ROCKY9-HEIMDAL:
               ansible_host: 192.168.65.14
-              vagrant_box: centos/stream8
+              vagrant_box: generic/rocky9
               krb_packages:
               - heimdal-devel
               - heimdal-libs
               - heimdal-path
               - heimdal-workstation
               - libcom_err-devel
               krb_provider: Heimdal
       vars:
         ansible_ssh_common_args: -o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no
         python_interpreters:
-        - /usr/bin/python3.8
+        - /usr/bin/python3.9
         python_venv_path: ~/venv
 
   vars:
     ansible_user: vagrant
     ansible_password: vagrant
 
     domain_name: spnego.test
```

### Comparing `pyspnego-0.8.0/tests/integration/main.yml` & `pyspnego-0.9.0/tests/integration/main.yml`

 * *Files 0% similar despite different names*

```diff
@@ -351,30 +351,30 @@
   tasks:
   - name: install base packages
     yum:
       name:
       - dnsmasq
       - epel-release
       - gcc
-      - python38
-      - python38-devel
+      - python39
+      - python3-devel
       - unzip
       - vim
       state: present
 
   - name: install kerberos packages
     yum:
       name: '{{ krb_packages }}'
       state: present
 
   - name: ensure virtualenv is installed on base Python interpreters
     pip:
       name:
       - virtualenv
-      executable: /usr/bin/pip3.8
+      executable: /usr/bin/pip3.9
 
   - name: setup NetworkManager to use dnsmasq
     copy:
       dest: /etc/NetworkManager/conf.d/dns.conf
       content: |
         [main]
         dns=dnsmasq
```

### Comparing `pyspnego-0.8.0/tests/integration/templates/generate_cert.sh.tmpl` & `pyspnego-0.9.0/tests/integration/templates/generate_cert.sh.tmpl`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/integration/templates/krb5.conf.tmpl` & `pyspnego-0.9.0/tests/integration/templates/krb5.conf.tmpl`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/integration/tests.yml` & `pyspnego-0.9.0/tests/integration/tests.yml`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/test_asn1.py` & `pyspnego-0.9.0/tests/test_asn1.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/test_auth.py` & `pyspnego-0.9.0/tests/test_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1611,14 +1611,17 @@
     assert client_credential.username == username
     assert client_credential.domain_name == domain
     assert client_credential.password == ntlm_cred[1]
 
     assert c.get_extra_info("protocol_version") == version
     assert s.get_extra_info("protocol_version") == version
 
+    assert isinstance(c.query_message_sizes().header, int)
+    assert isinstance(s.query_message_sizes().header, int)
+
     _message_test(c, s)
 
     plaintext = os.urandom(16)
     c_winrm_result = c.wrap_winrm(plaintext)
     assert isinstance(c_winrm_result, WinRMWrapResult)
     assert isinstance(c_winrm_result.header, bytes)
     assert isinstance(c_winrm_result.data, bytes)
```

### Comparing `pyspnego-0.8.0/tests/test_channel_bindings.py` & `pyspnego-0.9.0/tests/test_channel_bindings.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/test_context.py` & `pyspnego-0.9.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/test_credssp.py` & `pyspnego-0.9.0/tests/test_credssp.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 # MIT License (see LICENSE or https://opensource.org/licenses/MIT)
 
 import re
 import socket
 
 import pytest
 
+import spnego
 import spnego._credssp as credssp
 from spnego._credssp_structures import NegoData, TSRequest
 from spnego.exceptions import (
     BadBindingsError,
     FeatureMissingError,
     InvalidTokenError,
     NegotiateOptions,
+    NoContextError,
     OperationNotAvailableError,
     SpnegoError,
 )
 from spnego.tls import default_tls_context
 
 
 @pytest.mark.parametrize(
@@ -62,14 +64,23 @@
     assert actual == expected
 
 
 def test_credssp_no_iov():
     assert not credssp.CredSSPProxy("username", "password").iov_available()
 
 
+def test_credssp_iov_not_available():
+    expected = (
+        "The system is missing the GSSAPI IOV extension headers or CredSSP is being requested, "
+        "cannot utilize wrap_iov and unwrap_iov"
+    )
+    with pytest.raises(FeatureMissingError, match=re.escape(expected)):
+        credssp.CredSSPProxy("username", "password", options=spnego.NegotiateOptions.wrapping_iov)
+
+
 def test_credssp_no_session_key():
     with pytest.raises(FeatureMissingError, match="The protocol selected does not support getting the session key"):
         credssp.CredSSPProxy("user", "password", options=NegotiateOptions.session_key)
 
 
 def test_credssp_fail_getting_session_key():
     context = credssp.CredSSPProxy("username", "password")
@@ -99,14 +110,19 @@
 
 
 def test_credssp_wrap_no_context():
     with pytest.raises(SpnegoError, match="Invalid TLS state when wrapping data"):
         credssp.CredSSPProxy("username", "password").wrap(b"data")
 
 
+def test_credssp_query_message_sizes_fail():
+    with pytest.raises(NoContextError, match="Cannot get message sizes until context has been established"):
+        credssp.CredSSPProxy("username", "password").query_message_sizes()
+
+
 def test_credssp_invalid_handshake(ntlm_cred):
     c = credssp.CredSSPProxy(ntlm_cred[0], ntlm_cred[1], protocol="credssp")
     s = credssp.CredSSPProxy(None, None, protocol="credssp", usage="accept")
 
     server_hello = s.step(c.step())
     assert server_hello is not None
```

### Comparing `pyspnego-0.8.0/tests/test_credssp_structures.py` & `pyspnego-0.9.0/tests/test_credssp_structures.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/test_deprecation.py` & `pyspnego-0.9.0/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/test_exceptions.py` & `pyspnego-0.9.0/tests/test_exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     [
         (
             exceptions.NegotiateOptions.negotiate_kerberos,
             "The Python gssapi library is not installed so Kerberos cannot be negotiated.",
         ),
         (
             exceptions.NegotiateOptions.wrapping_iov,
-            "The system is missing the GSSAPI IOV extension headers or NTLM or "
-            "CredSSP is being requested, cannot utilize wrap_iov and unwrap_iov",
+            "The system is missing the GSSAPI IOV extension headers or CredSSP is being requested, "
+            "cannot utilize wrap_iov and unwrap_iov",
         ),
         (
             exceptions.NegotiateOptions.wrapping_winrm,
             "The system is missing the GSSAPI IOV extension headers required for WinRM encryption with Kerberos.",
         ),
         (exceptions.NegotiateOptions.session_key, "The protocol selected does not support getting the session key."),
     ],
```

### Comparing `pyspnego-0.8.0/tests/test_gss.py` & `pyspnego-0.9.0/tests/test_gss.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,21 @@
     assert actual[1] == (spnego.iov.BufferType.data, False, b"\x00")
     assert actual[2] == (spnego.iov.BufferType.padding, True, None)
     assert actual[3] == (spnego.iov.BufferType.header, True, None)
     assert actual[4] == (spnego.iov.BufferType.stream, False, None)
     assert actual[5] == (spnego.iov.BufferType.data, False, b"\x02")
 
 
+def test_gssapi_query_message_sizes_fail(kerb_cred):
+    c = spnego._gss.GSSAPIProxy(kerb_cred.user_princ, protocol="kerberos")
+
+    with pytest.raises(NoContextError, match="Cannot get message sizes until context has been established"):
+        c.query_message_sizes()
+
+
 def test_gssapi_wrap_no_context(kerb_cred):
     c = spnego._gss.GSSAPIProxy(kerb_cred.user_princ, protocol="kerberos")
 
     with pytest.raises(NoContextError, match="Cannot wrap until context has been established"):
         c.wrap(b"data")
```

### Comparing `pyspnego-0.8.0/tests/test_kerberos.py` & `pyspnego-0.9.0/tests/test_kerberos.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/test_main.py` & `pyspnego-0.9.0/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
     assert actual["MessageType"] == "NEGOTIATE_MESSAGE (1)"
     assert actual["RawData"] is not None
     assert actual["Data"] is not None
 
 
 def test_parse_output_yaml_not_installed(monkeypatch):
-    monkeypatch.setattr(entrypoint, "yaml", None)
+    monkeypatch.setattr(entrypoint, "HAS_YAML", False)
 
     with pytest.raises(ValueError, match="Cannot output as yaml as ruamel.yaml is not installed"):
         entrypoint.main(
             [
                 "--token",
                 base64.b64encode(get_data("ntlm_negotiate")).decode(),
                 "--format",
```

### Comparing `pyspnego-0.8.0/tests/test_negotiate.py` & `pyspnego-0.9.0/tests/test_negotiate.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/test_ntlm.py` & `pyspnego-0.9.0/tests/test_ntlm.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import socket
 
 import pytest
 
 import spnego
 import spnego._ntlm as ntlm
 import spnego.channel_bindings
+import spnego.iov
 from spnego._credential import CredentialCache
 from spnego._ntlm_raw.messages import (
     Authenticate,
     AvId,
     Challenge,
     FileTime,
     Negotiate,
@@ -23,15 +24,14 @@
     TargetInfo,
     Version,
 )
 from spnego._text import to_bytes, to_text
 from spnego.exceptions import (
     BadBindingsError,
     BadMICError,
-    FeatureMissingError,
     InvalidTokenError,
     NoContextError,
     OperationNotAvailableError,
     SpnegoError,
     UnsupportedQop,
 )
 
@@ -171,34 +171,31 @@
     with pytest.raises(
         OperationNotAvailableError, match="Retrieving NTLM store without NTLM_USER_FILE set to a " "filepath"
     ):
         ntlm.NTLMProxy(CredentialCache(), usage=usage)
 
 
 def test_iov_available():
-    assert ntlm.NTLMProxy.iov_available() is False
+    assert ntlm.NTLMProxy.iov_available() is True
 
 
 def test_ntlm_invalid_usage():
     with pytest.raises(ValueError, match="Invalid usage 'test', must be initiate or accept"):
         ntlm.NTLMProxy("user", "pass", usage="test")
 
 
 def test_ntlm_invalid_protocol():
     with pytest.raises(ValueError, match="Invalid protocol 'fake', must be ntlm, kerberos, negotiate, or credssp"):
         ntlm.NTLMProxy("user", "pass", protocol="fake")
 
 
-def test_ntlm_iov_not_available():
-    expected = (
-        "The system is missing the GSSAPI IOV extension headers or NTLM or CredSSP is being requested, "
-        "cannot utilize wrap_iov and unwrap_iov"
-    )
-    with pytest.raises(FeatureMissingError, match=re.escape(expected)):
-        ntlm.NTLMProxy("user", "pass", options=spnego.NegotiateOptions.wrapping_iov)
+def test_ntlm_query_message_sizes_fail():
+    n = ntlm.NTLMProxy("user", "pass")
+    with pytest.raises(NoContextError, match="Cannot get message sizes until context has been established"):
+        n.query_message_sizes()
 
 
 def test_ntlm_wrap_qop_invalid():
     n = ntlm.NTLMProxy("user", "pass")
     with pytest.raises(UnsupportedQop, match="Unsupported QoP value 1 specified for NTLM"):
         n.wrap(b"data", qop=1)
 
@@ -231,26 +228,172 @@
 
 def test_ntlm_unwrap_winrm_no_context():
     n = ntlm.NTLMProxy("user", "pass")
     with pytest.raises(NoContextError, match="Cannot unwrap until context has been established"):
         n.unwrap_winrm(b"header", b"data")
 
 
-def test_ntlm_wrap_iov_fail():
+def test_ntlm_wrap_iov_with_qop_fail():
+    n = ntlm.NTLMProxy("user", "pass")
+    with pytest.raises(UnsupportedQop, match="Unsupported QoP value 1 specified for NTLM"):
+        n.wrap_iov([], qop=1)
+
+
+def test_ntlm_wrap_iov_no_sign_or_seal():
     n = ntlm.NTLMProxy("user", "pass")
-    with pytest.raises(OperationNotAvailableError, match="NTLM does not offer IOV wrapping"):
+    with pytest.raises(OperationNotAvailableError, match="NTLM wrap without integrity or confidentiality"):
         n.wrap_iov([])
 
 
-def test_ntlm_unwrap_iov_fail():
+def test_ntlm_wrap_iov_no_context():
     n = ntlm.NTLMProxy("user", "pass")
-    with pytest.raises(OperationNotAvailableError, match="NTLM does not offer IOV wrapping"):
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    with pytest.raises(NoContextError, match="Cannot wrap until context has been established"):
+        n.wrap_iov([])
+
+
+def test_ntlm_wrap_iov_no_header():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_out = n._handle_out = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="wrap_iov no IOV header buffer present"):
+        n.wrap_iov([b""])
+
+
+def test_ntlm_wrap_iov_no_data():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_out = n._handle_out = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="wrap_iov no IOV data buffer present"):
+        n.wrap_iov([spnego.iov.BufferType.header])
+
+
+def test_ntlm_wrap_iov_multiple_header():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_out = n._handle_out = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="wrap_iov must only be used with 1 header IOV buffer"):
+        n.wrap_iov([spnego.iov.BufferType.header, b"", spnego.iov.BufferType.header])
+
+
+def test_ntlm_wrap_iov_multiple_data():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_out = n._handle_out = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="wrap_iov must only be used with 1 data IOV buffer"):
+        n.wrap_iov([spnego.iov.BufferType.header, b"", b""])
+
+
+def test_ntlm_wrap_iov_invalid_type():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_out = n._handle_out = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="wrap_iov unsupported IOV buffer type padding"):
+        n.wrap_iov([spnego.iov.BufferType.header, b"", spnego.iov.BufferType.padding])
+
+
+def test_ntlm_wrap_iov_data_not_bytes():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_out = n._handle_out = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="wrap_iov IOV data buffer at \\[1\\] must be bytes"):
+        n.wrap_iov([spnego.iov.BufferType.header, (spnego.iov.BufferType.data, 1)])
+
+
+def test_ntlm_wrap_iov_signonly_not_bytes():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_out = n._handle_out = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="wrap_iov IOV sign_only buffer at \\[1\\] must be bytes"):
+        n.wrap_iov([spnego.iov.BufferType.header, (spnego.iov.BufferType.sign_only, 1)])
+
+
+def test_ntlm_unwrap_iov_no_sign_or_seal():
+    n = ntlm.NTLMProxy("user", "pass")
+    with pytest.raises(OperationNotAvailableError, match="NTLM unwrap without integrity or confidentiality"):
+        n.unwrap_iov([])
+
+
+def test_ntlm_unwrap_iov_no_context():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    with pytest.raises(NoContextError, match="Cannot unwrap until context has been established"):
         n.unwrap_iov([])
 
 
+def test_ntlm_unwrap_iov_no_header():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_in = n._handle_in = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="unwrap_iov no IOV header buffer present"):
+        n.unwrap_iov([b""])
+
+
+def test_ntlm_unwrap_iov_no_data():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_in = n._handle_in = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="unwrap_iov no IOV data buffer present"):
+        n.unwrap_iov([(spnego.iov.BufferType.header, b"")])
+
+
+def test_ntlm_unwrap_iov_multiple_header():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_in = n._handle_in = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="unwrap_iov must only be used with 1 header IOV buffer"):
+        n.unwrap_iov([(spnego.iov.BufferType.header, b""), b"", (spnego.iov.BufferType.header, b"")])
+
+
+def test_ntlm_unwrap_iov_multiple_data():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_in = n._handle_in = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="unwrap_iov must only be used with 1 data IOV buffer"):
+        n.unwrap_iov([(spnego.iov.BufferType.header, b""), b"", b""])
+
+
+def test_ntlm_unwrap_iov_invalid_type():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_in = n._handle_in = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="unwrap_iov unsupported IOV buffer type padding"):
+        n.unwrap_iov([(spnego.iov.BufferType.header, b""), b"", (spnego.iov.BufferType.padding, b"")])
+
+
+def test_ntlm_unwrap_iov_data_not_bytes():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_in = n._handle_in = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="unwrap_iov IOV data buffer at \\[1\\] must be bytes"):
+        n.unwrap_iov([(spnego.iov.BufferType.header, b""), (spnego.iov.BufferType.data, 1)])
+
+
+def test_ntlm_unwrap_iov_data_readonly_not_bytes():
+    n = ntlm.NTLMProxy("user", "pass")
+    n._context_attr = spnego.ContextReq.confidentiality | spnego.ContextReq.integrity
+    n._sign_key_in = n._handle_in = 1  # type: ignore
+
+    with pytest.raises(InvalidTokenError, match="unwrap_iov IOV data_readonly buffer at \\[1\\] must be bytes"):
+        n.unwrap_iov([(spnego.iov.BufferType.header, b""), (spnego.iov.BufferType.data_readonly, 1)])
+
+
 def test_ntlm_sign_qop_invalid():
     n = ntlm.NTLMProxy("user", "pass")
     with pytest.raises(UnsupportedQop, match="Unsupported QoP value 1 specified for NTLM"):
         n.sign(b"data", qop=1)
 
 
 def test_ntlm_sign_no_context():
@@ -633,7 +776,135 @@
     s = spnego.server(options=spnego.NegotiateOptions.use_ntlm, protocol="ntlm")
 
     auth = Authenticate.unpack(c.step(s.step(c.step())) or b"")
     anon_auth = Authenticate(flags=auth.flags, lm_challenge_response=b"\x00", nt_challenge_response=b"").pack()
 
     with pytest.raises(OperationNotAvailableError, match="Anonymous user authentication not implemented"):
         s.step(anon_auth)
+
+
+def test_ntlm_iov_wrapping(ntlm_cred):
+    c = spnego.client(
+        ntlm_cred[0],
+        ntlm_cred[1],
+        hostname=socket.gethostname(),
+        protocol="ntlm",
+        options=spnego.NegotiateOptions.use_ntlm,
+    )
+    s = spnego.server(protocol="ntlm")
+
+    s.step(c.step(s.step(c.step())))
+
+    res1 = c.wrap_iov(
+        [
+            (spnego.iov.BufferType.sign_only, b"sign 1"),
+            b"data",
+            (spnego.iov.BufferType.data_readonly, b"sign 2"),
+            spnego.iov.BufferType.header,
+        ]
+    )
+    assert isinstance(res1, spnego.IOVWrapResult)
+    assert res1.encrypted
+    assert len(res1.buffers) == 4
+    assert res1.buffers[0].data == b"sign 1"
+    assert res1.buffers[1].data != b"data"
+    assert res1.buffers[2].data == b"sign 2"
+    assert len(res1.buffers[3].data or b"") == 16
+
+    res2 = s.unwrap_iov(res1.buffers)
+    assert isinstance(res2, spnego.IOVUnwrapResult)
+    assert res2.encrypted
+    assert res2.qop == 0
+    assert len(res2.buffers) == 4
+    assert res2.buffers[0].data == b"sign 1"
+    assert res2.buffers[1].data == b"data"
+    assert res2.buffers[2].data == b"sign 2"
+    assert res2.buffers[3].data == res1.buffers[3].data
+
+    res3 = s.wrap_iov(
+        [
+            (spnego.iov.BufferType.sign_only, b"sign 1"),
+            b"data",
+            (spnego.iov.BufferType.data_readonly, b"sign 2"),
+            spnego.iov.BufferType.header,
+        ]
+    )
+    assert isinstance(res3, spnego.IOVWrapResult)
+    assert res3.encrypted
+    assert len(res3.buffers) == 4
+    assert res3.buffers[0].data == b"sign 1"
+    assert res3.buffers[1].data != b"data"
+    assert res3.buffers[2].data == b"sign 2"
+    assert len(res3.buffers[3].data or b"") == 16
+
+    res4 = c.unwrap_iov(res3.buffers)
+    assert isinstance(res4, spnego.IOVUnwrapResult)
+    assert res4.encrypted
+    assert res4.qop == 0
+    assert len(res4.buffers) == 4
+    assert res4.buffers[0].data == b"sign 1"
+    assert res4.buffers[1].data == b"data"
+    assert res4.buffers[2].data == b"sign 2"
+    assert res4.buffers[3].data == res3.buffers[3].data
+
+
+def test_ntlm_iov_unwrapping_as_stream(ntlm_cred):
+    c = spnego.client(
+        ntlm_cred[0],
+        ntlm_cred[1],
+        hostname=socket.gethostname(),
+        protocol="ntlm",
+        options=spnego.NegotiateOptions.use_ntlm,
+    )
+    s = spnego.server(protocol="ntlm")
+
+    s.step(c.step(s.step(c.step())))
+
+    res1 = c.wrap_iov(
+        [
+            b"data",
+            spnego.iov.BufferType.header,
+        ]
+    )
+    assert isinstance(res1, spnego.IOVWrapResult)
+    assert res1.encrypted
+    assert len(res1.buffers) == 2
+    assert res1.buffers[0].data != b"data"
+    assert len(res1.buffers[1].data or b"") == 16
+
+    msg = (res1.buffers[1].data or b"") + (res1.buffers[0].data or b"")
+    res2 = s.unwrap_iov(
+        [
+            (spnego.iov.BufferType.stream, msg),
+            spnego.iov.BufferType.data,
+        ]
+    )
+    assert isinstance(res2, spnego.IOVUnwrapResult)
+    assert res2.encrypted
+    assert res2.qop == 0
+    assert len(res2.buffers) == 2
+    assert res2.buffers[1].data == b"data"
+
+    res3 = s.wrap_iov(
+        [
+            spnego.iov.BufferType.header,
+            b"data",
+        ]
+    )
+    assert isinstance(res3, spnego.IOVWrapResult)
+    assert res3.encrypted
+    assert len(res3.buffers) == 2
+    assert len(res3.buffers[0].data or b"") == 16
+    assert res3.buffers[1].data != b"data"
+
+    msg = (res3.buffers[0].data or b"") + (res3.buffers[1].data or b"")
+    res4 = c.unwrap_iov(
+        [
+            (spnego.iov.BufferType.stream, msg),
+            spnego.iov.BufferType.data,
+        ]
+    )
+    assert isinstance(res4, spnego.IOVUnwrapResult)
+    assert res4.encrypted
+    assert res4.qop == 0
+    assert len(res4.buffers) == 2
+    assert res4.buffers[1].data == b"data"
```

### Comparing `pyspnego-0.8.0/tests/test_spnego.py` & `pyspnego-0.9.0/tests/test_spnego.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/test_sspi.py` & `pyspnego-0.9.0/tests/test_sspi.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/test_text.py` & `pyspnego-0.9.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.8.0/tests/test_tls_struct.py` & `pyspnego-0.9.0/tests/test_tls_struct.py`

 * *Files identical despite different names*

