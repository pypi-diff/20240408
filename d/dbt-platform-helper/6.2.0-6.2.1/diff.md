# Comparing `tmp/dbt_platform_helper-6.2.0.tar.gz` & `tmp/dbt_platform_helper-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_platform_helper-6.2.0.tar", max compression
+gzip compressed data, was "dbt_platform_helper-6.2.1.tar", max compression
```

## Comparing `dbt_platform_helper-6.2.0.tar` & `dbt_platform_helper-6.2.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     1090 2024-03-12 15:16:39.913884 dbt_platform_helper-6.2.0/LICENSE
--rw-r--r--   0        0        0    19003 2024-04-05 09:36:23.425488 dbt_platform_helper-6.2.0/dbt_platform_helper/COMMANDS.md
--rw-r--r--   0        0        0     1762 2024-04-05 09:30:20.384763 dbt_platform_helper-6.2.0/dbt_platform_helper/README.md
--rw-r--r--   0        0        0        0 2024-03-14 13:13:32.491170 dbt_platform_helper-6.2.0/dbt_platform_helper/__init__.py
--rw-r--r--   0        0        0     3842 2024-03-14 13:13:32.492175 dbt_platform_helper-6.2.0/dbt_platform_helper/addon-plans.yml
--rw-r--r--   0        0        0     1278 2024-03-14 13:13:32.492883 dbt_platform_helper-6.2.0/dbt_platform_helper/addons-template-map.yml
--rw-r--r--   0        0        0        0 2024-03-14 13:13:32.493207 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/__init__.py
--rw-r--r--   0        0        0     9957 2024-03-14 13:13:32.494282 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/application.py
--rwxr-xr-x   0        0        0    10582 2024-03-14 13:13:32.494998 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/bootstrap.py
--rwxr-xr-x   0        0        0     3226 2024-03-14 13:13:32.495667 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/check_cloudformation.py
--rw-r--r--   0        0        0    11192 2024-03-14 13:13:32.496393 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/codebase.py
--rw-r--r--   0        0        0    12855 2024-03-14 13:13:32.497098 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/conduit.py
--rw-r--r--   0        0        0     7949 2024-03-14 13:13:32.498464 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/config.py
--rwxr-xr-x   0        0        0    14591 2024-04-05 09:30:20.385437 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/copilot.py
--rwxr-xr-x   0        0        0    35037 2024-04-05 09:30:20.385728 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/dns.py
--rw-r--r--   0        0        0     8670 2024-03-14 13:13:32.500669 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/environment.py
--rw-r--r--   0        0        0      722 2024-03-14 13:13:32.501961 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/generate.py
--rw-r--r--   0        0        0     6218 2024-03-14 13:13:32.503292 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-14 13:13:32.503639 dbt_platform_helper-6.2.0/dbt_platform_helper/custom_resources/__init__.py
--rw-r--r--   0        0        0     2396 2024-03-14 13:13:32.504820 dbt_platform_helper-6.2.0/dbt_platform_helper/custom_resources/s3_object.py
--rw-r--r--   0        0        0      346 2024-03-14 13:13:32.505501 dbt_platform_helper-6.2.0/dbt_platform_helper/default-addons.yml
--rw-r--r--   0        0        0      499 2024-03-14 13:13:32.506174 dbt_platform_helper-6.2.0/dbt_platform_helper/exceptions.py
--rw-r--r--   0        0        0      369 2024-03-14 13:13:32.507457 dbt_platform_helper-6.2.0/dbt_platform_helper/jinja2_tags.py
--rw-r--r--   0        0        0      158 2024-03-14 13:13:32.508797 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/config.yml
--rwxr-xr-x   0        0        0      164 2024-03-14 13:13:32.509606 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
--rwxr-xr-x   0        0        0      121 2024-03-14 13:13:32.510795 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/phases/build.sh
--rwxr-xr-x   0        0        0      123 2024-03-14 13:13:32.511480 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/phases/install.sh
--rwxr-xr-x   0        0        0      126 2024-03-14 13:13:32.512145 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
--rwxr-xr-x   0        0        0      125 2024-03-14 13:13:32.512941 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
--rw-r--r--   0        0        0     1081 2024-03-14 13:13:32.513655 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/COMMANDS.md.jinja
--rw-r--r--   0        0        0      622 2024-03-14 13:13:32.514385 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addon-instructions.txt
--rw-r--r--   0        0        0      412 2024-03-14 13:13:32.515427 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/README.md
--rw-r--r--   0        0        0      734 2024-03-14 13:13:32.516450 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
--rw-r--r--   0        0        0    26381 2024-03-14 13:13:32.517134 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
--rw-r--r--   0        0        0     6064 2024-03-18 09:47:04.985223 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/monitoring.yml
--rw-r--r--   0        0        0    10853 2024-04-05 09:30:20.386403 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/opensearch.yml
--rw-r--r--   0        0        0    25624 2024-03-14 13:13:32.519316 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
--rw-r--r--   0        0        0     7613 2024-04-05 09:30:20.387232 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
--rw-r--r--   0        0        0     7626 2024-03-14 13:13:32.520784 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/s3.yml
--rw-r--r--   0        0        0     3662 2024-03-14 13:13:32.521623 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/vpc.yml
--rw-r--r--   0        0        0      956 2024-03-14 13:13:32.522636 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
--rw-r--r--   0        0        0     2134 2024-03-14 13:13:32.523308 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
--rw-r--r--   0        0        0      893 2024-03-14 13:13:32.523980 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
--rw-r--r--   0        0        0     1836 2024-03-14 13:13:32.524657 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
--rw-r--r--   0        0        0      197 2024-03-14 13:13:32.525328 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/create-codebuild-role.json
--rw-r--r--   0        0        0     1180 2024-03-14 13:13:32.525988 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
--rw-r--r--   0        0        0      691 2024-03-14 13:13:32.526569 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/manifest.yml
--rw-r--r--   0        0        0      169 2024-03-14 13:13:32.527131 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/.gitignore
--rw-r--r--   0        0        0      439 2024-03-14 13:13:32.527546 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/README.md
--rw-r--r--   0        0        0      284 2024-03-14 13:13:32.528133 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
--rw-r--r--   0        0        0      339 2024-03-14 13:13:32.528741 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/cdk.json
--rw-r--r--   0        0        0     1760 2024-03-14 13:13:32.529367 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
--rw-r--r--   0        0        0   150965 2024-03-14 13:13:32.530032 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/package-lock.json
--rw-r--r--   0        0        0      534 2024-03-14 13:13:32.530472 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/package.json
--rw-r--r--   0        0        0     1906 2024-03-14 13:13:32.531017 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/stack.ts
--rw-r--r--   0        0        0      710 2024-03-14 13:13:32.531424 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
--rw-r--r--   0        0        0     1959 2024-03-14 13:13:32.532600 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
--rw-r--r--   0        0        0      169 2024-03-14 13:13:32.532763 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
--rw-r--r--   0        0        0      227 2024-03-14 13:13:32.532939 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
--rw-r--r--   0        0        0      287 2024-03-14 13:13:32.533040 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
--rw-r--r--   0        0        0      781 2024-03-14 13:13:32.533130 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
--rw-r--r--   0        0        0      339 2024-03-14 13:13:32.533332 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
--rw-r--r--   0        0        0   148134 2024-03-14 13:13:32.533676 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
--rw-r--r--   0        0        0      534 2024-03-14 13:13:32.533791 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
--rw-r--r--   0        0        0    20142 2024-03-14 13:13:32.533945 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
--rw-r--r--   0        0        0      651 2024-03-14 13:13:32.534054 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
--rw-r--r--   0        0        0     1205 2024-03-14 13:13:32.534187 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
--rw-r--r--   0        0        0     3178 2024-03-15 12:01:06.702704 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
--rw-r--r--   0        0        0     1778 2024-03-14 13:13:32.534482 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
--rw-r--r--   0        0        0      617 2024-03-14 13:13:32.534637 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
--rw-r--r--   0        0        0      741 2024-03-14 13:13:32.534954 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
--rw-r--r--   0        0        0      783 2024-03-14 13:13:32.535055 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
--rw-r--r--   0        0        0     2881 2024-03-14 13:13:32.535205 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/manifest-backend.yml
--rw-r--r--   0        0        0     3921 2024-03-14 13:13:32.535341 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/manifest-public.yml
--rw-r--r--   0        0        0      386 2024-03-14 13:13:32.535470 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
--rw-r--r--   0        0        0        0 2024-03-14 13:13:32.535503 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/__init__.py
--rw-r--r--   0        0        0     3907 2024-03-14 13:13:32.535619 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/application.py
--rw-r--r--   0        0        0    10704 2024-03-14 13:13:32.535803 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/aws.py
--rw-r--r--   0        0        0     2943 2024-03-14 13:13:32.535890 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/click.py
--rw-r--r--   0        0        0     1053 2024-03-14 13:13:32.535972 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/cloudformation.py
--rw-r--r--   0        0        0      484 2024-03-14 13:13:32.536056 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/cloudfoundry.py
--rw-r--r--   0        0        0     1720 2024-03-14 13:13:32.536141 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/files.py
--rw-r--r--   0        0        0      304 2024-03-14 13:13:32.536225 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/git.py
--rw-r--r--   0        0        0      507 2024-03-14 13:13:32.536457 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/manifests.py
--rw-r--r--   0        0        0      115 2024-03-14 13:13:32.536567 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/messages.py
--rw-r--r--   0        0        0      469 2024-03-14 13:13:32.536666 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/template.py
--rw-r--r--   0        0        0    16301 2024-04-05 09:30:20.387725 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/validation.py
--rw-r--r--   0        0        0     6408 2024-03-14 13:13:32.537042 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/versioning.py
--rwxr-xr-x   0        0        0     1936 2024-03-14 13:13:32.541196 dbt_platform_helper-6.2.0/platform_helper.py
--rw-r--r--   0        0        0     1393 2024-04-05 10:08:26.991689 dbt_platform_helper-6.2.0/pyproject.toml
--rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-6.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/LICENSE
+-rw-r--r--   0        0        0    19003 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/COMMANDS.md
+-rw-r--r--   0        0        0     1762 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/__init__.py
+-rw-r--r--   0        0        0     3842 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/addon-plans.yml
+-rw-r--r--   0        0        0     1278 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/addons-template-map.yml
+-rw-r--r--   0        0        0        0 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/__init__.py
+-rw-r--r--   0        0        0     9957 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/application.py
+-rwxr-xr-x   0        0        0    10582 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/bootstrap.py
+-rwxr-xr-x   0        0        0     3226 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/check_cloudformation.py
+-rw-r--r--   0        0        0    11192 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/codebase.py
+-rw-r--r--   0        0        0    12855 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/conduit.py
+-rw-r--r--   0        0        0     7949 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/config.py
+-rwxr-xr-x   0        0        0    14591 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/copilot.py
+-rwxr-xr-x   0        0        0    35037 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/dns.py
+-rw-r--r--   0        0        0     8670 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/environment.py
+-rw-r--r--   0        0        0      722 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/generate.py
+-rw-r--r--   0        0        0     6218 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/pipeline.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/custom_resources/__init__.py
+-rw-r--r--   0        0        0     2396 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/custom_resources/s3_object.py
+-rw-r--r--   0        0        0      346 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/default-addons.yml
+-rw-r--r--   0        0        0      499 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/exceptions.py
+-rw-r--r--   0        0        0      369 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/jinja2_tags.py
+-rw-r--r--   0        0        0      158 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/config.yml
+-rwxr-xr-x   0        0        0      164 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/image_build_run.sh
+-rwxr-xr-x   0        0        0      121 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/phases/build.sh
+-rwxr-xr-x   0        0        0      123 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/phases/install.sh
+-rwxr-xr-x   0        0        0      126 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/phases/post_build.sh
+-rwxr-xr-x   0        0        0      125 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
+-rw-r--r--   0        0        0     1081 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/COMMANDS.md.jinja
+-rw-r--r--   0        0        0      622 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addon-instructions.txt
+-rw-r--r--   0        0        0      412 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/README.md
+-rw-r--r--   0        0        0      734 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/addons.parameters.yml
+-rw-r--r--   0        0        0    26381 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
+-rw-r--r--   0        0        0     6064 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/monitoring.yml
+-rw-r--r--   0        0        0    10853 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/opensearch.yml
+-rw-r--r--   0        0        0    25624 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/rds-postgres.yml
+-rw-r--r--   0        0        0     7613 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/redis-cluster.yml
+-rw-r--r--   0        0        0     7626 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/s3.yml
+-rw-r--r--   0        0        0     3662 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/vpc.yml
+-rw-r--r--   0        0        0      956 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
+-rw-r--r--   0        0        0     2134 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/s3-policy.yml
+-rw-r--r--   0        0        0      893 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
+-rw-r--r--   0        0        0     1836 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/ci-codebuild-role-policy.json
+-rw-r--r--   0        0        0      197 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/create-codebuild-role.json
+-rw-r--r--   0        0        0     1180 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/custom-codebuild-role-policy.json
+-rw-r--r--   0        0        0      691 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/manifest.yml
+-rw-r--r--   0        0        0      169 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/.gitignore
+-rw-r--r--   0        0        0      439 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/README.md
+-rw-r--r--   0        0        0      284 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/bin/override.ts
+-rw-r--r--   0        0        0      339 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/cdk.json
+-rw-r--r--   0        0        0     1760 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
+-rw-r--r--   0        0        0   150965 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/package-lock.json
+-rw-r--r--   0        0        0      534 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/package.json
+-rw-r--r--   0        0        0     1906 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/stack.ts
+-rw-r--r--   0        0        0      710 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/tsconfig.json
+-rw-r--r--   0        0        0     1959 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
+-rw-r--r--   0        0        0      169 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
+-rw-r--r--   0        0        0      227 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
+-rw-r--r--   0        0        0      287 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
+-rw-r--r--   0        0        0      781 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
+-rw-r--r--   0        0        0      339 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
+-rw-r--r--   0        0        0   148134 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
+-rw-r--r--   0        0        0      534 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
+-rw-r--r--   0        0        0    20142 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
+-rw-r--r--   0        0        0      651 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
+-rw-r--r--   0        0        0     1205 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
+-rw-r--r--   0        0        0     3178 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
+-rw-r--r--   0        0        0     1778 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/manifest.yml
+-rw-r--r--   0        0        0      617 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0      741 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/maintenance_pages/default.html
+-rw-r--r--   0        0        0      783 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
+-rw-r--r--   0        0        0     2881 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/manifest-backend.yml
+-rw-r--r--   0        0        0     3921 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/manifest-public.yml
+-rw-r--r--   0        0        0      386 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0        0 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/__init__.py
+-rw-r--r--   0        0        0     3907 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/application.py
+-rw-r--r--   0        0        0    10704 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/aws.py
+-rw-r--r--   0        0        0     2943 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/click.py
+-rw-r--r--   0        0        0     1053 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/cloudformation.py
+-rw-r--r--   0        0        0      484 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/cloudfoundry.py
+-rw-r--r--   0        0        0     1720 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/files.py
+-rw-r--r--   0        0        0      304 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/git.py
+-rw-r--r--   0        0        0      507 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/manifests.py
+-rw-r--r--   0        0        0      115 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/messages.py
+-rw-r--r--   0        0        0      469 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/template.py
+-rw-r--r--   0        0        0    16301 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/validation.py
+-rw-r--r--   0        0        0     6408 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/versioning.py
+-rwxr-xr-x   0        0        0     1936 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/platform_helper.py
+-rw-r--r--   0        0        0     1393 2024-04-08 10:54:29.307222 dbt_platform_helper-6.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-6.2.1/PKG-INFO
```

### Comparing `dbt_platform_helper-6.2.0/LICENSE` & `dbt_platform_helper-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/COMMANDS.md` & `dbt_platform_helper-6.2.1/dbt_platform_helper/COMMANDS.md`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/README.md` & `dbt_platform_helper-6.2.1/dbt_platform_helper/README.md`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/addon-plans.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/addon-plans.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/addons-template-map.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/addons-template-map.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/application.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/bootstrap.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/check_cloudformation.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/check_cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/codebase.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/codebase.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/conduit.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/conduit.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/config.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/config.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/copilot.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/copilot.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/dns.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/dns.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/environment.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/environment.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/generate.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/generate.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/pipeline.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/pipeline.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/custom_resources/s3_object.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/custom_resources/s3_object.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/COMMANDS.md.jinja` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/COMMANDS.md.jinja`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addon-instructions.txt` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addon-instructions.txt`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/addons.parameters.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/aurora-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/monitoring.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/monitoring.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/opensearch.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/opensearch.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/rds-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/redis-cluster.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/s3.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/s3.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/vpc.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/vpc.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/s3-policy.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/subscription-filter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/ci-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/custom-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/manifest.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/log_resource_policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/package-lock.json` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/package.json` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/stack.ts` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/tsconfig.json` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/buildspec.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/maintenance_pages/default.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/maintenance_pages/migration.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/manifest-backend.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/manifest-backend.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/manifest-public.yml` & `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/manifest-public.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/application.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/aws.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/aws.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/click.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/click.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/cloudformation.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/files.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/files.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/validation.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/validation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/versioning.py` & `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/platform_helper.py` & `dbt_platform_helper-6.2.1/platform_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.0/pyproject.toml` & `dbt_platform_helper-6.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "dbt-platform-helper"
-version = "6.2.0"
+version = "6.2.1"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "dbt_platform_helper/README.md"
 packages = [
     { include = "dbt_platform_helper" },
     { include = "platform_helper.py" }
```

### Comparing `dbt_platform_helper-6.2.0/PKG-INFO` & `dbt_platform_helper-6.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-platform-helper
-Version: 6.2.0
+Version: 6.2.1
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

