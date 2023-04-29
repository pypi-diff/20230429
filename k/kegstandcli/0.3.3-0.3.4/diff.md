# Comparing `tmp/kegstandcli-0.3.3.tar.gz` & `tmp/kegstandcli-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegstandcli-0.3.3.tar", max compression
+gzip compressed data, was "kegstandcli-0.3.4.tar", max compression
```

## Comparing `kegstandcli-0.3.3.tar` & `kegstandcli-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1077 2023-04-23 18:42:25.686572 kegstandcli-0.3.3/LICENSE
--rw-r--r--   0        0        0     6568 2023-04-28 20:24:54.296230 kegstandcli-0.3.3/README.md
--rw-r--r--   0        0        0     1545 2023-04-28 20:29:39.806778 kegstandcli-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-03 20:22:59.696056 kegstandcli-0.3.3/src/kegstandcli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 20:23:08.893322 kegstandcli-0.3.3/src/kegstandcli/cli/__init__.py
--rw-r--r--   0        0        0    16328 2023-04-12 22:03:29.066576 kegstandcli-0.3.3/src/kegstandcli/cli/__main__.py
--rw-r--r--   0        0        0     3158 2023-04-12 22:03:29.067785 kegstandcli-0.3.3/src/kegstandcli/cli/build.py
--rw-r--r--   0        0        0     1995 2023-04-23 18:42:31.185993 kegstandcli-0.3.3/src/kegstandcli/cli/config.py
--rw-r--r--   0        0        0      154 2023-04-12 22:03:29.068379 kegstandcli-0.3.3/src/kegstandcli/cli/default_lambda.py.tmpl
--rw-r--r--   0        0        0     1887 2023-04-12 22:03:29.068881 kegstandcli-0.3.3/src/kegstandcli/cli/deploy.py
--rw-r--r--   0        0        0     1179 2023-04-25 19:33:46.541089 kegstandcli-0.3.3/src/kegstandcli/cli/new.py
--rw-r--r--   0        0        0      985 2023-04-27 20:31:45.006926 kegstandcli-0.3.3/src/kegstandcli/cli/teardown.py
--rw-r--r--   0        0        0        0 2023-04-03 20:23:36.547617 kegstandcli-0.3.3/src/kegstandcli/infra/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-26 17:37:46.125480 kegstandcli-0.3.3/src/kegstandcli/infra/app.py
--rw-r--r--   0        0        0      275 2023-04-27 20:31:57.718526 kegstandcli-0.3.3/src/kegstandcli/infra/cdk.json
--rw-r--r--   0        0        0        0 2023-04-03 20:23:50.899135 kegstandcli-0.3.3/src/kegstandcli/infra/stacks/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-12 22:03:29.071990 kegstandcli-0.3.3/src/kegstandcli/infra/stacks/lambda_rest_api.py
--rw-r--r--   0        0        0     1491 2023-04-12 22:03:29.073183 kegstandcli-0.3.3/src/kegstandcli/utils.py
--rw-r--r--   0        0        0     7887 1970-01-01 00:00:00.000000 kegstandcli-0.3.3/setup.py
--rw-r--r--   0        0        0     7946 1970-01-01 00:00:00.000000 kegstandcli-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-23 18:42:25.686572 kegstandcli-0.3.4/LICENSE
+-rw-r--r--   0        0        0     6518 2023-04-29 20:52:25.087043 kegstandcli-0.3.4/README.md
+-rw-r--r--   0        0        0     1545 2023-04-29 20:54:05.619630 kegstandcli-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 20:22:59.696056 kegstandcli-0.3.4/src/kegstandcli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:08.893322 kegstandcli-0.3.4/src/kegstandcli/cli/__init__.py
+-rw-r--r--   0        0        0    16328 2023-04-12 22:03:29.066576 kegstandcli-0.3.4/src/kegstandcli/cli/__main__.py
+-rw-r--r--   0        0        0     3158 2023-04-12 22:03:29.067785 kegstandcli-0.3.4/src/kegstandcli/cli/build.py
+-rw-r--r--   0        0        0     1995 2023-04-23 18:42:31.185993 kegstandcli-0.3.4/src/kegstandcli/cli/config.py
+-rw-r--r--   0        0        0      154 2023-04-12 22:03:29.068379 kegstandcli-0.3.4/src/kegstandcli/cli/default_lambda.py.tmpl
+-rw-r--r--   0        0        0     1887 2023-04-12 22:03:29.068881 kegstandcli-0.3.4/src/kegstandcli/cli/deploy.py
+-rw-r--r--   0        0        0     1179 2023-04-25 19:33:46.541089 kegstandcli-0.3.4/src/kegstandcli/cli/new.py
+-rw-r--r--   0        0        0     1230 2023-04-29 20:41:27.128807 kegstandcli-0.3.4/src/kegstandcli/cli/teardown.py
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:36.547617 kegstandcli-0.3.4/src/kegstandcli/infra/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-26 17:37:46.125480 kegstandcli-0.3.4/src/kegstandcli/infra/app.py
+-rw-r--r--   0        0        0      275 2023-04-27 20:31:57.718526 kegstandcli-0.3.4/src/kegstandcli/infra/cdk.json
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:50.899135 kegstandcli-0.3.4/src/kegstandcli/infra/stacks/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-12 22:03:29.071990 kegstandcli-0.3.4/src/kegstandcli/infra/stacks/lambda_rest_api.py
+-rw-r--r--   0        0        0      989 2023-04-29 20:18:46.411400 kegstandcli-0.3.4/src/kegstandcli/utils.py
+-rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 kegstandcli-0.3.4/setup.py
+-rw-r--r--   0        0        0     7896 1970-01-01 00:00:00.000000 kegstandcli-0.3.4/PKG-INFO
```

### Comparing `kegstandcli-0.3.3/LICENSE` & `kegstandcli-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.3/README.md` & `kegstandcli-0.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,20 +55,18 @@
 
 ```shell
 my-service
 ├── .gitignore                        # Standard .gitignore file
 ├── pyproject.toml                    # Project configuration
 └── src
     └── api
-        └── resources
-            └── hello
-                └── any.py            # Logic for /hello/
+        └── hello.py                  # Logic for /hello/
 ```
 
-Kegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a few empty `__init__.py` gatecrashers, but we can safely ignore those.
+Kegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a single, empty `__init__.py` gatecrasher, but we can safely ignore that one.
 
 To install the dependencies for the new project:
 
 ```shell
 > cd my-service
 > poetry install
 ```
@@ -89,15 +87,15 @@
 
 Here are some notable changes, fixes and features that are planned for development:
 
 ## 0.4.0
 
 - [ ] More content on [kegstand.dev](https://kegstand.dev)
 - [ ] Custom domain names
-- [ ] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
+- [X] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
 
 ### Pre-1.0.0
 
 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.
 - [ ] Pagination helper
 - [ ] [Record a screencast](https://asciinema.org/) for the README
 - [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)
```

#### html2text {}

```diff
@@ -30,52 +30,52 @@
 can create this in a few seconds, either with the Kegstand CLI or using
 [Copier](https://copier.readthedocs.io/en/stable/#installation). ```shell #
 Using the Kegstand CLI > pipx install kegstandcli > keg new my-service # Using
 Copier > copier gh:JensRoland/kegstand-project-template my-service ``` Either
 method will create a new project folder called `my-service` containing:
 ```shell my-service âââ .gitignore # Standard .gitignore file âââ
 pyproject.toml # Project configuration âââ src âââ api âââ
-resources âââ hello âââ any.py # Logic for /hello/ ``` Kegstand
-projects are minimal by design, so a fresh project folder contains just those 3
-files. Well, apart from a few empty `__init__.py` gatecrashers, but we can
-safely ignore those. To install the dependencies for the new project: ```shell
-> cd my-service > poetry install ``` Finally, to build and deploy the service
-to AWS: ```shell > poetry run keg deploy ``` You should now be able to access
-the API endpoint at `https://.execute-api..amazonaws.com/prod/hello`. ##
-Documentation For further examples and more advanced usage, see the [official
-documentation](https://github.com/JensRoland/kegstand/blob/main/docs/index.md).
-## Roadmap Here are some notable changes, fixes and features that are planned
-for development: ## 0.4.0 - [ ] More content on [kegstand.dev](https://
-kegstand.dev) - [ ] Custom domain names - [ ] Maybe simplify the folder
-structure from `src/api/resources//.py` to `src/api/.py` ### Pre-1.0.0 - [ ]
-Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch
-CRON scheduled events, etc. - [ ] Pagination helper - [ ] [Record a screencast]
-(https://asciinema.org/) for the README - [ ] Autogenerated docs using [MkDocs]
-(https://www.mkdocs.org/) - [ ] GitHub Actions workflow for pushing docs to the
-website ### 1.0.0 - [ ] Intuitive and mostly automated API Versioning - [ ]
-Simple way to define/override core API/Lambda properties such as CPU/MEM,
-Python runtime version, warm pool (!), and concurrency - [ ] Deploy Lambda-only
-microservices with no API Gateway ### Future - [ ] Configurable log level - [ ]
-Add AWS tags in the Kegstand config and they will be applied to the generated
-resources - [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/
-lambda/latest/dg/configuration-layers.html) - [ ] Add support for APIs using
-[FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/
+hello.py # Logic for /hello/ ``` Kegstand projects are minimal by design, so a
+fresh project folder contains just those 3 files. Well, apart from a single,
+empty `__init__.py` gatecrasher, but we can safely ignore that one. To install
+the dependencies for the new project: ```shell > cd my-service > poetry install
+``` Finally, to build and deploy the service to AWS: ```shell > poetry run keg
+deploy ``` You should now be able to access the API endpoint at `https:/
+/.execute-api..amazonaws.com/prod/hello`. ## Documentation For further examples
+and more advanced usage, see the [official documentation](https://github.com/
+JensRoland/kegstand/blob/main/docs/index.md). ## Roadmap Here are some notable
+changes, fixes and features that are planned for development: ## 0.4.0 - [ ]
+More content on [kegstand.dev](https://kegstand.dev) - [ ] Custom domain names
+- [X] Maybe simplify the folder structure from `src/api/resources//.py` to
+`src/api/.py` ### Pre-1.0.0 - [ ] Specify event triggers for Lambda functions:
+S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc. - [ ] Pagination
+helper - [ ] [Record a screencast](https://asciinema.org/) for the README - [ ]
+Autogenerated docs using [MkDocs](https://www.mkdocs.org/) - [ ] GitHub Actions
+workflow for pushing docs to the website ### 1.0.0 - [ ] Intuitive and mostly
+automated API Versioning - [ ] Simple way to define/override core API/Lambda
+properties such as CPU/MEM, Python runtime version, warm pool (!), and
+concurrency - [ ] Deploy Lambda-only microservices with no API Gateway ###
+Future - [ ] Configurable log level - [ ] Add AWS tags in the Kegstand config
+and they will be applied to the generated resources - [ ] Easily add [AWS
+Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
+layers.html) - [ ] Add support for APIs using [FastAPI](https://
+fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default
+Kegstand API framework, and just provide deployment helpers for the API Gateway
+and Lambda - [ ] Improved output from deploy command; friendly post-deploy
+instructions for testing your API - [ ] Version bumper with [bump2version]
+(https://pypi.org/project/bump2version/) - [ ] Include more goodies from
+[Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/
+2.11.0/) - tracing, metrics, etc. - [ ] Add support for APIs using pure [Lambda
+Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/
 ) instead of the default Kegstand API framework, and just provide deployment
-helpers for the API Gateway and Lambda - [ ] Improved output from deploy
-command; friendly post-deploy instructions for testing your API - [ ] Version
-bumper with [bump2version](https://pypi.org/project/bump2version/) - [ ]
-Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-
-lambda-powertools-python/2.11.0/) - tracing, metrics, etc. - [ ] Add support
-for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-
-powertools-python/2.11.0/) instead of the default Kegstand API framework, and
-just provide deployment helpers for the API Gateway and Lambda - [ ] Unit
-testing helpers (wrap moto and make it all a little more DRY and intuitive) -
-[ ] Secure endpoints which require re-authentication (and/or MFA) so a
-refreshed token isnât enough (to, say, delete your account or change your
-credit card info) - [ ] Live Lambda development a la SST - [ ] Build and deploy
-gRPC endpoints (or similar alternative) - [ ] Build and deploy GraphQL
-endpoints - [ ] Build and deploy stream processors? - [ ] Option to teardown
-before deploying: `keg deploy --force-redeploy` - [ ] Use env vars to populate
-values in kegstand.toml - [ ] Merge Kegstand and Beth into one tool - [ ] CDK
-Pipelines - [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`,
-etc.) - [ ] Upgrade Copier once the [template-deleting bugfix](https://
-github.com/copier-org/copier/pull/1037) is released
+helpers for the API Gateway and Lambda - [ ] Unit testing helpers (wrap moto
+and make it all a little more DRY and intuitive) - [ ] Secure endpoints which
+require re-authentication (and/or MFA) so a refreshed token isnât enough (to,
+say, delete your account or change your credit card info) - [ ] Live Lambda
+development a la SST - [ ] Build and deploy gRPC endpoints (or similar
+alternative) - [ ] Build and deploy GraphQL endpoints - [ ] Build and deploy
+stream processors? - [ ] Option to teardown before deploying: `keg deploy --
+force-redeploy` - [ ] Use env vars to populate values in kegstand.toml - [ ]
+Merge Kegstand and Beth into one tool - [ ] CDK Pipelines - [ ] Support HTTP
+method-specific files (e.g. `get.py`, `post.py`, etc.) - [ ] Upgrade Copier
+once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/
+1037) is released
```

### Comparing `kegstandcli-0.3.3/pyproject.toml` & `kegstandcli-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kegstandcli"
-version = "0.3.3"
+version = "0.3.4"
 description = "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/kegstand"
 homepage = "https://kegstand.dev"
 readme = "README.md"
 packages = [
@@ -39,12 +39,12 @@
 python = "^3.9"
 tomlkit = "^0.11.7"
 xxhash = "^3.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 pytest-subprocess = "^1.5.0"
-sentient-switchblade = "^0.2.1"
+sentient-switchblade = "^0.2.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kegstandcli-0.3.3/src/kegstandcli/cli/__main__.py` & `kegstandcli-0.3.4/src/kegstandcli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.3/src/kegstandcli/cli/build.py` & `kegstandcli-0.3.4/src/kegstandcli/cli/build.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.3/src/kegstandcli/cli/config.py` & `kegstandcli-0.3.4/src/kegstandcli/cli/config.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.3/src/kegstandcli/cli/deploy.py` & `kegstandcli-0.3.4/src/kegstandcli/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.3/src/kegstandcli/cli/new.py` & `kegstandcli-0.3.4/src/kegstandcli/cli/new.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.3/src/kegstandcli/cli/teardown.py` & `kegstandcli-0.3.4/src/kegstandcli/cli/teardown.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 @click.command()
 @click.pass_context
 @click.option(
     "--region", default="eu-west-1", help="AWS region the stack is deployed to"
 )
 def teardown(ctx, region):
     project_dir = ctx.obj["project_dir"]
-    teardown_command(project_dir, region)
+    config_file = ctx.obj["config"]
+    verbose = ctx.obj["verbose"]
+    teardown_command(verbose, project_dir, config_file, region)
 
 
-def teardown_command(project_dir, region):
+def teardown_command(verbose, project_dir, config_file, region):
     # Get the dir of the Kegstand CLI package itself (one level up from here)
     kegstandcli_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
     subprocess.run(
         [
             "cdk",
             "destroy",
@@ -27,12 +29,16 @@
             "--output",
             f"{project_dir}/cdk.out",
             "--all",
             "--context",
             f"region={region}",
             "--context",
             f"project_dir={project_dir}",
+            "--context",
+            f"config_file={config_file}",
+            "--context",
+            f"verbose={verbose}",
             "--force",
         ],
         cwd=kegstandcli_dir,
         check=True,
     )  # nosec B603, B607
```

### Comparing `kegstandcli-0.3.3/src/kegstandcli/infra/app.py` & `kegstandcli-0.3.4/src/kegstandcli/infra/app.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.3/src/kegstandcli/infra/stacks/lambda_rest_api.py` & `kegstandcli-0.3.4/src/kegstandcli/infra/stacks/lambda_rest_api.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.3/setup.py` & `kegstandcli-0.3.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,17 @@
  'xxhash>=3.2.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['keg = kegstandcli.cli.__main__:kegstandcli']}
 
 setup_kwargs = {
     'name': 'kegstandcli',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
-    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://kegstand.dev/">\n    <img src="https://kegstand.dev/assets/kegstand-logotype.png" width="540px" alt="Kegstand logo" />\n  </a>\n</p>\n\n<h3 align="center">The Developer\'s Toolbelt For Accelerating <em>Mean Time To Party</em> on AWS</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a> and fueled by a non-zero amount of alcohol</p>\n<p align="center"><a href="https://kegstand.dev/demo">Watch a 3-minute demo</a></p><!-- markdown-link-check-disable-line -->\n\n<br />\n\n## 🥂💃🕺 Welcome to the Party! 🥂💃🕺\n\nKegstand is a free and open-source framework for creating Python APIs and services. It allows you to rapidly build and deploy services on AWS. We all have better things to do than `print(json.dumps(event))` all day long, and Kegstand is here to help you get to the party &mdash; _and into Prod_ &mdash; a lot faster.\n\n**It provides:**\n\n- A CLI tool for creating and deploying your services.\n- A decorator based API abstracting away the boilerplate of Lambda, API Gateway, Cognito, and more.\n- The full power of CDK to define and deploy arbitrary AWS resources with your services.\n\n> _"Experience a streamlined cloud development process, enhanced productivity, and hit that "party" button sooner with Kegstand!"_ > **&mdash; GPT-4, official spokesbot for the Kegstand team**\n\nLearn more on the [Kegstand website](https://kegstand.dev/).\n\n## Prerequisites\n\n- [Python 3.8+](https://www.python.org/downloads/)\n- [Poetry](https://python-poetry.org/docs/#installation) (recommended)\n- An [AWS account](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)\n- The [CDK CLI configured on the local machine and initialized on the AWS account](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)\n- The AWS CLI [configured with credentials](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)\n- [Copier](https://copier.readthedocs.io/en/stable/#installation) project scaffolding tool (recommended)\n- [npx](https://docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended)\n- A well-poured [Belgian style brown ale](https://www.grimbergen.com/)\n\n## Quick start\n\nTo create a service with Kegstand, you\'ll need a Python project with a few dependencies and a folder structure following the Kegstand convention.\n\nYou can create this in a few seconds, either with the Kegstand CLI or using [Copier](https://copier.readthedocs.io/en/stable/#installation).\n\n```shell\n# Using the Kegstand CLI\n> pipx install kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier gh:JensRoland/kegstand-project-template my-service\n```\n\nEither method will create a new project folder called `my-service` containing:\n\n```shell\nmy-service\n├── .gitignore                        # Standard .gitignore file\n├── pyproject.toml                    # Project configuration\n└── src\n    └── api\n        └── resources\n            └── hello\n                └── any.py            # Logic for /hello/\n```\n\nKegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a few empty `__init__.py` gatecrashers, but we can safely ignore those.\n\nTo install the dependencies for the new project:\n\n```shell\n> cd my-service\n> poetry install\n```\n\nFinally, to build and deploy the service to AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to access the API endpoint at `https://<api-id>.execute-api.<region>.amazonaws.com/prod/hello`.\n\n## Documentation\n\nFor further examples and more advanced usage, see the [official documentation](https://github.com/JensRoland/kegstand/blob/main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on [kegstand.dev](https://kegstand.dev)\n- [ ] Custom domain names\n- [ ] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ] Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/override core API/Lambda properties such as CPU/MEM, Python runtime version, warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags in the Kegstand config and they will be applied to the generated resources\n- [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Improved output from deploy command; friendly post-deploy instructions for testing your API\n- [ ] Version bumper with [bump2version](https://pypi.org/project/bump2version/)\n- [ ] Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Unit testing helpers (wrap moto and make it all a little more DRY and intuitive)\n- [ ] Secure endpoints which require re-authentication (and/or MFA) so a refreshed token isn’t enough (to, say, delete your account or change your credit card info)\n- [ ] Live Lambda development a la SST\n- [ ] Build and deploy gRPC endpoints (or similar alternative)\n- [ ] Build and deploy GraphQL endpoints\n- [ ] Build and deploy stream processors?\n- [ ] Option to teardown before deploying: `keg deploy --force-redeploy`\n- [ ] Use env vars to populate values in kegstand.toml\n- [ ] Merge Kegstand and Beth into one tool\n- [ ] CDK Pipelines\n- [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`, etc.)\n- [ ] Upgrade Copier once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/1037) is released\n',
+    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://kegstand.dev/">\n    <img src="https://kegstand.dev/assets/kegstand-logotype.png" width="540px" alt="Kegstand logo" />\n  </a>\n</p>\n\n<h3 align="center">The Developer\'s Toolbelt For Accelerating <em>Mean Time To Party</em> on AWS</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a> and fueled by a non-zero amount of alcohol</p>\n<p align="center"><a href="https://kegstand.dev/demo">Watch a 3-minute demo</a></p><!-- markdown-link-check-disable-line -->\n\n<br />\n\n## 🥂💃🕺 Welcome to the Party! 🥂💃🕺\n\nKegstand is a free and open-source framework for creating Python APIs and services. It allows you to rapidly build and deploy services on AWS. We all have better things to do than `print(json.dumps(event))` all day long, and Kegstand is here to help you get to the party &mdash; _and into Prod_ &mdash; a lot faster.\n\n**It provides:**\n\n- A CLI tool for creating and deploying your services.\n- A decorator based API abstracting away the boilerplate of Lambda, API Gateway, Cognito, and more.\n- The full power of CDK to define and deploy arbitrary AWS resources with your services.\n\n> _"Experience a streamlined cloud development process, enhanced productivity, and hit that "party" button sooner with Kegstand!"_ > **&mdash; GPT-4, official spokesbot for the Kegstand team**\n\nLearn more on the [Kegstand website](https://kegstand.dev/).\n\n## Prerequisites\n\n- [Python 3.8+](https://www.python.org/downloads/)\n- [Poetry](https://python-poetry.org/docs/#installation) (recommended)\n- An [AWS account](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)\n- The [CDK CLI configured on the local machine and initialized on the AWS account](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)\n- The AWS CLI [configured with credentials](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)\n- [Copier](https://copier.readthedocs.io/en/stable/#installation) project scaffolding tool (recommended)\n- [npx](https://docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended)\n- A well-poured [Belgian style brown ale](https://www.grimbergen.com/)\n\n## Quick start\n\nTo create a service with Kegstand, you\'ll need a Python project with a few dependencies and a folder structure following the Kegstand convention.\n\nYou can create this in a few seconds, either with the Kegstand CLI or using [Copier](https://copier.readthedocs.io/en/stable/#installation).\n\n```shell\n# Using the Kegstand CLI\n> pipx install kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier gh:JensRoland/kegstand-project-template my-service\n```\n\nEither method will create a new project folder called `my-service` containing:\n\n```shell\nmy-service\n├── .gitignore                        # Standard .gitignore file\n├── pyproject.toml                    # Project configuration\n└── src\n    └── api\n        └── hello.py                  # Logic for /hello/\n```\n\nKegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a single, empty `__init__.py` gatecrasher, but we can safely ignore that one.\n\nTo install the dependencies for the new project:\n\n```shell\n> cd my-service\n> poetry install\n```\n\nFinally, to build and deploy the service to AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to access the API endpoint at `https://<api-id>.execute-api.<region>.amazonaws.com/prod/hello`.\n\n## Documentation\n\nFor further examples and more advanced usage, see the [official documentation](https://github.com/JensRoland/kegstand/blob/main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on [kegstand.dev](https://kegstand.dev)\n- [ ] Custom domain names\n- [X] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ] Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/override core API/Lambda properties such as CPU/MEM, Python runtime version, warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags in the Kegstand config and they will be applied to the generated resources\n- [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Improved output from deploy command; friendly post-deploy instructions for testing your API\n- [ ] Version bumper with [bump2version](https://pypi.org/project/bump2version/)\n- [ ] Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Unit testing helpers (wrap moto and make it all a little more DRY and intuitive)\n- [ ] Secure endpoints which require re-authentication (and/or MFA) so a refreshed token isn’t enough (to, say, delete your account or change your credit card info)\n- [ ] Live Lambda development a la SST\n- [ ] Build and deploy gRPC endpoints (or similar alternative)\n- [ ] Build and deploy GraphQL endpoints\n- [ ] Build and deploy stream processors?\n- [ ] Option to teardown before deploying: `keg deploy --force-redeploy`\n- [ ] Use env vars to populate values in kegstand.toml\n- [ ] Merge Kegstand and Beth into one tool\n- [ ] CDK Pipelines\n- [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`, etc.)\n- [ ] Upgrade Copier once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/1037) is released\n',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kegstand.dev',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 'src'} packages = \ ['kegstandcli', 'kegstandcli.cli', 'kegstandcli.infra',
 'kegstandcli.infra.stacks'] package_data = \ {'': ['*']} install_requires = \
 ['aws-cdk-lib>=2.67.0,<3.0.0', 'aws-solutions-constructs-aws-apigateway-
 lambda>=2.36.0,<3.0.0', 'boto3>=1.17.113,<2.0.0', 'click>=8.0.3,<9.0.0',
 'constructs>=10.0.0,<11.0.0', 'copier>=6.2.0,<7.0.0', 'pyjwt>=2.1.0,<3.0.0',
 'tomlkit>=0.11.7,<0.12.0', 'xxhash>=3.2.0,<4.0.0'] entry_points = \
 {'console_scripts': ['keg = kegstandcli.cli.__main__:kegstandcli']}
-setup_kwargs = { 'name': 'kegstandcli', 'version': '0.3.3', 'description': "The
+setup_kwargs = { 'name': 'kegstandcli', 'version': '0.3.4', 'description': "The
 Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
 'long_description': '\n
                            \n \n_[Kegstand_logo]\n\n
 \n\n
 **** The Developer\'s Toolbelt For Accelerating Mean Time To Party on AWS ****
 \n
        Created by Jens_Roland and fueled by a non-zero amount of alcohol
@@ -45,49 +45,48 @@
 CLI or using [Copier](https://copier.readthedocs.io/en/stable/
 #installation).\n\n```shell\n# Using the Kegstand CLI\n> pipx install
 kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier gh:JensRoland/
 kegstand-project-template my-service\n```\n\nEither method will create a new
 project folder called `my-service` containing:\n\n```shell\nmy-
 service\nâââ .gitignore # Standard .gitignore file\nâââ
 pyproject.toml # Project configuration\nâââ src\n âââ api\n
-âââ resources\n âââ hello\n âââ any.py # Logic for /hello/
-\n```\n\nKegstand projects are minimal by design, so a fresh project folder
-contains just those 3 files. Well, apart from a few empty `__init__.py`
-gatecrashers, but we can safely ignore those.\n\nTo install the dependencies
-for the new project:\n\n```shell\n> cd my-service\n> poetry
-install\n```\n\nFinally, to build and deploy the service to AWS:\n\n```shell\n>
-poetry run keg deploy\n```\n\nYou should now be able to access the API endpoint
-at `https://.execute-api..amazonaws.com/prod/hello`.\n\n## Documentation\n\nFor
-further examples and more advanced usage, see the [official documentation]
-(https://github.com/JensRoland/kegstand/blob/main/docs/index.md).\n\n##
-Roadmap\n\nHere are some notable changes, fixes and features that are planned
-for development:\n\n## 0.4.0\n\n- [ ] More content on [kegstand.dev](https://
-kegstand.dev)\n- [ ] Custom domain names\n- [ ] Maybe simplify the folder
-structure from `src/api/resources//.py` to `src/api/.py`\n\n### Pre-1.0.0\n\n-
-[ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB,
-Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n- [ ] [Record
-a screencast](https://asciinema.org/) for the README\n- [ ] Autogenerated docs
-using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub Actions workflow for
-pushing docs to the website\n\n### 1.0.0\n\n- [ ] Intuitive and mostly
-automated API Versioning\n- [ ] Simple way to define/override core API/Lambda
-properties such as CPU/MEM, Python runtime version, warm pool (!), and
-concurrency\n- [ ] Deploy Lambda-only microservices with no API Gateway\n\n###
-Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags in the Kegstand
-config and they will be applied to the generated resources\n- [ ] Easily add
-[AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
-layers.html)\n- [ ] Add support for APIs using [FastAPI](https://
-fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default
-Kegstand API framework, and just provide deployment helpers for the API Gateway
-and Lambda\n- [ ] Improved output from deploy command; friendly post-deploy
-instructions for testing your API\n- [ ] Version bumper with [bump2version]
-(https://pypi.org/project/bump2version/)\n- [ ] Include more goodies from
-[Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/
-2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs using pure
-[Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/
-2.11.0/) instead of the default Kegstand API framework, and just provide
+âââ hello.py # Logic for /hello/\n```\n\nKegstand projects are minimal by
+design, so a fresh project folder contains just those 3 files. Well, apart from
+a single, empty `__init__.py` gatecrasher, but we can safely ignore that
+one.\n\nTo install the dependencies for the new project:\n\n```shell\n> cd my-
+service\n> poetry install\n```\n\nFinally, to build and deploy the service to
+AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to
+access the API endpoint at `https://.execute-api..amazonaws.com/prod/
+hello`.\n\n## Documentation\n\nFor further examples and more advanced usage,
+see the [official documentation](https://github.com/JensRoland/kegstand/blob/
+main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and
+features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on
+[kegstand.dev](https://kegstand.dev)\n- [ ] Custom domain names\n- [X] Maybe
+simplify the folder structure from `src/api/resources//.py` to `src/
+api/.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions:
+S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ]
+Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the
+README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ]
+GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ]
+Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/
+override core API/Lambda properties such as CPU/MEM, Python runtime version,
+warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no
+API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags
+in the Kegstand config and they will be applied to the generated resources\n-
+[ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/
+dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI]
+(https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of
+the default Kegstand API framework, and just provide deployment helpers for the
+API Gateway and Lambda\n- [ ] Improved output from deploy command; friendly
+post-deploy instructions for testing your API\n- [ ] Version bumper with
+[bump2version](https://pypi.org/project/bump2version/)\n- [ ] Include more
+goodies from [Lambda Powertools](https://awslabs.github.io/aws-lambda-
+powertools-python/2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs
+using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-
+python/2.11.0/) instead of the default Kegstand API framework, and just provide
 deployment helpers for the API Gateway and Lambda\n- [ ] Unit testing helpers
 (wrap moto and make it all a little more DRY and intuitive)\n- [ ] Secure
 endpoints which require re-authentication (and/or MFA) so a refreshed token
 isnât enough (to, say, delete your account or change your credit card
 info)\n- [ ] Live Lambda development a la SST\n- [ ] Build and deploy gRPC
 endpoints (or similar alternative)\n- [ ] Build and deploy GraphQL endpoints\n-
 [ ] Build and deploy stream processors?\n- [ ] Option to teardown before
```

### Comparing `kegstandcli-0.3.3/PKG-INFO` & `kegstandcli-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegstandcli
-Version: 0.3.3
+Version: 0.3.4
 Summary: The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS
 Home-page: https://kegstand.dev
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -88,20 +88,18 @@
 
 ```shell
 my-service
 ├── .gitignore                        # Standard .gitignore file
 ├── pyproject.toml                    # Project configuration
 └── src
     └── api
-        └── resources
-            └── hello
-                └── any.py            # Logic for /hello/
+        └── hello.py                  # Logic for /hello/
 ```
 
-Kegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a few empty `__init__.py` gatecrashers, but we can safely ignore those.
+Kegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a single, empty `__init__.py` gatecrasher, but we can safely ignore that one.
 
 To install the dependencies for the new project:
 
 ```shell
 > cd my-service
 > poetry install
 ```
@@ -122,15 +120,15 @@
 
 Here are some notable changes, fixes and features that are planned for development:
 
 ## 0.4.0
 
 - [ ] More content on [kegstand.dev](https://kegstand.dev)
 - [ ] Custom domain names
-- [ ] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
+- [X] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
 
 ### Pre-1.0.0
 
 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.
 - [ ] Pagination helper
 - [ ] [Record a screencast](https://asciinema.org/) for the README
 - [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kegstandcli Version: 0.3.3 Summary: The Developer's
+Metadata-Version: 2.1 Name: kegstandcli Version: 0.3.4 Summary: The Developer's
 Toolbelt For Accelerating Mean-Time-To-Party on AWS Home-page: https://
 kegstand.dev License: MIT Author: JensRoland Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -49,52 +49,52 @@
 can create this in a few seconds, either with the Kegstand CLI or using
 [Copier](https://copier.readthedocs.io/en/stable/#installation). ```shell #
 Using the Kegstand CLI > pipx install kegstandcli > keg new my-service # Using
 Copier > copier gh:JensRoland/kegstand-project-template my-service ``` Either
 method will create a new project folder called `my-service` containing:
 ```shell my-service âââ .gitignore # Standard .gitignore file âââ
 pyproject.toml # Project configuration âââ src âââ api âââ
-resources âââ hello âââ any.py # Logic for /hello/ ``` Kegstand
-projects are minimal by design, so a fresh project folder contains just those 3
-files. Well, apart from a few empty `__init__.py` gatecrashers, but we can
-safely ignore those. To install the dependencies for the new project: ```shell
-> cd my-service > poetry install ``` Finally, to build and deploy the service
-to AWS: ```shell > poetry run keg deploy ``` You should now be able to access
-the API endpoint at `https://.execute-api..amazonaws.com/prod/hello`. ##
-Documentation For further examples and more advanced usage, see the [official
-documentation](https://github.com/JensRoland/kegstand/blob/main/docs/index.md).
-## Roadmap Here are some notable changes, fixes and features that are planned
-for development: ## 0.4.0 - [ ] More content on [kegstand.dev](https://
-kegstand.dev) - [ ] Custom domain names - [ ] Maybe simplify the folder
-structure from `src/api/resources//.py` to `src/api/.py` ### Pre-1.0.0 - [ ]
-Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch
-CRON scheduled events, etc. - [ ] Pagination helper - [ ] [Record a screencast]
-(https://asciinema.org/) for the README - [ ] Autogenerated docs using [MkDocs]
-(https://www.mkdocs.org/) - [ ] GitHub Actions workflow for pushing docs to the
-website ### 1.0.0 - [ ] Intuitive and mostly automated API Versioning - [ ]
-Simple way to define/override core API/Lambda properties such as CPU/MEM,
-Python runtime version, warm pool (!), and concurrency - [ ] Deploy Lambda-only
-microservices with no API Gateway ### Future - [ ] Configurable log level - [ ]
-Add AWS tags in the Kegstand config and they will be applied to the generated
-resources - [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/
-lambda/latest/dg/configuration-layers.html) - [ ] Add support for APIs using
-[FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/
+hello.py # Logic for /hello/ ``` Kegstand projects are minimal by design, so a
+fresh project folder contains just those 3 files. Well, apart from a single,
+empty `__init__.py` gatecrasher, but we can safely ignore that one. To install
+the dependencies for the new project: ```shell > cd my-service > poetry install
+``` Finally, to build and deploy the service to AWS: ```shell > poetry run keg
+deploy ``` You should now be able to access the API endpoint at `https:/
+/.execute-api..amazonaws.com/prod/hello`. ## Documentation For further examples
+and more advanced usage, see the [official documentation](https://github.com/
+JensRoland/kegstand/blob/main/docs/index.md). ## Roadmap Here are some notable
+changes, fixes and features that are planned for development: ## 0.4.0 - [ ]
+More content on [kegstand.dev](https://kegstand.dev) - [ ] Custom domain names
+- [X] Maybe simplify the folder structure from `src/api/resources//.py` to
+`src/api/.py` ### Pre-1.0.0 - [ ] Specify event triggers for Lambda functions:
+S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc. - [ ] Pagination
+helper - [ ] [Record a screencast](https://asciinema.org/) for the README - [ ]
+Autogenerated docs using [MkDocs](https://www.mkdocs.org/) - [ ] GitHub Actions
+workflow for pushing docs to the website ### 1.0.0 - [ ] Intuitive and mostly
+automated API Versioning - [ ] Simple way to define/override core API/Lambda
+properties such as CPU/MEM, Python runtime version, warm pool (!), and
+concurrency - [ ] Deploy Lambda-only microservices with no API Gateway ###
+Future - [ ] Configurable log level - [ ] Add AWS tags in the Kegstand config
+and they will be applied to the generated resources - [ ] Easily add [AWS
+Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
+layers.html) - [ ] Add support for APIs using [FastAPI](https://
+fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default
+Kegstand API framework, and just provide deployment helpers for the API Gateway
+and Lambda - [ ] Improved output from deploy command; friendly post-deploy
+instructions for testing your API - [ ] Version bumper with [bump2version]
+(https://pypi.org/project/bump2version/) - [ ] Include more goodies from
+[Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/
+2.11.0/) - tracing, metrics, etc. - [ ] Add support for APIs using pure [Lambda
+Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/
 ) instead of the default Kegstand API framework, and just provide deployment
-helpers for the API Gateway and Lambda - [ ] Improved output from deploy
-command; friendly post-deploy instructions for testing your API - [ ] Version
-bumper with [bump2version](https://pypi.org/project/bump2version/) - [ ]
-Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-
-lambda-powertools-python/2.11.0/) - tracing, metrics, etc. - [ ] Add support
-for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-
-powertools-python/2.11.0/) instead of the default Kegstand API framework, and
-just provide deployment helpers for the API Gateway and Lambda - [ ] Unit
-testing helpers (wrap moto and make it all a little more DRY and intuitive) -
-[ ] Secure endpoints which require re-authentication (and/or MFA) so a
-refreshed token isnât enough (to, say, delete your account or change your
-credit card info) - [ ] Live Lambda development a la SST - [ ] Build and deploy
-gRPC endpoints (or similar alternative) - [ ] Build and deploy GraphQL
-endpoints - [ ] Build and deploy stream processors? - [ ] Option to teardown
-before deploying: `keg deploy --force-redeploy` - [ ] Use env vars to populate
-values in kegstand.toml - [ ] Merge Kegstand and Beth into one tool - [ ] CDK
-Pipelines - [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`,
-etc.) - [ ] Upgrade Copier once the [template-deleting bugfix](https://
-github.com/copier-org/copier/pull/1037) is released
+helpers for the API Gateway and Lambda - [ ] Unit testing helpers (wrap moto
+and make it all a little more DRY and intuitive) - [ ] Secure endpoints which
+require re-authentication (and/or MFA) so a refreshed token isnât enough (to,
+say, delete your account or change your credit card info) - [ ] Live Lambda
+development a la SST - [ ] Build and deploy gRPC endpoints (or similar
+alternative) - [ ] Build and deploy GraphQL endpoints - [ ] Build and deploy
+stream processors? - [ ] Option to teardown before deploying: `keg deploy --
+force-redeploy` - [ ] Use env vars to populate values in kegstand.toml - [ ]
+Merge Kegstand and Beth into one tool - [ ] CDK Pipelines - [ ] Support HTTP
+method-specific files (e.g. `get.py`, `post.py`, etc.) - [ ] Upgrade Copier
+once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/
+1037) is released
```

