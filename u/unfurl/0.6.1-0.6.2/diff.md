# Comparing `tmp/unfurl-0.6.1.tar.gz` & `tmp/unfurl-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfurl-0.6.1.tar", last modified: Wed Mar 15 17:00:38 2023, max compression
+gzip compressed data, was "unfurl-0.6.2.tar", last modified: Sat Apr 29 08:02:00 2023, max compression
```

## Comparing `unfurl-0.6.1.tar` & `unfurl-0.6.2.tar`

### file list

```diff
@@ -1,189 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.206143 unfurl-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-15 17:00:35.000000 unfurl-0.6.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-03-15 17:00:35.000000 unfurl-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-03-15 17:00:38.206143 unfurl-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-03-15 17:00:35.000000 unfurl-0.6.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1218 2023-03-15 17:00:38.206143 unfurl-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-15 17:00:35.000000 unfurl-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.194143 unfurl-0.6.1/unfurl/
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41432 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/changelog-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    49776 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.194143 unfurl-0.6.1/unfurl/configurators/
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/dns-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/docker-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/helm-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16491 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/kompose.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/supervisor-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/configurators/terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)    29328 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.194143 unfurl-0.6.1/unfurl/filter_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/filter_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/filter_plugins/ref.py
--rw-r--r--   0 runner    (1001) docker     (123)    45656 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    57500 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    55656 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/localenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/lookup_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/lookup_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/lookup_plugins/unfurl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/manifest-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    25672 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    41243 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    44673 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/planrequests.py
--rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/projectpaths.py
--rw-r--r--   0 runner    (1001) docker     (123)    30016 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    26994 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    39270 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    51526 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    58023 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/aws/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/dashboard/manifest.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/dashboard/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/digitalocean/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/digitalocean/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/gcp/unfurl.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/gitignore.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/home/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/home/manifest-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/home/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/local/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/local/ensemble-examples.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/local-unfurl-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/manifest-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/manifest.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/python3.10/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/python3.10/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    73777 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/python3.10/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/python3.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/python3.11/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    69798 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/python3.11/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/python3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/python3.7/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    75670 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/python3.7/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/python3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/python3.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    75328 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/python3.8/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.198143 unfurl-0.6.1/unfurl/templates/python3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/python3.9/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    75111 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/python3.9/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/secrets.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/service-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/unfurl.local.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/templates/unfurl.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    64490 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    54844 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/tosca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.202143 unfurl-0.6.1/unfurl/tosca_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/tosca_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/tosca_plugins/artifacts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/tosca_plugins/googlecloud.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/tosca_plugins/k8s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/tosca_plugins/localhost.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/tosca_plugins/tosca-ext.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/unfurl-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    23855 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.202143 unfurl-0.6.1/unfurl/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.202143 unfurl-0.6.1/unfurl/vendor/sphinx-jsonschema/
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/vendor/sphinx-jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/vendor/sphinx-jsonschema/wide_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.202143 unfurl-0.6.1/unfurl/vendor/toscaparser/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.206143 unfurl-0.6.1/unfurl/vendor/toscaparser/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/dataentity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.206143 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/
--rw-r--r--   0 runner    (1001) docker     (123)    32477 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    33031 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/artifacttype.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/capabilitytype.py
--rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/grouptype.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/nodetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/policytype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/portspectype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/property_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/relationshiptype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/scalarunit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/statefulentitytype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/elements/tosca_type_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17924 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/entity_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.206143 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/exttools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.206143 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/mec/
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/mec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.206143 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/nfv/
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/nfv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.190143 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/nfv/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.206143 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/nfv/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py
--rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    25541 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/nodetemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.206143 unfurl-0.6.1/unfurl/vendor/toscaparser/prereq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/prereq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/prereq/csar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/relationship_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/substitution_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19241 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/topology_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/tosca_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/tpl_relationship_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/unsupportedtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.206143 unfurl-0.6.1/unfurl/vendor/toscaparser/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/utils/gettextutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/utils/urlutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/utils/validateutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/utils/yamlparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-03-15 17:00:36.000000 unfurl-0.6.1/unfurl/vendor/toscaparser/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    27237 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/yamlloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    39045 2023-03-15 17:00:35.000000 unfurl-0.6.1/unfurl/yamlmanifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:00:38.194143 unfurl-0.6.1/unfurl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-03-15 17:00:38.000000 unfurl-0.6.1/unfurl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-03-15 17:00:38.000000 unfurl-0.6.1/unfurl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 17:00:38.000000 unfurl-0.6.1/unfurl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-15 17:00:38.000000 unfurl-0.6.1/unfurl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 17:00:38.000000 unfurl-0.6.1/unfurl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-15 17:00:38.000000 unfurl-0.6.1/unfurl.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-15 17:00:38.000000 unfurl-0.6.1/unfurl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-15 17:00:38.000000 unfurl-0.6.1/unfurl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.987374 unfurl-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 08:01:57.000000 unfurl-0.6.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-04-29 08:01:57.000000 unfurl-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-04-29 08:02:00.987374 unfurl-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-29 08:01:57.000000 unfurl-0.6.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1218 2023-04-29 08:02:00.987374 unfurl-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-29 08:01:57.000000 unfurl-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.971373 unfurl-0.6.2/unfurl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43551 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/changelog-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34224 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/cloudmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49950 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/configurators/
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/dns-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/docker-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/helm-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16491 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/kompose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/supervisor-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20779 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29526 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/filter_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/filter_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/filter_plugins/ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45647 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57578 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55961 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/localenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/lookup_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/lookup_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/lookup_plugins/unfurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/manifest-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28145 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41448 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44834 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/planrequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21883 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/projectpaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30903 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26994 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39427 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51978 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58230 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/aws/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/dashboard/manifest.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/dashboard/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/digitalocean/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/gcp/unfurl.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/gitignore.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/home/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/home/manifest-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/home/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/local/ensemble-examples.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/local-unfurl-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/manifest-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/manifest.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/python3.10/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.10/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    72466 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.10/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/python3.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.11/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    68311 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.11/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/templates/python3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.7/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    74406 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.7/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/templates/python3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.8/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    74070 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.8/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/templates/python3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    73509 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.9/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/secrets.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/service-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/unfurl.local.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/unfurl.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    64983 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55031 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/tosca_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/artifacts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/googlecloud.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/k8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/localhost.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/tosca-ext.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/unfurl-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23855 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/vendor/sphinx-jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/vendor/sphinx-jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/vendor/sphinx-jsonschema/wide_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/dataentity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)    32477 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    33031 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/artifacttype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/capabilitytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/grouptype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15138 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/nodetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/policytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/portspectype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/property_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/relationshiptype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/scalarunit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/statefulentitytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/tosca_type_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17924 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/entity_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/exttools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.967373 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16716 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25407 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/nodetemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/prereq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/prereq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/prereq/csar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/relationship_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/substitution_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19241 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/topology_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/tosca_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/tpl_relationship_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/unsupportedtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.987374 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/gettextutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/urlutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/validateutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/yamlparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28193 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/yamlloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39094 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/yamlmanifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.971373 unfurl-0.6.2/unfurl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/top_level.txt
```

### Comparing `unfurl-0.6.1/LICENSE` & `unfurl-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/PKG-INFO` & `unfurl-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfurl
-Version: 0.6.1
+Version: 0.6.2
 Summary: use Git to record and deploy changes to your DevOps infrastructure
 Home-page: https://github.com/onecommons/unfurl
 Author: Adam Souzis
 Author-email: adam@onecommons.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -48,15 +48,15 @@
 
 1\. Use `unfurl init` to create an Unfurl-managed git repository. Or use `unfurl clone` to clone an existing one.
 
 2\. The repository will contain a few YAML files that you can edit. They will describe everything you'll need to deploy your application, such as:
 
 - Cloud provider and SaaS services account credentials and other secrets organized into environments.
 - Code repositories and container image registries.
-- A high-level model of your cloud infrastructure and their dependencies such as compute instances and databases, described using the [TOSCA](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=tosca) standard.
+- A high-level model of your cloud infrastructure and their dependencies such as compute instances and databases, described using the [OASIS TOSCA](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=tosca) (Topology and Orchestration Specification for Cloud Applications) standard.
 - Operations that invoke Terraform, Ansible, or other command-line tools (which Unfurl can automatically install).
 
 3\. Use `unfurl deploy` to deploy the infrastructure. Unfurl will generate a plan based on your target environment and high-level model and choose the correct operations to call. It will commit to git the latest configuration and a history of changes to your cloud accounts.
 
 4\. Now you have a reproducible description of your cloud infrastructure stored in git! So you can:
 
 - Push your repository to a git service such as Github or Gitlab to share it. For access control, each environment can be stored as separate git submodules or branches.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unfurl Version: 0.6.1 Summary: use Git to record
+Metadata-Version: 2.1 Name: unfurl Version: 0.6.2 Summary: use Git to record
 and deploy changes to your DevOps infrastructure Home-page: https://github.com/
 onecommons/unfurl Author: Adam Souzis Author-email: adam@onecommons.org
 License: MIT Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -25,24 +25,25 @@
 build open source software. ## How it works 1\. Use `unfurl init` to create an
 Unfurl-managed git repository. Or use `unfurl clone` to clone an existing one.
 2\. The repository will contain a few YAML files that you can edit. They will
 describe everything you'll need to deploy your application, such as: - Cloud
 provider and SaaS services account credentials and other secrets organized into
 environments. - Code repositories and container image registries. - A high-
 level model of your cloud infrastructure and their dependencies such as compute
-instances and databases, described using the [TOSCA](https://www.oasis-
-open.org/committees/tc_home.php?wg_abbrev=tosca) standard. - Operations that
-invoke Terraform, Ansible, or other command-line tools (which Unfurl can
-automatically install). 3\. Use `unfurl deploy` to deploy the infrastructure.
-Unfurl will generate a plan based on your target environment and high-level
-model and choose the correct operations to call. It will commit to git the
-latest configuration and a history of changes to your cloud accounts. 4\. Now
-you have a reproducible description of your cloud infrastructure stored in git!
-So you can: - Push your repository to a git service such as Github or Gitlab to
-share it. For access control, each environment can be stored as separate git
+instances and databases, described using the [OASIS TOSCA](https://www.oasis-
+open.org/committees/tc_home.php?wg_abbrev=tosca) (Topology and Orchestration
+Specification for Cloud Applications) standard. - Operations that invoke
+Terraform, Ansible, or other command-line tools (which Unfurl can automatically
+install). 3\. Use `unfurl deploy` to deploy the infrastructure. Unfurl will
+generate a plan based on your target environment and high-level model and
+choose the correct operations to call. It will commit to git the latest
+configuration and a history of changes to your cloud accounts. 4\. Now you have
+a reproducible description of your cloud infrastructure stored in git! So you
+can: - Push your repository to a git service such as Github or Gitlab to share
+it. For access control, each environment can be stored as separate git
 submodules or branches. - Pull incoming changes and review and approve pull
 requests before deploying. - Clone the repository and deploy to new
 environments even if they use different services -- because is your model is
 adaptable, manual changes are minimized. ## Features ### No server, agentless
 Simple, stand-alone CLI that can be used both in your local development
 environment or in an automated CI/CD pipeline. ### Deploy infrastructure from
 simple, application-centric descriptions - Model your cloud infrastructure with
```

### Comparing `unfurl-0.6.1/README.md` & `unfurl-0.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 1\. Use `unfurl init` to create an Unfurl-managed git repository. Or use `unfurl clone` to clone an existing one.
 
 2\. The repository will contain a few YAML files that you can edit. They will describe everything you'll need to deploy your application, such as:
 
 - Cloud provider and SaaS services account credentials and other secrets organized into environments.
 - Code repositories and container image registries.
-- A high-level model of your cloud infrastructure and their dependencies such as compute instances and databases, described using the [TOSCA](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=tosca) standard.
+- A high-level model of your cloud infrastructure and their dependencies such as compute instances and databases, described using the [OASIS TOSCA](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=tosca) (Topology and Orchestration Specification for Cloud Applications) standard.
 - Operations that invoke Terraform, Ansible, or other command-line tools (which Unfurl can automatically install).
 
 3\. Use `unfurl deploy` to deploy the infrastructure. Unfurl will generate a plan based on your target environment and high-level model and choose the correct operations to call. It will commit to git the latest configuration and a history of changes to your cloud accounts.
 
 4\. Now you have a reproducible description of your cloud infrastructure stored in git! So you can:
 
 - Push your repository to a git service such as Github or Gitlab to share it. For access control, each environment can be stored as separate git submodules or branches.
```

#### html2text {}

```diff
@@ -14,24 +14,25 @@
 build open source software. ## How it works 1\. Use `unfurl init` to create an
 Unfurl-managed git repository. Or use `unfurl clone` to clone an existing one.
 2\. The repository will contain a few YAML files that you can edit. They will
 describe everything you'll need to deploy your application, such as: - Cloud
 provider and SaaS services account credentials and other secrets organized into
 environments. - Code repositories and container image registries. - A high-
 level model of your cloud infrastructure and their dependencies such as compute
-instances and databases, described using the [TOSCA](https://www.oasis-
-open.org/committees/tc_home.php?wg_abbrev=tosca) standard. - Operations that
-invoke Terraform, Ansible, or other command-line tools (which Unfurl can
-automatically install). 3\. Use `unfurl deploy` to deploy the infrastructure.
-Unfurl will generate a plan based on your target environment and high-level
-model and choose the correct operations to call. It will commit to git the
-latest configuration and a history of changes to your cloud accounts. 4\. Now
-you have a reproducible description of your cloud infrastructure stored in git!
-So you can: - Push your repository to a git service such as Github or Gitlab to
-share it. For access control, each environment can be stored as separate git
+instances and databases, described using the [OASIS TOSCA](https://www.oasis-
+open.org/committees/tc_home.php?wg_abbrev=tosca) (Topology and Orchestration
+Specification for Cloud Applications) standard. - Operations that invoke
+Terraform, Ansible, or other command-line tools (which Unfurl can automatically
+install). 3\. Use `unfurl deploy` to deploy the infrastructure. Unfurl will
+generate a plan based on your target environment and high-level model and
+choose the correct operations to call. It will commit to git the latest
+configuration and a history of changes to your cloud accounts. 4\. Now you have
+a reproducible description of your cloud infrastructure stored in git! So you
+can: - Push your repository to a git service such as Github or Gitlab to share
+it. For access control, each environment can be stored as separate git
 submodules or branches. - Pull incoming changes and review and approve pull
 requests before deploying. - Clone the repository and deploy to new
 environments even if they use different services -- because is your model is
 adaptable, manual changes are minimized. ## Features ### No server, agentless
 Simple, stand-alone CLI that can be used both in your local development
 environment or in an automated CI/CD pipeline. ### Deploy infrastructure from
 simple, application-centric descriptions - Model your cloud infrastructure with
```

### Comparing `unfurl-0.6.1/setup.cfg` & `unfurl-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/__init__.py` & `unfurl-0.6.2/unfurl/__init__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/__main__.py` & `unfurl-0.6.2/unfurl/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 import sys
 import traceback
 from pathlib import Path
 from typing import Any, Optional, List, Union, TYPE_CHECKING
 from typing_extensions import Protocol
 
 import click
-import rich
 
 from . import DefaultNames, __version__, get_home_config_path, is_version_unreleased
 from . import init as initmod
 from . import logs, version_tuple
 from .job import start_job, Job
 from .localenv import LocalEnv, Project
 from .logs import Levels
@@ -1230,15 +1229,15 @@
 
 @cli.command()
 @click.pass_context
 @click.argument("ensemble", default=".", type=click.Path(exists=False))
 def validate(ctx, ensemble, **options):
     """Validate the given ensemble."""
     options.update(ctx.obj)
-    localEnv = LocalEnv(ensemble, options.get("home"))
+    localEnv = LocalEnv(ensemble, options.get("home"), override_context="")
     localEnv.get_manifest()
 
 
 @cli.command()
 @click.pass_context
 @click.option(
     "--semver",
@@ -1321,14 +1320,78 @@
     os.environ["UNFURL_SERVE_PATH"] = project_or_ensemble_path
     os.environ["UNFURL_CLONE_ROOT"] = clone_root
     from .server import serve as _serve
 
     _serve(address, port, secret, clone_root, project_or_ensemble_path, options)
 
 
+@cli.command(short_help="Manage a cloud map")
+@click.pass_context
+@click.argument("cloudmap", default="cloudmap")
+@click.option("--sync", default=None, help='Sync the given repository host ("local", name or url).')
+@click.option("--import", default=None, help='Update the cloudmap with the given repository host ("local", name or url).')
+@click.option(
+    "--namespace",
+    default=None,
+    help="Limit sync to the given repositories that match the given pattern.",
+)
+@click.option(
+    "--clone-root",
+    type=click.Path(exists=True),
+    help="Directory to clone repositories to.",
+)
+@click.option(
+    "--visibility",
+    type=click.Choice(["public", "any"]),
+    help='Only filter projects by visibility (overrides config).',
+)
+@click.option(
+    "--project",
+    type=click.Path(exists=True),
+    default=".",
+    help='Unfurl project to use. (Default: ".")',
+)
+def cloudmap(
+    ctx,
+    cloudmap: str,
+    sync: str,
+    project: str,
+    namespace: Optional[str] = None,
+    clone_root: Optional[str] = None,
+    visibility: Optional[str] = None,
+    **options,
+):
+    """Manage a cloud map.
+
+    [CLOUDMAP] is either a named cloudmap, a git url, or a local path.
+    (Default: "cloudmap")
+    """
+    from .cloudmap import CloudMap
+
+    options.update(ctx.obj)
+    localEnv = LocalEnv(project, options.get("home"), can_be_empty=True, readonly=True)
+    cloud_map = CloudMap.from_name(
+        localEnv, cloudmap, clone_root or "", sync, namespace or ""
+    )
+    if sync:
+        # sync is the provider name
+        cloud_map.sync(cloud_map.get_host(localEnv, sync, namespace or "", visibility))
+    elif options.get("import"):
+        host = cloud_map.get_host(localEnv, options.get("import") or "", namespace or "", visibility)
+        host.from_host(cloud_map.directory)
+        cloud_map.save(
+            f"Update cloudmap with latest from {'/'.join([host.name, host.path])}"
+        )
+    # elif clone_root:
+    #     cloud_map = CloudMap.from_name(localEnv, cloudmap, "local")
+    #     cloud_map.from_provider(namespace, download)
+    else:
+        print("nothing to do for", cloud_map)
+
+
 def main():
     obj = {"standalone_mode": False}
     try:
         rv = cli(standalone_mode=False, obj=obj)
         sys.exit(rv or 0)
     except click.Abort:
         click.secho("Aborted!", fg="red", err=True)
```

### Comparing `unfurl-0.6.1/unfurl/configurator.py` & `unfurl-0.6.2/unfurl/configurator.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,14 @@
         if name:
             register_class(cls.__module__ + "." + cls.__name__, cls, name)
         return cls
 
 
 @six.add_metaclass(AutoRegisterClass)
 class Configurator:
-
     short_name: Optional[str] = None
     """shortName can be used to customize the "short name" of the configurator
     as an alternative to using the full name ("module.class") when setting the implementation on an operation.
     (Titlecase recommended)"""
 
     exclude_from_digest: Tuple[str, ...] = ()
 
@@ -423,15 +422,15 @@
         self._inputs: Optional[ResultsMap] = None
         self._manifest = manifest
         self.messages: List[object] = []
         self._addedResources: List[NodeInstance] = []
         self._dependenciesChanged = False
         self.dependencies: List["Operational"] = dependencies or []
         self._resourceChanges = ResourceChanges()
-        self._workFolders: dict = {}
+        self._workFolders: Dict[str, WorkFolder] = {}
         self._rendering = False
         self._environ: object = None
         # public:
         self.operation_host = find_operation_host(target, configSpec.operation_host)
 
     @property
     def environ(self) -> Dict[str, str]:
@@ -1096,21 +1095,25 @@
             jobRequest = JobRequest(newResources, errors)
             if self.job:  # type: ignore
                 self.job.jobRequestQueue.append(jobRequest)  # type: ignore
             return jobRequest, errors
         return None, errors
 
     def set_work_folder(
-        self, location: str = "operation", preserve: Optional[bool] = None
+        self,
+        location: str = "operation",
+        preserve: Optional[bool] = None,
+        always_apply: bool = False,
     ) -> WorkFolder:
         if location in self._workFolders:
             return self._workFolders[location]
         if preserve is None:
             preserve = True if location in Folders.Persistent else False
         wf = WorkFolder(self, location, preserve)
+        wf.always_apply = always_apply
         self._workFolders[location] = wf
         return wf
         # XXX multiple tasks can be accessing the same workfolder, so:
         # return self.job.setFolder(
         #     self, location, preserve
         # )
 
@@ -1137,15 +1140,15 @@
             wf.failed()
 
     def apply_work_folders(self, *names: str) -> None:
         if not names:  # no args were passed, apply them all
             names = self._workFolders.keys()  # type: ignore
         for name in names:
             wf = self._workFolders.get(name)
-            if wf:
+            if wf and (wf.always_apply or self.status == Status.ok):  # type: ignore
                 wf.apply()
 
 
 class Dependency(Operational):
     """Represents a runtime dependency for a configuration.
 
     Dependencies are used to determine if a configuration needs re-run.
```

### Comparing `unfurl-0.6.1/unfurl/configurators/__init__.py` & `unfurl-0.6.2/unfurl/configurators/__init__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/ansible.py` & `unfurl-0.6.2/unfurl/configurators/ansible.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/dns-template.yaml` & `unfurl-0.6.2/unfurl/configurators/dns-template.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/dns.py` & `unfurl-0.6.2/unfurl/configurators/dns.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/docker-template.yaml` & `unfurl-0.6.2/unfurl/configurators/docker-template.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/gcp.py` & `unfurl-0.6.2/unfurl/configurators/gcp.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/helm-template.yaml` & `unfurl-0.6.2/unfurl/configurators/helm-template.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/k8s.py` & `unfurl-0.6.2/unfurl/configurators/k8s.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/kompose.py` & `unfurl-0.6.2/unfurl/configurators/kompose.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/shell.py` & `unfurl-0.6.2/unfurl/configurators/shell.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/supervisor-template.yaml` & `unfurl-0.6.2/unfurl/configurators/supervisor-template.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/supervisor.py` & `unfurl-0.6.2/unfurl/configurators/supervisor.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/configurators/terraform.py` & `unfurl-0.6.2/unfurl/configurators/terraform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (c) 2020 Adam Souzis
 # SPDX-License-Identifier: MIT
+from typing import TYPE_CHECKING
 from ..util import save_to_file, UnfurlTaskError, wrap_var, which
 from .shell import ShellConfigurator, clean_output, make_regex_filter
 from ..support import Status
 from ..result import Result
 from ..projectpaths import get_path, FilePath, Folders
 import json
 import os
@@ -483,15 +484,17 @@
                 with open(statePath) as sf:
                     state = json.load(sf)
                 state = mark_sensitive(
                     providerSchema, state, task, self.sensitive_names
                 )
                 # save state file in home as yaml, encrypting sensitive values
                 folderName = self._get_workfolder_name(task)
-                task.set_work_folder(folderName).write_file(
+                # set always_apply because we want to commit the terraform state file
+                # even if the terraform command failed (as it might have updated some resources)
+                task.set_work_folder(folderName, always_apply=True).write_file(
                     state, "terraform.tfstate.yaml"
                 )
                 outputs = {
                     name: wrap_var(attrs["value"])
                     for name, attrs in state["outputs"].items()
                 }
                 state.update(result.__dict__)
```

### Comparing `unfurl-0.6.1/unfurl/eval.py` & `unfurl-0.6.2/unfurl/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,23 +321,25 @@
     def __init__(
         self, exp: Union[str, Mapping], vars: dict = None, trace: Optional[int] = None
     ) -> None:
         self.vars = {"true": True, "false": False, "null": None}
 
         self.foreach = None
         self.select = None
+        self.strict = None
         trace = RefContext.DefaultTraceLevel if trace is None else trace
         self.trace = trace
         if isinstance(exp, Mapping):
             keys = list(exp)
             if keys and keys[0] not in _FuncsTop:
                 self.vars.update(exp.get("vars", {}))
                 self.foreach = exp.get("foreach")
                 self.select = exp.get("select")
                 self.trace = exp.get("trace", trace)
+                self.strict = exp.get("strict")
                 exp = exp.get("eval", exp.get("ref", exp))
 
         if vars:
             self.vars.update(vars)
         self.source = exp
 
     def resolve(
@@ -348,14 +350,17 @@
     ) -> Optional[Union[ResultsList, Result, List[Result], Any]]:
         """
         If wantList=True (default) returns a ResultList of matches
         Note that values in the list can be a list or None
         If wantList=False return `resolve_one` semantics
         If wantList='result' return a Result
         """
+        if self.strict is not None:
+            # overrides RefContext's strict
+            strict = self.strict
         ctx = ctx.copy(
             vars=self.vars, wantList=wantList, trace=self.trace, strict=strict
         )
         base_dir = getattr(self.source, "base_dir", None)
         if base_dir:
             ctx.base_dir = base_dir
         # $start is set in eval_ref but the user use that to override currentResource
@@ -417,15 +422,15 @@
         if isinstance(value, Mapping):
             if not value:
                 return False
             first = next(iter(value))
 
             if "ref" in value or "eval" in value:
                 return len(
-                    [x for x in ["vars", "trace", "foreach", "select"] if x in value]
+                    [x for x in ["vars", "trace", "foreach", "select", "strict"] if x in value]
                 ) + 1 == len(value)
             if len(value) == 1 and first in _FuncsTop:
                 return True
             return False
         return isinstance(value, Ref)
```

### Comparing `unfurl-0.6.1/unfurl/filter_plugins/ref.py` & `unfurl-0.6.2/unfurl/filter_plugins/ref.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/init.py` & `unfurl-0.6.2/unfurl/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -877,15 +877,15 @@
     def _needs_local_config(self, clonedProject):
         return self.skeleton_vars and not os.path.exists(
             os.path.join(clonedProject.projectRoot, "local", DefaultNames.LocalConfig)
         )
 
     def set_dest_project_and_path(
         self, existingSourceProject, existingDestProject, dest
-    ) -> bool:
+    ):
         assert self.dest_project is None
         if existingDestProject:
             #  set that as the dest_project
             self.dest_project = existingDestProject
         else:
             # otherwise set source_project as the dest_project
             self.dest_project = self.source_project
@@ -1030,23 +1030,22 @@
             builder.set_source(sourceProject)
             dest = os.path.abspath(dest)
 
     assert builder.source_project
 
     ##### step 2: create destination project if neccessary
     builder.set_dest_project_and_path(sourceProject, currentProject, dest)
+    if options.get("empty"):
+        # don't create an ensemble
+        return "Cloned empty project to " + builder.dest_project.projectRoot
 
     ##### step 3: examine source for template details and determine shared project
     builder.configure()
 
     ##### step 4 create ensemble in destination project if needed
-    if options.get("empty"):
-        # don't create an ensemble
-        return "Cloned empty project to " + builder.dest_project.projectRoot
-
     return builder.set_ensemble(isRemote, sourceProject, currentProject)
 
 
 def _create_local_config(clonedProject, logger, vars):
     local_template = os.path.join(
         clonedProject.projectRoot, DefaultNames.LocalConfigTemplate
     )
```

### Comparing `unfurl-0.6.1/unfurl/job.py` & `unfurl-0.6.2/unfurl/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,15 @@
         # XXX2 Check that configuration provided the metadata that it declared (check postCondition)
 
         if self.changeList:
             # merge changes together (will be saved with changeset)
             changes = self.changeList
             accum = changes.pop(0)
             while changes:
-                accum = merge_dicts(accum, changes.pop(0))
+                accum = cast(AttributeChanges, merge_dicts(accum, changes.pop(0)))
 
             # note: this might set _lastConfigChange on instances other than this target
             self._resourceChanges.update_changes(
                 accum, self._attributeManager.statuses, self.target, self.changeId
             )
             # XXX implement:
             # if not result.applied:
@@ -582,15 +582,15 @@
         super().__init__(self.parentJob, self.startTime, Status.ok, previousId)  # type: ignore
         self.dry_run = jobOptions.dryrun  # type: ignore
         self.jobOptions = jobOptions
         self.manifest = manifest
         self.rootResource = rootResource
         self.jobRequestQueue: List[JobRequest] = []
         self.unexpectedAbort: Optional[UnfurlError] = None
-        self.workDone: collections.OrderedDict = collections.OrderedDict()
+        self.workDone: Dict[int, ConfigTask] = collections.OrderedDict()
         self.timeElapsed: float = 0
         self.plan_requests: Optional[List[TaskRequestGroup]] = None
         self.task_count = 0
         self.external_requests: Optional[List[Tuple[Any, List[JobRequest]]]] = None
         self.external_jobs: Optional[List["Job"]] = None
 
     def get_operational_dependencies(self) -> Iterable[ConfigTask]:
@@ -786,16 +786,15 @@
                 manifest.commit_job(self)
             finally:
                 self.timeElapsed = perf_counter() - startTime
                 manifest.unlock()
 
     def _apply_workfolders(self) -> None:
         for task in self.workDone.values():
-            if task.status == Status.ok:
-                task.apply_work_folders()
+            task.apply_work_folders()
 
     def _update_joboption_instances(self) -> None:
         if not self.jobOptions.instances:  # type: ignore
             return
         # process any instances that are a full resource spec
         self.jobOptions.instances = [  # type: ignore
             resourceSpec
@@ -1127,15 +1126,15 @@
             return None, True
 
         task = req.task or self.create_task(
             req.configSpec, req.target, reason=req.reason
         )
         if task:
             start_collapsible(f"Task {req.target.name} ({req}", hash(req), True)
-            task.logger.info("started task.")
+            task.logger.info("started task.", extra=dict(json=task.summary(asJson=True)))
 
             resource = req.target
             startingStatus = resource._localStatus
             if req.startState is not None:
                 resource.state = req.startState
             startingState = resource.state
             self.add_work(task)
@@ -1176,15 +1175,16 @@
             #     task.target.state,
             #     req.startState,
             # )
             end_collapsible(hash(req))
             task_success = task.result and task.result.success
             status = task.target.status.name.upper()
             state_status = task.target.state.name if task.target.state else ""
-            extra = dict(rich=dict(style=task.target.status.color))
+            extra = dict(rich=dict(style=task.target.status.color),
+                         json=task.summary(asJson=True))
             if task_success:
                 task.logger.info(
                     "Task succeeded, Resource Status: %s State: %s",
                     status,
                     state_status,
                     extra=extra,
                 )
```

### Comparing `unfurl-0.6.1/unfurl/localenv.py` & `unfurl-0.6.2/unfurl/localenv.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,15 +609,15 @@
     def load_yaml_include(
         self,
         yamlConfig,
         templatePath,
         baseDir,
         warnWhenNotFound=False,
         expanded=None,
-        action=False,
+        action=None,
     ):
         """
         This is called while the YAML config is being loaded.
         Returns (url or fullpath, parsed yaml)
         """
         if isinstance(templatePath, dict):
             key = templatePath["file"]
@@ -625,18 +625,19 @@
         else:
             key = templatePath
             merge = None
 
         url_vars = {}
         url_vars.update(self.overrides)
         if action:
-            if isinstance(action, str):
-                return substitute_env(action, url_vars)
-            # check:
-            return True
+            if action.get_key:
+                return substitute_env(action.get_key, url_vars)
+            if action.check_include:
+                return True
+            return None  # unsupported action 
 
         if merge == "maplist" and "ENVIRONMENT" not in self.overrides:
             # don't load remote includes for LocalEnv that don't specify an environment
             # XXX (hackish way to avoid loads for transitory LocalEnv objects)
             logger.trace("skipping retrieving url with ENVIRONMENT: %s", key)
             return key, None
 
@@ -1281,14 +1282,15 @@
         return repo
 
     def find_or_create_working_dir(
         self,
         repoURL: str,
         revision: Optional[str] = None,
         basepath: Optional[str] = None,
+        checkout_args: dict = {},
     ) -> Tuple[Optional[GitRepo], Optional[str], Optional[bool]]:
         repo = self._find_git_repo(repoURL, revision)
         if isinstance(repo, GitRepo):
             logger.debug(
                 "Using existing repository at %s for %s", repo.working_dir, repoURL
             )
             if (
@@ -1306,16 +1308,19 @@
 
             repo = self._create_working_dir(repo, revision, basepath)
             if not repo:
                 return None, None, None
 
         assert isinstance(repo, GitRepo)
         if revision:
-            if repo.revision != repo.resolve_rev_spec(revision):
-                repo.checkout(revision)
+            if repo.revision != repo.resolve_rev_spec(revision) or checkout_args:
+                if repo.is_dirty():
+                    logger.warning(f"{repo.working_dir} is dirty, skipping checking out revision {revision}")
+                else:
+                    repo.checkout(revision, **checkout_args)
             return repo, repo.revision, False
         else:
             return repo, repo.revision, False
 
     def find_path_in_repos(
         self, path: str, importLoader: Optional[Any] = None
     ) -> Tuple[Optional[GitRepo], Optional[str], Optional[str], Optional[bool]]:
```

### Comparing `unfurl-0.6.1/unfurl/lock.py` & `unfurl-0.6.2/unfurl/lock.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/logs.py` & `unfurl-0.6.2/unfurl/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import collections.abc
+import json
 import logging
 import logging.config
 from enum import IntEnum
 import os
 import tempfile
 import time
 import types
@@ -129,14 +130,19 @@
         # the root logger.
         if record.name.startswith(HIDDEN_MSG_LOGGER):
             return
 
         level = Levels[record.levelname]
         try:
             console = getConsole(file=self.stream)
+            data = getattr(record, "json", None)
+            if data and os.environ.get("CI", False):
+                # Running in a CI environment (eg GitLab CI)
+                console.out(json.dumps(data), end="\x1b[2K\r", highlight=False, style=None)
+
             console.print(
                 f"[{self.RICH_STYLE_LEVEL[level]}] {level.name.center(8)}[/]", end=""
             )
             kw = dict(markup=False)
             if hasattr(record, "rich"):
                 kw.update(record.rich)  # type: ignore
             console.print(f" {record.name.upper()}", end="")
```

### Comparing `unfurl-0.6.1/unfurl/lookup_plugins/unfurl.py` & `unfurl-0.6.2/unfurl/lookup_plugins/unfurl.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/manifest-schema.json` & `unfurl-0.6.2/unfurl/manifest-schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999855407750144%*

 * *Differences: {"'definitions'": "{'environment': {'properties': {'cloudmaps': OrderedDict([('type', "*

 * *                  "'object')])}}}"}*

```diff
@@ -65,14 +65,17 @@
         "environment": {
             "$$target": [
                 "#/definitions/environment",
                 "./manifest-schema.json#/definitions/environment"
             ],
             "additionalProperties": true,
             "properties": {
+                "cloudmaps": {
+                    "type": "object"
+                },
                 "connections": {
                     "anyOf": [
                         {
                             "$ref": "#/definitions/namedObjects"
                         },
                         {
                             "type": "null"
```

### Comparing `unfurl-0.6.1/unfurl/manifest.py` & `unfurl-0.6.2/unfurl/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,14 +488,15 @@
             filePath = repo.find_repo_path(path)
             if filePath is not None:
                 return repo, filePath, repo.revision, False
         return None, None, None, None
 
     # NOTE: all the methods below may be called during config parse time via loadYamlInclude()
     def find_repo_from_git_url(self, path, isFile, importLoader):
+        revision: Optional[str]
         repoURL, filePath, revision = split_git_url(path)
         if not repoURL:
             raise UnfurlError(f"invalid git URL {path}")
         assert self.localEnv
         basePath = get_base_dir(importLoader.path)  # checks if dir or not
         repo, revision, bare = self.localEnv.find_or_create_working_dir(
             repoURL, revision, basePath
@@ -604,15 +605,15 @@
     def load_yaml_include(
         self,
         yamlConfig,
         templatePath,
         baseDir,
         warnWhenNotFound=False,
         expanded=None,
-        check=False,
+        action=None,
     ):
         """
         This is called while the YAML config is being loaded.
         Returns (url or fullpath, parsed yaml)
         """
 
         inlineRepository = None
@@ -626,24 +627,26 @@
                 # replace spec with just its name
                 artifactTpl["repository"] = reponame
                 assert repo.get("url"), f"bad inline repository definition: {repo}"
                 inlineRepository = {reponame: dict(url=repo["url"])}
         else:
             artifactTpl = dict(file=templatePath)
 
-        if check:
-            if isinstance(check, str):
-                return check
-            if not inlineRepository and "repository" in artifactTpl:
-                reponame = artifactTpl["repository"]
-                if reponame in ["spec", "self", "unfurl"]:  # builtin
-                    return True
-                repositories = self._get_repositories(expanded)
-                return reponame in repositories
-            return True
+        if action:
+            if action.get_key:
+                return action.get_key
+            if action.check_include:
+                if not inlineRepository and "repository" in artifactTpl:
+                    reponame = artifactTpl["repository"]
+                    if reponame in ["spec", "self", "unfurl"]:  # builtin
+                        return True
+                    repositories = self._get_repositories(expanded)
+                    return reponame in repositories
+                return True
+            return None  # unsupported action
 
         if not artifactTpl["file"]:
             msg = f"document include {templatePath} missing file (base: {baseDir})"
             if warnWhenNotFound:
                 logger.warning(msg)
                 return "", None
             raise UnfurlError(msg)
```

### Comparing `unfurl-0.6.1/unfurl/merge.py` & `unfurl-0.6.2/unfurl/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,33 +69,32 @@
     return factory
 
 
 # XXX?? because json keys are strings allow number keys to merge with lists
 # other values besides delete not supported because current code can leave those keys in final result
 mergeStrategyKey = "+%"  # supported values: "whiteout", "nullout", "merge", "error"
 
-
 # b is the merge patch, a is original dict
 def merge_dicts(
-    b,
-    a,
+    b: Mapping,
+    a: Mapping,
     cls=None,
     replaceKeys=None,
     defaultStrategy="merge",
     listStrategy="append_unique",
-):
+) -> dict:
     """
     Returns a new dict (or cls) that recursively merges b into a.
     b is base, a overrides.
 
     Similar to https://yaml.org/type/merge.html but does a recursive merge
     """
     if cls is not dict:
         cls = getattr(b, "mapCtor", cls or b.__class__)
-    cp = cls()
+    cp: dict = cls()
     skip = []
     for key, val in a.items():
         if key == mergeStrategyKey:
             continue
         if replaceKeys and key in replaceKeys:
             childStrategy = "replace"
         else:
@@ -427,15 +426,15 @@
     When appearing as a key in a map it will merge the result with the current dictionary.
     When appearing in a list it will insert the result in the list;
     if result is also a list, each item will be inserted separately.
     (If you don't want that behavior just wrap include in another list, e.g "[+list1]")
     """
     cp = cls()
     # first merge any includes includes into cp
-    templates = []
+    templates: List[Mapping] = []
     assert isinstance(current, Mapping), current
     for (key, value) in current.items():
         if not isinstance(key, str):
             cp[key] = value
             continue
         if key.startswith("+"):
             if key == mergeStrategyKey:
@@ -489,17 +488,18 @@
     for x in includes.values():
         for i in x:
             if isinstance(i, _MissingInclude):
                 yield i
 
 
 def _delete_deleted_keys(expanded):
-    for key, value in expanded.items():
+    for key in list(expanded):
+        value = expanded[key]
         if isinstance(value, Mapping):
-            if value.get(mergeStrategyKey) == "whiteout":
+            if value.get(mergeStrategyKey) in ["whiteout", "nullout"]:
                 del expanded[key]
             else:
                 _delete_deleted_keys(value)
 
 
 def expand_doc(doc, current=None, cls=dict):
     includes = cls()
@@ -511,15 +511,15 @@
     assert isinstance(expanded, Mapping), expanded
     if hasattr(doc, "_anchorCache"):
         expanded._anchorCache = doc._anchorCache  # type: ignore
     last = 0
     while True:
         missing = list(_find_missing_includes(includes))
         if len(missing) == 0:
-            # remove any stray keys with delete merge directive
+            # remove any stray merge directive that weren't applied
             _delete_deleted_keys(expanded)
             return includes, expanded
         if len(missing) == last:  # no progress
             raise UnfurlError(
                 "missing includes: %s"
                 % [f"{i.key.key}:{i.value or ''}" for i in missing]
             )
@@ -681,15 +681,15 @@
     expandedOriginalIncludes, expandedOriginalDoc = expand_doc(originalDoc, cls=cls)
     for key, value in includes.items():
         ref = lookup_path(changedDoc, key, cls)
         if ref is None:
             # inclusion point no longer exists
             continue
 
-        mergedIncludes: Dict = {}
+        mergedIncludes: Mapping = {}
         for (includeKey, includeValue) in value:
             if includeKey.include:
                 ref = None
                 continue
             stillHasTemplate = has_template(
                 changedDoc, includeKey, includeValue, key, cls
             )
```

### Comparing `unfurl-0.6.1/unfurl/packages.py` & `unfurl-0.6.2/unfurl/packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 from .repo import RepoView, is_url_or_git_path, split_git_url, get_remote_tags
 from .logs import getLogger
 from .util import UnfurlError
 from toscaparser.utils.validateutils import TOSCAVersionProperty
 
 logger = getLogger("unfurl")
 
+class UnfurlPackageUpdateNeeded(UnfurlError):
+    pass
+
 
 def is_semver(revision: Optional[str], include_unreleased=False) -> bool:
     """Return true if ``revision`` looks like a semver with major version >= 1"""
     return bool(
         revision
         and (include_unreleased or not revision.lstrip("v").startswith("0"))
         and TOSCAVersionProperty.VERSION_RE.match(revision) is not None
@@ -377,15 +380,16 @@
         existing = packages[package.package_id]
         if not existing:  # the repository isn't a package
             return None
         # we don't want different implementations of the same package so use the one
         # we already have. But we need to check if it compatible with the version requested here.
         if existing.repositories and not package.is_compatible_with(existing):
             # XXX if we need a later version, update the existing package and reload any content from it
-            # not yet implemented so just throw an error
+            # XXX update existing.repositories and invalidate associated file_refs in the cache
+            # XXX switch to raising UnfurlPackageUpdateNeeded after updating repositories and cache
             raise UnfurlError(
                 f"{package.package_id} has version {package.revision} but incompatible version {existing.revision} is already in use."
             )
         package = existing
 
     package.add_reference(repoview)
     return package
```

### Comparing `unfurl-0.6.1/unfurl/plan.py` & `unfurl-0.6.2/unfurl/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 raise UnfurlError(
                     f"specified template not found: {jobOptions.template}"
                 )
             self.filterTemplate = filterTemplate
         else:
             self.filterTemplate = None
 
-    def find_shadow_instance(self, template, match=is_external_template_compatible):
+    def find_shadow_instance(self, template: EntitySpec, match=is_external_template_compatible):
         imported = template.tpl.get("imported")
         if imported:
             external = self.root.imports.find_import(imported)
             if not external:
                 return None
             if external.shadow and external.root is self.root:
                 # shadowed instance already created
@@ -100,19 +100,19 @@
             if match(name, external.template, template):
                 if record.local_instance:
                     return record.local_instance
                 else:
                     return self.create_shadow_instance(external, name, template)
             if record.spec.get("instance") in ["root", "*"]:
                 # add root instance
-                searchAll.append((name, record.external_instance))
+                searchAll.append((name, external))
 
         # look in the topologies where were are importing everything
         for name, root in searchAll:
-            for external in root.get_self_and_descendents():
+            for external in root.get_self_and_descendants():
                 if match(name, external.template, template):
                     return self.create_shadow_instance(external, name, template)
 
         return None
 
     def create_shadow_instance(self, external, import_name, template):
         # create a local instance that "shadows" the external one we imported
@@ -961,32 +961,35 @@
                 operationHostSpec = templates.get(operation_host)
                 if operationHostSpec:
                     if operationHostSpec in seen:
                         continue
                     seen.add(operationHostSpec)
                     yield operationHostSpec
 
-        for ancestor in get_ancestor_templates(source.toscaEntityTemplate):
-            spec = templates.get(ancestor.name)
+        for spec in get_ancestor_templates(source, templates):
             if spec:
                 if spec is not source:
                     # ancestor is required by source
                     spec._isReferencedBy.append(source)  # type: ignore
                 if spec in seen:
                     continue
                 seen.add(spec)
                 yield spec
 
 
-def get_ancestor_templates(source):
-    # note: opposite direction as NodeSpec.relationships
-    for (rel, req, reqDef) in source.relationships:
-        if rel.target is not source:
-            for ancestor in get_ancestor_templates(rel.target):
-                yield ancestor
+def get_ancestor_templates(source, templates):
+    if not source.abstract:
+        # NodeTemplate.relationships return the node's requirements
+        # (the opposite of NodeSpec.relationships)
+        for (rel, req, reqDef) in source.toscaEntityTemplate.relationships:
+            if rel.target is not source.toscaEntityTemplate:
+                target = rel.target and templates.get(rel.target.name)
+                if target:
+                    for ancestor in get_ancestor_templates(target, templates):
+                        yield ancestor
     yield source
 
 
 def get_operational_dependents(resource, seen=None):
     if seen is None:
         seen = set()
     for dep in resource.get_operational_dependents():
```

### Comparing `unfurl-0.6.1/unfurl/planrequests.py` & `unfurl-0.6.2/unfurl/planrequests.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     find_schema_errors,
     UnfurlError,
     UnfurlTaskError,
     to_enum,
 )
 from .result import Result, ResultsList, serialize_value
 from .support import Defaults, NodeState, Priority, Status
-from .runtime import EntityInstance, InstanceKey
+from .runtime import EntityInstance, InstanceKey, HasInstancesInstance
 from .logs import getLogger
 import logging
 
 logger = getLogger("unfurl")
 
 
 # we want ConfigurationSpec to be independent of our object model and easily serializable
@@ -189,20 +189,22 @@
 
     def get_operation_artifacts(self):
         return []
 
     def include_in_plan(self):
         if self.task and self.task.priority == Priority.critical:
             return True  # XXX hackish, just used for primary_provider
-        if self.target.priority is not None:
-            return self.target.priority >= Priority.required
+        # calls self.target.template.required if _priority is None
+        priority = self.target.priority
+        if priority is not None:
+            return priority >= Priority.required
         if self.target.created:
             #  if already created then always include the resource
             return True
-        return self.target.template.required
+        return False
 
     def has_unfulfilled_refs(self) -> bool:
         for dep in self.get_unfulfilled_refs():
             return True
         return False
 
     def get_unfulfilled_refs(self, check_target="") -> Iterator["Dependency"]:
@@ -817,14 +819,15 @@
         error = UnfurlTaskError(task, "Configurator render failed", False)
     finally:
         task.restore_envvars()
     if task._errors:
         # we turned off strictness so templating errors got saved here instead
         req.render_errors = task._errors
         error = task._errors[0]
+        error_info = error.stackInfo  # type: ignore
         task._errors = []
     task._rendering = False
     task._attributeManager.mark_referenced_templates(task.target.template)
 
     workflow = req.group and req.group.workflow
     if workflow != "undeploy":
         # when removing an instance don't worry about depending values changing in the future
@@ -967,17 +970,17 @@
     for iDef in template.get_interfaces():
         if iDef.interfacename == interface or iDef.type == interface:
             if iDef.name == operation:
                 return iDef
     return default
 
 
-def find_resources_from_template_name(root, name):
+def find_resources_from_template_name(root: HasInstancesInstance, name: str):
     # XXX make faster
-    for resource in root.get_self_and_descendents():
+    for resource in root.get_self_and_descendants():
         if resource.template.name == name:
             yield resource
 
 
 def find_parent_template(source):
     for rel, req, reqDef in source.relationships:
         # special case "host" so it can be declared without full set of relationship / capability types
```

### Comparing `unfurl-0.6.1/unfurl/projectpaths.py` & `unfurl-0.6.2/unfurl/projectpaths.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,15 @@
     Updates to these directories through this class are performed transactionally --
     accessing a directory through this class marks it for writing and creates a
     copy of it in the ``planning`` directory.
 
     If a task completes successfully ``apply()`` is called, which copies it back to the
     permanent location of the folder.
     """
+    always_apply = False
 
     def __init__(self, task, location, preserve):
         self.task = task  # owner
         self.pending_state = True
         self.location = location
         self.preserve = preserve
         # the permanent location:
```

### Comparing `unfurl-0.6.1/unfurl/repo.py` & `unfurl-0.6.2/unfurl/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: MIT
 import abc
 import os
 import os.path
 from pathlib import Path
 import sys
 from functools import lru_cache
-from typing import TYPE_CHECKING, Dict, List, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
 from typing_extensions import Literal
 import git
 import git.exc
 
 from .logs import getLogger, PY_COLORS
 from urllib.parse import urlparse
 from .util import UnfurlError, save_to_file
@@ -43,15 +43,21 @@
 
 def normalize_git_url(url: str, hard: int = 0):
     if url.startswith("git-local://"):  # truncate url after commit digest
         return "git-local://" + urlparse(url).netloc.partition(":")[0]
 
     if "://" not in url:  # not an absolute URL, convert some common patterns
         if url.startswith("/"):
-            return "file://" + url
+            # abspath also normalizes the path
+            return "file://" + os.path.abspath(url)
+        elif url.startswith("~"):
+            return "file://" + os.path.abspath(os.path.expanduser(url))
+        elif url.startswith("file:"):
+            # git doesn't like relative file URLs
+            return "file://" + os.path.abspath(os.path.expanduser(url[5:]))
         elif "@" in url:  # scp style used by git: user@server:project.git
             # convert to ssh://user@server/project.git
             url = "ssh://" + url.replace(":", "/", 1)
     if hard:
         parts = urlparse(url)
         # remove password and .git
         user, sep, host = parts.netloc.rpartition("@")
@@ -97,22 +103,22 @@
         return True
     candidate, sep, frag = url.partition("#")
     if frag or candidate.rstrip("/").endswith(".git"):
         return True
     return False
 
 
-def split_git_url(url):
+def split_git_url(url) -> Tuple[str, str, str]:
     """
     Returns (repoURL, filePath, revision)
     RepoURL will be an empty string if it isn't a path to a git repo
     """
     if url.startswith("--"):
         # security: see https://github.com/gitpython-developers/GitPython/issues/1517
-        return False
+        return "", "", ""
     parts = urlparse(url)
     if parts.scheme == "git-local":
         return parts.scheme + "://" + parts.netloc, parts.path[1:], parts.fragment
 
     if parts.fragment:
         # treat fragment as a git revision spec; see https://git-scm.com/docs/gitrevisions
         # or https://docs.docker.com/engine/reference/commandline/build/#git-repositories
@@ -205,14 +211,18 @@
         ...
 
     @property
     @abc.abstractmethod
     def revision(self) -> str:
         ...
 
+    @property
+    def safe_url(self):
+        return sanitize_url(self.url, True)
+
     def find_repo_path(self, path):
         localPath = self.find_path(path)[0]
         if localPath is not None and not self.is_path_excluded(localPath):
             return localPath
         return None
 
     def is_path_excluded(self, localPath):
@@ -256,28 +266,33 @@
         assert not name.endswith(".git"), name
         return name
 
     def project_path(self) -> str:
         return self.get_path_for_git_repo(self.url, False)
 
     @classmethod
-    def create_working_dir(cls, gitUrl, localRepoPath, revision=None):
+    def create_working_dir(cls, gitUrl, localRepoPath, revision=None, depth=1):
         localRepoPath = localRepoPath or "."
         if os.path.exists(localRepoPath):
             if not os.path.isdir(localRepoPath) or os.listdir(localRepoPath):
                 raise UnfurlError(
                     f"couldn't create directory, it already exists and isn't empty: {localRepoPath}"
                 )
         parent_dir = os.path.dirname(localRepoPath)
         if parent_dir.strip("/"):
             os.makedirs(parent_dir, exist_ok=True)
         cleanurl = sanitize_url(gitUrl)
         logger.info("Fetching %s %s to %s", cleanurl, revision or "", localRepoPath)
-        kwargs = dict(recurse_submodules=True, depth=1, no_single_branch=True)
-        non_interactive = os.getenv("CI") or not PY_COLORS  # or color out disabled
+        kwargs: Dict[str, Any] = dict(recurse_submodules=True, no_single_branch=True)
+        if depth == 1:
+            kwargs["depth"] = depth
+            kwargs["shallow_submodules"] = True
+        non_interactive = (
+            os.getenv("CI") or not PY_COLORS
+        )  # if CI or color output disabled
         if not non_interactive:
             # we're running in an interactive session
             progress = _ProgressPrinter()
             progress.gitUrl = cleanurl
             kwargs["progress"] = progress  # type: ignore
         try:
             if revision:
@@ -335,14 +350,15 @@
             name = tpl.pop("name")
             tpl["url"] = normalize_git_url(tpl["url"])
             repository = Repository(name, tpl)
         assert repository or repo
         self.repository: Repository = repository
         self.yaml = None
         self.revision: Optional[str] = None
+        self.file_refs: List[str] = []
         self.set_repo_and_path(repo, path)
         self.package: Optional[Union[Literal[False], "Package"]] = None
 
     def set_repo_and_path(self, repo: Optional["GitRepo"], path: str):
         self.repo = repo
         self.path = path
         if repo and path and self.repository:
@@ -392,14 +408,18 @@
     def is_dirty(self):
         if self.readOnly or not self.repo:
             return False
         for filepath, dotsecrets in find_dirty_secrets(self.working_dir):
             return True
         return self.repo.is_dirty(untracked_files=True, path=self.path)
 
+    def add_file_ref(self, file_name: str):
+        if file_name not in self.file_refs:
+            self.file_refs.append(file_name)
+
     def add_all(self):
         assert not self.readOnly and self.repo
         self.repo.repo.git.add("--all", self.path or ".")
 
     def load_secrets(self, _loader):
         logger.trace("looking for secrets %s", self.working_dir)
         for root, dirs, files in os.walk(self.working_dir):
@@ -644,18 +664,18 @@
             path = os.path.abspath(path)[len(self.working_dir) :]
         # XXX this won't work if path is in a submodule
         # if in path startswith a submodule: git log -1 -p [commitid] --  [submodule]
         # submoduleCommit = re."\+Subproject commit (.+)".group(1)
         # return self.repo.submodules[submodule].git.show(submoduleCommit+':'+path[len(submodule)+1:])
         return self.repo.git.show(commitId + ":" + path)
 
-    def checkout(self, revision=""):
+    def checkout(self, revision="", **kw):
         # if revision isn't specified and repo is not pinned:
         #  save the ref of current head
-        self.repo.git.checkout(revision)
+        self.repo.git.checkout(revision, **kw)
         logger.info(
             "checking out '%s' at %s to %s",
             self.url,
             revision or "HEAD",
             self.working_dir,
         )
         return self.working_dir
@@ -691,31 +711,33 @@
         # https://gitpython.readthedocs.io/en/stable/reference.html?highlight=is_dirty#git.repo.base.Repo.is_dirty
         return self.repo.is_dirty(untracked_files=untracked_files, path=path or None)
 
     def pull(
         self, remote="origin", revision=None, ff_only=True, with_exceptions=False, **kw
     ) -> bool:
         if remote in self.repo.remotes:
-            cmd = ["pull", remote, revision or "HEAD"]
+            cmd = ["pull", remote, revision or "HEAD", "--tags"]
             if ff_only:
                 cmd.append("--ff-only")
             code, out, err = self.run_cmd(cmd, with_exceptions=with_exceptions, **kw)
             if code:
                 logger.info(
-                    "attempt to pull latest from %s into %s failed: %s %s",
+                    "attempt to pull latest from %s %s into %s failed: %s %s",
                     sanitize_url(self.url, True),
+                    revision or "",
                     self.working_dir,
                     out,
                     err,
                 )
                 return False
             else:
                 logger.verbose(
-                    "pull latest from %s into %s: %s %s",
+                    "pull latest from %s %s into %s: %s %s",
                     sanitize_url(self.url, True),
+                    revision or "",
                     self.working_dir,
                     out,
                     err,
                 )
                 return True
         else:
             return False
```

### Comparing `unfurl-0.6.1/unfurl/reporting.py` & `unfurl-0.6.2/unfurl/reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 from rich import box
 from rich.segment import Segment
 from rich.markup import escape
 import re
 import os
 
 if TYPE_CHECKING:
-    from unfurl.yamlmanifest import YamlManifest
+    from .yamlmanifest import YamlManifest
     from rich.console import RenderableType
     from rich.style import StyleType
+    from .job import Job
 
 logger = getLogger("unfurl")
 
 
 class JobTable(Table):
     def __init__(self, **kwargs):
         super().__init__(box=box.HORIZONTALS, show_lines=True, expand=True, **kwargs)
@@ -150,15 +151,15 @@
                     request.children, target, sequence, include_rendered, workflow
                 )
             else:
                 summary_list.append(request._summary_dict(include_rendered))
 
     @staticmethod
     def json_plan_summary(
-        job, pretty: bool = False, include_rendered: bool = True
+        job: "Job", pretty: bool = False, include_rendered: bool = True
     ) -> Union[str, list]:
         """
         Return a list of items that look like:
 
           {
           instance: target_name,
           status: target_status,
@@ -200,15 +201,15 @@
             return "{total} tasks ({changed} changed, {ok} ok, {error} failed, {unknown} unknown, {skipped} skipped)".format(
                 **stats
             )
         return stats
 
     @staticmethod
     def plan_summary(
-        job,
+        job: "Job",
         plan_requests: List[TaskRequest],
         external_requests: Iterable[Tuple[Any, Any]],
     ) -> Tuple[str, int]:
         """
         Node "site" (status, state, created):
           check: Install.check
           workflow: # if group
@@ -275,37 +276,38 @@
                             output.append(" " * indent + "   (errors while rendering)")
 
         opts = job.jobOptions.get_user_settings()
         options = ",".join([f"{k} = {opts[k]}" for k in opts if k != "planOnly"])
         header = f"Plan for {job.workflow}"  # type: ignore
         if options:
             header += f" ({options})"
-        output = [header + ":\n"]
+        output: List[str] = [header + ":\n"]
 
         for m, jr in external_requests:
             if jr:
                 count += 1
                 output += [f" External jobs on {m.path}:"]
                 for j in jr:
                     output.append(" " * INDENT + j.name)
 
         _summary(plan_requests, None, 0)  # type: ignore
         if not count:
             output.append("Nothing to do.")
         return "\n".join(output), count
 
     @staticmethod
-    def summary_table(job) -> str:
+    def summary_table(job: "Job") -> str:
         console = getConsole(record=True)
         if not job.workDone:
             console.print(
                 f"Job {job.changeId} completed: [{job.status.color}]{job.status.name}[/]. No tasks ran."
             )
             return console.export_text()
 
+        logger.info("", extra=dict(json=job.json_summary()))
         title = "Job %s completed in %.3fs: [%s]%s[/]. %s:\n    " % (
             job.changeId,
             job.timeElapsed,
             job.status.color,
             job.status.name,
             job.stats(asMessage=True),
         )
```

### Comparing `unfurl-0.6.1/unfurl/result.py` & `unfurl-0.6.2/unfurl/result.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/runtime.py` & `unfurl-0.6.2/unfurl/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 from datetime import datetime
 import os
 from typing import (
     Any,
     Dict,
     Iterable,
+    Iterator,
     List,
     Optional,
     Union,
     TYPE_CHECKING,
     cast,
     NewType,
     AnyStr,
@@ -358,18 +359,18 @@
     def __init__(self, resource):
         self.resource = resource
 
     def __getitem__(self, key):
         return self.resource.find_resource(key)
 
     def __iter__(self):
-        return iter(r.name for r in self.resource.get_self_and_descendents())
+        return iter(r.name for r in self.resource.get_self_and_descendants())
 
     def __len__(self):
-        return len(tuple(self.resource.get_self_and_descendents()))
+        return len(tuple(self.resource.get_self_and_descendants()))
 
 
 class EntityInstance(OperationalInstance, ResourceRef):
     attributeManager: Optional[AttributeManager] = None
     created: Optional[Union[bool, str]] = None
     protected: Optional[bool] = None
     imports: Optional[Imports] = None
@@ -604,35 +605,40 @@
         if parent:
             # only node instances have unique names
             if parent.root.find_resource(name):
                 raise UnfurlError(
                     f'can not create node instance "{name}", its name is already in use'
                 )
 
-        self.instances = []
+        self.instances: List[HasInstancesInstance] = []
         EntityInstance.__init__(self, name, attributes, parent, template, status)
         if self.root is self:
             self._all = _ChildResources(self)
             self._templar = Templar(DataLoader())
             self._environ = os.environ.copy()
 
     @property
     def key(self) -> InstanceKey:
         return cast(InstanceKey, f"::{self.name}")
 
-    def get_self_and_descendents(self):
+    def get_self_and_descendants(self) -> Iterator["HasInstancesInstance"]:
         "Recursive descendent including self"
         yield self
         for r in self.instances:
-            for descendent in r.get_self_and_descendents():
+            for descendent in r.get_self_and_descendants():
                 yield descendent
 
     @property
+    def descendants(self):
+        return list(self.get_self_and_descendants())
+
+    @property
     def descendents(self):
-        return list(self.get_self_and_descendents())
+        # backward compatibility
+        return self.descendants
 
     # XXX use find_instance instead and remove find_resource
     def find_resource(self, resourceid):
         if self.name == resourceid:
             return self
         for r in self.instances:
             child = r.find_resource(resourceid)
@@ -1089,15 +1095,14 @@
 
     def __init__(self, template, status=None):
         attributes = dict(inputs=template.inputs, outputs=template.outputs)
         HasInstancesInstance.__init__(self, "root", attributes, None, template, status)
 
         self._relationships = None
         self._tmpDir = None
-        self.imports = None
 
     def set_base_dir(self, baseDir):
         self._baseDir = baseDir
         if not self._templar or self._templar._basedir != baseDir:
             loader = DataLoader()
             loader.set_basedir(baseDir)
             self._templar = Templar(loader)
```

### Comparing `unfurl-0.6.1/unfurl/server.py` & `unfurl-0.6.2/unfurl/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from flask_caching import Cache
 from flask_cors import CORS
 
 import git
 from git.objects import Commit
 
 from unfurl.projectpaths import rmtree
-from .localenv import LocalEnv
-from .repo import GitRepo, add_user_to_url, normalize_git_url_hard, sanitize_url
+from .localenv import LocalEnv, Project
+from .repo import GitRepo, Repo, add_user_to_url, normalize_git_url_hard, sanitize_url
 from .util import UnfurlError, get_package_digest
 from .logs import getLogger, add_log_file
 from .yamlmanifest import YamlManifest
 from . import to_json
 from . import init
 from . import __version__
 
@@ -70,14 +70,54 @@
 app.config["UNFURL_SECRET"] = os.getenv("UNFURL_SERVE_SECRET")
 cors = app.config["UNFURL_SERVE_CORS"] = os.getenv("UNFURL_SERVE_CORS")
 if cors:
     CORS(app, origins=cors.split())
 os.environ["GIT_TERMINAL_PROMPT"] = "0"
 
 
+def clear_cache(cache: Cache, starts_with: str) -> Optional[List[Any]]:
+    backend = cache.cache
+    backend.ignore_errors = True
+    redis = getattr(backend, "_read_client", None)
+    if redis:
+        keys = [k.decode()[len(backend.key_prefix) :] for k in redis.keys(backend.key_prefix + starts_with + "*")]  # type: ignore
+    else:
+        simple = getattr(backend, "_cache", None)
+        if simple is not None:
+            keys = [key for key in simple if key.startswith(starts_with)]
+        else:
+            logger.error(
+                f"clearing cache prefix '{starts_with}': couldn't find cache {type(backend)}"
+            )
+            return None
+    logger.info(f"clearing cache {starts_with}, found keys: {repr(keys)}, {len(keys)}")
+    return cache.delete_many(*keys)  # type: ignore
+
+
+def clear_all(cache, prefix):
+    backend = cache.cache
+    redis = getattr(backend, "_write_client", None)
+    if redis:
+        keys = redis.keys(pattern=prefix + "*")
+        if keys:
+            redis.delete(*keys)
+    else:
+        clear_cache(cache, "")
+
+
+if os.environ.get("CACHE_CLEAR_ON_START"):
+    prefix = os.environ.get("CACHE_CLEAR_ON_START")
+    # if set, use the given prefix, otherwise the current prefix
+    if prefix in ["1", "true"]:
+        prefix = flask_config["CACHE_KEY_PREFIX"]
+    clear_all(cache, prefix)
+
+DEFAULT_BRANCH = "main"
+
+
 def set_current_ensemble_git_url():
     project_or_ensemble_path = os.getenv("UNFURL_SERVE_PATH")
     if not project_or_ensemble_path:
         return
     try:
         local_env = LocalEnv(project_or_ensemble_path, can_be_empty=True)
         if (
@@ -103,23 +143,25 @@
 def get_project_id(request):
     project_id = request.args.get("auth_project")
     if project_id:
         return project_id
     return ""
 
 
-def _get_project_repo_dir(project_id: str) -> str:
+def _get_project_repo_dir(project_id: str, branch: str) -> str:
     clone_root = current_app.config.get("UNFURL_CLONE_ROOT", ".")
-    return os.path.join(clone_root, project_id)
+    if not project_id:
+        return clone_root
+    return os.path.join(clone_root, project_id, branch)
 
 
 def _get_project_repo(
-    project_id: str, args: Optional[dict] = None
+    project_id: str, branch: str, args: Optional[dict] = None
 ) -> Optional[GitRepo]:
-    path = _get_project_repo_dir(project_id)
+    path = _get_project_repo_dir(project_id, branch)
     if os.path.isdir(path):
         repo = GitRepo(git.Repo(path))
         if args:
             # make sure we are using the latest credentials:
             username, password = args.get("username"), args.get(
                 "private_token", args.get("password")
             )
@@ -156,15 +198,15 @@
     key: str
     repo: Optional[GitRepo] = None
     strict: bool = False
     commitinfo: Union[bool, Optional["Commit"]] = None
     hit: Optional[bool] = None
 
     def _set_project_repo(self) -> Optional[GitRepo]:
-        self.repo = _get_project_repo(self.project_id)
+        self.repo = _get_project_repo(self.project_id, self.branch or DEFAULT_BRANCH)
         return self.repo
 
     def cache_key(self) -> str:
         return f"{self.project_id}:{self.branch or ''}:{self.file_path}:{self.key}"
 
     def _inflight_key(self) -> str:
         return "_inflight::" + self.cache_key()
@@ -367,33 +409,14 @@
         found_inflight = self._cancel_inflight(cache)
         # skip caching work if not `found_inflight` -- that means invalidate_cache deleted it
         if found_inflight and not err:
             self.set_cache(cache, latest_commit, value)
         return err, value
 
 
-def clear_cache(cache: Cache, starts_with: str) -> Optional[List[Any]]:
-    backend = cache.cache
-    backend.ignore_errors = True
-    redis = getattr(backend, "_read_client", None)
-    if redis:
-        keys = [k.decode()[len(backend.key_prefix) :] for k in redis.keys(backend.key_prefix + starts_with + "*")]  # type: ignore
-    else:
-        simple = getattr(backend, "_cache", None)
-        if simple:
-            keys = [key for key in simple if key.startswith(starts_with)]
-        else:
-            logger.error(
-                f"clearing cache prefix '{starts_with}': couldn't find cache {type(backend)}"
-            )
-            return None
-    logger.info(f"clearing cache {starts_with}, found keys: {repr(keys)}, {len(keys)}")
-    return cache.delete_many(*keys)  # type: ignore
-
-
 @app.before_request
 def hook():
     """
     Run before every request. If the secret is specified, check all requests for the secret.
     Secret can be in the secret query parameter (localhost:8080/health?secret=<secret>) or as an
     Authorization bearer token (Authorization=Bearer <secret>).
     """
@@ -405,15 +428,17 @@
     header_secret = request.headers.get(
         "Authorization"
     )  # Get secret from Authorization header
     if header_secret is not None:
         try:
             # Remove "Bearer " from header
             header_secret = header_secret.split(" ")[1]
-        except IndexError:  # Quick sanity check to make sure the header is formatted correctly
+        except (
+            IndexError
+        ):  # Quick sanity check to make sure the header is formatted correctly
             return create_error_response(
                 "BAD_REQUEST",
                 "The Authorization header must be in the format 'Bearer <secret>'",
             )
 
     if secret not in [
         qs_secret,
@@ -444,39 +469,37 @@
             netloc = f"{username}:{password}@{url_parts.netloc}"
         else:
             netloc = f"{username}@{url_parts.netloc}"
         base_url = urlunsplit(url_parts._replace(netloc=netloc))
     return urljoin(base_url, project_id + ".git")
 
 
-def _stage(project_id: str, args: dict, pull: bool) -> Optional[str]:
+def _stage(project_id: str, branch: str, args: dict, pull: bool) -> Optional[str]:
     """
     Clones or pulls the latest from the given project repository and returns the repository's working directory
     or None if clone failed.
     """
     username, password = args.get("username"), args.get(
         "private_token", args.get("password")
     )
     repo = None
-    repo_path = _get_project_repo_dir(project_id)
-    repo = _get_project_repo(project_id, args)
+    repo_path = _get_project_repo_dir(project_id, branch)
+    repo = _get_project_repo(project_id, branch, args)
     if repo:
         logger.info(f"found repo at {repo.working_dir}")
         if pull and not repo.is_dirty():
             repo.pull(with_exceptions=True)
     else:
         # repo doesn't exists, clone it
         os.makedirs(os.path.dirname(repo_path), exist_ok=True)
         git_url = get_project_url(project_id, username, password)
-        result = init.clone(git_url, repo_path, empty=True)
-        clean_url = sanitize_url(git_url, True)
-        logger.info(f"cloned {clean_url}: {result} in pid {os.getpid()}")
-        repo = _get_project_repo(project_id)
+        Repo.create_working_dir(git_url, repo_path, branch)
+        repo = _get_project_repo(project_id, branch)
         if repo:
-            logger.info("clone success: %s to %s", clean_url, repo.working_dir)
+            logger.info("clone success: %s to %s", repo.safe_url, repo.working_dir)
     return repo and repo.working_dir or None
 
 
 def _get_filepath(format, deployment_path):
     if deployment_path:
         if not deployment_path.endswith(".yaml"):
             return os.path.join(deployment_path, "ensemble.yaml")
@@ -494,15 +517,15 @@
         return "blueprint"
     elif path.endswith("unfurl.yaml"):
         return "environments"
     else:
         return "deployment"
 
 
-def _cache_work(args: dict, cache_entry: CacheEntry, latest_commit: str) -> Any:
+def _export_cache_work(args: dict, cache_entry: CacheEntry, latest_commit: str) -> Any:
     return _do_export(
         cache_entry.project_id,
         cache_entry.key,
         cache_entry.file_path,
         cache_entry,
         latest_commit,
         args,
@@ -527,16 +550,15 @@
     return True
 
 
 def _make_etag(latest_commit: str):
     return f'W/"{latest_commit}"'
 
 
-def json_response(obj, pretty):
-    dump_args: Dict = {}
+def json_response(obj, pretty, **dump_args):
     if pretty:
         dump_args.setdefault("indent", 2)
     else:
         dump_args.setdefault("separators", (",", ":"))
 
     dumps = flask.json.dumps
     mimetype = current_app.config["JSONIFY_MIMETYPE"]
@@ -557,25 +579,25 @@
         )
 
     latest_commit = request.args.get("latest_commit")
     project_id = get_project_id(request)
     deployment_path = request.args.get("deployment_path") or ""
     cache_entry = None
     file_path = _get_filepath(requested_format, deployment_path)
-    branch = request.args.get("branch")
+    branch = request.args.get("branch", DEFAULT_BRANCH)
     if request.headers.get("X-Git-Credentials"):
         args = dict(request.args)
         args["username"], args["password"] = (
             b64decode(request.headers["X-Git-Credentials"]).decode().split(":", 1)
         )
     else:
         args = request.args
 
-    repo = _get_project_repo(project_id, args)
-    workfn = partial(_cache_work, args)
+    repo = _get_project_repo(project_id, branch, args)
+    workfn = partial(_export_cache_work, args)
     cache_entry = CacheEntry(project_id, branch, file_path, requested_format, repo)
     err, json_summary = cache_entry.get_or_set(
         cache, workfn, latest_commit, _validate_export
     )
     if not err:
         hit = cache_entry and cache_entry.hit
         if request.args.get("include_all_deployments"):
@@ -594,29 +616,31 @@
                     hit = hit and dcache_entry.hit
             json_summary["deployments"] = deployments
         if hit:
             etag = request.headers.get("If-None-Match")
             if latest_commit and _make_etag(latest_commit) == etag:
                 return "Not Modified", 304
 
-        response = json_response(json_summary, request.args.get("pretty"))
+        response = json_response(
+            json_summary, request.args.get("pretty"), sort_keys=False
+        )
         if latest_commit:
             response.headers["Etag"] = _make_etag(latest_commit)
         return response
     else:
         if isinstance(err, Exception):
             return create_error_response("INTERNAL_ERROR", "An internal error occurred")
         else:
             return err
 
 
 @app.route("/populate_cache", methods=["POST"])
 def populate_cache():
     project_id = get_project_id(request)
-    branch = request.args.get("branch")
+    branch = request.args.get("branch", DEFAULT_BRANCH)
     path = request.args["path"]
     latest_commit = request.args["latest_commit"]
     requested_format = format_from_path(path)
     removed = request.args.get("removed")
     cache_entry = CacheEntry(project_id, branch, path, requested_format)
     visibility = request.args.get("visibility")
     logger.info(
@@ -626,22 +650,22 @@
         removed,
         visibility,
     )
     if removed and removed not in ["0", "false"]:
         cache_entry.delete_cache(cache)
         cache_entry._cancel_inflight(cache)
         return "OK"
-    project_dir = _get_project_repo_dir(project_id)
+    project_dir = _get_project_repo_dir(project_id, branch)
     if not os.path.isdir(project_dir):
         # don't try to clone private repository
         if visibility != "public":
             logger.info("skipping populate cache for private repository %s", project_id)
             return "OK"
     err, json_summary = cache_entry.get_or_set(
-        cache, partial(_cache_work, request.args), latest_commit
+        cache, partial(_export_cache_work, request.args), latest_commit
     )
     if err:
         if isinstance(err, Exception):
             return create_error_response("INTERNAL_ERROR", "An internal error occurred")
         else:
             return err
     else:
@@ -651,15 +675,15 @@
 @app.route("/clear_project_file_cache", methods=["POST"])
 def clear_project():
     project_id = get_project_id(request)
     return _clear_project(project_id)
 
 
 def _clear_project(project_id):
-    project_dir = _get_project_repo_dir(project_id)
+    project_dir = _get_project_repo_dir(project_id, "")
     if os.path.isdir(project_dir):
         logger.info("clear_project: removing %s", project_dir)
         rmtree(project_dir, logger)
     else:
         logger.info("clear_project: %s not found", project_id)
     cleared = clear_cache(cache, project_id + ":")
     if cleared is None:
@@ -697,112 +721,94 @@
         localEnv and localEnv.project and os.path.isdir(localEnv.project.projectRoot)
     )
 
 
 def _localenv_from_cache(
     cache,
     project_id: str,
-    branch: Optional[str],
+    branch: str,
     deployment_path: str,
     latest_commit: str,
     args: dict,
 ) -> Tuple[Any, Optional[LocalEnv]]:
     # we want to make cloning a project cache work to prevent concurrent cloning
     def _cache_localenv_work(
         cache_entry: CacheEntry, latest_commit: str
     ) -> Tuple[Any, Any]:
         # don't try to pull -- cache will have already pulled
-        # or _localenv_from_cache_pull will do it next if needed
-        clone_location = _fetch_working_dir(cache_entry.project_id, args, False)
+        clone_location = _fetch_working_dir(cache_entry.project_id, branch, args, False)
         if clone_location is None:
             return (
                 create_error_response("INTERNAL_ERROR", "Could not find repository"),
                 None,
             )
         clone_location = os.path.join(clone_location, deployment_path)
         return _make_readonly_localenv(clone_location)
 
-    repo = _get_project_repo(project_id, args)
+    repo = _get_project_repo(project_id, branch, args)
     return CacheEntry(
         project_id, branch, "unfurl.yaml", "localenv", repo, bool(latest_commit)
     ).get_or_set(cache, _cache_localenv_work, latest_commit, _validate_localenv)
 
 
 def _localenv_from_cache_pull(
     cache,
     project_id: str,
-    branch: Optional[str],
+    branch: str,
     deployment_path: str,
     latest_commit: str,
     args: dict,
-    pull: bool = True,
+    check_lastcommit: bool = True,
 ) -> Tuple[Any, Optional[LocalEnv]]:
     err, readonly_localEnv = _localenv_from_cache(
         cache, project_id, branch, deployment_path, latest_commit, args
     )
     if err:
         return err, readonly_localEnv
     assert readonly_localEnv
     assert readonly_localEnv.project
     repo = readonly_localEnv.project.project_repoview.repo
     assert repo
-    if latest_commit and repo.revision != latest_commit:
+    if check_lastcommit and latest_commit and repo.revision != latest_commit:
         logger.warning(f"Conflict in {project_id}: {latest_commit} != {repo.revision}")
         err = create_error_response("CONFLICT", "Repository at wrong revision")
         return err, readonly_localEnv
     return None, readonly_localEnv
 
 
 def _do_export(
     project_id: str,
     requested_format: str,
     deployment_path: str,
-    cache_entry: Optional[CacheEntry],
+    cache_entry: CacheEntry,
     latest_commit: str,
     args: dict,
 ) -> Tuple[Optional[Any], Optional[str]]:
-    # load the ensemble
-    if cache_entry:
-        err, parent_localenv = _localenv_from_cache(
-            cache, project_id, cache_entry.branch, deployment_path, latest_commit, args
-        )
-        if err:
-            return err, None
-        assert (
-            parent_localenv
-            and parent_localenv.project
-            and parent_localenv.project.project_repoview.repo
-        )
-        working_dir = parent_localenv.project.project_repoview.repo.working_dir
-    else:
-        err, parent_localenv = None, None
-        if not project_id:
-            # use the current ensemble
-            working_dir = current_app.config.get("UNFURL_CURRENT_WORKING_DIR") or "."
-        else:
-            working_dir = _fetch_working_dir(project_id, args, True)  # type: ignore
-            if working_dir is None:
-                return (
-                    create_error_response(
-                        "INTERNAL_ERROR", "Could not find repository"
-                    ),
-                    None,
-                )
-
+    assert cache_entry.branch
+    err, parent_localenv = _localenv_from_cache(
+        cache, project_id, cache_entry.branch, deployment_path, latest_commit, args
+    )
+    if err:
+        return err, None
+    assert (
+        parent_localenv
+        and parent_localenv.project
+        and parent_localenv.project.project_repoview.repo
+    )
+    working_dir = parent_localenv.project.project_repoview.repo.working_dir
     clone_location = os.path.join(working_dir, deployment_path)
-    if not err:
-        err, local_env = _make_readonly_localenv(clone_location, parent_localenv)
-        if args.get("environment"):
-            local_env.manifest_context_name = args["environment"]
-
+    err, local_env = _make_readonly_localenv(clone_location, parent_localenv)
     if err:
         return (
             create_error_response("INTERNAL_ERROR", "An internal error occurred"),
             None,
         )
+    assert local_env
+    if args.get("environment"):
+        local_env.manifest_context_name = args["environment"]
 
     exporter = getattr(to_json, "to_" + requested_format)
     json_summary = exporter(local_env)
 
     return None, json_summary
 
 
@@ -881,17 +887,21 @@
             tpl[key] = value
         elif key == "title":
             if value != patch["name"]:
                 tpl.setdefault("metadata", {})["title"] = value
         elif key == "properties":
             props = tpl.setdefault("properties", {})
             assert isinstance(props, dict), f"bad props {props} in {tpl}"
-            assert isinstance(value, list), f"bad patch value {value} for {key} in {patch}"
+            assert isinstance(
+                value, list
+            ), f"bad patch value {value} for {key} in {patch}"
             for prop in value:
-                assert isinstance(prop, dict), f"bad {prop} in {value} for {key} in {patch}"
+                assert isinstance(
+                    prop, dict
+                ), f"bad {prop} in {value} for {key} in {patch}"
                 props[prop["name"]] = prop["value"]
         elif key == "dependencies":
             requirements = [
                 {dependency["name"]: _make_requirement(dependency)}
                 for dependency in value
                 if "match" in dependency
             ]
@@ -944,47 +954,21 @@
         localConfig.config.save()
 
 
 def _patch_response(repo: Optional[GitRepo]):
     return jsonify(dict(commit=repo and repo.revision or None))
 
 
-def _patch_environment(body: dict, project_id: str):
-    patch = body.get("patch")
-    assert isinstance(patch, list)
-    latest_commit = body.get("latest_commit") or ""
-    branch = body.get("branch")
-    err, readonly_localEnv = _localenv_from_cache_pull(
-        cache, project_id, branch, "", latest_commit, body
-    )
-    if err:
-        return err
-    assert readonly_localEnv and readonly_localEnv.project
-    invalidate_cache(body, "environments", project_id)
-    localEnv = LocalEnv(readonly_localEnv.project.projectRoot, can_be_empty=True)
-    assert localEnv.project
-    repo = localEnv.project.project_repoview.repo
-    assert repo
-    username = cast(str, body.get("username"))
-    password = cast(str, body.get("private_token", body.get("password")))
-    if not password and repo.url.startswith("http"):
-        return create_error_response("UNAUTHORIZED", "Missing credentials")
-    was_dirty = repo.is_dirty()
-    starting_revision = (
-        localEnv.project.project_repoview.repo
-        and localEnv.project.project_repoview.repo.revision
-        or ""
-    )
-    localConfig = localEnv.project.localConfig
+def _apply_environment_patch(patch: list, project: Project):
+    localConfig = project.localConfig
     for patch_inner in patch:
         assert isinstance(patch_inner, dict)
         typename = patch_inner.get("__typename")
         deleted = patch_inner.get("__deleted") or False
         assert isinstance(deleted, bool)
-        assert localEnv.project
         if typename == "DeploymentEnvironment":
             environments = localConfig.config.config.setdefault("environments", {})
             name = patch_inner["name"]
             if deleted:
                 if name in environments:
                     del environments[name]
             else:
@@ -998,17 +982,45 @@
                             if not isinstance(tpl, dict):
                                 # connections keys can be a string or null
                                 tpl = {}
                             _patch_node_template(node_patch, tpl)
                             new_target[node_name] = tpl
                         environment[key] = new_target  # replace
         elif typename == "DeploymentPath":
-            update_deployment(
-                localEnv.project, patch_inner["name"], patch_inner, False, deleted
-            )
+            update_deployment(project, patch_inner["name"], patch_inner, False, deleted)
+
+
+def _patch_environment(body: dict, project_id: str):
+    patch = body.get("patch")
+    assert isinstance(patch, list)
+    latest_commit = body.get("latest_commit") or ""
+    branch = body.get("branch", DEFAULT_BRANCH)
+    err, readonly_localEnv = _localenv_from_cache_pull(
+        cache, project_id, branch, "", latest_commit, body
+    )
+    if err:
+        return err
+    assert readonly_localEnv and readonly_localEnv.project
+    invalidate_cache(body, "environments", project_id)
+    localEnv = LocalEnv(readonly_localEnv.project.projectRoot, can_be_empty=True)
+    assert localEnv.project
+    repo = localEnv.project.project_repoview.repo
+    assert repo
+    username = cast(str, body.get("username"))
+    password = cast(str, body.get("private_token", body.get("password")))
+    if not password and repo.url.startswith("http"):
+        return create_error_response("UNAUTHORIZED", "Missing credentials")
+    was_dirty = repo.is_dirty()
+    starting_revision = (
+        localEnv.project.project_repoview.repo
+        and localEnv.project.project_repoview.repo.revision
+        or ""
+    )
+    localConfig = localEnv.project.localConfig
+    _apply_environment_patch(patch, localEnv.project)
     localConfig.config.save()
     if not was_dirty:
         if repo.is_dirty():
             commit_msg = body.get("commit_msg", "Update environment")
             err = _commit_and_push(
                 repo,
                 cast(str, localConfig.config.path),
@@ -1042,31 +1054,67 @@
         logger.debug(
             f"invalidate cache: cancel inflight {entry.cache_key()}: {was_inflight}"
         )
         return success
     return False
 
 
-def _patch_ensemble(body: dict, create: bool, project_id: str, pull=True) -> str:
+def _apply_ensemble_patch(patch: list, manifest: YamlManifest):
+    for patch_inner in patch:
+        assert isinstance(patch_inner, dict)
+        typename = patch_inner.get("__typename")
+        deleted = patch_inner.get("__deleted") or False
+        assert isinstance(deleted, bool)
+        if typename == "DeploymentTemplate":
+            _patch_deployment_blueprint(patch_inner, manifest, deleted)
+        elif typename == "ResourceTemplate":
+            # notes: only update or delete node_templates declared directly in the manifest
+            doc = manifest.manifest.config
+            for key in [
+                "spec",
+                "service_template",
+                "topology_template",
+                "node_templates",
+                patch_inner["name"],
+            ]:
+                if deleted:
+                    if key not in doc:
+                        break
+                    elif key == patch_inner["name"]:
+                        del doc[key]
+                    else:
+                        doc = doc[key]
+                else:
+                    if not doc.get(key):
+                        doc[key] = doc = {}
+                    else:
+                        doc = doc[key]
+            if not deleted:
+                _patch_node_template(patch_inner, doc)
+
+
+def _patch_ensemble(
+    body: dict, create: bool, project_id: str, check_lastcommit=True
+) -> str:
     patch = body.get("patch")
     assert isinstance(patch, list)
     environment = body.get("environment") or ""  # cloud_vars_url need the ""!
     deployment_path = body.get("deployment_path") or ""
-    existing_repo = _get_project_repo(project_id, body)
+    branch = body.get("branch", DEFAULT_BRANCH)
+    existing_repo = _get_project_repo(project_id, branch, body)
 
     username = body.get("username")
     password = body.get("private_token", body.get("password"))
     push_url = existing_repo.url if existing_repo else app.config["UNFURL_CLOUD_SERVER"]
     if push_url and not password and push_url.startswith("http"):
         return create_error_response("UNAUTHORIZED", "Missing credentials")
 
     latest_commit = body.get("latest_commit") or ""
-    branch = body.get("branch")
     err, parent_localenv = _localenv_from_cache_pull(
-        cache, project_id, branch, "", latest_commit, body, pull
+        cache, project_id, branch, "", latest_commit, body, check_lastcommit
     )
     if err:
         return err
     assert (
         parent_localenv
         and parent_localenv.project
         and parent_localenv.project.project_repoview.repo
@@ -1111,46 +1159,15 @@
         apply_url_credentials=True,
     )
     # don't validate in case we are still an incomplete draft
     manifest = LocalEnv(clone_location, overrides=overrides).get_manifest(
         skip_validation=True
     )
     # logger.info("vault secrets %s", manifest.manifest.vault.secrets)
-    for patch_inner in patch:
-        assert isinstance(patch_inner, dict)
-        typename = patch_inner.get("__typename")
-        deleted = patch_inner.get("__deleted") or False
-        assert isinstance(deleted, bool)
-        if typename == "DeploymentTemplate":
-            _patch_deployment_blueprint(patch_inner, manifest, deleted)
-        elif typename == "ResourceTemplate":
-            # notes: only update or delete node_templates declared directly in the manifest
-            doc = manifest.manifest.config
-            for key in [
-                "spec",
-                "service_template",
-                "topology_template",
-                "node_templates",
-                patch_inner["name"],
-            ]:
-                if deleted:
-                    if key not in doc:
-                        break
-                    elif key == patch_inner["name"]:
-                        del doc[key]
-                    else:
-                        doc = doc[key]
-                else:
-                    if not doc.get(key):
-                        doc[key] = doc = {}
-                    else:
-                        doc = doc[key]
-            if not deleted:
-                _patch_node_template(patch_inner, doc)
-
+    _apply_ensemble_patch(patch, manifest)
     manifest.manifest.save()
     if was_dirty:
         logger.warning(
             "local repository at %s was dirty, not committing or pushing",
             clone_location,
         )
     else:
@@ -1254,15 +1271,17 @@
         # this is mainly for security if we couldn't push because the user wasn't authorized
         repo.reset(f"--hard {starting_revision or 'HEAD~1'}")
         logger.error("push failed", exc_info=True)
         return create_error_response("INTERNAL_ERROR", "Could not push repository")
     return None
 
 
-def _fetch_working_dir(project_path: str, args: dict, pull: bool) -> Optional[str]:
+def _fetch_working_dir(
+    project_path: str, branch: str, args: dict, pull: bool
+) -> Optional[str]:
     # if successful, returns the repository's working directory or None if clone failed
     current_working_dir = current_app.config.get("UNFURL_CURRENT_WORKING_DIR") or "."
     if not project_path or project_path == ".":
         clone_location = current_working_dir
     else:
         current_git_url = current_app.config.get("UNFURL_CURRENT_GIT_URL")
         if (
@@ -1271,15 +1290,15 @@
         ):
             # developer mode: use the project we are serving from if the project_path matches
             logger.debug("exporting from local repo %s", current_git_url)
             clone_location = current_working_dir
         else:
             # otherwise clone the project if necessary
             # root of repo not necessarily unfurl project
-            clone_location = _stage(project_path, args, pull)
+            clone_location = _stage(project_path, branch, args, pull)
         if not clone_location:
             return clone_location
     # XXX: deployment_path must be in the project repo, split repos are not supported
     # we want the caching and staging infrastructure to only know about git, not unfurl projects
     # so we can't reference a file path outside of the git repository
     return clone_location
```

### Comparing `unfurl-0.6.1/unfurl/support.py` & `unfurl-0.6.2/unfurl/support.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,18 @@
         # if path is relative, treat as relative to current src location
         path = get_path(ctx, path, "src", False)
         mod = load_module(path)
         funcName = mod.__name__ + "." + fragment
     else:
         funcName = arg
     func = load_class(funcName)
-    assert callable(func)
+    if not func:
+        raise UnfurlError(f"Could not find python function {funcName}")
+    if not callable(func):
+        raise UnfurlError(f"Invalid python function {funcName}: {type(funcName)} is not callable.")
 
     kw = ctx.kw
     if "args" in kw:
         args = map_value(kw["args"], ctx)
         return func(ctx, args)
     else:
         return func(ctx)
@@ -514,15 +517,15 @@
     if isinstance(args, Mapping) and "path" in args:
         path = args["path"]
         if is_template(path, ctx):  # path could be a template expression
             path = apply_template(path, ctx)
         with open(path) as f:
             value = f.read()
     else:
-        value = args
+        value = cast(str, args)
     return apply_template(value, ctx, ctx.kw.get("overrides"))
 
 
 set_eval_func("template", _template_func, safe=True)
 
 
 def run_lookup(name, templar, *args, **kw):
@@ -826,15 +829,15 @@
         # only apply digest to values
         return {
             to_label(n, **kw): to_label(v, digest=digest, **kw)
             for n, v in arg.items()
             if v is not None
         }
 
-    trunc: int = kw.pop("max", _label_defaults["max"])
+    trunc = int(kw.pop("max", _label_defaults["max"]))
     assert trunc >= 1, trunc
     checksum: int = kw.pop("digestlen", _label_defaults["digestlen"])
 
     if checksum == -1:
         checksum = 2 if trunc < 32 else 3
     if checksum:
         maxchecksum = min(trunc, checksum)
@@ -1020,18 +1023,18 @@
         query = start + "::" + candidate_name
     return ctx.query(query)
 
 
 set_eval_func("get_attribute", get_attribute, True, True)
 
 
-def get_nodes_of_type(type_name, ctx: RefContext):
+def get_nodes_of_type(type_name: str, ctx: RefContext) :
     return [
         r
-        for r in ctx.currentResource.root.get_self_and_descendents()
+        for r in ctx.currentResource.root.get_self_and_descendants()
         if r.template.is_compatible_type(type_name)
         and r.name not in ["inputs", "outputs"]
     ]
 
 
 set_eval_func("get_nodes_of_type", get_nodes_of_type, True, True)
 
@@ -1532,18 +1535,18 @@
         r = self.resource.find_resource(key)
         if r:
             return r.attributes
         else:
             raise KeyError(key)
 
     def __iter__(self):
-        return iter(r.name for r in self.resource.get_self_and_descendents())
+        return iter(r.name for r in self.resource.get_self_and_descendants())
 
     def __len__(self):
-        return len(tuple(self.resource.get_self_and_descendents()))
+        return len(tuple(self.resource.get_self_and_descendants()))
 
 
 LiveDependencies = NewType(
     "LiveDependencies",
     Dict[
         "InstanceKey",
         Tuple["EntityInstance", Dict[str, Tuple[bool, Union[Result, Any]]]],
```

### Comparing `unfurl-0.6.1/unfurl/templates/aws/unfurl.yaml.j2` & `unfurl-0.6.2/unfurl/templates/aws/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/dashboard/manifest.yaml.j2` & `unfurl-0.6.2/unfurl/templates/dashboard/manifest.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/digitalocean/unfurl.yaml.j2` & `unfurl-0.6.2/unfurl/templates/digitalocean/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/gcp/unfurl.yaml.j2` & `unfurl-0.6.2/unfurl/templates/gcp/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/home/manifest-template.yaml.j2` & `unfurl-0.6.2/unfurl/templates/home/manifest-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/home/unfurl.yaml.j2` & `unfurl-0.6.2/unfurl/templates/home/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/local/ensemble-examples.yaml` & `unfurl-0.6.2/unfurl/templates/local/ensemble-examples.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/local-unfurl-template.yaml.j2` & `unfurl-0.6.2/unfurl/templates/local-unfurl-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/manifest-template.yaml.j2` & `unfurl-0.6.2/unfurl/templates/manifest-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/manifest.yaml.j2` & `unfurl-0.6.2/unfurl/templates/manifest.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/python3.10/Pipfile` & `unfurl-0.6.2/unfurl/templates/python3.10/Pipfile`

 * *Files 1% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 rich = "==12.4.4"
 flask = "<=2.1.3"
 flask-caching = "<=2.0.1"
 uvicorn = "<=0.18.2"
 google-cloud-compute = "==1.3.2"
 google-cloud-dns = "==0.34.0"
 grpcio = "==1.50.0"
-python-gitlab = "<=3.4.0"
+python-gitlab = "==3.13.0"
 certifi = "*"
 kubernetes = "==24.2.0"
 gunicorn = "==20.1.0"
-redis = "==4.3.5"
+redis = "==4.4.4"
 flask-cors = "==3.0.10"
 
 [dev-packages]
 
 [requires]
 python_version = "3.10"
```

### Comparing `unfurl-0.6.1/unfurl/templates/python3.10/Pipfile.lock` & `unfurl-0.6.2/unfurl/templates/python3.10/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9825068123679234%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'1f2fc413f7089087ad6857f55c65f38dd76253dd99b9b5189a49f6c09d3e3345'}}",*

 * * "'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:308c5a8293d9b76e74921f4d945be19cc467b92e5f128df1db76e31c71345bb3', "*

 * *              "'sha256:bcd09f16bdf3d71ab7d0fab20e97242f09c63f4cea0943329521ab35a950f900'], "*

 * *              "'version': '==1.26.104'}, 'botocore': {'hashes': "*

 * *              "['sha256:7e7a01cef10b1daa9cb01ec25a15e831e7359fc43d1b591359710f203c3620a8', "*

 * *           […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "bfe03d0cb9032a282161ebf8615f6becf4bb6bed3b1dc13be30f28e978eed9ec"
+            "sha256": "1f2fc413f7089087ad6857f55c65f38dd76253dd99b9b5189a49f6c09d3e3345"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.10"
         },
         "sources": [
             {
@@ -60,43 +60,43 @@
                 "sha256:ea0d3b40a2d852767be77ca343b58a9e3a4b00d9db440efb8da74b4e58025e5a"
             ],
             "index": "pypi",
             "version": "==2.49.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:0b1f82d4565ed875c7975ac0be5665e8d948613c01bcb0e49df6d4f5af670cc8",
-                "sha256:319ddb274f8f83b035b88a3b127c465bf6fe3e3fc2d668869b489e992c47ca77"
+                "sha256:308c5a8293d9b76e74921f4d945be19cc467b92e5f128df1db76e31c71345bb3",
+                "sha256:bcd09f16bdf3d71ab7d0fab20e97242f09c63f4cea0943329521ab35a950f900"
             ],
             "index": "pypi",
-            "version": "==1.26.52"
+            "version": "==1.26.104"
         },
         "botocore": {
             "hashes": [
-                "sha256:a0b89a33305cfa6251c6e1142deb7567e216e37e25363159f45fb81dc5b474e5",
-                "sha256:de55b6333fb13c66da9055972d7e4efff5dcc5a087478a2b70e99d888b29a24c"
+                "sha256:7e7a01cef10b1daa9cb01ec25a15e831e7359fc43d1b591359710f203c3620a8",
+                "sha256:932bfbf580a2ae53f471df4bfbebce531985ee27468cf7c37d7ccfb3cf8bc9e4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.52"
+            "version": "==1.29.104"
         },
         "cachelib": {
             "hashes": [
-                "sha256:292e89d5f9201fb9570e9f222c202f59085c66f9cb8bdfeefcfffff2b442fb2a",
-                "sha256:6fbbae4637491cc78a5e82f7cf623eb6778ea21ad8aa92197f45a1add51dab02"
+                "sha256:42d49f2fad9310dd946d7be73d46776bcd4d5fde4f49ad210cfdd447fbdfc346",
+                "sha256:593faeee62a7c037d50fc835617a01b887503f972fb52b188ae7e50e9cb69740"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.10.0"
+            "version": "==0.10.2"
         },
         "cachetools": {
             "hashes": [
-                "sha256:5991bc0e08a1319bb618d3195ca5b6bc76646a49c21d55962977197b301cc1fe",
-                "sha256:8462eebf3a6c15d25430a8c27c56ac61340b2ecf60c9ce57afc2b97e450e47da"
+                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
+                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
-            "version": "==5.2.1"
+            "version": "==5.3.0"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "index": "pypi",
@@ -169,104 +169,92 @@
                 "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
                 "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
             "version": "==1.15.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "version": "==3.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
@@ -286,115 +274,111 @@
                 "sha256:a21da482714b9f0b0e9bafaaf2f6a8b3b14161bb47f62e10e28d2fe4ff4b1626"
             ],
             "index": "pypi",
             "version": "==3.10.1"
         },
         "cmd2": {
             "hashes": [
-                "sha256:073e555c05853b0f6965f3d03329babdf9e38a5f2cea028e61a64cd7eeb74ad5",
-                "sha256:a77e3056751393270b4125c990cf527db132f15951a20a3a5dd2df4290aadf20"
+                "sha256:71873c11f72bd19e2b1db578214716f0d4f7c8fa250093c601265a9a717dee52",
+                "sha256:f1988ff2fff0ed812a2d25218a081b0fa0108d45b48ba2a9272bb98091b654e6"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.4.2"
+            "version": "==2.4.3"
         },
         "commonmark": {
             "hashes": [
                 "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60",
                 "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"
             ],
             "version": "==0.9.1"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:051afcbd6d2ac39298d62d340f94dbb6a1f31de06dfaf6fcef7b759dd3860c45",
-                "sha256:0a1890fca2962c4f1ad16551d660b46ea77291fba2cc21c024cd527b9d9c8809",
-                "sha256:0ee30375b409d9a7ea0f30c50645d436b6f5dfee254edffd27e45a980ad2c7f4",
-                "sha256:13250b1f0bd023e0c9f11838bdeb60214dd5b6aaf8e8d2f110c7e232a1bff83b",
-                "sha256:17e01dd8666c445025c29684d4aabf5a90dc6ef1ab25328aa52bedaa95b65ad7",
-                "sha256:19245c249aa711d954623d94f23cc94c0fd65865661f20b7781210cb97c471c0",
-                "sha256:1caed2367b32cc80a2b7f58a9f46658218a19c6cfe5bc234021966dc3daa01f0",
-                "sha256:1f66862d3a41674ebd8d1a7b6f5387fe5ce353f8719040a986551a545d7d83ea",
-                "sha256:220e3fa77d14c8a507b2d951e463b57a1f7810a6443a26f9b7591ef39047b1b2",
-                "sha256:276f4cd0001cd83b00817c8db76730938b1ee40f4993b6a905f40a7278103b3a",
-                "sha256:29de916ba1099ba2aab76aca101580006adfac5646de9b7c010a0f13867cba45",
-                "sha256:2a7f23bbaeb2a87f90f607730b45564076d870f1fb07b9318d0c21f36871932b",
-                "sha256:2c407b1950b2d2ffa091f4e225ca19a66a9bd81222f27c56bd12658fc5ca1209",
-                "sha256:30b5fec1d34cc932c1bc04017b538ce16bf84e239378b8f75220478645d11fca",
-                "sha256:3c2155943896ac78b9b0fd910fb381186d0c345911f5333ee46ac44c8f0e43ab",
-                "sha256:411d4ff9d041be08fdfc02adf62e89c735b9468f6d8f6427f8a14b6bb0a85095",
-                "sha256:436e103950d05b7d7f55e39beeb4d5be298ca3e119e0589c0227e6d0b01ee8c7",
-                "sha256:49640bda9bda35b057b0e65b7c43ba706fa2335c9a9896652aebe0fa399e80e6",
-                "sha256:4a950f83fd3f9bca23b77442f3a2b2ea4ac900944d8af9993743774c4fdc57af",
-                "sha256:50a6adc2be8edd7ee67d1abc3cd20678987c7b9d79cd265de55941e3d0d56499",
-                "sha256:52ab14b9e09ce052237dfe12d6892dd39b0401690856bcfe75d5baba4bfe2831",
-                "sha256:54f7e9705e14b2c9f6abdeb127c390f679f6dbe64ba732788d3015f7f76ef637",
-                "sha256:66e50680e888840c0995f2ad766e726ce71ca682e3c5f4eee82272c7671d38a2",
-                "sha256:790e4433962c9f454e213b21b0fd4b42310ade9c077e8edcb5113db0818450cb",
-                "sha256:7a38362528a9115a4e276e65eeabf67dcfaf57698e17ae388599568a78dcb029",
-                "sha256:7b05ed4b35bf6ee790832f68932baf1f00caa32283d66cc4d455c9e9d115aafc",
-                "sha256:7e109f1c9a3ece676597831874126555997c48f62bddbcace6ed17be3e372de8",
-                "sha256:949844af60ee96a376aac1ded2a27e134b8c8d35cc006a52903fc06c24a3296f",
-                "sha256:95304068686545aa368b35dfda1cdfbbdbe2f6fe43de4a2e9baa8ebd71be46e2",
-                "sha256:9e662e6fc4f513b79da5d10a23edd2b87685815b337b1a30cd11307a6679148d",
-                "sha256:a9fed35ca8c6e946e877893bbac022e8563b94404a605af1d1e6accc7eb73289",
-                "sha256:b69522b168a6b64edf0c33ba53eac491c0a8f5cc94fa4337f9c6f4c8f2f5296c",
-                "sha256:b78729038abea6a5df0d2708dce21e82073463b2d79d10884d7d591e0f385ded",
-                "sha256:b8c56bec53d6e3154eaff6ea941226e7bd7cc0d99f9b3756c2520fc7a94e6d96",
-                "sha256:b9727ac4f5cf2cbf87880a63870b5b9730a8ae3a4a360241a0fdaa2f71240ff0",
-                "sha256:ba3027deb7abf02859aca49c865ece538aee56dcb4871b4cced23ba4d5088904",
-                "sha256:be9fcf32c010da0ba40bf4ee01889d6c737658f4ddff160bd7eb9cac8f094b21",
-                "sha256:c18d47f314b950dbf24a41787ced1474e01ca816011925976d90a88b27c22b89",
-                "sha256:c76a3075e96b9c9ff00df8b5f7f560f5634dffd1658bafb79eb2682867e94f78",
-                "sha256:cbfcba14a3225b055a28b3199c3d81cd0ab37d2353ffd7f6fd64844cebab31ad",
-                "sha256:d254666d29540a72d17cc0175746cfb03d5123db33e67d1020e42dae611dc196",
-                "sha256:d66187792bfe56f8c18ba986a0e4ae44856b1c645336bd2c776e3386da91e1dd",
-                "sha256:d8d04e755934195bdc1db45ba9e040b8d20d046d04d6d77e71b3b34a8cc002d0",
-                "sha256:d8f3e2e0a1d6777e58e834fd5a04657f66affa615dae61dd67c35d1568c38882",
-                "sha256:e057e74e53db78122a3979f908973e171909a58ac20df05c33998d52e6d35757",
-                "sha256:e4ce984133b888cc3a46867c8b4372c7dee9cee300335e2925e197bcd45b9e16",
-                "sha256:ea76dbcad0b7b0deb265d8c36e0801abcddf6cc1395940a24e3595288b405ca0",
-                "sha256:ecb0f73954892f98611e183f50acdc9e21a4653f294dfbe079da73c6378a6f47",
-                "sha256:ef14d75d86f104f03dea66c13188487151760ef25dd6b2dbd541885185f05f40",
-                "sha256:f26648e1b3b03b6022b48a9b910d0ae209e2d51f50441db5dce5b530fad6d9b1",
-                "sha256:f67472c09a0c7486e27f3275f617c964d25e35727af952869dd496b9b5b7f6a3"
+                "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d",
+                "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4",
+                "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e",
+                "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab",
+                "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90",
+                "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6",
+                "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731",
+                "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540",
+                "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2",
+                "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292",
+                "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5",
+                "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b",
+                "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2",
+                "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0",
+                "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57",
+                "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3",
+                "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140",
+                "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84",
+                "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988",
+                "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67",
+                "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d",
+                "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2",
+                "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5",
+                "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9",
+                "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8",
+                "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd",
+                "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6",
+                "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be",
+                "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88",
+                "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25",
+                "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137",
+                "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968",
+                "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9",
+                "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef",
+                "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54",
+                "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512",
+                "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005",
+                "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f",
+                "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149",
+                "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d",
+                "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8",
+                "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7",
+                "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5",
+                "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016",
+                "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69",
+                "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212",
+                "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc",
+                "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8",
+                "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d",
+                "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd",
+                "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.0.5"
+            "version": "==7.2.2"
         },
         "cryptography": {
             "hashes": [
-                "sha256:1a6915075c6d3a5e1215eab5d99bcec0da26036ff2102a1038401d6ef5bef25b",
-                "sha256:1ee1fd0de9851ff32dbbb9362a4d833b579b4a6cc96883e8e6d2ff2a6bc7104f",
-                "sha256:407cec680e811b4fc829de966f88a7c62a596faa250fc1a4b520a0355b9bc190",
-                "sha256:50386acb40fbabbceeb2986332f0287f50f29ccf1497bae31cf5c3e7b4f4b34f",
-                "sha256:6f97109336df5c178ee7c9c711b264c502b905c2d2a29ace99ed761533a3460f",
-                "sha256:754978da4d0457e7ca176f58c57b1f9de6556591c19b25b8bcce3c77d314f5eb",
-                "sha256:76c24dd4fd196a80f9f2f5405a778a8ca132f16b10af113474005635fe7e066c",
-                "sha256:7dacfdeee048814563eaaec7c4743c8aea529fe3dd53127313a792f0dadc1773",
-                "sha256:80ee674c08aaef194bc4627b7f2956e5ba7ef29c3cc3ca488cf15854838a8f72",
-                "sha256:844ad4d7c3850081dffba91cdd91950038ee4ac525c575509a42d3fc806b83c8",
-                "sha256:875aea1039d78557c7c6b4db2fe0e9d2413439f4676310a5f269dd342ca7a717",
-                "sha256:887cbc1ea60786e534b00ba8b04d1095f4272d380ebd5f7a7eb4cc274710fad9",
-                "sha256:ad04f413436b0781f20c52a661660f1e23bcd89a0e9bb1d6d20822d048cf2856",
-                "sha256:bae6c7f4a36a25291b619ad064a30a07110a805d08dc89984f4f441f6c1f3f96",
-                "sha256:c52a1a6f81e738d07f43dab57831c29e57d21c81a942f4602fac7ee21b27f288",
-                "sha256:e0a05aee6a82d944f9b4edd6a001178787d1546ec7c6223ee9a848a7ade92e39",
-                "sha256:e324de6972b151f99dc078defe8fb1b0a82c6498e37bff335f5bc6b1e3ab5a1e",
-                "sha256:e5d71c5d5bd5b5c3eebcf7c5c2bb332d62ec68921a8c593bea8c394911a005ce",
-                "sha256:f3ed2d864a2fa1666e749fe52fb8e23d8e06b8012e8bd8147c73797c506e86f1",
-                "sha256:f671c1bb0d6088e94d61d80c606d65baacc0d374e67bf895148883461cd848de",
-                "sha256:f6c0db08d81ead9576c4d94bbb27aed8d7a430fa27890f39084c2d0e2ec6b0df",
-                "sha256:f964c7dcf7802d133e8dbd1565914fa0194f9d683d82411989889ecd701e8adf",
-                "sha256:fec8b932f51ae245121c4671b4bbc030880f363354b2f0e0bd1366017d891458"
+                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
+                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
+                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
+                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
+                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
+                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
+                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
+                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
+                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
+                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
+                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
+                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
+                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
+                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
+                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
+                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
+                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
+                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
+                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==39.0.0"
+            "version": "==40.0.1"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
@@ -416,27 +400,27 @@
                 "sha256:dbcb3bd2fa80dca0788ed908218bf43972772009b881ed1e20dfc29a65e49782"
             ],
             "index": "pypi",
             "version": "==6.0.1"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e",
-                "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"
+                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
+                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.0"
+            "version": "==1.1.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:892be14aa8efc01673b5ed6589dbccb95f9a8596f0507e232626155495c18105",
+                "sha256:bde48477b15fde2c7e5a0713cbe72721cb5a5ad32ee0b8f419907960b9d75536"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.0"
+            "version": "==3.10.7"
         },
         "flask": {
             "hashes": [
                 "sha256:15972e5017df0575c3d6c090ba168b6db90259e620ac8d7ea813a396bad5b6cb",
                 "sha256:9013281a7402ad527f8fd56375164f3aa021ecfaff89bfe3825346c24f87e04c"
             ],
             "index": "pypi",
@@ -491,19 +475,19 @@
                 "sha256:ce222e27b0de0d7bc63eb043b956996d6dccab14cc3b690aaea91c9cc99dc16e"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.11.0"
         },
         "google-auth": {
             "hashes": [
-                "sha256:5045648c821fb72384cdc0e82cc326df195f113a33049d9b62b74589243d2acc",
-                "sha256:ed7057a101af1146f0554a769930ac9de506aeca4fd5af6543ebe791851a9fbd"
+                "sha256:357ff22a75b4c0f6093470f21816a825d2adee398177569824e37b6c10069e19",
+                "sha256:8f379b46bad381ad2a0b989dfb0c13ad28d3c2a79f27348213f8946a1d15d55a"
             ],
             "index": "pypi",
-            "version": "==2.16.0"
+            "version": "==2.17.1"
         },
         "google-cloud-compute": {
             "hashes": [
                 "sha256:1ddd1be44d278754fc2643be7aa8d66838235ce44cfbacbeeadf3952ec020e95",
                 "sha256:21bd66251356d70bfd5f40211b42b936335490f7433b3b6fae7c498077e2c3fa"
             ],
             "index": "pypi",
@@ -523,19 +507,19 @@
                 "sha256:bd75d6e9fd456ce643ee936a113a1ead5405704515caa679db30d7f036e447f3"
             ],
             "index": "pypi",
             "version": "==0.34.0"
         },
         "googleapis-common-protos": {
             "hashes": [
-                "sha256:c727251ec025947d545184ba17e3578840fc3a24a0516a020479edab660457df",
-                "sha256:ca3befcd4580dab6ad49356b46bf165bb68ff4b32389f028f1abd7c10ab9519a"
+                "sha256:4168fcb568a826a52f23510412da405abd93f4d23ba544bb68d943b14ba3cb44",
+                "sha256:b287dc48449d1d41af0c69f4ea26242b5ae4c3d7249a38b0984c86a4caffff1f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.58.0"
+            "version": "==1.59.0"
         },
         "grpcio": {
             "hashes": [
                 "sha256:05f7c248e440f538aaad13eee78ef35f0541e73498dd6f832fe284542ac4b298",
                 "sha256:080b66253f29e1646ac53ef288c12944b131a2829488ac3bac8f52abb4413c0d",
                 "sha256:12b479839a5e753580b5e6053571de14006157f2ef9b71f38c56dc9b23b95ad6",
                 "sha256:156f8009e36780fab48c979c5605eda646065d4695deea4cfcbcfdd06627ddb6",
@@ -724,19 +708,19 @@
                 "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
             ],
             "index": "pypi",
             "version": "==2.1.1"
         },
         "natsort": {
             "hashes": [
-                "sha256:04fe18fdd2b9e5957f19f687eb117f102ef8dde6b574764e536e91194bed4f5f",
-                "sha256:57f85b72c688b09e053cdac302dd5b5b53df5f73ae20b4874fcbffd8bf783d11"
+                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
+                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==8.2.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==8.3.1"
         },
         "oauthlib": {
             "hashes": [
                 "sha256:8139f29aac13e25d502680e9e19963e83f16838d48a0d71c287fe40e7067fbca",
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
@@ -771,35 +755,35 @@
                 "sha256:e8dca2f4b43560edef58813969f52a56cef023146cbb8931626db80e6c1c4308"
             ],
             "index": "pypi",
             "version": "==5.9.0"
         },
         "pip": {
             "hashes": [
-                "sha256:65fd48317359f3af8e593943e6ae1506b66325085ea64b706a998c6e83eeaf38",
-                "sha256:908c78e6bc29b676ede1c4d57981d490cb892eb45cd8c214ab6298125119e077"
+                "sha256:236bcb61156d76c4b8a05821b988c7b8c35bf0da28a4b614e8d6ab5212c25c6f",
+                "sha256:cd015ea1bfb0fcef59d8a286c1f8bebcb983f6317719d415dc5351efb7cd7024"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==22.3.1"
+            "version": "==23.0.1"
         },
         "pipenv": {
             "hashes": [
                 "sha256:3b80b4512934b9d8e8ce12c988394642ff96bb697680e5b092e59af503178327",
                 "sha256:f84d7119239b22ab2ac2b8fbc7d619d83cf41135206d72a17c4f151cda529fd0"
             ],
             "index": "pypi",
             "version": "==2022.1.8"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490",
-                "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"
+                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
+                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.6.2"
+            "version": "==3.2.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -940,19 +924,19 @@
                 "sha256:cdc7b5e3ed77bed61270a47d35434a30617b9becdf2478af76ad2c6ade307280"
             ],
             "index": "pypi",
             "version": "==0.15.7"
         },
         "pytest": {
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
+                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.2.1"
+            "version": "==7.2.2"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b",
                 "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
             ],
             "markers": "python_version >= '3.6'",
@@ -972,19 +956,19 @@
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "index": "pypi",
             "version": "==2.8.2"
         },
         "python-gitlab": {
             "hashes": [
-                "sha256:251b63f0589d51f854516948c84e9eb8df26e1e9dea595cf86b43f17c43007dd",
-                "sha256:6180b81ee2f265ad8d8412956a1740b4d3ceca7b28ae2f707dfe62375fed0082"
+                "sha256:85ae778d8953aba87ad4b78aef7fbb5dae053980d2c20ff200bea29799685743",
+                "sha256:ad502b72b5d1137f4af37d4a68ae20fe7d6c9778f67cbe2aec566f7995053c7d"
             ],
             "index": "pypi",
-            "version": "==3.4.0"
+            "version": "==3.13.0"
         },
         "python-string-utils": {
             "hashes": [
                 "sha256:dcf9060b03f07647c0a603408dc8b03f807f3b54a05c6e19eb14460256fac0cb",
                 "sha256:f1a88700baf99db1a9b6953f44181ad9ca56623c81e257e6009707e2e7851fa4"
             ],
             "markers": "python_version >= '3.5'",
@@ -1034,19 +1018,19 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "index": "pypi",
             "version": "==6.0"
         },
         "redis": {
             "hashes": [
-                "sha256:30c07511627a4c5c4d970e060000772f323174f75e745a26938319817ead7a12",
-                "sha256:46652271dc7525cd5a9667e5b0ca983c848c75b2b8f7425403395bb8379dcf25"
+                "sha256:68226f7ede928db8302f29ab088a157f41061fa946b7ae865452b6d7838bbffb",
+                "sha256:da92a39fec86438d3f1e2a1db33c312985806954fe860120b582a8430e231d8f"
             ],
             "index": "pypi",
-            "version": "==4.3.5"
+            "version": "==4.4.4"
         },
         "repoze.lru": {
             "hashes": [
                 "sha256:0429a75e19380e4ed50c0694e26ac8819b4ea7851ee1fc7583c8572db80aff77",
                 "sha256:f77bf0e1096ea445beadd35f3479c5cff2aa1efe604a133e67150bc8630a62ea"
             ],
             "version": "==0.7"
@@ -1146,39 +1130,41 @@
                 "sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b",
                 "sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b",
                 "sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640",
                 "sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7",
                 "sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a",
                 "sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71",
                 "sha256:d5e51e2901ec2366b79f16c2299a03e74ba4531ddcfacc1416639c557aef0ad8",
+                "sha256:da538167284de58a52109a9b89b8f6a53ff8437dd6dc26d33b57bf6699153122",
                 "sha256:debc87a9516b237d0466a711b18b6ebeb17ba9f391eb7f91c649c5c4ec5006c7",
                 "sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80",
                 "sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e",
                 "sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab",
                 "sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0",
-                "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646"
+                "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646",
+                "sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38"
             ],
             "markers": "platform_python_implementation == 'CPython' and python_version < '3.11'",
             "version": "==0.2.7"
         },
         "s3transfer": {
             "hashes": [
                 "sha256:06176b74f3a15f61f1b4f25a1fc29a4429040b7647133a463da8fa5bd28d5ecd",
                 "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:a78d01d1e2c175c474884671dde039962c9d74c7223db7369771fcf6e29ceeab",
-                "sha256:bd6eb2d6722568de6d14b87c44a96fac54b2a45ff5e940e639979a3d1792adb6"
+                "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a",
+                "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==66.0.0"
+            "version": "==67.6.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
@@ -1222,35 +1208,35 @@
                 "sha256:21c85e0fe4b9a155d0799430b0ad741cdce7e359660ccbd8b530613e8df88ce2"
             ],
             "index": "pypi",
             "version": "==4.1.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         },
         "uvicorn": {
             "hashes": [
                 "sha256:c19a057deb1c5bb060946e2e5c262fc01590c6529c0af2c3d9ce941e89bc30e0",
                 "sha256:cade07c403c397f9fe275492a48c1b869efd175d5d8a692df649e6e7e2ed8f4e"
             ],
             "index": "pypi",
             "version": "==0.18.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:ce3b1684d6e1a20a3e5ed36795a97dfc6af29bc3970ca8dab93e11ac6094b3c4",
-                "sha256:f8b927684efc6f1cc206c9db297a570ab9ad0e51c16fa9e45487d36d1905c058"
+                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
+                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==20.17.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.21.0"
         },
         "virtualenv-clone": {
             "hashes": [
                 "sha256:418ee935c36152f8f153c79824bb93eaf6f0f7984bae31d3f48f350b9183501a",
                 "sha256:44d5263bceed0bac3e1424d64f798095233b64def1c5689afa43dc3223caf5b0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1261,47 +1247,47 @@
                 "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e",
                 "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"
             ],
             "version": "==0.2.6"
         },
         "webcolors": {
             "hashes": [
-                "sha256:16d043d3a08fd6a1b1b7e3e9e62640d09790dce80d2bdd4792a175b35fe794a9",
-                "sha256:d98743d81d498a2d3eaf165196e65481f0d2ea85281463d856b1e51b09f62dce"
+                "sha256:29bc7e8752c0a1bd4a1f03c14d6e6a72e93d82193738fa860cbff59d0fcc11bf",
+                "sha256:c225b674c83fa923be93d235330ce0300373d02885cef23238813b0d5668304a"
             ],
-            "version": "==1.12"
+            "version": "==1.13"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:d6b06432f184438d99ac1f456eaf22fe1ade524c3dd16e661142dc54e9cba574",
-                "sha256:d6e8f90ca8e2dd4e8027c4561adeb9456b54044312dba655e7cae652ceb9ae59"
+                "sha256:3f09e6d8230892547132177f575a4e3e73cfdf06526e20cc02aa1c3b47184d40",
+                "sha256:cdf5877568b7e83aa7cf2244ab56a3213de587bbe0ce9d8b9600fc77b455d89e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.4.2"
+            "version": "==1.5.1"
         },
         "werkzeug": {
             "hashes": [
-                "sha256:7ea2d48322cc7c0f8b3a215ed73eabd7b5d75d0b50e31ab006286ccff9e00b8f",
-                "sha256:f979ab81f58d7318e064e99c4506445d60135ac5cd2e177a2de0089bfd4c9bd5"
+                "sha256:2e1ccc9417d4da358b9de6f174e3ac094391ea1d4fbef2d667865d819dfd0afe",
+                "sha256:56433961bc1f12533306c624f3be5e744389ac61d722175d543e1751285da612"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.2.2"
+            "version": "==2.2.3"
         },
         "wheel": {
             "hashes": [
-                "sha256:965f5259b566725405b05e7cf774052044b1ed30119b5d586b2703aafe8719ac",
-                "sha256:b60533f3f5d530e971d6737ca6d58681ee434818fab630c83a734bb10c083ce8"
+                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
+                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.38.4"
+            "version": "==0.40.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa",
-                "sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.11.0"
+            "version": "==3.15.0"
         }
     },
     "develop": {}
 }
```

### Comparing `unfurl-0.6.1/unfurl/templates/python3.11/Pipfile` & `unfurl-0.6.2/unfurl/templates/python3.11/Pipfile`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [packages]
 pipenv = "==2022.1.8"
 click = ">=8.0.1"
 click-log = "*"
 pyrsistent = "==0.15.7"
 jsonschema = {version = "==3.2", extras = ["format_nongpl"]}
 "ruamel.yaml" = ">=0.16.13"
-ansible = "<5.0,>=4.2.0"
+ansible = ">=4.2.0,<5.0"
 gitpython = "==3.1.30"
 rich = "==12.4.4"
 pbr = "==5.9.0"
 cliff = "==3.10.1"
 pyyaml = ">=6.0"
 python-dateutil = ">=2.8"
 stevedore = "==3.5.0"
@@ -33,18 +33,18 @@
 boto = "*"
 boto3 = "*"
 supervisor = "*"
 google-cloud-compute = "==1.3.2"
 google-cloud-dns = "==0.34.0"
 google-auth = "*"
 grpcio = "==1.50.0"
-python-gitlab = "<=3.4.0"
+python-gitlab = "==3.13.0"
 certifi = "*"
 kubernetes = "==24.2.0"
 gunicorn = "==20.1.0"
-redis = "==4.3.5"
+redis = "==4.4.4"
 flask-cors = "==3.0.10"
 
 [dev-packages]
 
 [requires]
 python_version = "3.11"
```

### Comparing `unfurl-0.6.1/unfurl/templates/python3.11/Pipfile.lock` & `unfurl-0.6.2/unfurl/templates/python3.11/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821887860082305%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'527524221926f74b48ddc182cd8e487f90327a2e06ea2fc942f8e889530dc03d'}}",*

 * * "'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:308c5a8293d9b76e74921f4d945be19cc467b92e5f128df1db76e31c71345bb3', "*

 * *              "'sha256:bcd09f16bdf3d71ab7d0fab20e97242f09c63f4cea0943329521ab35a950f900'], "*

 * *              "'version': '==1.26.104'}, 'botocore': {'hashes': "*

 * *              "['sha256:7e7a01cef10b1daa9cb01ec25a15e831e7359fc43d1b591359710f203c3620a8', "*

 * *           […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "dfaff3ce975f9f48f2338192b9206b6b865ac0362b50bd1ea2ebe021f5585fd2"
+            "sha256": "527524221926f74b48ddc182cd8e487f90327a2e06ea2fc942f8e889530dc03d"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.11"
         },
         "sources": [
             {
@@ -60,43 +60,43 @@
                 "sha256:ea0d3b40a2d852767be77ca343b58a9e3a4b00d9db440efb8da74b4e58025e5a"
             ],
             "index": "pypi",
             "version": "==2.49.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:0b1f82d4565ed875c7975ac0be5665e8d948613c01bcb0e49df6d4f5af670cc8",
-                "sha256:319ddb274f8f83b035b88a3b127c465bf6fe3e3fc2d668869b489e992c47ca77"
+                "sha256:308c5a8293d9b76e74921f4d945be19cc467b92e5f128df1db76e31c71345bb3",
+                "sha256:bcd09f16bdf3d71ab7d0fab20e97242f09c63f4cea0943329521ab35a950f900"
             ],
             "index": "pypi",
-            "version": "==1.26.52"
+            "version": "==1.26.104"
         },
         "botocore": {
             "hashes": [
-                "sha256:a0b89a33305cfa6251c6e1142deb7567e216e37e25363159f45fb81dc5b474e5",
-                "sha256:de55b6333fb13c66da9055972d7e4efff5dcc5a087478a2b70e99d888b29a24c"
+                "sha256:7e7a01cef10b1daa9cb01ec25a15e831e7359fc43d1b591359710f203c3620a8",
+                "sha256:932bfbf580a2ae53f471df4bfbebce531985ee27468cf7c37d7ccfb3cf8bc9e4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.52"
+            "version": "==1.29.104"
         },
         "cachelib": {
             "hashes": [
-                "sha256:292e89d5f9201fb9570e9f222c202f59085c66f9cb8bdfeefcfffff2b442fb2a",
-                "sha256:6fbbae4637491cc78a5e82f7cf623eb6778ea21ad8aa92197f45a1add51dab02"
+                "sha256:42d49f2fad9310dd946d7be73d46776bcd4d5fde4f49ad210cfdd447fbdfc346",
+                "sha256:593faeee62a7c037d50fc835617a01b887503f972fb52b188ae7e50e9cb69740"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.10.0"
+            "version": "==0.10.2"
         },
         "cachetools": {
             "hashes": [
-                "sha256:5991bc0e08a1319bb618d3195ca5b6bc76646a49c21d55962977197b301cc1fe",
-                "sha256:8462eebf3a6c15d25430a8c27c56ac61340b2ecf60c9ce57afc2b97e450e47da"
+                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
+                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
-            "version": "==5.2.1"
+            "version": "==5.3.0"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "index": "pypi",
@@ -169,104 +169,92 @@
                 "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
                 "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
             "version": "==1.15.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "version": "==3.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
@@ -286,129 +274,125 @@
                 "sha256:a21da482714b9f0b0e9bafaaf2f6a8b3b14161bb47f62e10e28d2fe4ff4b1626"
             ],
             "index": "pypi",
             "version": "==3.10.1"
         },
         "cmd2": {
             "hashes": [
-                "sha256:073e555c05853b0f6965f3d03329babdf9e38a5f2cea028e61a64cd7eeb74ad5",
-                "sha256:a77e3056751393270b4125c990cf527db132f15951a20a3a5dd2df4290aadf20"
+                "sha256:71873c11f72bd19e2b1db578214716f0d4f7c8fa250093c601265a9a717dee52",
+                "sha256:f1988ff2fff0ed812a2d25218a081b0fa0108d45b48ba2a9272bb98091b654e6"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.4.2"
+            "version": "==2.4.3"
         },
         "commonmark": {
             "hashes": [
                 "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60",
                 "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"
             ],
             "version": "==0.9.1"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:051afcbd6d2ac39298d62d340f94dbb6a1f31de06dfaf6fcef7b759dd3860c45",
-                "sha256:0a1890fca2962c4f1ad16551d660b46ea77291fba2cc21c024cd527b9d9c8809",
-                "sha256:0ee30375b409d9a7ea0f30c50645d436b6f5dfee254edffd27e45a980ad2c7f4",
-                "sha256:13250b1f0bd023e0c9f11838bdeb60214dd5b6aaf8e8d2f110c7e232a1bff83b",
-                "sha256:17e01dd8666c445025c29684d4aabf5a90dc6ef1ab25328aa52bedaa95b65ad7",
-                "sha256:19245c249aa711d954623d94f23cc94c0fd65865661f20b7781210cb97c471c0",
-                "sha256:1caed2367b32cc80a2b7f58a9f46658218a19c6cfe5bc234021966dc3daa01f0",
-                "sha256:1f66862d3a41674ebd8d1a7b6f5387fe5ce353f8719040a986551a545d7d83ea",
-                "sha256:220e3fa77d14c8a507b2d951e463b57a1f7810a6443a26f9b7591ef39047b1b2",
-                "sha256:276f4cd0001cd83b00817c8db76730938b1ee40f4993b6a905f40a7278103b3a",
-                "sha256:29de916ba1099ba2aab76aca101580006adfac5646de9b7c010a0f13867cba45",
-                "sha256:2a7f23bbaeb2a87f90f607730b45564076d870f1fb07b9318d0c21f36871932b",
-                "sha256:2c407b1950b2d2ffa091f4e225ca19a66a9bd81222f27c56bd12658fc5ca1209",
-                "sha256:30b5fec1d34cc932c1bc04017b538ce16bf84e239378b8f75220478645d11fca",
-                "sha256:3c2155943896ac78b9b0fd910fb381186d0c345911f5333ee46ac44c8f0e43ab",
-                "sha256:411d4ff9d041be08fdfc02adf62e89c735b9468f6d8f6427f8a14b6bb0a85095",
-                "sha256:436e103950d05b7d7f55e39beeb4d5be298ca3e119e0589c0227e6d0b01ee8c7",
-                "sha256:49640bda9bda35b057b0e65b7c43ba706fa2335c9a9896652aebe0fa399e80e6",
-                "sha256:4a950f83fd3f9bca23b77442f3a2b2ea4ac900944d8af9993743774c4fdc57af",
-                "sha256:50a6adc2be8edd7ee67d1abc3cd20678987c7b9d79cd265de55941e3d0d56499",
-                "sha256:52ab14b9e09ce052237dfe12d6892dd39b0401690856bcfe75d5baba4bfe2831",
-                "sha256:54f7e9705e14b2c9f6abdeb127c390f679f6dbe64ba732788d3015f7f76ef637",
-                "sha256:66e50680e888840c0995f2ad766e726ce71ca682e3c5f4eee82272c7671d38a2",
-                "sha256:790e4433962c9f454e213b21b0fd4b42310ade9c077e8edcb5113db0818450cb",
-                "sha256:7a38362528a9115a4e276e65eeabf67dcfaf57698e17ae388599568a78dcb029",
-                "sha256:7b05ed4b35bf6ee790832f68932baf1f00caa32283d66cc4d455c9e9d115aafc",
-                "sha256:7e109f1c9a3ece676597831874126555997c48f62bddbcace6ed17be3e372de8",
-                "sha256:949844af60ee96a376aac1ded2a27e134b8c8d35cc006a52903fc06c24a3296f",
-                "sha256:95304068686545aa368b35dfda1cdfbbdbe2f6fe43de4a2e9baa8ebd71be46e2",
-                "sha256:9e662e6fc4f513b79da5d10a23edd2b87685815b337b1a30cd11307a6679148d",
-                "sha256:a9fed35ca8c6e946e877893bbac022e8563b94404a605af1d1e6accc7eb73289",
-                "sha256:b69522b168a6b64edf0c33ba53eac491c0a8f5cc94fa4337f9c6f4c8f2f5296c",
-                "sha256:b78729038abea6a5df0d2708dce21e82073463b2d79d10884d7d591e0f385ded",
-                "sha256:b8c56bec53d6e3154eaff6ea941226e7bd7cc0d99f9b3756c2520fc7a94e6d96",
-                "sha256:b9727ac4f5cf2cbf87880a63870b5b9730a8ae3a4a360241a0fdaa2f71240ff0",
-                "sha256:ba3027deb7abf02859aca49c865ece538aee56dcb4871b4cced23ba4d5088904",
-                "sha256:be9fcf32c010da0ba40bf4ee01889d6c737658f4ddff160bd7eb9cac8f094b21",
-                "sha256:c18d47f314b950dbf24a41787ced1474e01ca816011925976d90a88b27c22b89",
-                "sha256:c76a3075e96b9c9ff00df8b5f7f560f5634dffd1658bafb79eb2682867e94f78",
-                "sha256:cbfcba14a3225b055a28b3199c3d81cd0ab37d2353ffd7f6fd64844cebab31ad",
-                "sha256:d254666d29540a72d17cc0175746cfb03d5123db33e67d1020e42dae611dc196",
-                "sha256:d66187792bfe56f8c18ba986a0e4ae44856b1c645336bd2c776e3386da91e1dd",
-                "sha256:d8d04e755934195bdc1db45ba9e040b8d20d046d04d6d77e71b3b34a8cc002d0",
-                "sha256:d8f3e2e0a1d6777e58e834fd5a04657f66affa615dae61dd67c35d1568c38882",
-                "sha256:e057e74e53db78122a3979f908973e171909a58ac20df05c33998d52e6d35757",
-                "sha256:e4ce984133b888cc3a46867c8b4372c7dee9cee300335e2925e197bcd45b9e16",
-                "sha256:ea76dbcad0b7b0deb265d8c36e0801abcddf6cc1395940a24e3595288b405ca0",
-                "sha256:ecb0f73954892f98611e183f50acdc9e21a4653f294dfbe079da73c6378a6f47",
-                "sha256:ef14d75d86f104f03dea66c13188487151760ef25dd6b2dbd541885185f05f40",
-                "sha256:f26648e1b3b03b6022b48a9b910d0ae209e2d51f50441db5dce5b530fad6d9b1",
-                "sha256:f67472c09a0c7486e27f3275f617c964d25e35727af952869dd496b9b5b7f6a3"
+                "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d",
+                "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4",
+                "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e",
+                "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab",
+                "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90",
+                "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6",
+                "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731",
+                "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540",
+                "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2",
+                "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292",
+                "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5",
+                "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b",
+                "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2",
+                "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0",
+                "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57",
+                "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3",
+                "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140",
+                "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84",
+                "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988",
+                "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67",
+                "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d",
+                "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2",
+                "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5",
+                "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9",
+                "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8",
+                "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd",
+                "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6",
+                "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be",
+                "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88",
+                "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25",
+                "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137",
+                "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968",
+                "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9",
+                "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef",
+                "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54",
+                "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512",
+                "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005",
+                "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f",
+                "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149",
+                "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d",
+                "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8",
+                "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7",
+                "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5",
+                "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016",
+                "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69",
+                "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212",
+                "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc",
+                "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8",
+                "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d",
+                "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd",
+                "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.0.5"
+            "version": "==7.2.2"
         },
         "cryptography": {
             "hashes": [
-                "sha256:1a6915075c6d3a5e1215eab5d99bcec0da26036ff2102a1038401d6ef5bef25b",
-                "sha256:1ee1fd0de9851ff32dbbb9362a4d833b579b4a6cc96883e8e6d2ff2a6bc7104f",
-                "sha256:407cec680e811b4fc829de966f88a7c62a596faa250fc1a4b520a0355b9bc190",
-                "sha256:50386acb40fbabbceeb2986332f0287f50f29ccf1497bae31cf5c3e7b4f4b34f",
-                "sha256:6f97109336df5c178ee7c9c711b264c502b905c2d2a29ace99ed761533a3460f",
-                "sha256:754978da4d0457e7ca176f58c57b1f9de6556591c19b25b8bcce3c77d314f5eb",
-                "sha256:76c24dd4fd196a80f9f2f5405a778a8ca132f16b10af113474005635fe7e066c",
-                "sha256:7dacfdeee048814563eaaec7c4743c8aea529fe3dd53127313a792f0dadc1773",
-                "sha256:80ee674c08aaef194bc4627b7f2956e5ba7ef29c3cc3ca488cf15854838a8f72",
-                "sha256:844ad4d7c3850081dffba91cdd91950038ee4ac525c575509a42d3fc806b83c8",
-                "sha256:875aea1039d78557c7c6b4db2fe0e9d2413439f4676310a5f269dd342ca7a717",
-                "sha256:887cbc1ea60786e534b00ba8b04d1095f4272d380ebd5f7a7eb4cc274710fad9",
-                "sha256:ad04f413436b0781f20c52a661660f1e23bcd89a0e9bb1d6d20822d048cf2856",
-                "sha256:bae6c7f4a36a25291b619ad064a30a07110a805d08dc89984f4f441f6c1f3f96",
-                "sha256:c52a1a6f81e738d07f43dab57831c29e57d21c81a942f4602fac7ee21b27f288",
-                "sha256:e0a05aee6a82d944f9b4edd6a001178787d1546ec7c6223ee9a848a7ade92e39",
-                "sha256:e324de6972b151f99dc078defe8fb1b0a82c6498e37bff335f5bc6b1e3ab5a1e",
-                "sha256:e5d71c5d5bd5b5c3eebcf7c5c2bb332d62ec68921a8c593bea8c394911a005ce",
-                "sha256:f3ed2d864a2fa1666e749fe52fb8e23d8e06b8012e8bd8147c73797c506e86f1",
-                "sha256:f671c1bb0d6088e94d61d80c606d65baacc0d374e67bf895148883461cd848de",
-                "sha256:f6c0db08d81ead9576c4d94bbb27aed8d7a430fa27890f39084c2d0e2ec6b0df",
-                "sha256:f964c7dcf7802d133e8dbd1565914fa0194f9d683d82411989889ecd701e8adf",
-                "sha256:fec8b932f51ae245121c4671b4bbc030880f363354b2f0e0bd1366017d891458"
+                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
+                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
+                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
+                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
+                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
+                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
+                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
+                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
+                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
+                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
+                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
+                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
+                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
+                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
+                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
+                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
+                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
+                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
+                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==39.0.0"
+            "version": "==40.0.1"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
         "dnspython": {
             "hashes": [
                 "sha256:224e32b03eb46be70e12ef6d64e0be123a64e621ab4c0822ff6d450d52a540b9",
                 "sha256:89141536394f909066cabd112e3e1a37e4e654db00a25308b0f130bc3152eb46"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
+            "markers": "python_version >= '3.7' and python_version < '4.0'",
             "version": "==2.3.0"
         },
         "docker": {
             "extras": [
                 "tls"
             ],
             "hashes": [
@@ -416,19 +400,19 @@
                 "sha256:dbcb3bd2fa80dca0788ed908218bf43972772009b881ed1e20dfc29a65e49782"
             ],
             "index": "pypi",
             "version": "==6.0.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:892be14aa8efc01673b5ed6589dbccb95f9a8596f0507e232626155495c18105",
+                "sha256:bde48477b15fde2c7e5a0713cbe72721cb5a5ad32ee0b8f419907960b9d75536"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.0"
+            "version": "==3.10.7"
         },
         "flask": {
             "hashes": [
                 "sha256:15972e5017df0575c3d6c090ba168b6db90259e620ac8d7ea813a396bad5b6cb",
                 "sha256:9013281a7402ad527f8fd56375164f3aa021ecfaff89bfe3825346c24f87e04c"
             ],
             "index": "pypi",
@@ -451,15 +435,15 @@
             "version": "==3.0.10"
         },
         "fqdn": {
             "hashes": [
                 "sha256:105ed3677e767fb5ca086a0c1f4bb66ebc3c100be518f0e0d755d9eae164d89f",
                 "sha256:3a179af3761e4df6eb2e026ff9e1a3033d3587bf980a0b1b2e1e5d08d7358014"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4.0'",
             "version": "==1.5.1"
         },
         "gitdb": {
             "hashes": [
                 "sha256:6eb990b69df4e15bad899ea868dc46572c3f75339735663b81de79b06f17eb9a",
                 "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"
             ],
@@ -483,19 +467,19 @@
                 "sha256:34f24bd1d5f72a8c4519773d99ca6bf080a6c4e041b4e9f024fe230191dda62e"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.10.2"
         },
         "google-auth": {
             "hashes": [
-                "sha256:5045648c821fb72384cdc0e82cc326df195f113a33049d9b62b74589243d2acc",
-                "sha256:ed7057a101af1146f0554a769930ac9de506aeca4fd5af6543ebe791851a9fbd"
+                "sha256:357ff22a75b4c0f6093470f21816a825d2adee398177569824e37b6c10069e19",
+                "sha256:8f379b46bad381ad2a0b989dfb0c13ad28d3c2a79f27348213f8946a1d15d55a"
             ],
             "index": "pypi",
-            "version": "==2.16.0"
+            "version": "==2.17.1"
         },
         "google-cloud-compute": {
             "hashes": [
                 "sha256:1ddd1be44d278754fc2643be7aa8d66838235ce44cfbacbeeadf3952ec020e95",
                 "sha256:21bd66251356d70bfd5f40211b42b936335490f7433b3b6fae7c498077e2c3fa"
             ],
             "index": "pypi",
@@ -515,19 +499,19 @@
                 "sha256:bd75d6e9fd456ce643ee936a113a1ead5405704515caa679db30d7f036e447f3"
             ],
             "index": "pypi",
             "version": "==0.34.0"
         },
         "googleapis-common-protos": {
             "hashes": [
-                "sha256:c727251ec025947d545184ba17e3578840fc3a24a0516a020479edab660457df",
-                "sha256:ca3befcd4580dab6ad49356b46bf165bb68ff4b32389f028f1abd7c10ab9519a"
+                "sha256:4168fcb568a826a52f23510412da405abd93f4d23ba544bb68d943b14ba3cb44",
+                "sha256:b287dc48449d1d41af0c69f4ea26242b5ae4c3d7249a38b0984c86a4caffff1f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.58.0"
+            "version": "==1.59.0"
         },
         "grpcio": {
             "hashes": [
                 "sha256:05f7c248e440f538aaad13eee78ef35f0541e73498dd6f832fe284542ac4b298",
                 "sha256:080b66253f29e1646ac53ef288c12944b131a2829488ac3bac8f52abb4413c0d",
                 "sha256:12b479839a5e753580b5e6053571de14006157f2ef9b71f38c56dc9b23b95ad6",
                 "sha256:156f8009e36780fab48c979c5605eda646065d4695deea4cfcbcfdd06627ddb6",
@@ -716,19 +700,19 @@
                 "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
             ],
             "index": "pypi",
             "version": "==2.1.1"
         },
         "natsort": {
             "hashes": [
-                "sha256:04fe18fdd2b9e5957f19f687eb117f102ef8dde6b574764e536e91194bed4f5f",
-                "sha256:57f85b72c688b09e053cdac302dd5b5b53df5f73ae20b4874fcbffd8bf783d11"
+                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
+                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==8.2.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==8.3.1"
         },
         "oauthlib": {
             "hashes": [
                 "sha256:8139f29aac13e25d502680e9e19963e83f16838d48a0d71c287fe40e7067fbca",
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
@@ -763,35 +747,35 @@
                 "sha256:e8dca2f4b43560edef58813969f52a56cef023146cbb8931626db80e6c1c4308"
             ],
             "index": "pypi",
             "version": "==5.9.0"
         },
         "pip": {
             "hashes": [
-                "sha256:65fd48317359f3af8e593943e6ae1506b66325085ea64b706a998c6e83eeaf38",
-                "sha256:908c78e6bc29b676ede1c4d57981d490cb892eb45cd8c214ab6298125119e077"
+                "sha256:236bcb61156d76c4b8a05821b988c7b8c35bf0da28a4b614e8d6ab5212c25c6f",
+                "sha256:cd015ea1bfb0fcef59d8a286c1f8bebcb983f6317719d415dc5351efb7cd7024"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==22.3.1"
+            "version": "==23.0.1"
         },
         "pipenv": {
             "hashes": [
                 "sha256:3b80b4512934b9d8e8ce12c988394642ff96bb697680e5b092e59af503178327",
                 "sha256:f84d7119239b22ab2ac2b8fbc7d619d83cf41135206d72a17c4f151cda529fd0"
             ],
             "index": "pypi",
             "version": "==2022.1.8"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490",
-                "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"
+                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
+                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.6.2"
+            "version": "==3.2.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -884,15 +868,15 @@
             ],
             "version": "==0.2.8"
         },
         "pycountry": {
             "hashes": [
                 "sha256:b2163a246c585894d808f18783e19137cb70a0c18fb36748dc01fc6f109c1646"
             ],
-            "markers": "python_version >= '3.6' and python_version < '4'",
+            "markers": "python_version >= '3.6' and python_version < '4.0'",
             "version": "==22.3.5"
         },
         "pycountry-convert": {
             "hashes": [
                 "sha256:095d310f746bf2a5ef713b3a82eea28a27262286223765b1e7be8a5c4fa7e9b9",
                 "sha256:5e33883a88b3cb752d332ca2358ac6c4de4defc86a2b93b713b36338e914952e"
             ],
@@ -932,19 +916,19 @@
                 "sha256:cdc7b5e3ed77bed61270a47d35434a30617b9becdf2478af76ad2c6ade307280"
             ],
             "index": "pypi",
             "version": "==0.15.7"
         },
         "pytest": {
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
+                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.2.1"
+            "version": "==7.2.2"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b",
                 "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
             ],
             "markers": "python_version >= '3.6'",
@@ -964,19 +948,19 @@
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "index": "pypi",
             "version": "==2.8.2"
         },
         "python-gitlab": {
             "hashes": [
-                "sha256:251b63f0589d51f854516948c84e9eb8df26e1e9dea595cf86b43f17c43007dd",
-                "sha256:6180b81ee2f265ad8d8412956a1740b4d3ceca7b28ae2f707dfe62375fed0082"
+                "sha256:85ae778d8953aba87ad4b78aef7fbb5dae053980d2c20ff200bea29799685743",
+                "sha256:ad502b72b5d1137f4af37d4a68ae20fe7d6c9778f67cbe2aec566f7995053c7d"
             ],
             "index": "pypi",
-            "version": "==3.4.0"
+            "version": "==3.13.0"
         },
         "python-string-utils": {
             "hashes": [
                 "sha256:dcf9060b03f07647c0a603408dc8b03f807f3b54a05c6e19eb14460256fac0cb",
                 "sha256:f1a88700baf99db1a9b6953f44181ad9ca56623c81e257e6009707e2e7851fa4"
             ],
             "markers": "python_version >= '3.5'",
@@ -1026,19 +1010,19 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "index": "pypi",
             "version": "==6.0"
         },
         "redis": {
             "hashes": [
-                "sha256:30c07511627a4c5c4d970e060000772f323174f75e745a26938319817ead7a12",
-                "sha256:46652271dc7525cd5a9667e5b0ca983c848c75b2b8f7425403395bb8379dcf25"
+                "sha256:68226f7ede928db8302f29ab088a157f41061fa946b7ae865452b6d7838bbffb",
+                "sha256:da92a39fec86438d3f1e2a1db33c312985806954fe860120b582a8430e231d8f"
             ],
             "index": "pypi",
-            "version": "==4.3.5"
+            "version": "==4.4.4"
         },
         "repoze.lru": {
             "hashes": [
                 "sha256:0429a75e19380e4ed50c0694e26ac8819b4ea7851ee1fc7583c8572db80aff77",
                 "sha256:f77bf0e1096ea445beadd35f3479c5cff2aa1efe604a133e67150bc8630a62ea"
             ],
             "version": "==0.7"
@@ -1118,19 +1102,19 @@
                 "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:a78d01d1e2c175c474884671dde039962c9d74c7223db7369771fcf6e29ceeab",
-                "sha256:bd6eb2d6722568de6d14b87c44a96fac54b2a45ff5e940e639979a3d1792adb6"
+                "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a",
+                "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==66.0.0"
+            "version": "==67.6.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
@@ -1166,35 +1150,35 @@
                 "sha256:21c85e0fe4b9a155d0799430b0ad741cdce7e359660ccbd8b530613e8df88ce2"
             ],
             "index": "pypi",
             "version": "==4.1.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         },
         "uvicorn": {
             "hashes": [
                 "sha256:c19a057deb1c5bb060946e2e5c262fc01590c6529c0af2c3d9ce941e89bc30e0",
                 "sha256:cade07c403c397f9fe275492a48c1b869efd175d5d8a692df649e6e7e2ed8f4e"
             ],
             "index": "pypi",
             "version": "==0.18.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:ce3b1684d6e1a20a3e5ed36795a97dfc6af29bc3970ca8dab93e11ac6094b3c4",
-                "sha256:f8b927684efc6f1cc206c9db297a570ab9ad0e51c16fa9e45487d36d1905c058"
+                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
+                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==20.17.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.21.0"
         },
         "virtualenv-clone": {
             "hashes": [
                 "sha256:418ee935c36152f8f153c79824bb93eaf6f0f7984bae31d3f48f350b9183501a",
                 "sha256:44d5263bceed0bac3e1424d64f798095233b64def1c5689afa43dc3223caf5b0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1205,47 +1189,47 @@
                 "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e",
                 "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"
             ],
             "version": "==0.2.6"
         },
         "webcolors": {
             "hashes": [
-                "sha256:16d043d3a08fd6a1b1b7e3e9e62640d09790dce80d2bdd4792a175b35fe794a9",
-                "sha256:d98743d81d498a2d3eaf165196e65481f0d2ea85281463d856b1e51b09f62dce"
+                "sha256:29bc7e8752c0a1bd4a1f03c14d6e6a72e93d82193738fa860cbff59d0fcc11bf",
+                "sha256:c225b674c83fa923be93d235330ce0300373d02885cef23238813b0d5668304a"
             ],
-            "version": "==1.12"
+            "version": "==1.13"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:d6b06432f184438d99ac1f456eaf22fe1ade524c3dd16e661142dc54e9cba574",
-                "sha256:d6e8f90ca8e2dd4e8027c4561adeb9456b54044312dba655e7cae652ceb9ae59"
+                "sha256:3f09e6d8230892547132177f575a4e3e73cfdf06526e20cc02aa1c3b47184d40",
+                "sha256:cdf5877568b7e83aa7cf2244ab56a3213de587bbe0ce9d8b9600fc77b455d89e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.4.2"
+            "version": "==1.5.1"
         },
         "werkzeug": {
             "hashes": [
-                "sha256:7ea2d48322cc7c0f8b3a215ed73eabd7b5d75d0b50e31ab006286ccff9e00b8f",
-                "sha256:f979ab81f58d7318e064e99c4506445d60135ac5cd2e177a2de0089bfd4c9bd5"
+                "sha256:2e1ccc9417d4da358b9de6f174e3ac094391ea1d4fbef2d667865d819dfd0afe",
+                "sha256:56433961bc1f12533306c624f3be5e744389ac61d722175d543e1751285da612"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.2.2"
+            "version": "==2.2.3"
         },
         "wheel": {
             "hashes": [
-                "sha256:965f5259b566725405b05e7cf774052044b1ed30119b5d586b2703aafe8719ac",
-                "sha256:b60533f3f5d530e971d6737ca6d58681ee434818fab630c83a734bb10c083ce8"
+                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
+                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.38.4"
+            "version": "==0.40.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa",
-                "sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.11.0"
+            "version": "==3.15.0"
         }
     },
     "develop": {}
 }
```

### Comparing `unfurl-0.6.1/unfurl/templates/python3.7/Pipfile` & `unfurl-0.6.2/unfurl/templates/python3.7/Pipfile`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 rich = "==12.4.4"
 flask = "<=2.1.3"
 flask-caching = "<=2.0.1"
 uvicorn = "<=0.18.2"
 google-cloud-compute = "==1.3.2"
 google-cloud-dns = "==0.34.0"
 grpcio = "==1.50.0"
-python-gitlab = "<=3.4.0"
+python-gitlab = "==3.13.0"
 certifi = "*"
 kubernetes = "==24.2.0"
 gunicorn = "==20.1.0"
-redis = "==4.3.5"
+redis = "==4.4.4"
 flask-cors = "==3.0.10"
 
 [requires]
 python_version = "3.7"
```

### Comparing `unfurl-0.6.1/unfurl/templates/python3.7/Pipfile.lock` & `unfurl-0.6.2/unfurl/templates/python3.7/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9823948770708029%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'9e05caabe1cfec2cdf6d24b8fe0ad5fb007cff5a4f97898f0a6a4c49dd2abad2'}}",*

 * * "'default'": "{'babel': {'hashes': "*

 * *              "['sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610', "*

 * *              "'sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455'], "*

 * *              "'version': '==2.12.1'}, 'boto3': {'hashes': "*

 * *              "['sha256:308c5a8293d9b76e74921f4d945be19cc467b92e5f128df1db76e31c71345bb3', "*

 * *              " […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "d033c87105dd8ae02f07031f5d7b217cad986426118d34ecdb9959d2dd760903"
+            "sha256": "9e05caabe1cfec2cdf6d24b8fe0ad5fb007cff5a4f97898f0a6a4c49dd2abad2"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.7"
         },
         "sources": [
             {
@@ -52,67 +52,67 @@
                 "sha256:0fbf5efbe78d466a26753e1dee3272423a3adc989d6a778c700e89a3f8ff0d88"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.5.1"
         },
         "babel": {
             "hashes": [
-                "sha256:1ad3eca1c885218f6dce2ab67291178944f810a10a9b5f3cb8382a5a232b64fe",
-                "sha256:5ef4b3226b0180dedded4229651c8b0e1a3a6a2837d45a073272f313e4cf97f6"
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "index": "pypi",
-            "version": "==2.11.0"
+            "version": "==2.12.1"
         },
         "boto": {
             "hashes": [
                 "sha256:147758d41ae7240dc989f0039f27da8ca0d53734be0eb869ef16e3adcfa462e8",
                 "sha256:ea0d3b40a2d852767be77ca343b58a9e3a4b00d9db440efb8da74b4e58025e5a"
             ],
             "index": "pypi",
             "version": "==2.49.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:0b1f82d4565ed875c7975ac0be5665e8d948613c01bcb0e49df6d4f5af670cc8",
-                "sha256:319ddb274f8f83b035b88a3b127c465bf6fe3e3fc2d668869b489e992c47ca77"
+                "sha256:308c5a8293d9b76e74921f4d945be19cc467b92e5f128df1db76e31c71345bb3",
+                "sha256:bcd09f16bdf3d71ab7d0fab20e97242f09c63f4cea0943329521ab35a950f900"
             ],
             "index": "pypi",
-            "version": "==1.26.52"
+            "version": "==1.26.104"
         },
         "botocore": {
             "hashes": [
-                "sha256:a0b89a33305cfa6251c6e1142deb7567e216e37e25363159f45fb81dc5b474e5",
-                "sha256:de55b6333fb13c66da9055972d7e4efff5dcc5a087478a2b70e99d888b29a24c"
+                "sha256:7e7a01cef10b1daa9cb01ec25a15e831e7359fc43d1b591359710f203c3620a8",
+                "sha256:932bfbf580a2ae53f471df4bfbebce531985ee27468cf7c37d7ccfb3cf8bc9e4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.52"
+            "version": "==1.29.104"
         },
         "cached-property": {
             "hashes": [
                 "sha256:9fa5755838eecbb2d234c3aa390bd80fbd3ac6b6869109bfc1b499f7bd89a130",
                 "sha256:df4f613cf7ad9a588cc381aaf4a512d26265ecebd5eb9e1ba12f1319eb85a6a0"
             ],
             "markers": "python_version < '3.8'",
             "version": "==1.5.2"
         },
         "cachelib": {
             "hashes": [
-                "sha256:292e89d5f9201fb9570e9f222c202f59085c66f9cb8bdfeefcfffff2b442fb2a",
-                "sha256:6fbbae4637491cc78a5e82f7cf623eb6778ea21ad8aa92197f45a1add51dab02"
+                "sha256:42d49f2fad9310dd946d7be73d46776bcd4d5fde4f49ad210cfdd447fbdfc346",
+                "sha256:593faeee62a7c037d50fc835617a01b887503f972fb52b188ae7e50e9cb69740"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.10.0"
+            "version": "==0.10.2"
         },
         "cachetools": {
             "hashes": [
-                "sha256:5991bc0e08a1319bb618d3195ca5b6bc76646a49c21d55962977197b301cc1fe",
-                "sha256:8462eebf3a6c15d25430a8c27c56ac61340b2ecf60c9ce57afc2b97e450e47da"
+                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
+                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
-            "version": "==5.2.1"
+            "version": "==5.3.0"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "index": "pypi",
@@ -185,104 +185,92 @@
                 "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
                 "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
             "version": "==1.15.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "version": "==3.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
@@ -302,115 +290,111 @@
                 "sha256:a21da482714b9f0b0e9bafaaf2f6a8b3b14161bb47f62e10e28d2fe4ff4b1626"
             ],
             "index": "pypi",
             "version": "==3.10.1"
         },
         "cmd2": {
             "hashes": [
-                "sha256:073e555c05853b0f6965f3d03329babdf9e38a5f2cea028e61a64cd7eeb74ad5",
-                "sha256:a77e3056751393270b4125c990cf527db132f15951a20a3a5dd2df4290aadf20"
+                "sha256:71873c11f72bd19e2b1db578214716f0d4f7c8fa250093c601265a9a717dee52",
+                "sha256:f1988ff2fff0ed812a2d25218a081b0fa0108d45b48ba2a9272bb98091b654e6"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.4.2"
+            "version": "==2.4.3"
         },
         "commonmark": {
             "hashes": [
                 "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60",
                 "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"
             ],
             "version": "==0.9.1"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:051afcbd6d2ac39298d62d340f94dbb6a1f31de06dfaf6fcef7b759dd3860c45",
-                "sha256:0a1890fca2962c4f1ad16551d660b46ea77291fba2cc21c024cd527b9d9c8809",
-                "sha256:0ee30375b409d9a7ea0f30c50645d436b6f5dfee254edffd27e45a980ad2c7f4",
-                "sha256:13250b1f0bd023e0c9f11838bdeb60214dd5b6aaf8e8d2f110c7e232a1bff83b",
-                "sha256:17e01dd8666c445025c29684d4aabf5a90dc6ef1ab25328aa52bedaa95b65ad7",
-                "sha256:19245c249aa711d954623d94f23cc94c0fd65865661f20b7781210cb97c471c0",
-                "sha256:1caed2367b32cc80a2b7f58a9f46658218a19c6cfe5bc234021966dc3daa01f0",
-                "sha256:1f66862d3a41674ebd8d1a7b6f5387fe5ce353f8719040a986551a545d7d83ea",
-                "sha256:220e3fa77d14c8a507b2d951e463b57a1f7810a6443a26f9b7591ef39047b1b2",
-                "sha256:276f4cd0001cd83b00817c8db76730938b1ee40f4993b6a905f40a7278103b3a",
-                "sha256:29de916ba1099ba2aab76aca101580006adfac5646de9b7c010a0f13867cba45",
-                "sha256:2a7f23bbaeb2a87f90f607730b45564076d870f1fb07b9318d0c21f36871932b",
-                "sha256:2c407b1950b2d2ffa091f4e225ca19a66a9bd81222f27c56bd12658fc5ca1209",
-                "sha256:30b5fec1d34cc932c1bc04017b538ce16bf84e239378b8f75220478645d11fca",
-                "sha256:3c2155943896ac78b9b0fd910fb381186d0c345911f5333ee46ac44c8f0e43ab",
-                "sha256:411d4ff9d041be08fdfc02adf62e89c735b9468f6d8f6427f8a14b6bb0a85095",
-                "sha256:436e103950d05b7d7f55e39beeb4d5be298ca3e119e0589c0227e6d0b01ee8c7",
-                "sha256:49640bda9bda35b057b0e65b7c43ba706fa2335c9a9896652aebe0fa399e80e6",
-                "sha256:4a950f83fd3f9bca23b77442f3a2b2ea4ac900944d8af9993743774c4fdc57af",
-                "sha256:50a6adc2be8edd7ee67d1abc3cd20678987c7b9d79cd265de55941e3d0d56499",
-                "sha256:52ab14b9e09ce052237dfe12d6892dd39b0401690856bcfe75d5baba4bfe2831",
-                "sha256:54f7e9705e14b2c9f6abdeb127c390f679f6dbe64ba732788d3015f7f76ef637",
-                "sha256:66e50680e888840c0995f2ad766e726ce71ca682e3c5f4eee82272c7671d38a2",
-                "sha256:790e4433962c9f454e213b21b0fd4b42310ade9c077e8edcb5113db0818450cb",
-                "sha256:7a38362528a9115a4e276e65eeabf67dcfaf57698e17ae388599568a78dcb029",
-                "sha256:7b05ed4b35bf6ee790832f68932baf1f00caa32283d66cc4d455c9e9d115aafc",
-                "sha256:7e109f1c9a3ece676597831874126555997c48f62bddbcace6ed17be3e372de8",
-                "sha256:949844af60ee96a376aac1ded2a27e134b8c8d35cc006a52903fc06c24a3296f",
-                "sha256:95304068686545aa368b35dfda1cdfbbdbe2f6fe43de4a2e9baa8ebd71be46e2",
-                "sha256:9e662e6fc4f513b79da5d10a23edd2b87685815b337b1a30cd11307a6679148d",
-                "sha256:a9fed35ca8c6e946e877893bbac022e8563b94404a605af1d1e6accc7eb73289",
-                "sha256:b69522b168a6b64edf0c33ba53eac491c0a8f5cc94fa4337f9c6f4c8f2f5296c",
-                "sha256:b78729038abea6a5df0d2708dce21e82073463b2d79d10884d7d591e0f385ded",
-                "sha256:b8c56bec53d6e3154eaff6ea941226e7bd7cc0d99f9b3756c2520fc7a94e6d96",
-                "sha256:b9727ac4f5cf2cbf87880a63870b5b9730a8ae3a4a360241a0fdaa2f71240ff0",
-                "sha256:ba3027deb7abf02859aca49c865ece538aee56dcb4871b4cced23ba4d5088904",
-                "sha256:be9fcf32c010da0ba40bf4ee01889d6c737658f4ddff160bd7eb9cac8f094b21",
-                "sha256:c18d47f314b950dbf24a41787ced1474e01ca816011925976d90a88b27c22b89",
-                "sha256:c76a3075e96b9c9ff00df8b5f7f560f5634dffd1658bafb79eb2682867e94f78",
-                "sha256:cbfcba14a3225b055a28b3199c3d81cd0ab37d2353ffd7f6fd64844cebab31ad",
-                "sha256:d254666d29540a72d17cc0175746cfb03d5123db33e67d1020e42dae611dc196",
-                "sha256:d66187792bfe56f8c18ba986a0e4ae44856b1c645336bd2c776e3386da91e1dd",
-                "sha256:d8d04e755934195bdc1db45ba9e040b8d20d046d04d6d77e71b3b34a8cc002d0",
-                "sha256:d8f3e2e0a1d6777e58e834fd5a04657f66affa615dae61dd67c35d1568c38882",
-                "sha256:e057e74e53db78122a3979f908973e171909a58ac20df05c33998d52e6d35757",
-                "sha256:e4ce984133b888cc3a46867c8b4372c7dee9cee300335e2925e197bcd45b9e16",
-                "sha256:ea76dbcad0b7b0deb265d8c36e0801abcddf6cc1395940a24e3595288b405ca0",
-                "sha256:ecb0f73954892f98611e183f50acdc9e21a4653f294dfbe079da73c6378a6f47",
-                "sha256:ef14d75d86f104f03dea66c13188487151760ef25dd6b2dbd541885185f05f40",
-                "sha256:f26648e1b3b03b6022b48a9b910d0ae209e2d51f50441db5dce5b530fad6d9b1",
-                "sha256:f67472c09a0c7486e27f3275f617c964d25e35727af952869dd496b9b5b7f6a3"
+                "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d",
+                "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4",
+                "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e",
+                "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab",
+                "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90",
+                "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6",
+                "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731",
+                "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540",
+                "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2",
+                "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292",
+                "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5",
+                "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b",
+                "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2",
+                "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0",
+                "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57",
+                "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3",
+                "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140",
+                "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84",
+                "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988",
+                "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67",
+                "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d",
+                "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2",
+                "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5",
+                "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9",
+                "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8",
+                "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd",
+                "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6",
+                "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be",
+                "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88",
+                "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25",
+                "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137",
+                "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968",
+                "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9",
+                "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef",
+                "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54",
+                "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512",
+                "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005",
+                "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f",
+                "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149",
+                "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d",
+                "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8",
+                "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7",
+                "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5",
+                "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016",
+                "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69",
+                "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212",
+                "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc",
+                "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8",
+                "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d",
+                "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd",
+                "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.0.5"
+            "version": "==7.2.2"
         },
         "cryptography": {
             "hashes": [
-                "sha256:1a6915075c6d3a5e1215eab5d99bcec0da26036ff2102a1038401d6ef5bef25b",
-                "sha256:1ee1fd0de9851ff32dbbb9362a4d833b579b4a6cc96883e8e6d2ff2a6bc7104f",
-                "sha256:407cec680e811b4fc829de966f88a7c62a596faa250fc1a4b520a0355b9bc190",
-                "sha256:50386acb40fbabbceeb2986332f0287f50f29ccf1497bae31cf5c3e7b4f4b34f",
-                "sha256:6f97109336df5c178ee7c9c711b264c502b905c2d2a29ace99ed761533a3460f",
-                "sha256:754978da4d0457e7ca176f58c57b1f9de6556591c19b25b8bcce3c77d314f5eb",
-                "sha256:76c24dd4fd196a80f9f2f5405a778a8ca132f16b10af113474005635fe7e066c",
-                "sha256:7dacfdeee048814563eaaec7c4743c8aea529fe3dd53127313a792f0dadc1773",
-                "sha256:80ee674c08aaef194bc4627b7f2956e5ba7ef29c3cc3ca488cf15854838a8f72",
-                "sha256:844ad4d7c3850081dffba91cdd91950038ee4ac525c575509a42d3fc806b83c8",
-                "sha256:875aea1039d78557c7c6b4db2fe0e9d2413439f4676310a5f269dd342ca7a717",
-                "sha256:887cbc1ea60786e534b00ba8b04d1095f4272d380ebd5f7a7eb4cc274710fad9",
-                "sha256:ad04f413436b0781f20c52a661660f1e23bcd89a0e9bb1d6d20822d048cf2856",
-                "sha256:bae6c7f4a36a25291b619ad064a30a07110a805d08dc89984f4f441f6c1f3f96",
-                "sha256:c52a1a6f81e738d07f43dab57831c29e57d21c81a942f4602fac7ee21b27f288",
-                "sha256:e0a05aee6a82d944f9b4edd6a001178787d1546ec7c6223ee9a848a7ade92e39",
-                "sha256:e324de6972b151f99dc078defe8fb1b0a82c6498e37bff335f5bc6b1e3ab5a1e",
-                "sha256:e5d71c5d5bd5b5c3eebcf7c5c2bb332d62ec68921a8c593bea8c394911a005ce",
-                "sha256:f3ed2d864a2fa1666e749fe52fb8e23d8e06b8012e8bd8147c73797c506e86f1",
-                "sha256:f671c1bb0d6088e94d61d80c606d65baacc0d374e67bf895148883461cd848de",
-                "sha256:f6c0db08d81ead9576c4d94bbb27aed8d7a430fa27890f39084c2d0e2ec6b0df",
-                "sha256:f964c7dcf7802d133e8dbd1565914fa0194f9d683d82411989889ecd701e8adf",
-                "sha256:fec8b932f51ae245121c4671b4bbc030880f363354b2f0e0bd1366017d891458"
+                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
+                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
+                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
+                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
+                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
+                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
+                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
+                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
+                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
+                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
+                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
+                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
+                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
+                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
+                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
+                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
+                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
+                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
+                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
             ],
             "index": "pypi",
-            "version": "==39.0.0"
+            "version": "==40.0.1"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
@@ -441,27 +425,27 @@
                 "sha256:cce6a7477ed816bd2542d03d53db9f0db935dd013b70f336a95c73979289f248"
             ],
             "index": "pypi",
             "version": "==1.1.10"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e",
-                "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"
+                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
+                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.0"
+            "version": "==1.1.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:892be14aa8efc01673b5ed6589dbccb95f9a8596f0507e232626155495c18105",
+                "sha256:bde48477b15fde2c7e5a0713cbe72721cb5a5ad32ee0b8f419907960b9d75536"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.0"
+            "version": "==3.10.7"
         },
         "flask": {
             "hashes": [
                 "sha256:15972e5017df0575c3d6c090ba168b6db90259e620ac8d7ea813a396bad5b6cb",
                 "sha256:9013281a7402ad527f8fd56375164f3aa021ecfaff89bfe3825346c24f87e04c"
             ],
             "index": "pypi",
@@ -516,19 +500,19 @@
                 "sha256:ce222e27b0de0d7bc63eb043b956996d6dccab14cc3b690aaea91c9cc99dc16e"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.11.0"
         },
         "google-auth": {
             "hashes": [
-                "sha256:5045648c821fb72384cdc0e82cc326df195f113a33049d9b62b74589243d2acc",
-                "sha256:ed7057a101af1146f0554a769930ac9de506aeca4fd5af6543ebe791851a9fbd"
+                "sha256:357ff22a75b4c0f6093470f21816a825d2adee398177569824e37b6c10069e19",
+                "sha256:8f379b46bad381ad2a0b989dfb0c13ad28d3c2a79f27348213f8946a1d15d55a"
             ],
             "index": "pypi",
-            "version": "==2.16.0"
+            "version": "==2.17.1"
         },
         "google-cloud-compute": {
             "hashes": [
                 "sha256:1ddd1be44d278754fc2643be7aa8d66838235ce44cfbacbeeadf3952ec020e95",
                 "sha256:21bd66251356d70bfd5f40211b42b936335490f7433b3b6fae7c498077e2c3fa"
             ],
             "index": "pypi",
@@ -548,19 +532,19 @@
                 "sha256:bd75d6e9fd456ce643ee936a113a1ead5405704515caa679db30d7f036e447f3"
             ],
             "index": "pypi",
             "version": "==0.34.0"
         },
         "googleapis-common-protos": {
             "hashes": [
-                "sha256:c727251ec025947d545184ba17e3578840fc3a24a0516a020479edab660457df",
-                "sha256:ca3befcd4580dab6ad49356b46bf165bb68ff4b32389f028f1abd7c10ab9519a"
+                "sha256:4168fcb568a826a52f23510412da405abd93f4d23ba544bb68d943b14ba3cb44",
+                "sha256:b287dc48449d1d41af0c69f4ea26242b5ae4c3d7249a38b0984c86a4caffff1f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.58.0"
+            "version": "==1.59.0"
         },
         "grpcio": {
             "hashes": [
                 "sha256:05f7c248e440f538aaad13eee78ef35f0541e73498dd6f832fe284542ac4b298",
                 "sha256:080b66253f29e1646ac53ef288c12944b131a2829488ac3bac8f52abb4413c0d",
                 "sha256:12b479839a5e753580b5e6053571de14006157f2ef9b71f38c56dc9b23b95ad6",
                 "sha256:156f8009e36780fab48c979c5605eda646065d4695deea4cfcbcfdd06627ddb6",
@@ -756,19 +740,19 @@
                 "sha256:c2dd28d6b964699822455f6c91acedc16324913586837f046a76e2e4ac1d716c"
             ],
             "index": "pypi",
             "version": "==0.2.7"
         },
         "natsort": {
             "hashes": [
-                "sha256:04fe18fdd2b9e5957f19f687eb117f102ef8dde6b574764e536e91194bed4f5f",
-                "sha256:57f85b72c688b09e053cdac302dd5b5b53df5f73ae20b4874fcbffd8bf783d11"
+                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
+                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==8.2.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==8.3.1"
         },
         "oauthlib": {
             "hashes": [
                 "sha256:8139f29aac13e25d502680e9e19963e83f16838d48a0d71c287fe40e7067fbca",
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
@@ -803,19 +787,19 @@
                 "sha256:e8dca2f4b43560edef58813969f52a56cef023146cbb8931626db80e6c1c4308"
             ],
             "index": "pypi",
             "version": "==5.9.0"
         },
         "pip": {
             "hashes": [
-                "sha256:65fd48317359f3af8e593943e6ae1506b66325085ea64b706a998c6e83eeaf38",
-                "sha256:908c78e6bc29b676ede1c4d57981d490cb892eb45cd8c214ab6298125119e077"
+                "sha256:236bcb61156d76c4b8a05821b988c7b8c35bf0da28a4b614e8d6ab5212c25c6f",
+                "sha256:cd015ea1bfb0fcef59d8a286c1f8bebcb983f6317719d415dc5351efb7cd7024"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==22.3.1"
+            "version": "==23.0.1"
         },
         "pipenv": {
             "hashes": [
                 "sha256:3b80b4512934b9d8e8ce12c988394642ff96bb697680e5b092e59af503178327",
                 "sha256:f84d7119239b22ab2ac2b8fbc7d619d83cf41135206d72a17c4f151cda529fd0"
             ],
             "index": "pypi",
@@ -972,19 +956,19 @@
                 "sha256:cdc7b5e3ed77bed61270a47d35434a30617b9becdf2478af76ad2c6ade307280"
             ],
             "index": "pypi",
             "version": "==0.15.7"
         },
         "pytest": {
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
+                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.2.1"
+            "version": "==7.2.2"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b",
                 "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
             ],
             "markers": "python_version >= '3.6'",
@@ -1004,34 +988,35 @@
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "index": "pypi",
             "version": "==2.8.2"
         },
         "python-gitlab": {
             "hashes": [
-                "sha256:251b63f0589d51f854516948c84e9eb8df26e1e9dea595cf86b43f17c43007dd",
-                "sha256:6180b81ee2f265ad8d8412956a1740b4d3ceca7b28ae2f707dfe62375fed0082"
+                "sha256:85ae778d8953aba87ad4b78aef7fbb5dae053980d2c20ff200bea29799685743",
+                "sha256:ad502b72b5d1137f4af37d4a68ae20fe7d6c9778f67cbe2aec566f7995053c7d"
             ],
             "index": "pypi",
-            "version": "==3.4.0"
+            "version": "==3.13.0"
         },
         "python-string-utils": {
             "hashes": [
                 "sha256:dcf9060b03f07647c0a603408dc8b03f807f3b54a05c6e19eb14460256fac0cb",
                 "sha256:f1a88700baf99db1a9b6953f44181ad9ca56623c81e257e6009707e2e7851fa4"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
         "pytz": {
             "hashes": [
-                "sha256:01a0681c4b9684a28304615eba55d1ab31ae00bf68ec157ec3708a8182dbbcd0",
-                "sha256:78f4f37d8198e0627c5f1143240bb0206b8691d8d7ac6d78fee88b78733f8c4a"
+                "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
+                "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
             ],
-            "version": "==2022.7.1"
+            "markers": "python_version < '3.9'",
+            "version": "==2023.3"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
@@ -1073,19 +1058,19 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "index": "pypi",
             "version": "==6.0"
         },
         "redis": {
             "hashes": [
-                "sha256:30c07511627a4c5c4d970e060000772f323174f75e745a26938319817ead7a12",
-                "sha256:46652271dc7525cd5a9667e5b0ca983c848c75b2b8f7425403395bb8379dcf25"
+                "sha256:68226f7ede928db8302f29ab088a157f41061fa946b7ae865452b6d7838bbffb",
+                "sha256:da92a39fec86438d3f1e2a1db33c312985806954fe860120b582a8430e231d8f"
             ],
             "index": "pypi",
-            "version": "==4.3.5"
+            "version": "==4.4.4"
         },
         "repoze.lru": {
             "hashes": [
                 "sha256:0429a75e19380e4ed50c0694e26ac8819b4ea7851ee1fc7583c8572db80aff77",
                 "sha256:f77bf0e1096ea445beadd35f3479c5cff2aa1efe604a133e67150bc8630a62ea"
             ],
             "version": "==0.7"
@@ -1185,39 +1170,41 @@
                 "sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b",
                 "sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b",
                 "sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640",
                 "sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7",
                 "sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a",
                 "sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71",
                 "sha256:d5e51e2901ec2366b79f16c2299a03e74ba4531ddcfacc1416639c557aef0ad8",
+                "sha256:da538167284de58a52109a9b89b8f6a53ff8437dd6dc26d33b57bf6699153122",
                 "sha256:debc87a9516b237d0466a711b18b6ebeb17ba9f391eb7f91c649c5c4ec5006c7",
                 "sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80",
                 "sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e",
                 "sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab",
                 "sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0",
-                "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646"
+                "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646",
+                "sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38"
             ],
             "markers": "platform_python_implementation == 'CPython' and python_version < '3.11'",
             "version": "==0.2.7"
         },
         "s3transfer": {
             "hashes": [
                 "sha256:06176b74f3a15f61f1b4f25a1fc29a4429040b7647133a463da8fa5bd28d5ecd",
                 "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:a78d01d1e2c175c474884671dde039962c9d74c7223db7369771fcf6e29ceeab",
-                "sha256:bd6eb2d6722568de6d14b87c44a96fac54b2a45ff5e940e639979a3d1792adb6"
+                "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a",
+                "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==66.0.0"
+            "version": "==67.6.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "index": "pypi",
@@ -1270,35 +1257,35 @@
                 "sha256:21c85e0fe4b9a155d0799430b0ad741cdce7e359660ccbd8b530613e8df88ce2"
             ],
             "index": "pypi",
             "version": "==4.1.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         },
         "uvicorn": {
             "hashes": [
                 "sha256:c19a057deb1c5bb060946e2e5c262fc01590c6529c0af2c3d9ce941e89bc30e0",
                 "sha256:cade07c403c397f9fe275492a48c1b869efd175d5d8a692df649e6e7e2ed8f4e"
             ],
             "index": "pypi",
             "version": "==0.18.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:ce3b1684d6e1a20a3e5ed36795a97dfc6af29bc3970ca8dab93e11ac6094b3c4",
-                "sha256:f8b927684efc6f1cc206c9db297a570ab9ad0e51c16fa9e45487d36d1905c058"
+                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
+                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==20.17.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.21.0"
         },
         "virtualenv-clone": {
             "hashes": [
                 "sha256:418ee935c36152f8f153c79824bb93eaf6f0f7984bae31d3f48f350b9183501a",
                 "sha256:44d5263bceed0bac3e1424d64f798095233b64def1c5689afa43dc3223caf5b0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1309,47 +1296,47 @@
                 "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e",
                 "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"
             ],
             "version": "==0.2.6"
         },
         "webcolors": {
             "hashes": [
-                "sha256:16d043d3a08fd6a1b1b7e3e9e62640d09790dce80d2bdd4792a175b35fe794a9",
-                "sha256:d98743d81d498a2d3eaf165196e65481f0d2ea85281463d856b1e51b09f62dce"
+                "sha256:29bc7e8752c0a1bd4a1f03c14d6e6a72e93d82193738fa860cbff59d0fcc11bf",
+                "sha256:c225b674c83fa923be93d235330ce0300373d02885cef23238813b0d5668304a"
             ],
-            "version": "==1.12"
+            "version": "==1.13"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:d6b06432f184438d99ac1f456eaf22fe1ade524c3dd16e661142dc54e9cba574",
-                "sha256:d6e8f90ca8e2dd4e8027c4561adeb9456b54044312dba655e7cae652ceb9ae59"
+                "sha256:3f09e6d8230892547132177f575a4e3e73cfdf06526e20cc02aa1c3b47184d40",
+                "sha256:cdf5877568b7e83aa7cf2244ab56a3213de587bbe0ce9d8b9600fc77b455d89e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.4.2"
+            "version": "==1.5.1"
         },
         "werkzeug": {
             "hashes": [
-                "sha256:7ea2d48322cc7c0f8b3a215ed73eabd7b5d75d0b50e31ab006286ccff9e00b8f",
-                "sha256:f979ab81f58d7318e064e99c4506445d60135ac5cd2e177a2de0089bfd4c9bd5"
+                "sha256:2e1ccc9417d4da358b9de6f174e3ac094391ea1d4fbef2d667865d819dfd0afe",
+                "sha256:56433961bc1f12533306c624f3be5e744389ac61d722175d543e1751285da612"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.2.2"
+            "version": "==2.2.3"
         },
         "wheel": {
             "hashes": [
-                "sha256:965f5259b566725405b05e7cf774052044b1ed30119b5d586b2703aafe8719ac",
-                "sha256:b60533f3f5d530e971d6737ca6d58681ee434818fab630c83a734bb10c083ce8"
+                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
+                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.38.4"
+            "version": "==0.40.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa",
-                "sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.11.0"
+            "version": "==3.15.0"
         }
     },
     "develop": {}
 }
```

### Comparing `unfurl-0.6.1/unfurl/templates/python3.8/Pipfile` & `unfurl-0.6.2/unfurl/templates/python3.8/Pipfile`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 rich = "==12.4.4"
 flask = "<=2.1.3"
 flask-caching = "<=2.0.1"
 uvicorn = "<=0.18.2"
 google-cloud-compute = "==1.3.2"
 google-cloud-dns = "==0.34.0"
 grpcio = "==1.50.0"
-python-gitlab = "<=3.4.0"
+python-gitlab = "==3.13.0"
 certifi = "*"
 kubernetes = "==24.2.0"
 gunicorn = "==20.1.0"
-redis = "==4.3.5"
+redis = "==4.4.4"
 flask-cors = "==3.0.10"
 
 [requires]
 python_version = "3.8"
```

### Comparing `unfurl-0.6.1/unfurl/templates/python3.8/Pipfile.lock` & `unfurl-0.6.2/unfurl/templates/python3.9/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.969282141336739%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'2c0e8afe32a66f671d6ad42ede9d35f518ace83f0d0968409f8a326afdd14e93'}, 'requires': "*

 * *            "{'python_version': '3.9'}}",*

 * * "'default'": "{'babel': {'hashes': "*

 * *              "['sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610', "*

 * *              "'sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455'], "*

 * *              "'version': '==2.12.1'}, 'boto3': {'hashes': "*

 * *              "['sha256:308c5a8293d9b76e74921f4d945be1 […]*

```diff
@@ -1,15 +1,15 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "ca32bfe36fffdf66c6ea29650ba7fd1ab2144819b095d2a41e06bcb206f8816d"
+            "sha256": "2c0e8afe32a66f671d6ad42ede9d35f518ace83f0d0968409f8a326afdd14e93"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.8"
+            "python_version": "3.9"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
@@ -52,59 +52,59 @@
                 "sha256:0fbf5efbe78d466a26753e1dee3272423a3adc989d6a778c700e89a3f8ff0d88"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.5.1"
         },
         "babel": {
             "hashes": [
-                "sha256:1ad3eca1c885218f6dce2ab67291178944f810a10a9b5f3cb8382a5a232b64fe",
-                "sha256:5ef4b3226b0180dedded4229651c8b0e1a3a6a2837d45a073272f313e4cf97f6"
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "index": "pypi",
-            "version": "==2.11.0"
+            "version": "==2.12.1"
         },
         "boto": {
             "hashes": [
                 "sha256:147758d41ae7240dc989f0039f27da8ca0d53734be0eb869ef16e3adcfa462e8",
                 "sha256:ea0d3b40a2d852767be77ca343b58a9e3a4b00d9db440efb8da74b4e58025e5a"
             ],
             "index": "pypi",
             "version": "==2.49.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:0b1f82d4565ed875c7975ac0be5665e8d948613c01bcb0e49df6d4f5af670cc8",
-                "sha256:319ddb274f8f83b035b88a3b127c465bf6fe3e3fc2d668869b489e992c47ca77"
+                "sha256:308c5a8293d9b76e74921f4d945be19cc467b92e5f128df1db76e31c71345bb3",
+                "sha256:bcd09f16bdf3d71ab7d0fab20e97242f09c63f4cea0943329521ab35a950f900"
             ],
             "index": "pypi",
-            "version": "==1.26.52"
+            "version": "==1.26.104"
         },
         "botocore": {
             "hashes": [
-                "sha256:a0b89a33305cfa6251c6e1142deb7567e216e37e25363159f45fb81dc5b474e5",
-                "sha256:de55b6333fb13c66da9055972d7e4efff5dcc5a087478a2b70e99d888b29a24c"
+                "sha256:7e7a01cef10b1daa9cb01ec25a15e831e7359fc43d1b591359710f203c3620a8",
+                "sha256:932bfbf580a2ae53f471df4bfbebce531985ee27468cf7c37d7ccfb3cf8bc9e4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.52"
+            "version": "==1.29.104"
         },
         "cachelib": {
             "hashes": [
-                "sha256:292e89d5f9201fb9570e9f222c202f59085c66f9cb8bdfeefcfffff2b442fb2a",
-                "sha256:6fbbae4637491cc78a5e82f7cf623eb6778ea21ad8aa92197f45a1add51dab02"
+                "sha256:42d49f2fad9310dd946d7be73d46776bcd4d5fde4f49ad210cfdd447fbdfc346",
+                "sha256:593faeee62a7c037d50fc835617a01b887503f972fb52b188ae7e50e9cb69740"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.10.0"
+            "version": "==0.10.2"
         },
         "cachetools": {
             "hashes": [
-                "sha256:5991bc0e08a1319bb618d3195ca5b6bc76646a49c21d55962977197b301cc1fe",
-                "sha256:8462eebf3a6c15d25430a8c27c56ac61340b2ecf60c9ce57afc2b97e450e47da"
+                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
+                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
-            "version": "==5.2.1"
+            "version": "==5.3.0"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "index": "pypi",
@@ -177,104 +177,92 @@
                 "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
                 "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
             "version": "==1.15.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "version": "==3.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
@@ -294,115 +282,111 @@
                 "sha256:a21da482714b9f0b0e9bafaaf2f6a8b3b14161bb47f62e10e28d2fe4ff4b1626"
             ],
             "index": "pypi",
             "version": "==3.10.1"
         },
         "cmd2": {
             "hashes": [
-                "sha256:073e555c05853b0f6965f3d03329babdf9e38a5f2cea028e61a64cd7eeb74ad5",
-                "sha256:a77e3056751393270b4125c990cf527db132f15951a20a3a5dd2df4290aadf20"
+                "sha256:71873c11f72bd19e2b1db578214716f0d4f7c8fa250093c601265a9a717dee52",
+                "sha256:f1988ff2fff0ed812a2d25218a081b0fa0108d45b48ba2a9272bb98091b654e6"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.4.2"
+            "version": "==2.4.3"
         },
         "commonmark": {
             "hashes": [
                 "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60",
                 "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"
             ],
             "version": "==0.9.1"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:051afcbd6d2ac39298d62d340f94dbb6a1f31de06dfaf6fcef7b759dd3860c45",
-                "sha256:0a1890fca2962c4f1ad16551d660b46ea77291fba2cc21c024cd527b9d9c8809",
-                "sha256:0ee30375b409d9a7ea0f30c50645d436b6f5dfee254edffd27e45a980ad2c7f4",
-                "sha256:13250b1f0bd023e0c9f11838bdeb60214dd5b6aaf8e8d2f110c7e232a1bff83b",
-                "sha256:17e01dd8666c445025c29684d4aabf5a90dc6ef1ab25328aa52bedaa95b65ad7",
-                "sha256:19245c249aa711d954623d94f23cc94c0fd65865661f20b7781210cb97c471c0",
-                "sha256:1caed2367b32cc80a2b7f58a9f46658218a19c6cfe5bc234021966dc3daa01f0",
-                "sha256:1f66862d3a41674ebd8d1a7b6f5387fe5ce353f8719040a986551a545d7d83ea",
-                "sha256:220e3fa77d14c8a507b2d951e463b57a1f7810a6443a26f9b7591ef39047b1b2",
-                "sha256:276f4cd0001cd83b00817c8db76730938b1ee40f4993b6a905f40a7278103b3a",
-                "sha256:29de916ba1099ba2aab76aca101580006adfac5646de9b7c010a0f13867cba45",
-                "sha256:2a7f23bbaeb2a87f90f607730b45564076d870f1fb07b9318d0c21f36871932b",
-                "sha256:2c407b1950b2d2ffa091f4e225ca19a66a9bd81222f27c56bd12658fc5ca1209",
-                "sha256:30b5fec1d34cc932c1bc04017b538ce16bf84e239378b8f75220478645d11fca",
-                "sha256:3c2155943896ac78b9b0fd910fb381186d0c345911f5333ee46ac44c8f0e43ab",
-                "sha256:411d4ff9d041be08fdfc02adf62e89c735b9468f6d8f6427f8a14b6bb0a85095",
-                "sha256:436e103950d05b7d7f55e39beeb4d5be298ca3e119e0589c0227e6d0b01ee8c7",
-                "sha256:49640bda9bda35b057b0e65b7c43ba706fa2335c9a9896652aebe0fa399e80e6",
-                "sha256:4a950f83fd3f9bca23b77442f3a2b2ea4ac900944d8af9993743774c4fdc57af",
-                "sha256:50a6adc2be8edd7ee67d1abc3cd20678987c7b9d79cd265de55941e3d0d56499",
-                "sha256:52ab14b9e09ce052237dfe12d6892dd39b0401690856bcfe75d5baba4bfe2831",
-                "sha256:54f7e9705e14b2c9f6abdeb127c390f679f6dbe64ba732788d3015f7f76ef637",
-                "sha256:66e50680e888840c0995f2ad766e726ce71ca682e3c5f4eee82272c7671d38a2",
-                "sha256:790e4433962c9f454e213b21b0fd4b42310ade9c077e8edcb5113db0818450cb",
-                "sha256:7a38362528a9115a4e276e65eeabf67dcfaf57698e17ae388599568a78dcb029",
-                "sha256:7b05ed4b35bf6ee790832f68932baf1f00caa32283d66cc4d455c9e9d115aafc",
-                "sha256:7e109f1c9a3ece676597831874126555997c48f62bddbcace6ed17be3e372de8",
-                "sha256:949844af60ee96a376aac1ded2a27e134b8c8d35cc006a52903fc06c24a3296f",
-                "sha256:95304068686545aa368b35dfda1cdfbbdbe2f6fe43de4a2e9baa8ebd71be46e2",
-                "sha256:9e662e6fc4f513b79da5d10a23edd2b87685815b337b1a30cd11307a6679148d",
-                "sha256:a9fed35ca8c6e946e877893bbac022e8563b94404a605af1d1e6accc7eb73289",
-                "sha256:b69522b168a6b64edf0c33ba53eac491c0a8f5cc94fa4337f9c6f4c8f2f5296c",
-                "sha256:b78729038abea6a5df0d2708dce21e82073463b2d79d10884d7d591e0f385ded",
-                "sha256:b8c56bec53d6e3154eaff6ea941226e7bd7cc0d99f9b3756c2520fc7a94e6d96",
-                "sha256:b9727ac4f5cf2cbf87880a63870b5b9730a8ae3a4a360241a0fdaa2f71240ff0",
-                "sha256:ba3027deb7abf02859aca49c865ece538aee56dcb4871b4cced23ba4d5088904",
-                "sha256:be9fcf32c010da0ba40bf4ee01889d6c737658f4ddff160bd7eb9cac8f094b21",
-                "sha256:c18d47f314b950dbf24a41787ced1474e01ca816011925976d90a88b27c22b89",
-                "sha256:c76a3075e96b9c9ff00df8b5f7f560f5634dffd1658bafb79eb2682867e94f78",
-                "sha256:cbfcba14a3225b055a28b3199c3d81cd0ab37d2353ffd7f6fd64844cebab31ad",
-                "sha256:d254666d29540a72d17cc0175746cfb03d5123db33e67d1020e42dae611dc196",
-                "sha256:d66187792bfe56f8c18ba986a0e4ae44856b1c645336bd2c776e3386da91e1dd",
-                "sha256:d8d04e755934195bdc1db45ba9e040b8d20d046d04d6d77e71b3b34a8cc002d0",
-                "sha256:d8f3e2e0a1d6777e58e834fd5a04657f66affa615dae61dd67c35d1568c38882",
-                "sha256:e057e74e53db78122a3979f908973e171909a58ac20df05c33998d52e6d35757",
-                "sha256:e4ce984133b888cc3a46867c8b4372c7dee9cee300335e2925e197bcd45b9e16",
-                "sha256:ea76dbcad0b7b0deb265d8c36e0801abcddf6cc1395940a24e3595288b405ca0",
-                "sha256:ecb0f73954892f98611e183f50acdc9e21a4653f294dfbe079da73c6378a6f47",
-                "sha256:ef14d75d86f104f03dea66c13188487151760ef25dd6b2dbd541885185f05f40",
-                "sha256:f26648e1b3b03b6022b48a9b910d0ae209e2d51f50441db5dce5b530fad6d9b1",
-                "sha256:f67472c09a0c7486e27f3275f617c964d25e35727af952869dd496b9b5b7f6a3"
+                "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d",
+                "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4",
+                "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e",
+                "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab",
+                "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90",
+                "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6",
+                "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731",
+                "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540",
+                "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2",
+                "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292",
+                "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5",
+                "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b",
+                "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2",
+                "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0",
+                "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57",
+                "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3",
+                "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140",
+                "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84",
+                "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988",
+                "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67",
+                "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d",
+                "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2",
+                "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5",
+                "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9",
+                "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8",
+                "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd",
+                "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6",
+                "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be",
+                "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88",
+                "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25",
+                "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137",
+                "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968",
+                "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9",
+                "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef",
+                "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54",
+                "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512",
+                "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005",
+                "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f",
+                "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149",
+                "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d",
+                "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8",
+                "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7",
+                "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5",
+                "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016",
+                "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69",
+                "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212",
+                "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc",
+                "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8",
+                "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d",
+                "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd",
+                "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.0.5"
+            "version": "==7.2.2"
         },
         "cryptography": {
             "hashes": [
-                "sha256:1a6915075c6d3a5e1215eab5d99bcec0da26036ff2102a1038401d6ef5bef25b",
-                "sha256:1ee1fd0de9851ff32dbbb9362a4d833b579b4a6cc96883e8e6d2ff2a6bc7104f",
-                "sha256:407cec680e811b4fc829de966f88a7c62a596faa250fc1a4b520a0355b9bc190",
-                "sha256:50386acb40fbabbceeb2986332f0287f50f29ccf1497bae31cf5c3e7b4f4b34f",
-                "sha256:6f97109336df5c178ee7c9c711b264c502b905c2d2a29ace99ed761533a3460f",
-                "sha256:754978da4d0457e7ca176f58c57b1f9de6556591c19b25b8bcce3c77d314f5eb",
-                "sha256:76c24dd4fd196a80f9f2f5405a778a8ca132f16b10af113474005635fe7e066c",
-                "sha256:7dacfdeee048814563eaaec7c4743c8aea529fe3dd53127313a792f0dadc1773",
-                "sha256:80ee674c08aaef194bc4627b7f2956e5ba7ef29c3cc3ca488cf15854838a8f72",
-                "sha256:844ad4d7c3850081dffba91cdd91950038ee4ac525c575509a42d3fc806b83c8",
-                "sha256:875aea1039d78557c7c6b4db2fe0e9d2413439f4676310a5f269dd342ca7a717",
-                "sha256:887cbc1ea60786e534b00ba8b04d1095f4272d380ebd5f7a7eb4cc274710fad9",
-                "sha256:ad04f413436b0781f20c52a661660f1e23bcd89a0e9bb1d6d20822d048cf2856",
-                "sha256:bae6c7f4a36a25291b619ad064a30a07110a805d08dc89984f4f441f6c1f3f96",
-                "sha256:c52a1a6f81e738d07f43dab57831c29e57d21c81a942f4602fac7ee21b27f288",
-                "sha256:e0a05aee6a82d944f9b4edd6a001178787d1546ec7c6223ee9a848a7ade92e39",
-                "sha256:e324de6972b151f99dc078defe8fb1b0a82c6498e37bff335f5bc6b1e3ab5a1e",
-                "sha256:e5d71c5d5bd5b5c3eebcf7c5c2bb332d62ec68921a8c593bea8c394911a005ce",
-                "sha256:f3ed2d864a2fa1666e749fe52fb8e23d8e06b8012e8bd8147c73797c506e86f1",
-                "sha256:f671c1bb0d6088e94d61d80c606d65baacc0d374e67bf895148883461cd848de",
-                "sha256:f6c0db08d81ead9576c4d94bbb27aed8d7a430fa27890f39084c2d0e2ec6b0df",
-                "sha256:f964c7dcf7802d133e8dbd1565914fa0194f9d683d82411989889ecd701e8adf",
-                "sha256:fec8b932f51ae245121c4671b4bbc030880f363354b2f0e0bd1366017d891458"
+                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
+                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
+                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
+                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
+                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
+                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
+                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
+                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
+                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
+                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
+                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
+                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
+                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
+                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
+                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
+                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
+                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
+                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
+                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
             ],
             "index": "pypi",
-            "version": "==39.0.0"
+            "version": "==40.0.1"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
@@ -433,27 +417,27 @@
                 "sha256:cce6a7477ed816bd2542d03d53db9f0db935dd013b70f336a95c73979289f248"
             ],
             "index": "pypi",
             "version": "==1.1.10"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e",
-                "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"
+                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
+                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.0"
+            "version": "==1.1.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:892be14aa8efc01673b5ed6589dbccb95f9a8596f0507e232626155495c18105",
+                "sha256:bde48477b15fde2c7e5a0713cbe72721cb5a5ad32ee0b8f419907960b9d75536"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.0"
+            "version": "==3.10.7"
         },
         "flask": {
             "hashes": [
                 "sha256:15972e5017df0575c3d6c090ba168b6db90259e620ac8d7ea813a396bad5b6cb",
                 "sha256:9013281a7402ad527f8fd56375164f3aa021ecfaff89bfe3825346c24f87e04c"
             ],
             "index": "pypi",
@@ -508,19 +492,19 @@
                 "sha256:ce222e27b0de0d7bc63eb043b956996d6dccab14cc3b690aaea91c9cc99dc16e"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.11.0"
         },
         "google-auth": {
             "hashes": [
-                "sha256:5045648c821fb72384cdc0e82cc326df195f113a33049d9b62b74589243d2acc",
-                "sha256:ed7057a101af1146f0554a769930ac9de506aeca4fd5af6543ebe791851a9fbd"
+                "sha256:357ff22a75b4c0f6093470f21816a825d2adee398177569824e37b6c10069e19",
+                "sha256:8f379b46bad381ad2a0b989dfb0c13ad28d3c2a79f27348213f8946a1d15d55a"
             ],
             "index": "pypi",
-            "version": "==2.16.0"
+            "version": "==2.17.1"
         },
         "google-cloud-compute": {
             "hashes": [
                 "sha256:1ddd1be44d278754fc2643be7aa8d66838235ce44cfbacbeeadf3952ec020e95",
                 "sha256:21bd66251356d70bfd5f40211b42b936335490f7433b3b6fae7c498077e2c3fa"
             ],
             "index": "pypi",
@@ -540,19 +524,19 @@
                 "sha256:bd75d6e9fd456ce643ee936a113a1ead5405704515caa679db30d7f036e447f3"
             ],
             "index": "pypi",
             "version": "==0.34.0"
         },
         "googleapis-common-protos": {
             "hashes": [
-                "sha256:c727251ec025947d545184ba17e3578840fc3a24a0516a020479edab660457df",
-                "sha256:ca3befcd4580dab6ad49356b46bf165bb68ff4b32389f028f1abd7c10ab9519a"
+                "sha256:4168fcb568a826a52f23510412da405abd93f4d23ba544bb68d943b14ba3cb44",
+                "sha256:b287dc48449d1d41af0c69f4ea26242b5ae4c3d7249a38b0984c86a4caffff1f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.58.0"
+            "version": "==1.59.0"
         },
         "grpcio": {
             "hashes": [
                 "sha256:05f7c248e440f538aaad13eee78ef35f0541e73498dd6f832fe284542ac4b298",
                 "sha256:080b66253f29e1646ac53ef288c12944b131a2829488ac3bac8f52abb4413c0d",
                 "sha256:12b479839a5e753580b5e6053571de14006157f2ef9b71f38c56dc9b23b95ad6",
                 "sha256:156f8009e36780fab48c979c5605eda646065d4695deea4cfcbcfdd06627ddb6",
@@ -739,28 +723,21 @@
                 "sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933",
                 "sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a",
                 "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
             ],
             "index": "pypi",
             "version": "==2.1.1"
         },
-        "mitogen": {
-            "hashes": [
-                "sha256:c2dd28d6b964699822455f6c91acedc16324913586837f046a76e2e4ac1d716c"
-            ],
-            "index": "pypi",
-            "version": "==0.2.7"
-        },
         "natsort": {
             "hashes": [
-                "sha256:04fe18fdd2b9e5957f19f687eb117f102ef8dde6b574764e536e91194bed4f5f",
-                "sha256:57f85b72c688b09e053cdac302dd5b5b53df5f73ae20b4874fcbffd8bf783d11"
+                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
+                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==8.2.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==8.3.1"
         },
         "oauthlib": {
             "hashes": [
                 "sha256:8139f29aac13e25d502680e9e19963e83f16838d48a0d71c287fe40e7067fbca",
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
@@ -795,35 +772,35 @@
                 "sha256:e8dca2f4b43560edef58813969f52a56cef023146cbb8931626db80e6c1c4308"
             ],
             "index": "pypi",
             "version": "==5.9.0"
         },
         "pip": {
             "hashes": [
-                "sha256:65fd48317359f3af8e593943e6ae1506b66325085ea64b706a998c6e83eeaf38",
-                "sha256:908c78e6bc29b676ede1c4d57981d490cb892eb45cd8c214ab6298125119e077"
+                "sha256:236bcb61156d76c4b8a05821b988c7b8c35bf0da28a4b614e8d6ab5212c25c6f",
+                "sha256:cd015ea1bfb0fcef59d8a286c1f8bebcb983f6317719d415dc5351efb7cd7024"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==22.3.1"
+            "version": "==23.0.1"
         },
         "pipenv": {
             "hashes": [
                 "sha256:3b80b4512934b9d8e8ce12c988394642ff96bb697680e5b092e59af503178327",
                 "sha256:f84d7119239b22ab2ac2b8fbc7d619d83cf41135206d72a17c4f151cda529fd0"
             ],
             "index": "pypi",
             "version": "==2022.1.8"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490",
-                "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"
+                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
+                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.6.2"
+            "version": "==3.2.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -964,19 +941,19 @@
                 "sha256:cdc7b5e3ed77bed61270a47d35434a30617b9becdf2478af76ad2c6ade307280"
             ],
             "index": "pypi",
             "version": "==0.15.7"
         },
         "pytest": {
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
+                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.2.1"
+            "version": "==7.2.2"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b",
                 "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
             ],
             "markers": "python_version >= '3.6'",
@@ -996,35 +973,28 @@
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "index": "pypi",
             "version": "==2.8.2"
         },
         "python-gitlab": {
             "hashes": [
-                "sha256:251b63f0589d51f854516948c84e9eb8df26e1e9dea595cf86b43f17c43007dd",
-                "sha256:6180b81ee2f265ad8d8412956a1740b4d3ceca7b28ae2f707dfe62375fed0082"
+                "sha256:85ae778d8953aba87ad4b78aef7fbb5dae053980d2c20ff200bea29799685743",
+                "sha256:ad502b72b5d1137f4af37d4a68ae20fe7d6c9778f67cbe2aec566f7995053c7d"
             ],
             "index": "pypi",
-            "version": "==3.4.0"
+            "version": "==3.13.0"
         },
         "python-string-utils": {
             "hashes": [
                 "sha256:dcf9060b03f07647c0a603408dc8b03f807f3b54a05c6e19eb14460256fac0cb",
                 "sha256:f1a88700baf99db1a9b6953f44181ad9ca56623c81e257e6009707e2e7851fa4"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
-        "pytz": {
-            "hashes": [
-                "sha256:01a0681c4b9684a28304615eba55d1ab31ae00bf68ec157ec3708a8182dbbcd0",
-                "sha256:78f4f37d8198e0627c5f1143240bb0206b8691d8d7ac6d78fee88b78733f8c4a"
-            ],
-            "version": "==2022.7.1"
-        },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
                 "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
@@ -1065,19 +1035,19 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "index": "pypi",
             "version": "==6.0"
         },
         "redis": {
             "hashes": [
-                "sha256:30c07511627a4c5c4d970e060000772f323174f75e745a26938319817ead7a12",
-                "sha256:46652271dc7525cd5a9667e5b0ca983c848c75b2b8f7425403395bb8379dcf25"
+                "sha256:68226f7ede928db8302f29ab088a157f41061fa946b7ae865452b6d7838bbffb",
+                "sha256:da92a39fec86438d3f1e2a1db33c312985806954fe860120b582a8430e231d8f"
             ],
             "index": "pypi",
-            "version": "==4.3.5"
+            "version": "==4.4.4"
         },
         "repoze.lru": {
             "hashes": [
                 "sha256:0429a75e19380e4ed50c0694e26ac8819b4ea7851ee1fc7583c8572db80aff77",
                 "sha256:f77bf0e1096ea445beadd35f3479c5cff2aa1efe604a133e67150bc8630a62ea"
             ],
             "version": "==0.7"
@@ -1177,39 +1147,41 @@
                 "sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b",
                 "sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b",
                 "sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640",
                 "sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7",
                 "sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a",
                 "sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71",
                 "sha256:d5e51e2901ec2366b79f16c2299a03e74ba4531ddcfacc1416639c557aef0ad8",
+                "sha256:da538167284de58a52109a9b89b8f6a53ff8437dd6dc26d33b57bf6699153122",
                 "sha256:debc87a9516b237d0466a711b18b6ebeb17ba9f391eb7f91c649c5c4ec5006c7",
                 "sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80",
                 "sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e",
                 "sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab",
                 "sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0",
-                "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646"
+                "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646",
+                "sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38"
             ],
             "markers": "platform_python_implementation == 'CPython' and python_version < '3.11'",
             "version": "==0.2.7"
         },
         "s3transfer": {
             "hashes": [
                 "sha256:06176b74f3a15f61f1b4f25a1fc29a4429040b7647133a463da8fa5bd28d5ecd",
                 "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:a78d01d1e2c175c474884671dde039962c9d74c7223db7369771fcf6e29ceeab",
-                "sha256:bd6eb2d6722568de6d14b87c44a96fac54b2a45ff5e940e639979a3d1792adb6"
+                "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a",
+                "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==66.0.0"
+            "version": "==67.6.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "index": "pypi",
@@ -1262,35 +1234,35 @@
                 "sha256:21c85e0fe4b9a155d0799430b0ad741cdce7e359660ccbd8b530613e8df88ce2"
             ],
             "index": "pypi",
             "version": "==4.1.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         },
         "uvicorn": {
             "hashes": [
                 "sha256:c19a057deb1c5bb060946e2e5c262fc01590c6529c0af2c3d9ce941e89bc30e0",
                 "sha256:cade07c403c397f9fe275492a48c1b869efd175d5d8a692df649e6e7e2ed8f4e"
             ],
             "index": "pypi",
             "version": "==0.18.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:ce3b1684d6e1a20a3e5ed36795a97dfc6af29bc3970ca8dab93e11ac6094b3c4",
-                "sha256:f8b927684efc6f1cc206c9db297a570ab9ad0e51c16fa9e45487d36d1905c058"
+                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
+                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==20.17.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.21.0"
         },
         "virtualenv-clone": {
             "hashes": [
                 "sha256:418ee935c36152f8f153c79824bb93eaf6f0f7984bae31d3f48f350b9183501a",
                 "sha256:44d5263bceed0bac3e1424d64f798095233b64def1c5689afa43dc3223caf5b0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1301,47 +1273,47 @@
                 "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e",
                 "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"
             ],
             "version": "==0.2.6"
         },
         "webcolors": {
             "hashes": [
-                "sha256:16d043d3a08fd6a1b1b7e3e9e62640d09790dce80d2bdd4792a175b35fe794a9",
-                "sha256:d98743d81d498a2d3eaf165196e65481f0d2ea85281463d856b1e51b09f62dce"
+                "sha256:29bc7e8752c0a1bd4a1f03c14d6e6a72e93d82193738fa860cbff59d0fcc11bf",
+                "sha256:c225b674c83fa923be93d235330ce0300373d02885cef23238813b0d5668304a"
             ],
-            "version": "==1.12"
+            "version": "==1.13"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:d6b06432f184438d99ac1f456eaf22fe1ade524c3dd16e661142dc54e9cba574",
-                "sha256:d6e8f90ca8e2dd4e8027c4561adeb9456b54044312dba655e7cae652ceb9ae59"
+                "sha256:3f09e6d8230892547132177f575a4e3e73cfdf06526e20cc02aa1c3b47184d40",
+                "sha256:cdf5877568b7e83aa7cf2244ab56a3213de587bbe0ce9d8b9600fc77b455d89e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.4.2"
+            "version": "==1.5.1"
         },
         "werkzeug": {
             "hashes": [
-                "sha256:7ea2d48322cc7c0f8b3a215ed73eabd7b5d75d0b50e31ab006286ccff9e00b8f",
-                "sha256:f979ab81f58d7318e064e99c4506445d60135ac5cd2e177a2de0089bfd4c9bd5"
+                "sha256:2e1ccc9417d4da358b9de6f174e3ac094391ea1d4fbef2d667865d819dfd0afe",
+                "sha256:56433961bc1f12533306c624f3be5e744389ac61d722175d543e1751285da612"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.2.2"
+            "version": "==2.2.3"
         },
         "wheel": {
             "hashes": [
-                "sha256:965f5259b566725405b05e7cf774052044b1ed30119b5d586b2703aafe8719ac",
-                "sha256:b60533f3f5d530e971d6737ca6d58681ee434818fab630c83a734bb10c083ce8"
+                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
+                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.38.4"
+            "version": "==0.40.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa",
-                "sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.11.0"
+            "version": "==3.15.0"
         }
     },
     "develop": {}
 }
```

### Comparing `unfurl-0.6.1/unfurl/templates/python3.9/Pipfile` & `unfurl-0.6.2/unfurl/templates/python3.9/Pipfile`

 * *Files 11% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 rich = "==12.4.4"  # MIT
 flask = "<=2.1.3"
 flask-caching = "<=2.0.1"
 uvicorn = "<=0.18.2"
 google-cloud-compute = "==1.3.2"
 google-cloud-dns = "==0.34.0"
 grpcio = "==1.50.0"
-python-gitlab = "<=3.4.0"
+python-gitlab = "==3.13.0"
 certifi = "*"
 kubernetes = "==24.2.0"
 gunicorn = "==20.1.0"
-redis = "==4.3.5"
+redis = "==4.4.4"
 flask-cors = "==3.0.10"
 
 [dev-packages]
 
 [requires]
 python_version = "3.9"
```

### Comparing `unfurl-0.6.1/unfurl/templates/python3.9/Pipfile.lock` & `unfurl-0.6.2/unfurl/templates/python3.8/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702399957428692%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'47f7a05c79d365f4aef9ce334494ee41fb7acf4699e68e4f9b3bac8971818025'}, 'requires': "*

 * *            "{'python_version': '3.8'}}",*

 * * "'default'": "{'babel': {'hashes': "*

 * *              "['sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610', "*

 * *              "'sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455'], "*

 * *              "'version': '==2.12.1'}, 'boto3': {'hashes': "*

 * *              "['sha256:308c5a8293d9b76e74921f4d945be1 […]*

```diff
@@ -1,15 +1,15 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "12a09d8b57ef311b09acb9238aec5c53755f93f02df51fbbbc9dfaf431367627"
+            "sha256": "47f7a05c79d365f4aef9ce334494ee41fb7acf4699e68e4f9b3bac8971818025"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.9"
+            "python_version": "3.8"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
@@ -52,59 +52,59 @@
                 "sha256:0fbf5efbe78d466a26753e1dee3272423a3adc989d6a778c700e89a3f8ff0d88"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.5.1"
         },
         "babel": {
             "hashes": [
-                "sha256:1ad3eca1c885218f6dce2ab67291178944f810a10a9b5f3cb8382a5a232b64fe",
-                "sha256:5ef4b3226b0180dedded4229651c8b0e1a3a6a2837d45a073272f313e4cf97f6"
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "index": "pypi",
-            "version": "==2.11.0"
+            "version": "==2.12.1"
         },
         "boto": {
             "hashes": [
                 "sha256:147758d41ae7240dc989f0039f27da8ca0d53734be0eb869ef16e3adcfa462e8",
                 "sha256:ea0d3b40a2d852767be77ca343b58a9e3a4b00d9db440efb8da74b4e58025e5a"
             ],
             "index": "pypi",
             "version": "==2.49.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:0b1f82d4565ed875c7975ac0be5665e8d948613c01bcb0e49df6d4f5af670cc8",
-                "sha256:319ddb274f8f83b035b88a3b127c465bf6fe3e3fc2d668869b489e992c47ca77"
+                "sha256:308c5a8293d9b76e74921f4d945be19cc467b92e5f128df1db76e31c71345bb3",
+                "sha256:bcd09f16bdf3d71ab7d0fab20e97242f09c63f4cea0943329521ab35a950f900"
             ],
             "index": "pypi",
-            "version": "==1.26.52"
+            "version": "==1.26.104"
         },
         "botocore": {
             "hashes": [
-                "sha256:a0b89a33305cfa6251c6e1142deb7567e216e37e25363159f45fb81dc5b474e5",
-                "sha256:de55b6333fb13c66da9055972d7e4efff5dcc5a087478a2b70e99d888b29a24c"
+                "sha256:7e7a01cef10b1daa9cb01ec25a15e831e7359fc43d1b591359710f203c3620a8",
+                "sha256:932bfbf580a2ae53f471df4bfbebce531985ee27468cf7c37d7ccfb3cf8bc9e4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.52"
+            "version": "==1.29.104"
         },
         "cachelib": {
             "hashes": [
-                "sha256:292e89d5f9201fb9570e9f222c202f59085c66f9cb8bdfeefcfffff2b442fb2a",
-                "sha256:6fbbae4637491cc78a5e82f7cf623eb6778ea21ad8aa92197f45a1add51dab02"
+                "sha256:42d49f2fad9310dd946d7be73d46776bcd4d5fde4f49ad210cfdd447fbdfc346",
+                "sha256:593faeee62a7c037d50fc835617a01b887503f972fb52b188ae7e50e9cb69740"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.10.0"
+            "version": "==0.10.2"
         },
         "cachetools": {
             "hashes": [
-                "sha256:5991bc0e08a1319bb618d3195ca5b6bc76646a49c21d55962977197b301cc1fe",
-                "sha256:8462eebf3a6c15d25430a8c27c56ac61340b2ecf60c9ce57afc2b97e450e47da"
+                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
+                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
-            "version": "==5.2.1"
+            "version": "==5.3.0"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "index": "pypi",
@@ -177,104 +177,92 @@
                 "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
                 "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
             "version": "==1.15.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "version": "==3.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
@@ -294,115 +282,111 @@
                 "sha256:a21da482714b9f0b0e9bafaaf2f6a8b3b14161bb47f62e10e28d2fe4ff4b1626"
             ],
             "index": "pypi",
             "version": "==3.10.1"
         },
         "cmd2": {
             "hashes": [
-                "sha256:073e555c05853b0f6965f3d03329babdf9e38a5f2cea028e61a64cd7eeb74ad5",
-                "sha256:a77e3056751393270b4125c990cf527db132f15951a20a3a5dd2df4290aadf20"
+                "sha256:71873c11f72bd19e2b1db578214716f0d4f7c8fa250093c601265a9a717dee52",
+                "sha256:f1988ff2fff0ed812a2d25218a081b0fa0108d45b48ba2a9272bb98091b654e6"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.4.2"
+            "version": "==2.4.3"
         },
         "commonmark": {
             "hashes": [
                 "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60",
                 "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"
             ],
             "version": "==0.9.1"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:051afcbd6d2ac39298d62d340f94dbb6a1f31de06dfaf6fcef7b759dd3860c45",
-                "sha256:0a1890fca2962c4f1ad16551d660b46ea77291fba2cc21c024cd527b9d9c8809",
-                "sha256:0ee30375b409d9a7ea0f30c50645d436b6f5dfee254edffd27e45a980ad2c7f4",
-                "sha256:13250b1f0bd023e0c9f11838bdeb60214dd5b6aaf8e8d2f110c7e232a1bff83b",
-                "sha256:17e01dd8666c445025c29684d4aabf5a90dc6ef1ab25328aa52bedaa95b65ad7",
-                "sha256:19245c249aa711d954623d94f23cc94c0fd65865661f20b7781210cb97c471c0",
-                "sha256:1caed2367b32cc80a2b7f58a9f46658218a19c6cfe5bc234021966dc3daa01f0",
-                "sha256:1f66862d3a41674ebd8d1a7b6f5387fe5ce353f8719040a986551a545d7d83ea",
-                "sha256:220e3fa77d14c8a507b2d951e463b57a1f7810a6443a26f9b7591ef39047b1b2",
-                "sha256:276f4cd0001cd83b00817c8db76730938b1ee40f4993b6a905f40a7278103b3a",
-                "sha256:29de916ba1099ba2aab76aca101580006adfac5646de9b7c010a0f13867cba45",
-                "sha256:2a7f23bbaeb2a87f90f607730b45564076d870f1fb07b9318d0c21f36871932b",
-                "sha256:2c407b1950b2d2ffa091f4e225ca19a66a9bd81222f27c56bd12658fc5ca1209",
-                "sha256:30b5fec1d34cc932c1bc04017b538ce16bf84e239378b8f75220478645d11fca",
-                "sha256:3c2155943896ac78b9b0fd910fb381186d0c345911f5333ee46ac44c8f0e43ab",
-                "sha256:411d4ff9d041be08fdfc02adf62e89c735b9468f6d8f6427f8a14b6bb0a85095",
-                "sha256:436e103950d05b7d7f55e39beeb4d5be298ca3e119e0589c0227e6d0b01ee8c7",
-                "sha256:49640bda9bda35b057b0e65b7c43ba706fa2335c9a9896652aebe0fa399e80e6",
-                "sha256:4a950f83fd3f9bca23b77442f3a2b2ea4ac900944d8af9993743774c4fdc57af",
-                "sha256:50a6adc2be8edd7ee67d1abc3cd20678987c7b9d79cd265de55941e3d0d56499",
-                "sha256:52ab14b9e09ce052237dfe12d6892dd39b0401690856bcfe75d5baba4bfe2831",
-                "sha256:54f7e9705e14b2c9f6abdeb127c390f679f6dbe64ba732788d3015f7f76ef637",
-                "sha256:66e50680e888840c0995f2ad766e726ce71ca682e3c5f4eee82272c7671d38a2",
-                "sha256:790e4433962c9f454e213b21b0fd4b42310ade9c077e8edcb5113db0818450cb",
-                "sha256:7a38362528a9115a4e276e65eeabf67dcfaf57698e17ae388599568a78dcb029",
-                "sha256:7b05ed4b35bf6ee790832f68932baf1f00caa32283d66cc4d455c9e9d115aafc",
-                "sha256:7e109f1c9a3ece676597831874126555997c48f62bddbcace6ed17be3e372de8",
-                "sha256:949844af60ee96a376aac1ded2a27e134b8c8d35cc006a52903fc06c24a3296f",
-                "sha256:95304068686545aa368b35dfda1cdfbbdbe2f6fe43de4a2e9baa8ebd71be46e2",
-                "sha256:9e662e6fc4f513b79da5d10a23edd2b87685815b337b1a30cd11307a6679148d",
-                "sha256:a9fed35ca8c6e946e877893bbac022e8563b94404a605af1d1e6accc7eb73289",
-                "sha256:b69522b168a6b64edf0c33ba53eac491c0a8f5cc94fa4337f9c6f4c8f2f5296c",
-                "sha256:b78729038abea6a5df0d2708dce21e82073463b2d79d10884d7d591e0f385ded",
-                "sha256:b8c56bec53d6e3154eaff6ea941226e7bd7cc0d99f9b3756c2520fc7a94e6d96",
-                "sha256:b9727ac4f5cf2cbf87880a63870b5b9730a8ae3a4a360241a0fdaa2f71240ff0",
-                "sha256:ba3027deb7abf02859aca49c865ece538aee56dcb4871b4cced23ba4d5088904",
-                "sha256:be9fcf32c010da0ba40bf4ee01889d6c737658f4ddff160bd7eb9cac8f094b21",
-                "sha256:c18d47f314b950dbf24a41787ced1474e01ca816011925976d90a88b27c22b89",
-                "sha256:c76a3075e96b9c9ff00df8b5f7f560f5634dffd1658bafb79eb2682867e94f78",
-                "sha256:cbfcba14a3225b055a28b3199c3d81cd0ab37d2353ffd7f6fd64844cebab31ad",
-                "sha256:d254666d29540a72d17cc0175746cfb03d5123db33e67d1020e42dae611dc196",
-                "sha256:d66187792bfe56f8c18ba986a0e4ae44856b1c645336bd2c776e3386da91e1dd",
-                "sha256:d8d04e755934195bdc1db45ba9e040b8d20d046d04d6d77e71b3b34a8cc002d0",
-                "sha256:d8f3e2e0a1d6777e58e834fd5a04657f66affa615dae61dd67c35d1568c38882",
-                "sha256:e057e74e53db78122a3979f908973e171909a58ac20df05c33998d52e6d35757",
-                "sha256:e4ce984133b888cc3a46867c8b4372c7dee9cee300335e2925e197bcd45b9e16",
-                "sha256:ea76dbcad0b7b0deb265d8c36e0801abcddf6cc1395940a24e3595288b405ca0",
-                "sha256:ecb0f73954892f98611e183f50acdc9e21a4653f294dfbe079da73c6378a6f47",
-                "sha256:ef14d75d86f104f03dea66c13188487151760ef25dd6b2dbd541885185f05f40",
-                "sha256:f26648e1b3b03b6022b48a9b910d0ae209e2d51f50441db5dce5b530fad6d9b1",
-                "sha256:f67472c09a0c7486e27f3275f617c964d25e35727af952869dd496b9b5b7f6a3"
+                "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d",
+                "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4",
+                "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e",
+                "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab",
+                "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90",
+                "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6",
+                "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731",
+                "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540",
+                "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2",
+                "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292",
+                "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5",
+                "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b",
+                "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2",
+                "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0",
+                "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57",
+                "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3",
+                "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140",
+                "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84",
+                "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988",
+                "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67",
+                "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d",
+                "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2",
+                "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5",
+                "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9",
+                "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8",
+                "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd",
+                "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6",
+                "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be",
+                "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88",
+                "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25",
+                "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137",
+                "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968",
+                "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9",
+                "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef",
+                "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54",
+                "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512",
+                "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005",
+                "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f",
+                "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149",
+                "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d",
+                "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8",
+                "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7",
+                "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5",
+                "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016",
+                "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69",
+                "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212",
+                "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc",
+                "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8",
+                "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d",
+                "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd",
+                "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.0.5"
+            "version": "==7.2.2"
         },
         "cryptography": {
             "hashes": [
-                "sha256:1a6915075c6d3a5e1215eab5d99bcec0da26036ff2102a1038401d6ef5bef25b",
-                "sha256:1ee1fd0de9851ff32dbbb9362a4d833b579b4a6cc96883e8e6d2ff2a6bc7104f",
-                "sha256:407cec680e811b4fc829de966f88a7c62a596faa250fc1a4b520a0355b9bc190",
-                "sha256:50386acb40fbabbceeb2986332f0287f50f29ccf1497bae31cf5c3e7b4f4b34f",
-                "sha256:6f97109336df5c178ee7c9c711b264c502b905c2d2a29ace99ed761533a3460f",
-                "sha256:754978da4d0457e7ca176f58c57b1f9de6556591c19b25b8bcce3c77d314f5eb",
-                "sha256:76c24dd4fd196a80f9f2f5405a778a8ca132f16b10af113474005635fe7e066c",
-                "sha256:7dacfdeee048814563eaaec7c4743c8aea529fe3dd53127313a792f0dadc1773",
-                "sha256:80ee674c08aaef194bc4627b7f2956e5ba7ef29c3cc3ca488cf15854838a8f72",
-                "sha256:844ad4d7c3850081dffba91cdd91950038ee4ac525c575509a42d3fc806b83c8",
-                "sha256:875aea1039d78557c7c6b4db2fe0e9d2413439f4676310a5f269dd342ca7a717",
-                "sha256:887cbc1ea60786e534b00ba8b04d1095f4272d380ebd5f7a7eb4cc274710fad9",
-                "sha256:ad04f413436b0781f20c52a661660f1e23bcd89a0e9bb1d6d20822d048cf2856",
-                "sha256:bae6c7f4a36a25291b619ad064a30a07110a805d08dc89984f4f441f6c1f3f96",
-                "sha256:c52a1a6f81e738d07f43dab57831c29e57d21c81a942f4602fac7ee21b27f288",
-                "sha256:e0a05aee6a82d944f9b4edd6a001178787d1546ec7c6223ee9a848a7ade92e39",
-                "sha256:e324de6972b151f99dc078defe8fb1b0a82c6498e37bff335f5bc6b1e3ab5a1e",
-                "sha256:e5d71c5d5bd5b5c3eebcf7c5c2bb332d62ec68921a8c593bea8c394911a005ce",
-                "sha256:f3ed2d864a2fa1666e749fe52fb8e23d8e06b8012e8bd8147c73797c506e86f1",
-                "sha256:f671c1bb0d6088e94d61d80c606d65baacc0d374e67bf895148883461cd848de",
-                "sha256:f6c0db08d81ead9576c4d94bbb27aed8d7a430fa27890f39084c2d0e2ec6b0df",
-                "sha256:f964c7dcf7802d133e8dbd1565914fa0194f9d683d82411989889ecd701e8adf",
-                "sha256:fec8b932f51ae245121c4671b4bbc030880f363354b2f0e0bd1366017d891458"
+                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
+                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
+                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
+                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
+                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
+                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
+                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
+                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
+                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
+                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
+                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
+                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
+                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
+                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
+                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
+                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
+                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
+                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
+                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
             ],
             "index": "pypi",
-            "version": "==39.0.0"
+            "version": "==40.0.1"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
@@ -433,27 +417,27 @@
                 "sha256:cce6a7477ed816bd2542d03d53db9f0db935dd013b70f336a95c73979289f248"
             ],
             "index": "pypi",
             "version": "==1.1.10"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e",
-                "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"
+                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
+                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.0"
+            "version": "==1.1.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:892be14aa8efc01673b5ed6589dbccb95f9a8596f0507e232626155495c18105",
+                "sha256:bde48477b15fde2c7e5a0713cbe72721cb5a5ad32ee0b8f419907960b9d75536"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.0"
+            "version": "==3.10.7"
         },
         "flask": {
             "hashes": [
                 "sha256:15972e5017df0575c3d6c090ba168b6db90259e620ac8d7ea813a396bad5b6cb",
                 "sha256:9013281a7402ad527f8fd56375164f3aa021ecfaff89bfe3825346c24f87e04c"
             ],
             "index": "pypi",
@@ -508,19 +492,19 @@
                 "sha256:ce222e27b0de0d7bc63eb043b956996d6dccab14cc3b690aaea91c9cc99dc16e"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.11.0"
         },
         "google-auth": {
             "hashes": [
-                "sha256:5045648c821fb72384cdc0e82cc326df195f113a33049d9b62b74589243d2acc",
-                "sha256:ed7057a101af1146f0554a769930ac9de506aeca4fd5af6543ebe791851a9fbd"
+                "sha256:357ff22a75b4c0f6093470f21816a825d2adee398177569824e37b6c10069e19",
+                "sha256:8f379b46bad381ad2a0b989dfb0c13ad28d3c2a79f27348213f8946a1d15d55a"
             ],
             "index": "pypi",
-            "version": "==2.16.0"
+            "version": "==2.17.1"
         },
         "google-cloud-compute": {
             "hashes": [
                 "sha256:1ddd1be44d278754fc2643be7aa8d66838235ce44cfbacbeeadf3952ec020e95",
                 "sha256:21bd66251356d70bfd5f40211b42b936335490f7433b3b6fae7c498077e2c3fa"
             ],
             "index": "pypi",
@@ -540,19 +524,19 @@
                 "sha256:bd75d6e9fd456ce643ee936a113a1ead5405704515caa679db30d7f036e447f3"
             ],
             "index": "pypi",
             "version": "==0.34.0"
         },
         "googleapis-common-protos": {
             "hashes": [
-                "sha256:c727251ec025947d545184ba17e3578840fc3a24a0516a020479edab660457df",
-                "sha256:ca3befcd4580dab6ad49356b46bf165bb68ff4b32389f028f1abd7c10ab9519a"
+                "sha256:4168fcb568a826a52f23510412da405abd93f4d23ba544bb68d943b14ba3cb44",
+                "sha256:b287dc48449d1d41af0c69f4ea26242b5ae4c3d7249a38b0984c86a4caffff1f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.58.0"
+            "version": "==1.59.0"
         },
         "grpcio": {
             "hashes": [
                 "sha256:05f7c248e440f538aaad13eee78ef35f0541e73498dd6f832fe284542ac4b298",
                 "sha256:080b66253f29e1646ac53ef288c12944b131a2829488ac3bac8f52abb4413c0d",
                 "sha256:12b479839a5e753580b5e6053571de14006157f2ef9b71f38c56dc9b23b95ad6",
                 "sha256:156f8009e36780fab48c979c5605eda646065d4695deea4cfcbcfdd06627ddb6",
@@ -739,21 +723,28 @@
                 "sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933",
                 "sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a",
                 "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
             ],
             "index": "pypi",
             "version": "==2.1.1"
         },
+        "mitogen": {
+            "hashes": [
+                "sha256:c2dd28d6b964699822455f6c91acedc16324913586837f046a76e2e4ac1d716c"
+            ],
+            "index": "pypi",
+            "version": "==0.2.7"
+        },
         "natsort": {
             "hashes": [
-                "sha256:04fe18fdd2b9e5957f19f687eb117f102ef8dde6b574764e536e91194bed4f5f",
-                "sha256:57f85b72c688b09e053cdac302dd5b5b53df5f73ae20b4874fcbffd8bf783d11"
+                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
+                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==8.2.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==8.3.1"
         },
         "oauthlib": {
             "hashes": [
                 "sha256:8139f29aac13e25d502680e9e19963e83f16838d48a0d71c287fe40e7067fbca",
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
@@ -788,35 +779,35 @@
                 "sha256:e8dca2f4b43560edef58813969f52a56cef023146cbb8931626db80e6c1c4308"
             ],
             "index": "pypi",
             "version": "==5.9.0"
         },
         "pip": {
             "hashes": [
-                "sha256:65fd48317359f3af8e593943e6ae1506b66325085ea64b706a998c6e83eeaf38",
-                "sha256:908c78e6bc29b676ede1c4d57981d490cb892eb45cd8c214ab6298125119e077"
+                "sha256:236bcb61156d76c4b8a05821b988c7b8c35bf0da28a4b614e8d6ab5212c25c6f",
+                "sha256:cd015ea1bfb0fcef59d8a286c1f8bebcb983f6317719d415dc5351efb7cd7024"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==22.3.1"
+            "version": "==23.0.1"
         },
         "pipenv": {
             "hashes": [
                 "sha256:3b80b4512934b9d8e8ce12c988394642ff96bb697680e5b092e59af503178327",
                 "sha256:f84d7119239b22ab2ac2b8fbc7d619d83cf41135206d72a17c4f151cda529fd0"
             ],
             "index": "pypi",
             "version": "==2022.1.8"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490",
-                "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"
+                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
+                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.6.2"
+            "version": "==3.2.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -957,19 +948,19 @@
                 "sha256:cdc7b5e3ed77bed61270a47d35434a30617b9becdf2478af76ad2c6ade307280"
             ],
             "index": "pypi",
             "version": "==0.15.7"
         },
         "pytest": {
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
+                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.2.1"
+            "version": "==7.2.2"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b",
                 "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
             ],
             "markers": "python_version >= '3.6'",
@@ -989,34 +980,35 @@
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "index": "pypi",
             "version": "==2.8.2"
         },
         "python-gitlab": {
             "hashes": [
-                "sha256:251b63f0589d51f854516948c84e9eb8df26e1e9dea595cf86b43f17c43007dd",
-                "sha256:6180b81ee2f265ad8d8412956a1740b4d3ceca7b28ae2f707dfe62375fed0082"
+                "sha256:85ae778d8953aba87ad4b78aef7fbb5dae053980d2c20ff200bea29799685743",
+                "sha256:ad502b72b5d1137f4af37d4a68ae20fe7d6c9778f67cbe2aec566f7995053c7d"
             ],
             "index": "pypi",
-            "version": "==3.4.0"
+            "version": "==3.13.0"
         },
         "python-string-utils": {
             "hashes": [
                 "sha256:dcf9060b03f07647c0a603408dc8b03f807f3b54a05c6e19eb14460256fac0cb",
                 "sha256:f1a88700baf99db1a9b6953f44181ad9ca56623c81e257e6009707e2e7851fa4"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
         "pytz": {
             "hashes": [
-                "sha256:01a0681c4b9684a28304615eba55d1ab31ae00bf68ec157ec3708a8182dbbcd0",
-                "sha256:78f4f37d8198e0627c5f1143240bb0206b8691d8d7ac6d78fee88b78733f8c4a"
+                "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
+                "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
             ],
-            "version": "==2022.7.1"
+            "markers": "python_version < '3.9'",
+            "version": "==2023.3"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
@@ -1058,19 +1050,19 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "index": "pypi",
             "version": "==6.0"
         },
         "redis": {
             "hashes": [
-                "sha256:30c07511627a4c5c4d970e060000772f323174f75e745a26938319817ead7a12",
-                "sha256:46652271dc7525cd5a9667e5b0ca983c848c75b2b8f7425403395bb8379dcf25"
+                "sha256:68226f7ede928db8302f29ab088a157f41061fa946b7ae865452b6d7838bbffb",
+                "sha256:da92a39fec86438d3f1e2a1db33c312985806954fe860120b582a8430e231d8f"
             ],
             "index": "pypi",
-            "version": "==4.3.5"
+            "version": "==4.4.4"
         },
         "repoze.lru": {
             "hashes": [
                 "sha256:0429a75e19380e4ed50c0694e26ac8819b4ea7851ee1fc7583c8572db80aff77",
                 "sha256:f77bf0e1096ea445beadd35f3479c5cff2aa1efe604a133e67150bc8630a62ea"
             ],
             "version": "==0.7"
@@ -1170,39 +1162,41 @@
                 "sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b",
                 "sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b",
                 "sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640",
                 "sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7",
                 "sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a",
                 "sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71",
                 "sha256:d5e51e2901ec2366b79f16c2299a03e74ba4531ddcfacc1416639c557aef0ad8",
+                "sha256:da538167284de58a52109a9b89b8f6a53ff8437dd6dc26d33b57bf6699153122",
                 "sha256:debc87a9516b237d0466a711b18b6ebeb17ba9f391eb7f91c649c5c4ec5006c7",
                 "sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80",
                 "sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e",
                 "sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab",
                 "sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0",
-                "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646"
+                "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646",
+                "sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38"
             ],
             "markers": "platform_python_implementation == 'CPython' and python_version < '3.11'",
             "version": "==0.2.7"
         },
         "s3transfer": {
             "hashes": [
                 "sha256:06176b74f3a15f61f1b4f25a1fc29a4429040b7647133a463da8fa5bd28d5ecd",
                 "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:a78d01d1e2c175c474884671dde039962c9d74c7223db7369771fcf6e29ceeab",
-                "sha256:bd6eb2d6722568de6d14b87c44a96fac54b2a45ff5e940e639979a3d1792adb6"
+                "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a",
+                "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==66.0.0"
+            "version": "==67.6.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "index": "pypi",
@@ -1255,35 +1249,35 @@
                 "sha256:21c85e0fe4b9a155d0799430b0ad741cdce7e359660ccbd8b530613e8df88ce2"
             ],
             "index": "pypi",
             "version": "==4.1.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         },
         "uvicorn": {
             "hashes": [
                 "sha256:c19a057deb1c5bb060946e2e5c262fc01590c6529c0af2c3d9ce941e89bc30e0",
                 "sha256:cade07c403c397f9fe275492a48c1b869efd175d5d8a692df649e6e7e2ed8f4e"
             ],
             "index": "pypi",
             "version": "==0.18.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:ce3b1684d6e1a20a3e5ed36795a97dfc6af29bc3970ca8dab93e11ac6094b3c4",
-                "sha256:f8b927684efc6f1cc206c9db297a570ab9ad0e51c16fa9e45487d36d1905c058"
+                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
+                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==20.17.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.21.0"
         },
         "virtualenv-clone": {
             "hashes": [
                 "sha256:418ee935c36152f8f153c79824bb93eaf6f0f7984bae31d3f48f350b9183501a",
                 "sha256:44d5263bceed0bac3e1424d64f798095233b64def1c5689afa43dc3223caf5b0"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1294,47 +1288,47 @@
                 "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e",
                 "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"
             ],
             "version": "==0.2.6"
         },
         "webcolors": {
             "hashes": [
-                "sha256:16d043d3a08fd6a1b1b7e3e9e62640d09790dce80d2bdd4792a175b35fe794a9",
-                "sha256:d98743d81d498a2d3eaf165196e65481f0d2ea85281463d856b1e51b09f62dce"
+                "sha256:29bc7e8752c0a1bd4a1f03c14d6e6a72e93d82193738fa860cbff59d0fcc11bf",
+                "sha256:c225b674c83fa923be93d235330ce0300373d02885cef23238813b0d5668304a"
             ],
-            "version": "==1.12"
+            "version": "==1.13"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:d6b06432f184438d99ac1f456eaf22fe1ade524c3dd16e661142dc54e9cba574",
-                "sha256:d6e8f90ca8e2dd4e8027c4561adeb9456b54044312dba655e7cae652ceb9ae59"
+                "sha256:3f09e6d8230892547132177f575a4e3e73cfdf06526e20cc02aa1c3b47184d40",
+                "sha256:cdf5877568b7e83aa7cf2244ab56a3213de587bbe0ce9d8b9600fc77b455d89e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.4.2"
+            "version": "==1.5.1"
         },
         "werkzeug": {
             "hashes": [
-                "sha256:7ea2d48322cc7c0f8b3a215ed73eabd7b5d75d0b50e31ab006286ccff9e00b8f",
-                "sha256:f979ab81f58d7318e064e99c4506445d60135ac5cd2e177a2de0089bfd4c9bd5"
+                "sha256:2e1ccc9417d4da358b9de6f174e3ac094391ea1d4fbef2d667865d819dfd0afe",
+                "sha256:56433961bc1f12533306c624f3be5e744389ac61d722175d543e1751285da612"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.2.2"
+            "version": "==2.2.3"
         },
         "wheel": {
             "hashes": [
-                "sha256:965f5259b566725405b05e7cf774052044b1ed30119b5d586b2703aafe8719ac",
-                "sha256:b60533f3f5d530e971d6737ca6d58681ee434818fab630c83a734bb10c083ce8"
+                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
+                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.38.4"
+            "version": "==0.40.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa",
-                "sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.11.0"
+            "version": "==3.15.0"
         }
     },
     "develop": {}
 }
```

### Comparing `unfurl-0.6.1/unfurl/templates/secrets.yaml.j2` & `unfurl-0.6.2/unfurl/templates/secrets.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/service-template.yaml.j2` & `unfurl-0.6.2/unfurl/templates/service-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/unfurl.local.yaml.j2` & `unfurl-0.6.2/unfurl/templates/unfurl.local.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/templates/unfurl.yaml.j2` & `unfurl-0.6.2/unfurl/templates/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/to_json.py` & `unfurl-0.6.2/unfurl/to_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1071,14 +1071,17 @@
         local_resource_templates = {}
         resource_templates = template.pop("resource_templates", None)
         if resource_templates:
             for node_name, node_tpl in resource_templates.items():
                 # nodes here overrides node_templates
                 node_spec = spec.add_node_template(node_name, node_tpl, False)
                 node_template = node_spec.toscaEntityTemplate
+            # convert to json in second-pass template requirements can reference each other
+            for node_name, node_tpl in resource_templates.items():
+                node_template = spec.nodeTemplates[node_name].toscaEntityTemplate
                 t = nodetemplate_to_json(node_template, spec, db["ResourceType"])
                 if t.get("visibility") == "omit":
                     continue
                 local_resource_templates[node_name] = t
 
         # XXX assert that db["ResourceTemplate"] has already has all the node_templates
         # names of ResourceTemplates:
@@ -1124,15 +1127,19 @@
     if deployment_blueprint_name and deployment_blueprint_name in templates:
         deployment_blueprint = templates[deployment_blueprint_name]
         template = deployment_blueprint.copy()
 
     # the deployment template created for this deployment will have a "source" key
     # so if it doesn't (or one wasn't set) create a new one and set the current one as its "source"
     if "source" not in template:
-        title = os.path.basename(os.path.dirname(manifest.path)) if manifest.path else 'untitled'
+        title = (
+            os.path.basename(os.path.dirname(manifest.path))
+            if manifest.path
+            else "untitled"
+        )
         slug = slugify(title)
         template.update(
             dict(
                 __typename="DeploymentTemplate",
                 title=title,
                 name=slug,
                 slug=slug,
@@ -1207,15 +1214,15 @@
         primary_provider=connections.get("primary_provider"),
         instances=environment_instances,
         repositories=manifest.context.get("repositories") or {},
     )
     return db, manifest, env, connection_types
 
 
-def add_graphql_deployment(manifest, db, dtemplate):
+def add_graphql_deployment(manifest: YamlManifest, db, dtemplate):
     """
     type Deployment {
       title: String!
       primary: Resource
       resources: [Resource!]
       deploymentTemplate: DeploymentTemplate!
       url: url
@@ -1231,17 +1238,18 @@
     templates = db["ResourceTemplate"]
     relationships: Dict[str, List[Dict]] = {}
     for t in templates.values():
         if "dependencies" in t:
             for c in t["dependencies"]:
                 if c.get("match"):
                     relationships.setdefault(c["match"], []).append(c)
+    assert manifest.rootResource
     resources = [
         to_graphql_resource(instance, manifest, db, relationships)
-        for instance in manifest.rootResource.get_self_and_descendents()
+        for instance in manifest.rootResource.get_self_and_descendants()
         if instance is not manifest.rootResource
     ]
     db["Resource"] = {r["name"]: r for r in resources if r}
     deployment["resources"] = list(db["Resource"])
     primary_name = deployment["primary"] = dtemplate["primary"]
     deployment["deploymentTemplate"] = dtemplate["name"]
     if manifest.lastJob:
@@ -1360,23 +1368,27 @@
     # {i["name"]: inputsSchemaProperties
     for name, value in get_nodefilters(filters, "properties"):
         if not isinstance(value, dict) or "eval" in value:
             # the filter declared an expression to set the property's value
             # mark the property to be deleted from the target inputschema so the user can't set it
             # (since they can't shouldn't set this property now)
             jsonprops[name] = None
+        elif "default" in value:
+            jsonprops.setdefault(name, {})["default"] = value["default"]
         elif name not in jsonprops and name in inputsSchemaProperties:
             # check name in jsonprops so we only do this once
             # use the inputs schema definition to determine the node filter's constraints
             schema = inputsSchemaProperties[name]
             tosca_datatype = schema.get("$toscatype") or ONE_TO_ONE_MAP.get(
                 schema["type"], schema["type"]
             )
             constraints = ConditionClause(name, value, tosca_datatype).conditions
-            jsonprops[name] = map_constraints(schema["type"], constraints, schema)
+            jsonprops.setdefault(name, {}).update(
+                map_constraints(schema["type"], constraints, schema)
+            )
     return jsonprops
 
 
 def _set_shared_instances(instances):
     env_instances = {}
     # imported (aka shared) resources are just a reference and won't be part of the manifest unless referenced
     # so just copy them over now
```

### Comparing `unfurl-0.6.1/unfurl/tosca.py` & `unfurl-0.6.2/unfurl/tosca.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import toscaparser.artifacts
 import toscaparser.repositories
 from toscaparser.common.exception import ExceptionCollector
 import os
 from .logs import getLogger
 import logging
 import re
-from typing import Dict, Optional, Sequence
+from typing import Dict, Optional, Sequence, cast
 
 from ruamel.yaml.comments import CommentedMap
 
 logger = getLogger("unfurl")
 
 from toscaparser import functions
 
@@ -170,14 +170,16 @@
                 for prop, value in req.get_nodefilter_properties():
                     # the target already has a node so treat the node filter
                     # as coersive by annotating the target's properties
                     target = req.relationship and req.relationship.target
                     if target:
                         if isinstance(value, dict):
                             if "eval" in value:
+                                if value["eval"] is None:
+                                    continue
                                 value.setdefault("vars", {})["SOURCE"] = dict(
                                     eval="::" + nodespec.name
                                 )
                             elif "q" in value:
                                 value = value["q"]
                             else:
                                 # we assume this is a constraint, so don't assign the value
@@ -390,34 +392,34 @@
                 self.discovered = CommentedMap()
             self.discovered[name] = tpl
         # add custom_types back for serialization later
         if custom_types:
             tpl["custom_types"] = custom_types
         return nodeSpec
 
-    def load_decorators(self):
+    def load_decorators(self) -> CommentedMap:
         decorators = CommentedMap()
         for path, import_tpl in self.template.nested_tosca_tpls.items():
             imported = import_tpl.get("decorators")
             if imported:
-                decorators = merge_dicts(decorators, imported)
-        decorators = merge_dicts(decorators, self.template.tpl.get("decorators") or {})
+                decorators = cast(CommentedMap, merge_dicts(decorators, imported))
+        decorators = cast(CommentedMap, merge_dicts(decorators, self.template.tpl.get("decorators") or {}))
         return decorators
 
-    def load_imported_default_templates(self):
+    def load_imported_default_templates(self) -> None:
         for name, topology in self.template.nested_topologies.items():
             for nodeTemplate in topology.nodetemplates:
                 if (
                     "default" in nodeTemplate.directives
                     and nodeTemplate.name not in self.nodeTemplates
                 ):
                     nodeSpec = NodeSpec(nodeTemplate, self)
                     self.nodeTemplates[nodeSpec.name] = nodeSpec
 
-    def load_workflows(self):
+    def load_workflows(self) -> None:
         # we want to let different types defining standard workflows like deploy
         # so we need to support importing workflows
         workflows = {
             name: [Workflow(w)]
             for name, w in self.template.topology_template.workflows.items()
         }
         for topology in self.template.nested_topologies.values():
@@ -586,25 +588,25 @@
     def get_repository(self, name: str):
         return self.template and self.template.repositories.get(name)
 
 
 def find_env_vars(props_iter):
     for propdef, value in props_iter:
         datatype = propdef.entity
-        if datatype.type == "unfurl.datatypes.EnvVar":
-            yield propdef.name, env_var_value(value)
-        elif (
+        if (
             datatype.type == "map"
             and propdef.entry_schema_entity
             and propdef.entry_schema_entity.type == "unfurl.datatypes.EnvVar"
         ):
             if value:
                 for key, item in value.items():
                     yield key, env_var_value(item)
         else:
+            if datatype.type == "unfurl.datatypes.EnvVar":
+                yield propdef.name, env_var_value(value)
             metadata = propdef.schema.get("metadata", {})
             if metadata.get("env_vars"):
                 for name in metadata["env_vars"]:
                     yield name, env_var_value(value)
 
 
 def find_props(attributes, propertyDefs, flatten=False):
```

### Comparing `unfurl-0.6.1/unfurl/tosca_plugins/artifacts.yaml` & `unfurl-0.6.2/unfurl/tosca_plugins/artifacts.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/tosca_plugins/googlecloud.yaml` & `unfurl-0.6.2/unfurl/tosca_plugins/googlecloud.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/tosca_plugins/k8s.yaml` & `unfurl-0.6.2/unfurl/tosca_plugins/k8s.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/tosca_plugins/localhost.yaml` & `unfurl-0.6.2/unfurl/tosca_plugins/localhost.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/tosca_plugins/tosca-ext.yaml` & `unfurl-0.6.2/unfurl/tosca_plugins/tosca-ext.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -412,30 +412,56 @@
         metadata:
           user_settable: true
 
   unfurl.relationships.ConnectsTo.Azure:
     derived_from: unfurl.relationships.ConnectsTo.CloudAccount
     properties:
       AZURE_CLIENT_ID:
-        type: unfurl.datatypes.EnvVar
-        default: { get_env: AZURE_CLIENT_ID }
+        description: >
+          Also known as an Application ID or `appId`.
+          Can be created via [CLI](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/guides/service_principal_client_certificate)
+          or through the [Azure portal](https://learn.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
+        type: string
+        metadata:
+          env_vars: [ARM_CLIENT_ID, AZURE_CLIENT_ID]
+          title: Client ID
+          user_settable: true
+        default: { get_env: [ARM_CLIENT_ID, {get_env: AZURE_CLIENT_ID}] }
+        required: false
       AZURE_TENANT:
-        type: unfurl.datatypes.EnvVar
-        default: { get_env: AZURE_TENANT }
+        description: >
+          [Find your Azure active directory tenant](https://learn.microsoft.com/en-us/azure/azure-portal/get-subscription-tenant-id#find-your-azure-ad-tenant)
+        type: string
+        metadata:
+          env_vars: [ARM_TENANT_ID, AZURE_TENANT]
+          title: Tenant
+          user_settable: true
+        default: { get_env: [ARM_TENANT_ID, {get_env: AZURE_TENANT}] }
         required: false
       AZURE_SUBSCRIPTION_ID:
-        description: for authentication with service principal
-        type: unfurl.datatypes.EnvVar
-        default: { get_env: AZURE_SUBSCRIPTION_ID }
+        description: >
+          [Find your Azure subscription](https://learn.microsoft.com/en-us/azure/azure-portal/get-subscription-tenant-id#find-your-azure-subscription)
+        type: string
+        required: false
+        metadata:
+          env_vars: [ARM_SUBSCRIPTION_ID, AZURE_SUBSCRIPTION_ID]
+          title: Azure Subscription
+          user_settable: true
+        default: { get_env: [ARM_SUBSCRIPTION_ID, {get_env: AZURE_SUBSCRIPTION_ID}] }
       AZURE_SECRET:
-        description: for authentication with service principal
-        type: unfurl.datatypes.EnvVar
-        default: { get_env: AZURE_SECRET }
+        description: >
+          For authentication with service principal. [(Portal link)](https://learn.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal#option-2-create-a-new-application-secret)
+        type: string
+        required: false
+        default: { get_env: [ARM_CLIENT_SECRET, {get_env: AZURE_SECRET}] }
         metadata:
+          env_vars: [ARM_CLIENT_SECRET, AZURE_SECRET]
           sensitive: true
+          title: Client Secret
+          user_settable: true
       AZURE_AD_USER:
         description: for authentication with Active Directory
         type: unfurl.datatypes.EnvVar
         default: { get_env: AZURE_AD_USER }
         required: false
       AZURE_PASSWORD:
         description: for authentication with Active Directory
```

### Comparing `unfurl-0.6.1/unfurl/unfurl-schema.json` & `unfurl-0.6.2/unfurl/unfurl-schema.json`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/util.py` & `unfurl-0.6.2/unfurl/util.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/sphinx-jsonschema/__init__.py` & `unfurl-0.6.2/unfurl/vendor/sphinx-jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/sphinx-jsonschema/wide_format.py` & `unfurl-0.6.2/unfurl/vendor/sphinx-jsonschema/wide_format.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/__init__.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/__init__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/activities.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/activities.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/artifacts.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/artifacts.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/capabilities.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/capabilities.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/common/exception.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/common/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -145,14 +145,18 @@
                 'of output "%(output_name)s".')
 
 
 class InvalidPropertyValueError(TOSCAException):
     msg_fmt = _('Value of property "%(what)s" is invalid.')
 
 
+class InvalidOccurrences(TOSCAException):
+    msg_fmt = _('Value "%(what)s" of "occurrences" is invalid: %(why)s.')
+
+
 class InvalidTemplateVersion(TOSCAException):
     msg_fmt = _('The template version "%(what)s" is invalid. '
                 'Valid versions are "%(valid_versions)s".')
 
 
 class InvalidTOSCAVersionPropertyException(TOSCAException):
     msg_fmt = _('Value of TOSCA version property "%(what)s" is invalid.')
```

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/dataentity.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/dataentity.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/artifacttype.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/artifacttype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/attribute_definition.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/attribute_definition.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/capabilitytype.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/capabilitytype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/constraints.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/constraints.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/datatype.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/datatype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/entity_type.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/entity_type.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/grouptype.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/grouptype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/interfaces.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/interfaces.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/nodetype.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/nodetype.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,32 @@
 from toscaparser.elements.capabilitytype import CapabilityTypeDef
 import toscaparser.elements.interfaces as ifaces
 from toscaparser.elements.relationshiptype import RelationshipType
 from toscaparser.elements.statefulentitytype import StatefulEntityType
 from toscaparser.common.exception import InvalidTypeError, InvalidTypeDefinition
 
 
+def _find_key_in_list(seq, key):
+    for i, item in enumerate(seq):
+        if isinstance(item, dict) and len(item) == 1 and key in item:
+            return i
+    return -1
+
+
+def _merge_dict_lists(base, current):
+    merged = current[:]
+    for item in base:
+        key = next(iter(item))
+        # add base item if not present in current
+        index = _find_key_in_list(current, key)
+        if index == -1:
+            merged.append(item)
+    return merged
+
+
 class NodeType(StatefulEntityType):
     '''TOSCA built-in node type.'''
     SECTIONS = (DERIVED_FROM, METADATA, PROPERTIES, VERSION, DESCRIPTION, ATTRIBUTES,
                 REQUIREMENTS, CAPABILITIES, INTERFACES, ARTIFACTS, INSTANCE_KEYS, _SOURCE) = \
                ('derived_from', 'metadata', 'properties', 'version',
                 'description', 'attributes', 'requirements', 'capabilities',
                 'interfaces', 'artifacts', 'instance_keys', '_source')
@@ -173,14 +191,31 @@
         return {cap.name: cap
                 for cap in self.get_capability_typedefs()}
 
     @property
     def requirements(self):
         return self.get_value(self.REQUIREMENTS, None, True)
 
+    @staticmethod
+    def merge_requirement_definition(base, current):
+        tpl = dict(base, **current)
+        if base.get('node_filter') and current.get('node_filter'):
+            tpl["node_filter"] = {}
+            bfilters = base["node_filter"]
+            cfilters = current["node_filter"]
+            for key in ["requirements", "properties"]:
+                if bfilters.get(key):
+                    tpl["node_filter"][key] = _merge_dict_lists(bfilters[key], cfilters.get(key, []))
+                elif key in cfilters:
+                    tpl["node_filter"][key] = cfilters[key]
+        if base.get('metadata') and current.get('metadata'):
+            # merge metadata
+            tpl['metadata'] = dict(base['metadata'], **current['metadata'])
+        return tpl
+
     def get_all_requirements(self):
         # requirements with any shorthand syntax normalized
         reqs_tpl = self.requirements
         # avoid crashing:
         if reqs_tpl is None or self._requirement_definitions and "__invalid" in self._requirement_definitions:
             return []
         requirements = {}
@@ -191,18 +226,15 @@
             if name in requirements:
                 # update value with current (more derived) value
                 current = requirements[name][name]
                 if isinstance(current, str):
                     # diverges from 3.7.3.2.1 Simple grammar (Capability Type only)
                     tpl = {name: dict(value, node = current)}
                 else:
-                    tpl = {name: dict(value, **current)}
-                    if value.get('metadata') and current.get('metadata'):
-                        # merge metadata
-                        tpl[name]['metadata'] = dict(value['metadata'], **current['metadata'])
+                    tpl = {name: self.merge_requirement_definition(value, current)}
             elif isinstance(value, str):
                 # diverges from 3.7.3.2.1 Simple grammar (Capability Type only)
                 tpl = {name : dict(node = value)}
             requirements[name] = tpl
         return list(requirements.values())
 
     @property
```

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/policytype.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/policytype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/portspectype.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/portspectype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/property_definition.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/property_definition.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/relationshiptype.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/relationshiptype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/scalarunit.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/scalarunit.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/statefulentitytype.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/statefulentitytype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/elements/tosca_type_validation.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/tosca_type_validation.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/entity_template.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/entity_template.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/exttools.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/exttools.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml` & `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml` & `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml` & `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/functions.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/functions.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/groups.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/groups.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/imports.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,18 @@
             return full_url, False, None
         else:
             return None
 
     def load_yaml(self, importsLoader, path, isFile=True, fragment=None):
         return YAML_LOADER(path, isFile, importsLoader, fragment)
 
+    def load_imports(self, importsLoader, importslist):
+        importsLoader.importslist = importslist
+        importsLoader._validate_and_load_imports()
+
 
 class ImportsLoader(object):
 
     IMPORTS_SECTION = (FILE, REPOSITORY, NAMESPACE_URI, NAMESPACE_PREFIX, WHEN) = (
         "file",
         "repository",
         "namespace_uri",
```

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/nodetemplate.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/nodetemplate.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 
 import logging
 
+
 from toscaparser.common.exception import ExceptionCollector
 from toscaparser.common.exception import InvalidPropertyValueError
 from toscaparser.common.exception import MissingRequiredFieldError
 from toscaparser.common.exception import TypeMismatchError
-from toscaparser.common.exception import UnknownFieldError
 from toscaparser.common.exception import ValidationError
+from toscaparser.common.exception import InvalidOccurrences
 from toscaparser.dataentity import DataEntity
 from toscaparser.entity_template import EntityTemplate
 from toscaparser.relationship_template import RelationshipTemplate
 from toscaparser.utils.gettextutils import _
 from toscaparser.artifacts import Artifact
 from toscaparser.activities import ConditionClause
+from toscaparser.elements.nodetype import NodeType
 
 log = logging.getLogger('tosca')
 
 
 class NodeTemplate(EntityTemplate):
     '''Node template from a Tosca profile.'''
     def __init__(self, name, topology_template, custom_def=None,
@@ -146,23 +148,19 @@
 
         Returns a requirements dict and either RelationshipTemplate or None if there was a validation error.
 
         If no relationship was either assigned or defined by the node's type definition,
         one with type "tosca.relationships.Root" will be returned.
         """
         typeReqDef = self.type_definition.get_requirement_definition(name)
-        reqDef = typeReqDef.copy()
         if isinstance(value, dict):
             # see 3.8.2 Requirement assignment p. 140 for value
-            if typeReqDef.get("metadata") and "metadata" in value:
-                if value["metadata"]:
-                    typeReqDef["metadata"].update(value["metadata"])
-                value["metadata"] = typeReqDef["metadata"]
-            reqDef.update(value)
+            reqDef = NodeType.merge_requirement_definition(typeReqDef, value)
         else:
+            reqDef = typeReqDef.copy()
             reqDef['node'] = value
         return reqDef, self._relationship_from_req(name, reqDef)
 
     def _relationship_from_req(self, name, reqDef):
         relationship = reqDef['relationship']
         relTpl = None
         type = None
@@ -406,24 +404,22 @@
                 self._validate_occurrences(value)
                 break
 
     def _validate_occurrences(self, occurrences):
         DataEntity.validate_datatype('list', occurrences)
         if not isinstance(occurrences, list) or len(occurrences) != 2:
             ExceptionCollector.appendException(
-                InvalidPropertyValueError(what=(occurrences)))
+                InvalidOccurrences(what=(occurrences), why="not a list with 2 items"))
             return
-        if DataEntity.validate_datatype('integer', occurrences[0]):
-            ExceptionCollector.appendException(
-                InvalidPropertyValueError(what=(occurrences)))
-        if occurrences[1] != "UNBOUNDED":
-            DataEntity.validate_datatype('integer', occurrences[1])
-            if not (0 <= occurrences[0] <= occurrences[1]) or occurrences[1] == 0:
-                ExceptionCollector.appendException(
-                    InvalidPropertyValueError(what=(occurrences)))
+        if isinstance(DataEntity.validate_datatype('integer', occurrences[0]), int):
+            if occurrences[1] != "UNBOUNDED":
+                if isinstance(DataEntity.validate_datatype('integer', occurrences[1]), int):
+                    if not (0 <= occurrences[0] <= occurrences[1]) or occurrences[1] == 0:
+                        ExceptionCollector.appendException(
+                            InvalidOccurrences(what=(occurrences), why="invalid range"))
 
     def _validate_instancekeys(self):
         template = self.entity_tpl
         msg = (_('keys definition of "%s" must be a list of containing strings or lists') % self.name)
         keys = self.type_definition.get_value(self.INSTANCE_KEYS, template, parent=True) or []
         if not isinstance(keys, list):
             ExceptionCollector.appendException(
```

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/parameters.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/parameters.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/policy.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/policy.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/prereq/csar.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/prereq/csar.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/properties.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/properties.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/relationship_template.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/relationship_template.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/repositories.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/repositories.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/reservation.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/reservation.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/shell.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/shell.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/steps.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/steps.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/substitution_mappings.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/substitution_mappings.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/topology_template.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/topology_template.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/tosca_template.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/tosca_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,61 +178,58 @@
         return self.topology_template.policies
 
     def get_type_sections(self):
         return [TYPES, NODE_TYPES, CAPABILITY_TYPES, RELATIONSHIP_TYPES,
                  DATA_TYPES, ARTIFACT_TYPES, INTERFACE_TYPES, POLICY_TYPES, GROUP_TYPES]
 
     def _get_all_custom_defs(self):
-        custom_defs = self._get_custom_defs(self.tpl, self.path)
+        custom_defs, nested_tosca_tpls = self._get_custom_defs(self.tpl, self.path)
+        self.nested_tosca_tpls = nested_tosca_tpls
         # Handle custom types defined in current template file
         for type_def in self.get_type_sections():
             inner_custom_types = self.tpl.get(type_def)
             if inner_custom_types:
                 custom_defs.update(inner_custom_types)
         return custom_defs
 
     def _get_custom_defs(self, tpl, path):
         custom_defs_final = {}
+        tosca_tpls = {}
         custom_defs, nested_imports = self.load_imports(path, tpl)
         for imported in nested_imports:
             filename, import_tpl = list(imported.items())[0]
-            import_defs = self._get_custom_defs(import_tpl, filename)
+            tosca_tpls.update(imported)
+            import_defs, nested_tosca_tpls = self._get_custom_defs(import_tpl, filename)
             custom_defs_final.update(import_defs)
+            tosca_tpls.update(nested_tosca_tpls)
         if custom_defs:
             custom_defs_final.update(custom_defs)
-        return custom_defs_final
+        return custom_defs_final, tosca_tpls
 
     def load_imports(self, path, tpl):
         """Handle custom types defined in imported template files
 
         This method loads the custom type definitions referenced in "imports"
         section of the TOSCA YAML template.
         """
         imports = tpl.get("imports")
         if not imports:
             return {}, {}
 
         type_sections = self.get_type_sections()
         imports_loader = toscaparser.imports.ImportsLoader(
-            imports, path, type_sections, self.tpl.get("repositories"), self.import_resolver
+            None, path, type_sections, self.tpl.get("repositories"), self.import_resolver
         )
+        imports_loader.resolver.load_imports(imports_loader, imports)
         # nested_tosca_tpls is list of {file_path : tpl} of the imported templates
         nested_tosca_tpls = imports_loader.get_nested_tosca_tpls()
         # custom defs are merged together (with possibly namespace prefix)
         custom_defs = imports_loader.get_custom_defs()
-        self._update_nested_tosca_tpls(nested_tosca_tpls)
         return custom_defs, nested_tosca_tpls
 
-    def _update_nested_tosca_tpls(self, nested_tosca_tpls):
-        for tpl in nested_tosca_tpls:
-            # add every import (even if it doesn't have a topology)
-            filename, tosca_tpl = list(tpl.items())[0]
-            if filename not in self.nested_tosca_tpls:
-                self.nested_tosca_tpls.update(tpl)
-
     def _handle_nested_tosca_templates_with_topology(self, custom_types):
         for filename, tosca_tpl in self.nested_tosca_tpls.items():
             topology_tpl = tosca_tpl.get(TOPOLOGY_TEMPLATE)
             if topology_tpl:
                 custom_types = custom_types.copy()
                 custom_types.update(tosca_tpl.get('node_types', {})) # XXX isn't this redundant?
                 self.nested_topologies[filename] = TopologyTemplate(
```

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/tpl_relationship_graph.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/tpl_relationship_graph.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/triggers.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/triggers.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/unsupportedtype.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/unsupportedtype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/utils/gettextutils.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/utils/gettextutils.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/utils/urlutils.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/utils/urlutils.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/utils/validateutils.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/utils/validateutils.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/utils/yamlparser.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/utils/yamlparser.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/vendor/toscaparser/workflow.py` & `unfurl-0.6.2/unfurl/vendor/toscaparser/workflow.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.1/unfurl/yamlloader.py` & `unfurl-0.6.2/unfurl/yamlloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 # SPDX-License-Identifier: MIT
 import io
 import os.path
 import sys
 import codecs
 import json
 import os
-from typing import Optional, TextIO, Union, Tuple, List, cast, TYPE_CHECKING, Dict
+from typing import Any, Optional, TextIO, Union, Tuple, List, cast, TYPE_CHECKING, Dict
 import urllib
 import urllib.request
 from urllib.parse import urljoin, urlsplit
 import ssl
 import certifi
 from jsonschema import RefResolver
 from ruamel.yaml import YAML
 from ruamel.yaml.comments import CommentedMap
 from ruamel.yaml.representer import RepresenterError, SafeRepresenter
 from ruamel.yaml.constructor import ConstructorError
+
 if TYPE_CHECKING:
     from .manifest import Manifest
 
 pathname2url = urllib.request.pathname2url
 
 from .util import (
     filter_env,
@@ -40,15 +41,15 @@
     expand_doc,
     make_map_with_base,
     find_anchor,
     _cache_anchors,
     restore_includes,
 )
 from .repo import RepoView, GitRepo, is_url_or_git_path, split_git_url
-from .packages import resolve_package
+from .packages import UnfurlPackageUpdateNeeded, resolve_package
 from .logs import getLogger
 from toscaparser.common.exception import URLException, ExceptionCollector
 from toscaparser.utils.gettextutils import _
 import toscaparser.imports
 from toscaparser.repositories import Repository
 
 from ansible.parsing.vault import VaultLib, VaultSecret
@@ -260,14 +261,21 @@
 
     def set_cache(self, url, val):
         self.manifest.cache[url] = val
 
     def get_cache(self, url):
         return self.manifest.cache.get(url)
 
+    def load_imports(self, importsLoader, importslist):
+        while True:
+            try:
+                return super().load_imports(importsLoader, importslist)
+            except UnfurlPackageUpdateNeeded:
+                pass  # reload
+
     def get_repository(self, name: str, tpl: dict) -> Repository:
         # don't create another Repository instance
         if name in self.manifest.repositories:
             return self.manifest.repositories[name].repository
 
         if isinstance(tpl, dict) and "url" in tpl:
             url = tpl["url"]
@@ -352,14 +360,15 @@
         if repository_name:
             file_name, sep, fragment = file_name.partition("#")
             path, isFile, repo_view = self._get_repository_path(
                 importsLoader, repository_name
             )
             # if not isFile path will be git url possibly including revision in fragment
             if repo_view and repo_view.repo:
+                repo_view.add_file_ref(file_name)
                 return os.path.join(repo_view.working_dir, file_name), True, fragment
         else:
             url_info = cast(
                 GetURLType, super().get_url(importsLoader, None, file_name, isFile)
             )
             if not url_info:
                 return url_info
@@ -379,78 +388,92 @@
                     path, repo, filePath, revision, file_name, importsLoader
                 )
                 return path, False, fragment
             else:
                 if repo_view:
                     assert not repo_view.repo
                     repo_view.set_repo_and_path(repo, filePath)
+                    repo_view.add_file_ref(file_name)
                 path = os.path.join(repo.working_dir, filePath, file_name or "").rstrip(
                     "/"
                 )
         elif file_name:
             path = os.path.join(path, file_name)
 
         # always a local file path at this point
         return path, True, fragment
 
-    def load_yaml(self, importsLoader, path, isFile=True, fragment=None):
+    def _open(self, path: str, isFile: bool) -> Optional[TextIO]:
+        if path.startswith("git-ref:"):
+            url, filePath, revision = split_git_url(path)
+            return io.StringIO(self.repo_refs[url].show(filePath, revision))
+        else:
+            try:
+                if isFile:
+                    ignoreFileNotFound = self.ignoreFileNotFound
+                    if ignoreFileNotFound and not os.path.isfile(path):
+                        return None
+
+                    if self.yamlloader:
+                        # show == True if file was decrypted
+                        contents, show = self.yamlloader._get_file_contents(path)
+                        f: TextIO = io.StringIO(codecs.decode(contents))
+                    else:
+                        f = codecs.open(path, encoding="utf-8", errors="strict")
+                else:
+                    f = urlopen(path)
+                return f
+            except urllib.error.URLError as e:
+                if hasattr(e, "reason"):
+                    msg = _(
+                        (
+                            'Failed to reach server "%(path)s". Reason is: '
+                            + "%(reason)s."
+                        )
+                    ) % {"path": path, "reason": e.reason}
+                    ExceptionCollector.appendException(URLException(what=msg))
+                    return None
+                elif hasattr(e, "code"):
+                    msg = _(
+                        (
+                            'The server "%(path)s" couldn\'t fulfill the request. '
+                            + 'Error code: "%(code)s".'
+                        )
+                    ) % {
+                        "path": path,
+                        "code": e.code,  # type: ignore
+                    }
+                    ExceptionCollector.appendException(URLException(what=msg))
+                    return None
+                else:
+                    raise
+
+    def load_yaml(
+        self,
+        importsLoader: toscaparser.imports.ImportsLoader,
+        path: str,
+        isFile=True,
+        fragment=None,
+    ) -> Any:
         try:
             logger.trace(
                 "attempting to load YAML %s: %s", "file" if isFile else "url", path
             )
             originalPath = path
             doc = self.get_cache(path)
             if doc is not None:
                 if fragment and doc:
                     return _refResolver.resolve_fragment(doc, fragment)
                 else:
                     return doc
 
-            if path.startswith("git-ref:"):
-                url, filePath, revision = split_git_url(path)
-                f: TextIO = io.StringIO(self.repo_refs[url].show(filePath, revision))
-            else:
-                try:
-                    if isFile:
-                        ignoreFileNotFound = self.ignoreFileNotFound
-                        if ignoreFileNotFound and not os.path.isfile(path):
-                            return None
-
-                        if self.yamlloader:
-                            # show == True if file was decrypted
-                            contents, show = self.yamlloader._get_file_contents(path)
-                            f = io.StringIO(codecs.decode(contents))
-                        else:
-                            f = codecs.open(path, encoding="utf-8", errors="strict")
-                    else:
-                        f = urlopen(path)
-                except urllib.error.URLError as e:
-                    if hasattr(e, "reason"):
-                        msg = _(
-                            (
-                                'Failed to reach server "%(path)s". Reason is: '
-                                + "%(reason)s."
-                            )
-                        ) % {"path": path, "reason": e.reason}
-                        ExceptionCollector.appendException(URLException(what=msg))
-                        return
-                    elif hasattr(e, "code"):
-                        msg = _(
-                            (
-                                'The server "%(path)s" couldn\'t fulfill the request. '
-                                + 'Error code: "%(code)s".'
-                            )
-                        ) % {
-                            "path": path,
-                            "code": e.code,  # type: ignore
-                        }
-                        ExceptionCollector.appendException(URLException(what=msg))
-                        return
-                    else:
-                        raise
+            f = self._open(path, isFile)
+            if f is None:
+                return None
+
             with f:
                 contents = f.read()
                 doc = load_yaml(yaml, contents, path, self.readonly)
                 yaml_dict = yaml_dict_type(self.readonly)
                 if isinstance(doc, yaml_dict):
                     if self.expand:
                         includes, doc = expand_doc(
@@ -468,14 +491,20 @@
             if path != originalPath:
                 msg = f'Could not load "{path}" (originally "{originalPath}")'
             else:
                 msg = f'Could not load "{path}"'
             raise UnfurlError(msg, True)
 
 
+class LoadIncludeAction:
+    def __init__(self, check_include=False, get_key=None):
+        self.get_key = get_key
+        self.check_include = check_include
+
+
 class YamlConfig:
     def __init__(
         self,
         config=None,
         path=None,
         validate=True,
         schema=None,
@@ -508,43 +537,50 @@
             else:
                 self.config = config
             if not isinstance(self.config, dict):
                 raise UnfurlValidationError(
                     f'invalid YAML document with contents: "{self.config}"'
                 )
 
-            find_anchor(self.config, None)  # create _anchorCache
-            self._cachedDocIncludes = {}
             # schema should include defaults but can't validate because it doesn't understand includes
             # but should work most of time
             self.config.loadTemplate = self.load_include  # type: ignore
             self.loadHook = loadHook
-
             self.baseDirs = [self.get_base_dir()]
-            yaml_dict = yaml_dict_type(self.readonly)
-            self.includes, expandedConfig = expand_doc(
-                self.config,
-                cls=make_map_with_base(self.config, self.baseDirs[0], yaml_dict),
-            )
-            self.expanded = expandedConfig
-            errors = schema and self.validate(expandedConfig)
+            while True:
+                try:
+                    self.includes, self.expanded = self._expand()
+                except UnfurlPackageUpdateNeeded:
+                    pass  # reload
+                else:
+                    break
+            errors = schema and self.validate(self.expanded)
             if errors and validate:
                 (message, schemaErrors) = errors
                 raise UnfurlValidationError(
                     "JSON Schema validation failed: " + message, errors
                 )
             else:
                 self.valid = not not errors
         except Exception:
             if self.path:
                 msg = f"Unable to load yaml config at {self.path}"
             else:
                 msg = "Unable to parse yaml config"
             raise UnfurlError(msg, True)
 
+    def _expand(self) -> Tuple[dict, dict]:
+        find_anchor(self.config, None)  # create _anchorCache
+        self._cachedDocIncludes: Dict[str, Tuple[str, dict]] = {}
+        yaml_dict = yaml_dict_type(self.readonly)
+        return expand_doc(
+            self.config,
+            cls=make_map_with_base(self.config, self.baseDirs[0], yaml_dict),
+        )
+
     def load_yaml(self, path, baseDir=None, warnWhenNotFound=False):
         url = urlsplit(path)
         if url.scheme.startswith("http") and url.netloc:  # looks like an absolute url
             fragment = url.fragment
             logger.trace("attempting to load YAML url: %s", path)
             try:
                 f = urlopen(path)
@@ -669,15 +705,15 @@
             if self.loadHook:
                 return self.loadHook(
                     self,
                     templatePath,
                     self.baseDirs[-1],
                     warnWhenNotFound,
                     expanded,
-                    check,
+                    LoadIncludeAction(check_include=True),
                 )
             else:
                 return True
 
         if templatePath == self.baseDirs[-1]:  # pop hack
             self.baseDirs.pop()
             return
@@ -700,30 +736,30 @@
             # give loadHook change to transform key
             key = self.loadHook(
                 self,
                 templatePath,
                 self.baseDirs[-1],
                 warnWhenNotFound,
                 expanded,
-                key,
+                LoadIncludeAction(get_key=key),
             )
             if not key:
                 return value, None, ""
 
         if key in self._cachedDocIncludes:
             path, template = self._cachedDocIncludes[key]
             baseDir = os.path.dirname(path)
             self.baseDirs.append(baseDir)
             return value, template, baseDir
 
         try:
             baseDir = self.baseDirs[-1]
             if self.loadHook:
                 path, template = self.loadHook(
-                    self, templatePath, baseDir, warnWhenNotFound, expanded
+                    self, templatePath, baseDir, warnWhenNotFound, expanded, None
                 )
             else:
                 path, template = self.load_yaml(key, baseDir, warnWhenNotFound)
 
             if template is None:
                 return value, template, baseDir
 
@@ -737,9 +773,9 @@
         except Exception:
             raise UnfurlError(
                 f"unable to load document include: {templatePath} (base: {baseDir})",
                 True,
             )
         self.baseDirs.append(newBaseDir)
 
-        self._cachedDocIncludes[key] = [path, template]
+        self._cachedDocIncludes[key] = (path, template)
         return value, template, newBaseDir
```

### Comparing `unfurl-0.6.1/unfurl/yamlmanifest.py` & `unfurl-0.6.2/unfurl/yamlmanifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
         self.changeLogPath: str = manifest.get("jobsLog") or ""
         self.jobsFolder: str = manifest.get("jobsFolder", "jobs")
         if not self.changeLogPath and localEnv and manifest.get("changes") is None:
             # save changes to a separate file if we're in a local environment
             self.changeLogPath = DefaultNames.JobsLog
         self.load_changes(manifest.get("changes"), self.changeLogPath)
 
-        self.lastJob = manifest.get("lastJob")
+        self.lastJob: Optional[dict] = manifest.get("lastJob")
 
         if localEnv:
             for name in ["locals", "secrets"]:
                 instance, local_spec = localEnv.get_local_instance(name, self.context)
                 self.imports.add_import(name.rstrip("s"), instance, local_spec)
 
         rootResource = self.create_topology_instance(status)
@@ -529,15 +529,15 @@
                 parent=self.localEnv,
                 override_context=location.get("environment", ""),
             )
             if self.is_path_to_self(localEnv.manifestPath):
                 # don't import self (might happen when context is shared)
                 return
             logger.verbose("loading external ensemble at %s", localEnv.manifestPath)
-            importedManifest = localEnv.get_manifest()
+            importedManifest = localEnv.get_manifest(skip_validation=not self.validate)
 
         uri = value.get("uri")
         if uri and not importedManifest.has_uri(uri):
             raise UnfurlError(
                 f"Error importing external ensemble at '{path}', uri mismatch for '{uri}'"
             )
         rname = value.get("instance", "root")
```

### Comparing `unfurl-0.6.1/unfurl.egg-info/PKG-INFO` & `unfurl-0.6.2/unfurl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfurl
-Version: 0.6.1
+Version: 0.6.2
 Summary: use Git to record and deploy changes to your DevOps infrastructure
 Home-page: https://github.com/onecommons/unfurl
 Author: Adam Souzis
 Author-email: adam@onecommons.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -48,15 +48,15 @@
 
 1\. Use `unfurl init` to create an Unfurl-managed git repository. Or use `unfurl clone` to clone an existing one.
 
 2\. The repository will contain a few YAML files that you can edit. They will describe everything you'll need to deploy your application, such as:
 
 - Cloud provider and SaaS services account credentials and other secrets organized into environments.
 - Code repositories and container image registries.
-- A high-level model of your cloud infrastructure and their dependencies such as compute instances and databases, described using the [TOSCA](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=tosca) standard.
+- A high-level model of your cloud infrastructure and their dependencies such as compute instances and databases, described using the [OASIS TOSCA](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=tosca) (Topology and Orchestration Specification for Cloud Applications) standard.
 - Operations that invoke Terraform, Ansible, or other command-line tools (which Unfurl can automatically install).
 
 3\. Use `unfurl deploy` to deploy the infrastructure. Unfurl will generate a plan based on your target environment and high-level model and choose the correct operations to call. It will commit to git the latest configuration and a history of changes to your cloud accounts.
 
 4\. Now you have a reproducible description of your cloud infrastructure stored in git! So you can:
 
 - Push your repository to a git service such as Github or Gitlab to share it. For access control, each environment can be stored as separate git submodules or branches.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unfurl Version: 0.6.1 Summary: use Git to record
+Metadata-Version: 2.1 Name: unfurl Version: 0.6.2 Summary: use Git to record
 and deploy changes to your DevOps infrastructure Home-page: https://github.com/
 onecommons/unfurl Author: Adam Souzis Author-email: adam@onecommons.org
 License: MIT Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -25,24 +25,25 @@
 build open source software. ## How it works 1\. Use `unfurl init` to create an
 Unfurl-managed git repository. Or use `unfurl clone` to clone an existing one.
 2\. The repository will contain a few YAML files that you can edit. They will
 describe everything you'll need to deploy your application, such as: - Cloud
 provider and SaaS services account credentials and other secrets organized into
 environments. - Code repositories and container image registries. - A high-
 level model of your cloud infrastructure and their dependencies such as compute
-instances and databases, described using the [TOSCA](https://www.oasis-
-open.org/committees/tc_home.php?wg_abbrev=tosca) standard. - Operations that
-invoke Terraform, Ansible, or other command-line tools (which Unfurl can
-automatically install). 3\. Use `unfurl deploy` to deploy the infrastructure.
-Unfurl will generate a plan based on your target environment and high-level
-model and choose the correct operations to call. It will commit to git the
-latest configuration and a history of changes to your cloud accounts. 4\. Now
-you have a reproducible description of your cloud infrastructure stored in git!
-So you can: - Push your repository to a git service such as Github or Gitlab to
-share it. For access control, each environment can be stored as separate git
+instances and databases, described using the [OASIS TOSCA](https://www.oasis-
+open.org/committees/tc_home.php?wg_abbrev=tosca) (Topology and Orchestration
+Specification for Cloud Applications) standard. - Operations that invoke
+Terraform, Ansible, or other command-line tools (which Unfurl can automatically
+install). 3\. Use `unfurl deploy` to deploy the infrastructure. Unfurl will
+generate a plan based on your target environment and high-level model and
+choose the correct operations to call. It will commit to git the latest
+configuration and a history of changes to your cloud accounts. 4\. Now you have
+a reproducible description of your cloud infrastructure stored in git! So you
+can: - Push your repository to a git service such as Github or Gitlab to share
+it. For access control, each environment can be stored as separate git
 submodules or branches. - Pull incoming changes and review and approve pull
 requests before deploying. - Clone the repository and deploy to new
 environments even if they use different services -- because is your model is
 adaptable, manual changes are minimized. ## Features ### No server, agentless
 Simple, stand-alone CLI that can be used both in your local development
 environment or in an automated CI/CD pipeline. ### Deploy infrastructure from
 simple, application-centric descriptions - Model your cloud infrastructure with
```

### Comparing `unfurl-0.6.1/unfurl.egg-info/SOURCES.txt` & `unfurl-0.6.2/unfurl.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 unfurl/__init__.py
 unfurl/__main__.py
 unfurl/changelog-schema.json
+unfurl/cloudmap.py
 unfurl/configurator.py
 unfurl/eval.py
 unfurl/init.py
 unfurl/job.py
 unfurl/localenv.py
 unfurl/lock.py
 unfurl/logs.py
```

### Comparing `unfurl-0.6.1/unfurl.egg-info/requires.txt` & `unfurl-0.6.2/unfurl.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,14 @@
 moto[server]==3.1.4
 mypy==0.950
 pytest
 pytest-cov
 pytest-profiling
 pytest-xdist[psutil]
 types-six==1.16.15
-werkzeug==2.1.2
+werkzeug==2.2.3
 
 [test:( python_version<'3')]
 python-jose[cryptography]<3.3.0,>=3.1.0
 
 [test:( python_version=='2.7')]
 mock
```

