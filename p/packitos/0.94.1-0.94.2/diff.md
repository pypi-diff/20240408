# Comparing `tmp/packitos-0.94.1.tar.gz` & `tmp/packitos-0.94.2.tar.gz`

## Comparing `packitos-0.94.1.tar` & `packitos-0.94.2.tar`

### file list

```diff
@@ -1,407 +1,408 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 packitos-0.94.1/.git_archival.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 packitos-0.94.1/.gitattributes
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 packitos-0.94.1/.packit.yaml
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 packitos-0.94.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 packitos-0.94.1/.zuul.yaml
--rw-r--r--   0        0        0    56412 2020-02-02 00:00:00.000000 packitos-0.94.1/CHANGELOG.md
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 packitos-0.94.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 packitos-0.94.1/Containerfile
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 packitos-0.94.1/Containerfile.tests
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 packitos-0.94.1/DCO
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 packitos-0.94.1/LICENSE_HEADER.txt
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 packitos-0.94.1/Makefile
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 packitos-0.94.1/ansible.cfg
--rw-r--r--   0        0        0    13168 2020-02-02 00:00:00.000000 packitos-0.94.1/packit.spec
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 packitos-0.94.1/release-conf.yaml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 packitos-0.94.1/.fmf/version
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 packitos-0.94.1/.github/stale.yml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 packitos-0.94.1/.github/workflows/build-and-push.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 packitos-0.94.1/.github/workflows/check-release-notes.yml
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 packitos-0.94.1/.github/workflows/do_release.yml
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 packitos-0.94.1/.github/workflows/opened-issues-to-the-board.yml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 packitos-0.94.1/.github/workflows/prepare-release.yml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 packitos-0.94.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0  1843517 2020-02-02 00:00:00.000000 packitos-0.94.1/design/logo-packit.sketch
--rw-r--r--   0        0        0   135444 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/hexsticker.png
--rw-r--r--   0        0        0   132230 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-dark.png
--rw-r--r--   0        0        0    75002 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-extended.jpg
--rw-r--r--   0        0        0    48468 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-extended.png
--rw-r--r--   0        0        0    24881 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-extended.svg
--rw-r--r--   0        0        0   106567 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-guideline.pdf
--rw-r--r--   0        0        0    66141 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-no-borders.jpg
--rw-r--r--   0        0        0   143587 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-no-borders.png
--rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-small.png
--rw-r--r--   0        0        0    70268 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-square-small-borders.jpg
--rw-r--r--   0        0        0   150044 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-square-small-borders.png
--rw-r--r--   0        0        0    43972 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-stg-square-bigger-borders.svg
--rw-r--r--   0        0        0   107242 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-stg-square-small-borders.png
--rw-r--r--   0        0        0    43981 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-stg-square-small-borders.svg
--rw-r--r--   0        0        0    28826 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-stg.png
--rw-r--r--   0        0        0    24351 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-stg.svg
--rw-r--r--   0        0        0    18005 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-text.jpg
--rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-text.png
--rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-text.svg
--rw-r--r--   0        0        0   144552 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo-white.png
--rw-r--r--   0        0        0   158074 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo.png
--rw-r--r--   0        0        0    14697 2020-02-02 00:00:00.000000 packitos-0.94.1/design/export/logo.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 packitos-0.94.1/files/install-requirements-git.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 packitos-0.94.1/files/install-requirements-pip.yaml
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 packitos-0.94.1/files/install-requirements-rpms.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 packitos-0.94.1/files/local-tests-requirements.yaml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 packitos-0.94.1/files/packit-testing-farm-prepare-session-recording.yaml
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 packitos-0.94.1/files/packit-testing-farm-prepare.yaml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 packitos-0.94.1/files/zuul-reverse-dep-packit-service.yaml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.94.1/files/zuul-tests-session-recording.yaml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 packitos-0.94.1/files/zuul-tests.yaml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 packitos-0.94.1/files/bash-completion/packit
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/build-rpm-deps.yaml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/centpkg.yaml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/generic-dnf-requirements.yaml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/install-packit-service.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/install-packit.yaml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/ogr.yaml
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/packit-service-requirements.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/project-dir.yaml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/python-compile-deps.yaml
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/requre.yaml
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/rpm-test-deps.yaml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/sandcastle.yaml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 packitos-0.94.1/files/tasks/specfile.yaml
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/actions.py
--rw-r--r--   0        0        0    90699 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/api.py
--rw-r--r--   0        0        0    29435 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/base_git.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/command_handler.py
--rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/constants.py
--rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/copr_helper.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/dist_git_instance.py
--rw-r--r--   0        0        0    25019 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/distgit.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/exceptions.py
--rw-r--r--   0        0        0    40197 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/local_project.py
--rw-r--r--   0        0        0    35127 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/patches.py
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/pkgtool.py
--rw-r--r--   0        0        0    29471 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/schema.py
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/security.py
--rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/source_git.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/status.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/sync.py
--rw-r--r--   0        0        0    53439 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/upstream.py
--rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/vm_image_build.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/build.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/create_update.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/dist_git.py
--rw-r--r--   0        0        0    14719 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/dist_git_init.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/init.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/packit_base.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/prepare_sources.py
--rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/propose_downstream.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/push_updates.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/source_git.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/source_git_init.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/source_git_status.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/srpm.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/status.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/sync_from_downstream.py
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/types.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/update_dist_git.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/update_source_git.py
--rw-r--r--   0        0        0    13599 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/utils.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/validate_config.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/builds/__init__.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/builds/copr_build.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/builds/in_image_builder.py
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/builds/koji_build.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/builds/local_build.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/cli/builds/mock_build.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/config/__init__.py
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/config/aliases.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/config/commands.py
--rw-r--r--   0        0        0    24627 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/config/common_package_config.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/config/config.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/config/job_config.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/config/notifications.py
--rw-r--r--   0        0        0    19422 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/config/package_config.py
--rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/config/package_config_validator.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/config/requirements.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/config/sources.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/data/__init__.py
--rwxr-xr-x   0        0        0     3233 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/data/_packitpatch
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/bodhi.py
--rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/changelog_helper.py
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/commands.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/decorators.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/extensions.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/koji_helper.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/logging.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/lookaside.py
--rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/repo.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/source_script.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/upstream_version.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 packitos-0.94.1/packit/utils/versions.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 packitos-0.94.1/plans/README.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 packitos-0.94.1/plans/full.fmf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.94.1/plans/git_reference.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.94.1/plans/main.fmf
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.94.1/plans/rpmlint.fmf
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 packitos-0.94.1/plans/session-recording.fmf
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 packitos-0.94.1/plans/smoke.fmf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/__init__.py
--rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/conftest.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/full.fmf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/smoke.fmf
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/smoke.sh
--rw-r--r--   0        0        0    22298 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/spellbook.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/copr_config
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/cockpit-ostree/Makefile
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/cockpit-ostree/cockpit-ostree.spec.dg
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/cockpit-ostree/cockpit-ostree.spec.in
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/cockpit-ostree/packit.yaml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/cronie/.cronie.metadata
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/cronie/.gitignore
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/cronie/SOURCES/cronie-1.5.2-restart-on-failure.patch
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/cronie/SOURCES/fix-memory-leaks.patch
--rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/cronie/SOURCES/fix-unsafe-code.patch
--rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/cronie/SPECS/cronie.spec
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/dg-ogr/.packit.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/dg-ogr/README.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/dg-ogr/README.packit
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/dg-ogr/python-ogr.spec
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/dg-ogr/sources
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/dist_git/.packit.yaml
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/dist_git/beer.spec
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/dist_git_with_autochangelog/.packit.yaml
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/dist_git_with_autochangelog/beer.spec
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/edd/.packit.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/edd/LICENSE
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/edd/Makefile
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/edd/README.rst
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/edd/edd
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/edd/edd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/edd/docs/man.rst
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/empty_changelog/.packit.yaml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/empty_changelog/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/no_version_tag_in_spec/.packit.yaml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/no_version_tag_in_spec/beer.spec
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/no_version_tag_in_spec/source
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/osbuild/.packit.yaml
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/osbuild/__init__.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/osbuild/osbuild.spec
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/osbuild/setup.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/osbuild/sources/test
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/previous/git-diff.patch
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/previous/missing-diff-line.patch
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/previous/unified-diff.patch
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/previous/weird-identical.patch
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/regenerated/git-diff.patch
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/regenerated/missing-diff-line.patch
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/regenerated/unified-diff.patch
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/regenerated/weird-identical.patch
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/rpms/hello/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/rpms/hello/hello.spec
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/src/hello/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/src/hello/.distro/hello.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/patches/src/hello/.distro/source-git.yaml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/rpms/hello/0017-Patch-This..patch
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/rpms/hello/from-git.patch
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/rpms/hello/hello.spec
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/rpms/hello/sources
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/rpms/hello/turn-into-fedora.patch
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/snapd/.packit.yaml
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/snapd/packaging/fedora/fix-spec
--rwxr-xr-x   0        0        0     1866 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/snapd/packaging/fedora/pack-source
--rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/snapd/packaging/fedora/snapd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/snapd/packaging/fedora/some-file-to-add
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/snapd/vendor/vendor.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/sourcegit/source_git/ignored_file.txt
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/sourcegit/source_git/.distro/beer.spec
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/sourcegit/source_git/.distro/source-git.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/sourcegit/upstream/big-source-file.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/spec_not_in_root/upstream/.packit.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/spec_not_in_root/upstream/dir_with_spec/beer.spec
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/src/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/src/hello/Makefile
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/src/hello/README.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/src/hello/hello.rs
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/sync_files/a.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/sync_files/b.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/sync_files/c.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/sync_files/example_dir/d.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/sync_files/example_dir/e.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/sync_files/example_dir/f.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/upstream_git/.packit.yaml
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/upstream_git/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/upstream_git_macro_in_source/.packit.yaml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/upstream_git_macro_in_source/beer.spec
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/upstream_git_weird_sources/.packit.yaml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/upstream_git_weird_sources/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/upstream_git_with_multiple_sources/.packit.yaml
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/upstream_git_with_multiple_sources/beer.spec
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/.packit.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/AUDIT
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/BENCHMARKS
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/BUGS
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/COPYING
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/Changelog
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/FAQ
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/INSTALL
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/README
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/README.security
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/REWARD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/SIZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/SPEED
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/TODO
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/TUNING
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/vsftpd.8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/vsftpd.conf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/vsftpd.conf.5
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/EXAMPLE/example
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/Fedora/vsftpd-generator
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/Fedora/vsftpd.ftpusers
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/Fedora/vsftpd.pam
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/Fedora/vsftpd.service
--rw-r--r--   0        0        0    27817 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/Fedora/vsftpd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/Fedora/vsftpd.target
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/Fedora/vsftpd.user_list
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/Fedora/vsftpd.xinetd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/Fedora/vsftpd@.service
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/Fedora/vsftpd_conf_migrate.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/RedHat/vsftpd.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/data/vsftpd/SECURITY/security
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/functional/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/functional/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/functional/spellbook.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/functional/test_local_build.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/functional/test_prepare_sources.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/functional/test_srpm.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/functional/test_validate_config.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/README.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/bodhi_latest_builds.py
--rw-r--r--   0        0        0    42198 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/bodhi_status_updates.py
--rw-r--r--   0        0        0    15059 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/conftest.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_actions.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_api.py
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_base_git.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_build.py
--rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_changelog_helper.py
--rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_copr_build.py
--rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_create_update.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_distgit.py
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_get_api.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_init.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_local_project.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_pagure.py
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_patches.py
--rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_push_updates.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_security.py
--rw-r--r--   0        0        0    24135 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_source_git.py
--rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_source_git_init.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_source_git_status.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_source_git_synch_push.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_source_git_update_source_git.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_spec.py
--rw-r--r--   0        0        0    18153 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_update.py
--rw-r--r--   0        0        0    20720 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_upstream.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_using_cockpit.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_using_examples.py
--rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_validate_config.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/test_validate_synced_files.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/integration/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/conftest.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_actions.py
--rw-r--r--   0        0        0    19749 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_api.py
--rw-r--r--   0        0        0    34220 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_base_git.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_cli.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_cli_utils.py
--rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_copr_helper.py
--rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_dg.py
--rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_dist_git_init.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_image_builder.py
--rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_iterate_packages.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_koji_build.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_load_authentication.py
--rw-r--r--   0        0        0    34254 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_local_project.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_login_with_kerberos.py
--rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_patches.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_prepare_sources.py
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_propose_downstream.py
--rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_security.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_specfile.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_status.py
--rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_sync.py
--rw-r--r--   0        0        0    19993 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_upstream.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/test_utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/config/__init__.py
--rw-r--r--   0        0        0    22698 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/config/test_config.py
--rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/config/test_config_aliases.py
--rw-r--r--   0        0        0    94771 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/config/test_package_config.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/test_changelog_helper.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/test_commands.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/test_decorators.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/test_dist_git_instance.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/test_exceptions.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/test_koji_helper.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/test_lookaside.py
--rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/test_repo.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/test_source_script.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/test_upstream_version.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 packitos-0.94.1/tests/unit/utils/test_versions.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/main.fmf
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_api.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_base_git.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_image_builder.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_local_project.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_repository_cache.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_status.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/testbase.py
--rw-r--r--   0        0        0   513530 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml
--rw-r--r--   0        0        0    53824 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz
--rw-r--r--   0        0        0  1387468 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz
--rw-r--r--   0        0        0   162050 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.packit-dist-gitfnk035np_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0  1425896 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    86697 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml
--rw-r--r--   0        0        0    64940 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.tmp5bwaoc9m_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml
--rw-r--r--   0        0        0    34569 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr_no_merge.yaml
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone2_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0  2668265 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml.tmpgtdjxv_x_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    43243 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.packit-dist-gitzea090jp_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.tmpv3zw6n9v_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0   155977 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.packit-dist-gitl12hm88e_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.tmpyqn3l5sr_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0   152944 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml.tmp9u1xyoyx_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    40654 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_status.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_status.yaml.tmp620nfd0i_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    70501 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml.tmpco60quxn_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.94.1/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 packitos-0.94.1/LICENSE
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 packitos-0.94.1/README.md
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 packitos-0.94.1/pyproject.toml
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 packitos-0.94.1/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 packitos-0.94.2/.git_archival.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 packitos-0.94.2/.gitattributes
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 packitos-0.94.2/.packit.yaml
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 packitos-0.94.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 packitos-0.94.2/.zuul.yaml
+-rw-r--r--   0        0        0    56867 2020-02-02 00:00:00.000000 packitos-0.94.2/CHANGELOG.md
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 packitos-0.94.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 packitos-0.94.2/Containerfile
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 packitos-0.94.2/Containerfile.tests
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 packitos-0.94.2/DCO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 packitos-0.94.2/LICENSE_HEADER.txt
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 packitos-0.94.2/Makefile
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 packitos-0.94.2/ansible.cfg
+-rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 packitos-0.94.2/packit.spec
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 packitos-0.94.2/release-conf.yaml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 packitos-0.94.2/.fmf/version
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/stale.yml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/build-and-push.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/check-release-notes.yml
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/do_release.yml
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/opened-issues-to-the-board.yml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/prepare-release.yml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 packitos-0.94.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0  1843517 2020-02-02 00:00:00.000000 packitos-0.94.2/design/logo-packit.sketch
+-rw-r--r--   0        0        0   135444 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/hexsticker.png
+-rw-r--r--   0        0        0   132230 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-dark.png
+-rw-r--r--   0        0        0    75002 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-extended.jpg
+-rw-r--r--   0        0        0    48468 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-extended.png
+-rw-r--r--   0        0        0    24881 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-extended.svg
+-rw-r--r--   0        0        0   106567 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-guideline.pdf
+-rw-r--r--   0        0        0    66141 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-no-borders.jpg
+-rw-r--r--   0        0        0   143587 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-no-borders.png
+-rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-small.png
+-rw-r--r--   0        0        0    70268 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-square-small-borders.jpg
+-rw-r--r--   0        0        0   150044 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-square-small-borders.png
+-rw-r--r--   0        0        0    43972 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-stg-square-bigger-borders.svg
+-rw-r--r--   0        0        0   107242 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-stg-square-small-borders.png
+-rw-r--r--   0        0        0    43981 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-stg-square-small-borders.svg
+-rw-r--r--   0        0        0    28826 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-stg.png
+-rw-r--r--   0        0        0    24351 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-stg.svg
+-rw-r--r--   0        0        0    18005 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-text.jpg
+-rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-text.png
+-rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-text.svg
+-rw-r--r--   0        0        0   144552 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo-white.png
+-rw-r--r--   0        0        0   158074 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo.png
+-rw-r--r--   0        0        0    14697 2020-02-02 00:00:00.000000 packitos-0.94.2/design/export/logo.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 packitos-0.94.2/files/install-requirements-git.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 packitos-0.94.2/files/install-requirements-pip.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 packitos-0.94.2/files/install-requirements-rpms.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 packitos-0.94.2/files/local-tests-requirements.yaml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 packitos-0.94.2/files/packit-testing-farm-prepare-session-recording.yaml
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 packitos-0.94.2/files/packit-testing-farm-prepare.yaml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 packitos-0.94.2/files/zuul-reverse-dep-packit-service.yaml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.94.2/files/zuul-tests-session-recording.yaml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 packitos-0.94.2/files/zuul-tests.yaml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 packitos-0.94.2/files/bash-completion/packit
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/build-rpm-deps.yaml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/centpkg.yaml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/generic-dnf-requirements.yaml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/install-packit-service.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/install-packit.yaml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/ogr.yaml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/packit-service-requirements.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/project-dir.yaml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/python-compile-deps.yaml
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/requre.yaml
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/rpm-test-deps.yaml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/sandcastle.yaml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 packitos-0.94.2/files/tasks/specfile.yaml
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/actions.py
+-rw-r--r--   0        0        0    90697 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/api.py
+-rw-r--r--   0        0        0    29435 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/base_git.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/command_handler.py
+-rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/constants.py
+-rw-r--r--   0        0        0    20419 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/copr_helper.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/dist_git_instance.py
+-rw-r--r--   0        0        0    25019 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/distgit.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/exceptions.py
+-rw-r--r--   0        0        0    40197 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/local_project.py
+-rw-r--r--   0        0        0    35127 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/patches.py
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/pkgtool.py
+-rw-r--r--   0        0        0    29471 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/schema.py
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/security.py
+-rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/source_git.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/status.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/sync.py
+-rw-r--r--   0        0        0    53439 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/upstream.py
+-rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/vm_image_build.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/build.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/create_update.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/dist_git.py
+-rw-r--r--   0        0        0    14719 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/dist_git_init.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/init.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/packit_base.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/prepare_sources.py
+-rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/propose_downstream.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/push_updates.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/source_git.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/source_git_init.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/source_git_status.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/srpm.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/status.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/sync_from_downstream.py
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/types.py
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/update_dist_git.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/update_source_git.py
+-rw-r--r--   0        0        0    13599 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/utils.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/validate_config.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/__init__.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/copr_build.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/in_image_builder.py
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/koji_build.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/local_build.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/cli/builds/mock_build.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/__init__.py
+-rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/aliases.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/commands.py
+-rw-r--r--   0        0        0    24627 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/common_package_config.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/config.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/job_config.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/notifications.py
+-rw-r--r--   0        0        0    19422 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/package_config.py
+-rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/package_config_validator.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/requirements.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/config/sources.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/data/__init__.py
+-rwxr-xr-x   0        0        0     3233 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/data/_packitpatch
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/bodhi.py
+-rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/changelog_helper.py
+-rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/commands.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/decorators.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/extensions.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/koji_helper.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/logging.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/lookaside.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/monitoring.py
+-rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/repo.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/source_script.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/upstream_version.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 packitos-0.94.2/packit/utils/versions.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/README.md
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/full.fmf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/git_reference.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/main.fmf
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/rpmlint.fmf
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/session-recording.fmf
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 packitos-0.94.2/plans/smoke.fmf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/__init__.py
+-rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/conftest.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/full.fmf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/smoke.fmf
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/smoke.sh
+-rw-r--r--   0        0        0    22298 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/spellbook.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/copr_config
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cockpit-ostree/Makefile
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cockpit-ostree/cockpit-ostree.spec.dg
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cockpit-ostree/cockpit-ostree.spec.in
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cockpit-ostree/packit.yaml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/.cronie.metadata
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/.gitignore
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/SOURCES/cronie-1.5.2-restart-on-failure.patch
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/SOURCES/fix-memory-leaks.patch
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/SOURCES/fix-unsafe-code.patch
+-rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/cronie/SPECS/cronie.spec
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dg-ogr/.packit.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dg-ogr/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dg-ogr/README.packit
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dg-ogr/python-ogr.spec
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dg-ogr/sources
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dist_git/.packit.yaml
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dist_git/beer.spec
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dist_git_with_autochangelog/.packit.yaml
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/dist_git_with_autochangelog/beer.spec
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/.packit.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/LICENSE
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/Makefile
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/README.rst
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/edd
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/edd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/edd/docs/man.rst
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/empty_changelog/.packit.yaml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/empty_changelog/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/no_version_tag_in_spec/.packit.yaml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/no_version_tag_in_spec/beer.spec
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/no_version_tag_in_spec/source
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/osbuild/.packit.yaml
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/osbuild/__init__.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/osbuild/osbuild.spec
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/osbuild/setup.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/osbuild/sources/test
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/previous/git-diff.patch
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/previous/missing-diff-line.patch
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/previous/unified-diff.patch
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/previous/weird-identical.patch
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/regenerated/git-diff.patch
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/regenerated/missing-diff-line.patch
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/regenerated/unified-diff.patch
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/regenerated/weird-identical.patch
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/rpms/hello/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/rpms/hello/hello.spec
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/src/hello/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/src/hello/.distro/hello.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/patches/src/hello/.distro/source-git.yaml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/rpms/hello/0017-Patch-This..patch
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/rpms/hello/from-git.patch
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/rpms/hello/hello.spec
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/rpms/hello/sources
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/rpms/hello/turn-into-fedora.patch
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/.packit.yaml
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/packaging/fedora/fix-spec
+-rwxr-xr-x   0        0        0     1866 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/packaging/fedora/pack-source
+-rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/packaging/fedora/snapd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/packaging/fedora/some-file-to-add
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/snapd/vendor/vendor.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sourcegit/source_git/ignored_file.txt
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sourcegit/source_git/.distro/beer.spec
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sourcegit/source_git/.distro/source-git.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sourcegit/upstream/big-source-file.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/spec_not_in_root/upstream/.packit.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/spec_not_in_root/upstream/dir_with_spec/beer.spec
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/src/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/src/hello/Makefile
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/src/hello/README.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/src/hello/hello.rs
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/a.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/b.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/c.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/example_dir/d.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/example_dir/e.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/sync_files/example_dir/f.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git/.packit.yaml
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_macro_in_source/.packit.yaml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_macro_in_source/beer.spec
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_weird_sources/.packit.yaml
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_weird_sources/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_with_multiple_sources/.packit.yaml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/upstream_git_with_multiple_sources/beer.spec
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/.packit.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/AUDIT
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/BENCHMARKS
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/BUGS
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/COPYING
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Changelog
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/FAQ
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/INSTALL
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/README
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/README.security
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/REWARD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/SIZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/SPEED
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/TODO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/TUNING
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/vsftpd.8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/vsftpd.conf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/vsftpd.conf.5
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/EXAMPLE/example
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd-generator
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.ftpusers
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.pam
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.service
+-rw-r--r--   0        0        0    27817 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.target
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.user_list
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.xinetd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd@.service
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd_conf_migrate.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/RedHat/vsftpd.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/data/vsftpd/SECURITY/security
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/spellbook.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/test_local_build.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/test_prepare_sources.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/test_srpm.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/functional/test_validate_config.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/README.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/bodhi_latest_builds.py
+-rw-r--r--   0        0        0    42198 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/bodhi_status_updates.py
+-rw-r--r--   0        0        0    15059 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_actions.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_api.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_base_git.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_build.py
+-rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_changelog_helper.py
+-rw-r--r--   0        0        0    21951 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_copr_build.py
+-rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_create_update.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_distgit.py
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_get_api.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_init.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_local_project.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_pagure.py
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_patches.py
+-rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_push_updates.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_security.py
+-rw-r--r--   0        0        0    24135 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_source_git.py
+-rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_source_git_init.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_source_git_status.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_source_git_synch_push.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_source_git_update_source_git.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_spec.py
+-rw-r--r--   0        0        0    18153 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_update.py
+-rw-r--r--   0        0        0    20720 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_upstream.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_using_cockpit.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_using_examples.py
+-rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_validate_config.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/test_validate_synced_files.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/integration/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/conftest.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_actions.py
+-rw-r--r--   0        0        0    20019 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_api.py
+-rw-r--r--   0        0        0    34220 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_base_git.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_cli.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_cli_utils.py
+-rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_copr_helper.py
+-rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_dg.py
+-rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_dist_git_init.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_image_builder.py
+-rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_iterate_packages.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_koji_build.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_load_authentication.py
+-rw-r--r--   0        0        0    34254 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_local_project.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_login_with_kerberos.py
+-rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_patches.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_prepare_sources.py
+-rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_propose_downstream.py
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_security.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_specfile.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_status.py
+-rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_sync.py
+-rw-r--r--   0        0        0    19993 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_upstream.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/test_utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/config/__init__.py
+-rw-r--r--   0        0        0    22698 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/config/test_config.py
+-rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/config/test_config_aliases.py
+-rw-r--r--   0        0        0    94771 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/config/test_package_config.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_changelog_helper.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_commands.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_decorators.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_dist_git_instance.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_exceptions.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_koji_helper.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_lookaside.py
+-rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_repo.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_source_script.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_upstream_version.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 packitos-0.94.2/tests/unit/utils/test_versions.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/main.fmf
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_api.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_base_git.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_image_builder.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_local_project.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_repository_cache.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_status.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/testbase.py
+-rw-r--r--   0        0        0   513530 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml
+-rw-r--r--   0        0        0    53824 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz
+-rw-r--r--   0        0        0  1387468 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz
+-rw-r--r--   0        0        0   162050 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.packit-dist-gitfnk035np_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0  1425896 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    86697 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml
+-rw-r--r--   0        0        0    64940 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.tmp5bwaoc9m_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml
+-rw-r--r--   0        0        0    34569 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr_no_merge.yaml
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone2_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0  2668265 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml.tmpgtdjxv_x_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    43243 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.packit-dist-gitzea090jp_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.tmpv3zw6n9v_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0   155977 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.packit-dist-gitl12hm88e_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.tmpyqn3l5sr_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0   152944 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml.tmp9u1xyoyx_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    40654 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_status.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_status.yaml.tmp620nfd0i_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    70501 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml.tmpco60quxn_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.94.2/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 packitos-0.94.2/LICENSE
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 packitos-0.94.2/README.md
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 packitos-0.94.2/pyproject.toml
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 packitos-0.94.2/PKG-INFO
```

### Comparing `packitos-0.94.1/.packit.yaml` & `packitos-0.94.2/.packit.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/.pre-commit-config.yaml` & `packitos-0.94.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/.zuul.yaml` & `packitos-0.94.2/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/CHANGELOG.md` & `packitos-0.94.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# 0.94.2
+
+- Packit previously put the "[packit]" string as a prefix in the subject of pull-from-upstream commits. Now the prefix is no longer there - this is made unnecessary noise in autochangelog. This affects the default. Custom action can still override this behavior. (#2263)
+- We have fixed a race condition that could occur when multiple `copr_build` jobs sharing a Copr project but having different targets were running at the same time. (#2274)
+
 # 0.94.1
 
 - `packit validate-config` now checks whether `upstream_project_url` is set if `pull_from_upstream` job is configured. (#2254)
 - `Resolves` is changed to `Resolves:` for the dist-git commit since that's the correct format for CentOS Stream 9. (#2260)
 
 # 0.94.0
```

### Comparing `packitos-0.94.1/CONTRIBUTING.md` & `packitos-0.94.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/DCO` & `packitos-0.94.2/DCO`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/Makefile` & `packitos-0.94.2/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit.spec` & `packitos-0.94.2/packit.spec`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 %if 0%{?el9}
 %bcond_with tests
 %else
 %bcond_without tests
 %endif
 
 Name:           packit
-Version:        0.94.1
+Version:        0.94.2
 Release:        1%{?dist}
 Summary:        A tool for integrating upstream projects with Fedora operating system
 
 License:        MIT
 URL:            https://github.com/packit/packit
 Source0:        %{pypi_source packitos}
 BuildArch:      noarch
@@ -73,14 +73,17 @@
 # Epel9 does not tag the license file in pyproject_files as a license. Manually install it in this case
 %if 0%{?el9}
 %license LICENSE
 %endif
 %doc README.md
 
 %changelog
+* Mon Apr 08 2024 Packit Team <hello@packit.dev> - 0.94.2-1
+- New upstream release 0.94.2
+
 * Mon Mar 25 2024 Packit Team <hello@packit.dev> - 0.94.1-1
 - New upstream release 0.94.1
 
 * Sun Mar 17 2024 Packit Team <hello@packit.dev> - 0.94.0-1
 - New upstream release 0.94.0
 
 * Mon Feb 26 2024 Packit Team <hello@packit.dev> - 0.93.0-1
```

### Comparing `packitos-0.94.1/.github/stale.yml` & `packitos-0.94.2/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/.github/workflows/build-and-push.yml` & `packitos-0.94.2/.github/workflows/build-and-push.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/.github/workflows/do_release.yml` & `packitos-0.94.2/.github/workflows/do_release.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/.github/workflows/prepare-release.yml` & `packitos-0.94.2/.github/workflows/prepare-release.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/.github/workflows/pypi-publish.yml` & `packitos-0.94.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/logo-packit.sketch` & `packitos-0.94.2/design/logo-packit.sketch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/hexsticker.png` & `packitos-0.94.2/design/export/hexsticker.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-dark.png` & `packitos-0.94.2/design/export/logo-dark.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-extended.jpg` & `packitos-0.94.2/design/export/logo-extended.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-extended.png` & `packitos-0.94.2/design/export/logo-extended.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-extended.svg` & `packitos-0.94.2/design/export/logo-extended.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-guideline.pdf` & `packitos-0.94.2/design/export/logo-guideline.pdf`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-no-borders.jpg` & `packitos-0.94.2/design/export/logo-no-borders.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-no-borders.png` & `packitos-0.94.2/design/export/logo-no-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-small.png` & `packitos-0.94.2/design/export/logo-small.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-square-small-borders.jpg` & `packitos-0.94.2/design/export/logo-square-small-borders.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-square-small-borders.png` & `packitos-0.94.2/design/export/logo-square-small-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-stg-square-bigger-borders.svg` & `packitos-0.94.2/design/export/logo-stg-square-bigger-borders.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-stg-square-small-borders.png` & `packitos-0.94.2/design/export/logo-stg-square-small-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-stg-square-small-borders.svg` & `packitos-0.94.2/design/export/logo-stg-square-small-borders.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-stg.png` & `packitos-0.94.2/design/export/logo-stg.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-stg.svg` & `packitos-0.94.2/design/export/logo-stg.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-text.jpg` & `packitos-0.94.2/design/export/logo-text.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-text.png` & `packitos-0.94.2/design/export/logo-text.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-text.svg` & `packitos-0.94.2/design/export/logo-text.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo-white.png` & `packitos-0.94.2/design/export/logo-white.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo.png` & `packitos-0.94.2/design/export/logo.png`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/design/export/logo.svg` & `packitos-0.94.2/design/export/logo.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/files/local-tests-requirements.yaml` & `packitos-0.94.2/files/local-tests-requirements.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/files/zuul-reverse-dep-packit-service.yaml` & `packitos-0.94.2/files/zuul-reverse-dep-packit-service.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/files/zuul-tests-session-recording.yaml` & `packitos-0.94.2/files/zuul-tests-session-recording.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/files/tasks/packit-service-requirements.yaml` & `packitos-0.94.2/files/tasks/packit-service-requirements.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/files/tasks/rpm-test-deps.yaml` & `packitos-0.94.2/files/tasks/rpm-test-deps.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/actions.py` & `packitos-0.94.2/packit/actions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/api.py` & `packitos-0.94.2/packit/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1011,15 +1011,15 @@
                 self.dg.get_allowed_gpg_keys_from_downstream_config()
             )
 
             try:
                 downstream_spec_ver = self.dg.get_specfile_version()
                 if compare_versions(version, downstream_spec_ver) < 0:
                     msg = (
-                        f"Downstream specfile version {downstream_spec_ver} is lower "
+                        f"Downstream specfile version {downstream_spec_ver} is higher "
                         f"than the version to propose ({version}). Skipping the update."
                     )
                     logger.debug(msg)
                     raise ReleaseSkippedPackitException(msg)
                 self.dg.refresh_specfile()
 
             except FileNotFoundError:
@@ -1092,15 +1092,15 @@
                     else "",
                 }
                 | self.sync_release_env,
             )
 
             commit_title, commit_description = get_commit_message_from_action(
                 output=commit_msg_action_output,
-                default_title=title or f"[packit] {version} upstream release",
+                default_title=title or f"Update to {version} upstream release",
                 default_description=description
                 or self.get_default_commit_description(upstream_tag, resolved_bugs),
             )
 
             self.update_dist_git(
                 version,
                 upstream_ref,
@@ -1978,15 +1978,15 @@
         owner = owner or self.copr_helper.configured_owner
         if not owner:
             raise PackitCoprException(
                 "Copr owner not set. Use Copr config file or `--owner` when calling packit CLI.",
             )
         logger.info(f"We will operate with COPR owner {owner}.")
 
-        self.copr_helper.create_copr_project_if_not_exists(
+        self.copr_helper.create_or_update_copr_project(
             project=project,
             chroots=chroots,
             owner=owner,
             description=description,
             instructions=instructions,
             list_on_homepage=list_on_homepage,
             preserve_project=preserve_project,
```

### Comparing `packitos-0.94.1/packit/base_git.py` & `packitos-0.94.2/packit/base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/command_handler.py` & `packitos-0.94.2/packit/command_handler.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/constants.py` & `packitos-0.94.2/packit/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,16 @@
     "Use it multiple times to select multiple packages."
     "Defaults to all the packages listed inside the config."
 )
 
 SYNC_RELEASE_DEFAULT_COMMIT_DESCRIPTION = (
     "{resolved_bugs}Upstream tag: {upstream_tag}\n"
     "Upstream commit: {upstream_commit}\n"
+    "\n"
+    "Commit authored by Packit automation (https://packit.dev/)\n"
 )
 
 SYNC_RELEASE_PR_DESCRIPTION = (
     "Upstream tag: {upstream_tag_info}\n"
     "Upstream commit: {upstream_commit_info}\n"
     "{release_monitoring_info}"
     "{resolved_bugzillas_info}"
```

### Comparing `packitos-0.94.1/packit/copr_helper.py` & `packitos-0.94.2/packit/copr_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             self.copr_client.project_chroot_proxy.edit(
                 ownername=owner,
                 projectname=project,
                 chrootname=chroot,
                 **update_args,
             )
 
-    def create_copr_project_if_not_exists(
+    def create_or_update_copr_project(
         self,
         project: str,
         chroots: list[str],
         owner: Optional[str] = None,
         description: Optional[str] = None,
         instructions: Optional[str] = None,
         list_on_homepage: Optional[bool] = False,
@@ -183,59 +183,64 @@
         additional_repos: Optional[list[str]] = None,
         request_admin_if_needed: bool = False,
         targets_dict: Optional[dict] = None,  # chroot specific configuration
         module_hotfixes: bool = False,
         follow_fedora_branching: bool = False,
     ) -> None:
         """
-        Create a project in copr if it does not exists.
+        Create or update a project in copr.
 
         Raises PackitCoprException on any problems.
         """
-        logger.info(
-            f"Trying to get {owner}/{project} Copr project. "
-            "The project will be created if it does not exist.",
+        default_description = (
+            "Continuous builds initiated by Packit service.\n"
+            "For more info check out https://packit.dev/"
         )
+
+        default_instructions = (
+            (
+                "You can check out the upstream project "
+                f"{self.upstream_local_project.git_url} to find out how to consume these builds. "
+                f"This copr project is created and handled by the Packit project "
+                "(https://packit.dev/)."
+            )
+            if self.upstream_local_project
+            else None
+        )
+
+        delete_after_days: Optional[int] = (
+            None if preserve_project is None else -1 if preserve_project else 60
+        )
+
+        logger.info(f"Creating {owner}/{project} Copr project.")
         try:
-            copr_proj = self.copr_client.project_proxy.get(
+            copr_proj = self.copr_client.project_proxy.add(
                 ownername=owner,
                 projectname=project,
-            )
-        except CoprNoResultException as ex:
-            if owner != self.configured_owner:
-                raise PackitCoprProjectException(
-                    f"Copr project {owner}/{project} not found.",
-                ) from ex
-
-            logger.info(f"Copr project '{owner}/{project}' not found. Creating new.")
-            self.create_copr_project(
                 chroots=chroots,
-                description=description,
-                instructions=instructions,
-                owner=owner,
-                project=project,
-                list_on_homepage=list_on_homepage,
-                preserve_project=preserve_project,
-                additional_packages=additional_packages,
+                description=description or default_description,
+                contact="https://github.com/packit/packit/issues",
+                # don't show project on Copr homepage by default
+                unlisted_on_hp=not list_on_homepage,
+                # delete project after the specified period of time
+                delete_after_days=delete_after_days,
                 additional_repos=additional_repos,
-                targets_dict=targets_dict,
+                instructions=instructions or default_instructions,
                 module_hotfixes=module_hotfixes,
                 follow_fedora_branching=follow_fedora_branching,
+                exist_ok=True,
             )
-            return
-        except CoprRequestException as ex:
-            logger.debug(repr(ex))
-            logger.error(
-                f"We were not able to get copr project {owner}/{project}: {ex}",
+        except (CoprException, CoprRequestException) as ex:
+            error = (
+                f"Cannot create a new Copr project "
+                f"(owner={owner} project={project} chroots={chroots}): {ex}"
             )
-            raise
-
-        delete_after_days: Optional[int] = (
-            None if preserve_project is None else -1 if preserve_project else 60
-        )
+            logger.error(error)
+            logger.error(ex.result)
+            raise PackitCoprProjectException(error) from ex
 
         fields_to_change = self.get_fields_to_change(
             copr_proj=copr_proj,
             additional_repos=additional_repos,
             chroots=chroots,
             description=description,
             instructions=instructions,
@@ -396,80 +401,14 @@
             fields_to_change["module_hotfixes"] = (
                 copr_proj.module_hotfixes,
                 module_hotfixes,
             )
 
         return fields_to_change
 
-    def create_copr_project(
-        self,
-        chroots: list[str],
-        description: str,
-        instructions: str,
-        owner: str,
-        project: str,
-        list_on_homepage: bool = False,
-        preserve_project: bool = False,
-        additional_packages: Optional[list[str]] = None,
-        additional_repos: Optional[list[str]] = None,
-        targets_dict: Optional[dict] = None,  # chroot specific configuration
-        module_hotfixes: bool = False,
-        follow_fedora_branching: bool = False,
-    ) -> None:
-        try:
-            self.copr_client.project_proxy.add(
-                ownername=owner,
-                projectname=project,
-                chroots=chroots,
-                description=(
-                    description
-                    or "Continuous builds initiated by packit service.\n"
-                    "For more info check out https://packit.dev/"
-                ),
-                contact="https://github.com/packit/packit/issues",
-                # don't show project on Copr homepage by default
-                unlisted_on_hp=not list_on_homepage,
-                # delete project after the specified period of time
-                delete_after_days=60 if not preserve_project else None,
-                additional_repos=additional_repos,
-                instructions=instructions
-                or "You can check out the upstream project "
-                f"{self.upstream_local_project.git_url} to find out how to consume these builds. "
-                f"This copr project is created and handled by the packit project "
-                "(https://packit.dev/).",
-                module_hotfixes=module_hotfixes,
-                follow_fedora_branching=follow_fedora_branching,
-            )
-            # once created: update chroot-specific configuration if there is any
-            chroot_specific_config = self._get_chroot_specific_configuration_to_update(
-                project,
-                owner,
-                targets_dict,
-            )
-            self._update_chroot_specific_configuration(
-                project=project,
-                owner=owner,
-                update_dict=chroot_specific_config,
-            )
-        except CoprException as ex:
-            # TODO: Remove once Copr doesn't throw for existing projects or new
-            # API endpoint is established.
-            if "You already have a project named" in ex.result.error:
-                # race condition between workers
-                logger.debug(f"Copr project ({owner}/{project}) is already present.")
-                return
-
-            error = (
-                f"Cannot create a new Copr project "
-                f"(owner={owner} project={project} chroots={chroots}): {ex}"
-            )
-            logger.error(error)
-            logger.error(ex.result)
-            raise PackitCoprProjectException(error) from ex
-
     def watch_copr_build(
         self,
         build_id: int,
         timeout: int,
         report_func: Optional[Callable] = None,
     ) -> str:
         """returns copr build state"""
```

### Comparing `packitos-0.94.1/packit/dist_git_instance.py` & `packitos-0.94.2/packit/dist_git_instance.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/distgit.py` & `packitos-0.94.2/packit/distgit.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/exceptions.py` & `packitos-0.94.2/packit/exceptions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/local_project.py` & `packitos-0.94.2/packit/local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/patches.py` & `packitos-0.94.2/packit/patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/pkgtool.py` & `packitos-0.94.2/packit/pkgtool.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/schema.py` & `packitos-0.94.2/packit/schema.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/security.py` & `packitos-0.94.2/packit/security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/source_git.py` & `packitos-0.94.2/packit/source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/status.py` & `packitos-0.94.2/packit/status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/sync.py` & `packitos-0.94.2/packit/sync.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/upstream.py` & `packitos-0.94.2/packit/upstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/vm_image_build.py` & `packitos-0.94.2/packit/vm_image_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/build.py` & `packitos-0.94.2/packit/cli/build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/create_update.py` & `packitos-0.94.2/packit/cli/create_update.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/dist_git_init.py` & `packitos-0.94.2/packit/cli/dist_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/init.py` & `packitos-0.94.2/packit/cli/init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/packit_base.py` & `packitos-0.94.2/packit/cli/packit_base.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/prepare_sources.py` & `packitos-0.94.2/packit/cli/prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/propose_downstream.py` & `packitos-0.94.2/packit/cli/propose_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/push_updates.py` & `packitos-0.94.2/packit/cli/push_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/source_git.py` & `packitos-0.94.2/packit/cli/source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/source_git_init.py` & `packitos-0.94.2/packit/cli/source_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/source_git_status.py` & `packitos-0.94.2/packit/cli/source_git_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/srpm.py` & `packitos-0.94.2/packit/cli/srpm.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/status.py` & `packitos-0.94.2/packit/cli/status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/sync_from_downstream.py` & `packitos-0.94.2/packit/cli/sync_from_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/types.py` & `packitos-0.94.2/packit/cli/types.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/update_dist_git.py` & `packitos-0.94.2/packit/cli/update_dist_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/update_source_git.py` & `packitos-0.94.2/packit/cli/update_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/utils.py` & `packitos-0.94.2/packit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/validate_config.py` & `packitos-0.94.2/packit/cli/validate_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/builds/copr_build.py` & `packitos-0.94.2/packit/cli/builds/copr_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/builds/in_image_builder.py` & `packitos-0.94.2/packit/cli/builds/in_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/builds/koji_build.py` & `packitos-0.94.2/packit/cli/builds/koji_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/builds/local_build.py` & `packitos-0.94.2/packit/cli/builds/local_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/cli/builds/mock_build.py` & `packitos-0.94.2/packit/cli/builds/mock_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/config/__init__.py` & `packitos-0.94.2/packit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/config/aliases.py` & `packitos-0.94.2/packit/config/aliases.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from cachetools.func import ttl_cache
 
 from packit.exceptions import PackitException
 from packit.utils.bodhi import get_bodhi_client
 from packit.utils.commands import run_command
 from packit.utils.decorators import fallback_return_value
+from packit.utils.monitoring import Pushgateway
 
 ALIASES: dict[str, list[str]] = {
     "fedora-all": ["fedora-38", "fedora-39", "fedora-rawhide"],
     "fedora-stable": ["fedora-38", "fedora-39"],
     "fedora-development": ["fedora-rawhide"],
     "fedora-latest": ["fedora-39"],
     "fedora-latest-stable": ["fedora-39"],
@@ -38,14 +39,17 @@
 }
 
 DEFAULT_VERSION = "fedora-stable"
 
 logger = logging.getLogger(__name__)
 
 
+pushgateway = Pushgateway()
+
+
 def get_versions(*name: str, default=DEFAULT_VERSION) -> set[str]:
     """
     Expand the aliases to the name(s).
 
     :param name: name(s) of the system and version (e.g. "fedora-30" or "fedora-stable")
     :param default: used if no positional argument was given
     :return: set of string containing system name and version
@@ -201,16 +205,22 @@
     return targets
 
 
 def get_all_koji_targets() -> list[str]:
     return run_command(["koji", "list-targets", "--quiet"], output=True).stdout.split()
 
 
+def update_metrics():
+    if hasattr(pushgateway, "aliases_fallback_used"):
+        pushgateway.aliases_fallback_used.inc()
+    pushgateway.push()
+
+
 @ttl_cache(maxsize=1, ttl=timedelta(hours=12).seconds)
-@fallback_return_value(ALIASES)
+@fallback_return_value(ALIASES, callback=update_metrics)
 def get_aliases() -> dict[str, list[str]]:
     """
     Function to automatically determine fedora-* and epel-* aliases.
     Current data are fetched via bodhi client, with default base url
     `https://bodhi.fedoraproject.org/'.
 
     Returns:
```

### Comparing `packitos-0.94.1/packit/config/common_package_config.py` & `packitos-0.94.2/packit/config/common_package_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/config/config.py` & `packitos-0.94.2/packit/config/config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/config/job_config.py` & `packitos-0.94.2/packit/config/job_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/config/notifications.py` & `packitos-0.94.2/packit/config/notifications.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/config/package_config.py` & `packitos-0.94.2/packit/config/package_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/config/package_config_validator.py` & `packitos-0.94.2/packit/config/package_config_validator.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/config/requirements.py` & `packitos-0.94.2/packit/config/requirements.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/data/_packitpatch` & `packitos-0.94.2/packit/data/_packitpatch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/__init__.py` & `packitos-0.94.2/packit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/bodhi.py` & `packitos-0.94.2/packit/utils/bodhi.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/changelog_helper.py` & `packitos-0.94.2/packit/utils/changelog_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/commands.py` & `packitos-0.94.2/packit/utils/commands.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/decorators.py` & `packitos-0.94.2/packit/utils/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # Copyright Contributors to the Packit project.
 # SPDX-License-Identifier: MIT
 
+import contextlib
 import functools
 import logging
-from typing import Any, Callable, Union
+from typing import Any, Callable, Optional, Union
 
 logger = logging.getLogger(__name__)
 
 
 def fallback_return_value(
     fallback_value: Any,
     exceptions: Union[type[Exception], tuple[type[Exception]]] = Exception,
+    callback: Optional[Callable] = None,
 ) -> Any:
     """
     The function of this decorator is to return some fallback value in case an exception was raised
     during a function call.
 
     :param fallback_value: a value which will be returned if a specified exception was raised
     :param exceptions: exception(s) which should be handled, by default all exceptions are caught
+    :param callback: function to call if fallback happens
     :return: func original return value if no exception was raised
             fallback_return_value if a specified exception was caught
     """
 
     def decorator(func: Callable) -> Callable:
         @functools.wraps(func)
         def inner(*args: Any, **kwargs: Any) -> Any:
@@ -29,12 +32,15 @@
                 return func(*args, **kwargs)
             except exceptions as e:
                 logger.warning(
                     f"Fallback return value used while calling {func.__name__} because of "
                     f"{type(e).__name__}"
                     f"{': ' + str(e) if str(e) else ''} ",
                 )
+                if callback is not None:
+                    with contextlib.suppress(Exception):
+                        callback()
                 return fallback_value
 
         return inner
 
     return decorator
```

### Comparing `packitos-0.94.1/packit/utils/extensions.py` & `packitos-0.94.2/packit/utils/extensions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/koji_helper.py` & `packitos-0.94.2/packit/utils/koji_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/logging.py` & `packitos-0.94.2/packit/utils/logging.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/lookaside.py` & `packitos-0.94.2/packit/utils/lookaside.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/repo.py` & `packitos-0.94.2/packit/utils/repo.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/source_script.py` & `packitos-0.94.2/packit/utils/source_script.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/upstream_version.py` & `packitos-0.94.2/packit/utils/upstream_version.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/packit/utils/versions.py` & `packitos-0.94.2/packit/utils/versions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/plans/full.fmf` & `packitos-0.94.2/plans/full.fmf`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/plans/session-recording.fmf` & `packitos-0.94.2/plans/session-recording.fmf`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/conftest.py` & `packitos-0.94.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/full.fmf` & `packitos-0.94.2/tests/full.fmf`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/spellbook.py` & `packitos-0.94.2/tests/spellbook.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/cockpit-ostree/Makefile` & `packitos-0.94.2/tests/data/cockpit-ostree/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/cockpit-ostree/cockpit-ostree.spec.dg` & `packitos-0.94.2/tests/data/cockpit-ostree/cockpit-ostree.spec.dg`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/cockpit-ostree/cockpit-ostree.spec.in` & `packitos-0.94.2/tests/data/cockpit-ostree/cockpit-ostree.spec.in`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch` & `packitos-0.94.2/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/cronie/SOURCES/fix-memory-leaks.patch` & `packitos-0.94.2/tests/data/cronie/SOURCES/fix-memory-leaks.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/cronie/SOURCES/fix-unsafe-code.patch` & `packitos-0.94.2/tests/data/cronie/SOURCES/fix-unsafe-code.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/cronie/SPECS/cronie.spec` & `packitos-0.94.2/tests/data/cronie/SPECS/cronie.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/dg-ogr/.packit.yaml` & `packitos-0.94.2/tests/data/dg-ogr/.packit.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/dg-ogr/python-ogr.spec` & `packitos-0.94.2/tests/data/dg-ogr/python-ogr.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/edd/Makefile` & `packitos-0.94.2/tests/data/edd/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/edd/edd.spec` & `packitos-0.94.2/tests/data/edd/edd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/osbuild/osbuild.spec` & `packitos-0.94.2/tests/data/osbuild/osbuild.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/patches/previous/git-diff.patch` & `packitos-0.94.2/tests/data/patches/previous/git-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/patches/previous/missing-diff-line.patch` & `packitos-0.94.2/tests/data/patches/previous/missing-diff-line.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/patches/previous/unified-diff.patch` & `packitos-0.94.2/tests/data/patches/previous/unified-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/patches/previous/weird-identical.patch` & `packitos-0.94.2/tests/data/patches/previous/weird-identical.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/patches/regenerated/git-diff.patch` & `packitos-0.94.2/tests/data/patches/regenerated/git-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/patches/regenerated/missing-diff-line.patch` & `packitos-0.94.2/tests/data/patches/regenerated/missing-diff-line.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/patches/regenerated/unified-diff.patch` & `packitos-0.94.2/tests/data/patches/regenerated/unified-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/patches/regenerated/weird-identical.patch` & `packitos-0.94.2/tests/data/patches/regenerated/weird-identical.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/rpms/hello/0017-Patch-This..patch` & `packitos-0.94.2/tests/data/rpms/hello/0017-Patch-This..patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/rpms/hello/from-git.patch` & `packitos-0.94.2/tests/data/rpms/hello/from-git.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/snapd/packaging/fedora/fix-spec` & `packitos-0.94.2/tests/data/snapd/packaging/fedora/fix-spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/snapd/packaging/fedora/pack-source` & `packitos-0.94.2/tests/data/snapd/packaging/fedora/pack-source`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/snapd/packaging/fedora/snapd.spec` & `packitos-0.94.2/tests/data/snapd/packaging/fedora/snapd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/snapd/vendor/vendor.json` & `packitos-0.94.2/tests/data/snapd/vendor/vendor.json`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/sourcegit/source_git/.distro/beer.spec` & `packitos-0.94.2/tests/data/sourcegit/source_git/.distro/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/upstream_git/beer.spec` & `packitos-0.94.2/tests/data/upstream_git/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/upstream_git_macro_in_source/beer.spec` & `packitos-0.94.2/tests/data/upstream_git_macro_in_source/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/data/vsftpd/Fedora/vsftpd.spec` & `packitos-0.94.2/tests/data/vsftpd/Fedora/vsftpd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/functional/spellbook.py` & `packitos-0.94.2/tests/functional/spellbook.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/functional/test_local_build.py` & `packitos-0.94.2/tests/functional/test_local_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/functional/test_prepare_sources.py` & `packitos-0.94.2/tests/functional/test_prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/functional/test_srpm.py` & `packitos-0.94.2/tests/functional/test_srpm.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/bodhi_latest_builds.py` & `packitos-0.94.2/tests/integration/bodhi_latest_builds.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/bodhi_status_updates.py` & `packitos-0.94.2/tests/integration/bodhi_status_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/conftest.py` & `packitos-0.94.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_actions.py` & `packitos-0.94.2/tests/integration/test_actions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_api.py` & `packitos-0.94.2/tests/integration/test_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_base_git.py` & `packitos-0.94.2/tests/integration/test_base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_build.py` & `packitos-0.94.2/tests/integration/test_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_changelog_helper.py` & `packitos-0.94.2/tests/integration/test_changelog_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_copr_build.py` & `packitos-0.94.2/tests/integration/test_copr_build.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # SPDX-License-Identifier: MIT
 
 import pytest
 from copr.v3 import (
     BuildProxy,
     Client,
     CoprAuthException,
-    CoprNoResultException,
     ProjectProxy,
 )
 from flexmock import flexmock
 from munch import munchify
 
 import packit
 from packit.api import PackitAPI
@@ -24,15 +23,15 @@
     u, d, api = api_instance
     owner = "the-owner"
     project = "project-name"
     description = "some description"
     instructions = "the instructions"
     chroots = ["fedora-rawhide-x86_64"]
 
-    flexmock(ProjectProxy).should_receive("get").and_return(
+    flexmock(ProjectProxy).should_receive("add").and_return(
         flexmock(
             chroot_repos=flexmock(keys=lambda: chroots),
             description=description,
             instructions=instructions,
             unlisted_on_hp=True,
             delete_after_days=60,
             additional_repos=[],
@@ -73,15 +72,15 @@
     u, d, api = api_instance
     owner = "the-owner"
     project = "project-name"
     description = "some description"
     instructions = "the instructions"
     chroots = ["fedora-rawhide-x86_64"]
 
-    flexmock(ProjectProxy).should_receive("get").and_return(
+    flexmock(ProjectProxy).should_receive("add").and_return(
         flexmock(
             chroot_repos=flexmock(keys=lambda: chroots),
             description=description,
             instructions=instructions,
             unlisted_on_hp=True,
             delete_after_days=60,
             additional_repos=[],
@@ -144,15 +143,15 @@
     api_instance,
 ):
     u, d, api = api_instance
     owner = "the-owner"
     project = "project-name"
     chroots = ["fedora-rawhide-x86_64"]
 
-    flexmock(ProjectProxy).should_receive("get").and_return(
+    flexmock(ProjectProxy).should_receive("add").and_return(
         munchify(
             {
                 "additional_repos": [],
                 "auto_prune": True,
                 "chroot_repos": {
                     "fedora-rawhide-x86_64": "https://download.copr.fedorainfracloud.org/"
                     "results/packit/packit-hello-world-127-stg/fedora-rawhide-x86_64/",
@@ -203,15 +202,15 @@
     api_instance,
 ):
     u, d, api = api_instance
     owner = "the-owner"
     project = "project-name"
     chroots = ["fedora-rawhide-x86_64"]
 
-    flexmock(ProjectProxy).should_receive("get").and_return(
+    flexmock(ProjectProxy).should_receive("add").and_return(
         munchify(
             {
                 "additional_repos": [],
                 "auto_prune": True,
                 "chroot_repos": {
                     "fedora-rawhide-x86_64": "https://download.copr.fedorainfracloud.org/"
                     "results/packit/packit-hello-world-127-stg/fedora-rawhide-x86_64/",
@@ -266,15 +265,15 @@
     """
 
     u, d, api = api_instance
     owner = "the-owner"
     project = "project-name"
     chroots = ["fedora-rawhide-x86_64"]
 
-    flexmock(ProjectProxy).should_receive("get").and_return(
+    flexmock(ProjectProxy).should_receive("add").and_return(
         munchify(
             {
                 "additional_repos": [],
                 "auto_prune": True,
                 "chroot_repos": {
                     "fedora-rawhide-x86_64": "https://download.copr.fedorainfracloud.org/"
                     "results/packit/packit-hello-world-127-stg/fedora-rawhide-x86_64/",
@@ -326,15 +325,15 @@
     api_instance,
 ):
     u, d, api = api_instance
     owner = "the-owner"
     project = "project-name"
     chroots = ["fedora-rawhide-x86_64"]
 
-    flexmock(ProjectProxy).should_receive("get").and_return(
+    flexmock(ProjectProxy).should_receive("add").and_return(
         munchify(
             {
                 "additional_repos": [],
                 "auto_prune": True,
                 "chroot_repos": {
                     "fedora-rawhide-x86_64": "https://download.copr.fedorainfracloud.org/"
                     "results/packit/packit-hello-world-127-stg/fedora-rawhide-x86_64/",
@@ -403,15 +402,15 @@
     owner,
     requested_chroots,
     expected_chroots_for_edit,
 ):
     u, d, api = api_instance
     project = "project-name"
 
-    flexmock(ProjectProxy).should_receive("get").and_return(
+    flexmock(ProjectProxy).should_receive("add").and_return(
         munchify(
             {
                 "additional_repos": [],
                 "auto_prune": True,
                 "chroot_repos": {
                     "fedora-rawhide-x86_64": "https://download.copr.fedorainfracloud.org/"
                     "results/packit/packit-hello-world-127-stg/fedora-rawhide-x86_64/",
@@ -475,15 +474,15 @@
     u, d, api = api_instance
     owner = "the-owner"
     project = "project-name"
     description = "some description"
     instructions = "the instructions"
     chroots = ["fedora-rawhide-x86_64"]
 
-    flexmock(ProjectProxy).should_receive("get").and_return(
+    flexmock(ProjectProxy).should_receive("add").and_return(
         flexmock(
             chroot_repos=flexmock(keys=lambda: chroots),
             description=description,
             instructions=instructions,
             unlisted_on_hp=True,
             delete_after_days=60,
             additional_repos=[],
@@ -523,46 +522,14 @@
             instructions=instructions,
         )
     assert e_info.value.fields_to_change == {
         "description": ("some description", "different description"),
     }
 
 
-def test_copr_build_non_existing_project(cwd_upstream_or_distgit, api_instance):
-    u, d, api = api_instance
-    owner = "the-owner"
-    project = "project-name"
-
-    flexmock(ProjectProxy).should_receive("get").and_raise(
-        CoprNoResultException,
-        "project not found",
-    )
-    flexmock(ProjectProxy).should_receive("edit").and_return(None).times(0)
-    flexmock(ProjectProxy).should_receive("add").and_return(None)
-
-    flexmock(CoprHelper).should_receive("get_copr_client").and_return(
-        Client(
-            config={"copr_url": "https://copr.fedorainfracloud.org", "username": owner},
-        ),
-    )
-
-    build = flexmock(id="1", ownername=owner, projectname=project)
-    flexmock(BuildProxy).should_receive("create_from_file").and_return(build)
-    build_id, url = api.run_copr_build(
-        project=project,
-        chroots="fedora-rawhide-x86_64",
-        owner=owner,
-        description="some description",
-        instructions="the instructions",
-    )
-
-    assert build_id == "1"
-    assert url == f"https://copr.fedorainfracloud.org/coprs/build/{build.id}/"
-
-
 def test_copr_build_no_owner(cwd_upstream_or_distgit, api_instance):
     u, d, api = api_instance
     flexmock(CoprHelper).should_receive("get_copr_client").and_return(
         Client(config={"copr_url": "https://copr.fedorainfracloud.org"}),
     )
     with pytest.raises(PackitCoprException) as ex:
         api.run_copr_build(
@@ -659,34 +626,42 @@
         srpm_path=None,
         module_hotfixes=False,
     ).and_return(("id", "url")).once()
 
     run_packit(["build", "in-copr", "--no-wait"], working_dir=upstream)
 
 
-def test_create_copr_project(copr_client_mock):
+def test_create_or_update_copr_project(copr_client_mock):
     copr_helper = CoprHelper(flexmock(git_url="https://gitlab.com/"))
     flexmock(packit.copr_helper.CoprClient).should_receive(
         "create_from_config_file",
     ).and_return(copr_client_mock)
 
+    options = {
+        "chroots": ["centos-stream-8-x86_64"],
+        "description": "my fabulous test",
+        "instructions": None,
+        "owner": "me",
+        "project": "already-present",
+        "targets_dict": {"centos-stream-8": {"additional_packages": ["foo"]}},
+        "module_hotfixes": None,
+    }
+
     copr_client_mock.project_proxy = flexmock()
     copr_client_mock.project_chroot_proxy = flexmock()
-    flexmock(copr_client_mock.project_proxy).should_receive("add").and_return({})
+    flexmock(copr_client_mock.project_proxy).should_receive("add").and_return(
+        flexmock(
+            chroot_repos={"centos-stream-8-x86_64": "https://repo.url"},
+            **options,
+        ),
+    )
     flexmock(copr_client_mock.project_chroot_proxy).should_receive("get").and_return(
         {"additional_packages": []},
     )
     flexmock(copr_client_mock.project_chroot_proxy).should_receive("edit").with_args(
         ownername="me",
         projectname="already-present",
         chrootname="centos-stream-8-x86_64",
         additional_packages=["foo"],
     ).and_return({})
 
-    copr_helper.create_copr_project(
-        chroots=["centos-stream-8-x86_64"],
-        description="my fabulous test",
-        instructions=None,
-        owner="me",
-        project="already-present",
-        targets_dict={"centos-stream-8": {"additional_packages": ["foo"]}},
-    )
+    copr_helper.create_or_update_copr_project(**options)
```

### Comparing `packitos-0.94.1/tests/integration/test_create_update.py` & `packitos-0.94.2/tests/integration/test_create_update.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_get_api.py` & `packitos-0.94.2/tests/integration/test_get_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_init.py` & `packitos-0.94.2/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_local_project.py` & `packitos-0.94.2/tests/integration/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_pagure.py` & `packitos-0.94.2/tests/integration/test_pagure.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_patches.py` & `packitos-0.94.2/tests/integration/test_patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_push_updates.py` & `packitos-0.94.2/tests/integration/test_push_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_security.py` & `packitos-0.94.2/tests/integration/test_security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_source_git.py` & `packitos-0.94.2/tests/integration/test_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_source_git_init.py` & `packitos-0.94.2/tests/integration/test_source_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_source_git_status.py` & `packitos-0.94.2/tests/integration/test_source_git_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_source_git_synch_push.py` & `packitos-0.94.2/tests/integration/test_source_git_synch_push.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_source_git_update_source_git.py` & `packitos-0.94.2/tests/integration/test_source_git_update_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_spec.py` & `packitos-0.94.2/tests/integration/test_spec.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_update.py` & `packitos-0.94.2/tests/integration/test_update.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_upstream.py` & `packitos-0.94.2/tests/integration/test_upstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_using_cockpit.py` & `packitos-0.94.2/tests/integration/test_using_cockpit.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_using_examples.py` & `packitos-0.94.2/tests/integration/test_using_examples.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_validate_config.py` & `packitos-0.94.2/tests/integration/test_validate_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/integration/test_validate_synced_files.py` & `packitos-0.94.2/tests/integration/test_validate_synced_files.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/conftest.py` & `packitos-0.94.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_actions.py` & `packitos-0.94.2/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_api.py` & `packitos-0.94.2/tests/unit/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,24 +357,30 @@
 
 
 @pytest.mark.parametrize(
     "resolved_bugs, result",
     [
         pytest.param(
             ["rhbz#123"],
-            "- Resolves: rhbz#123\n\nUpstream tag: 1.0.0\nUpstream commit: _\n",
+            "- Resolves: rhbz#123\n\nUpstream tag: 1.0.0\nUpstream commit: _\n"
+            "\nCommit authored by Packit automation (https://packit.dev/)\n",
         ),
         pytest.param(
             ["rhbz#123", "rhbz#222"],
             (
                 "- Resolves: rhbz#123\n- Resolves: rhbz#222\n\n"
                 "Upstream tag: 1.0.0\nUpstream commit: _\n"
+                "\nCommit authored by Packit automation (https://packit.dev/)\n"
             ),
         ),
-        pytest.param(None, "Upstream tag: 1.0.0\nUpstream commit: _\n"),
+        pytest.param(
+            None,
+            "Upstream tag: 1.0.0\nUpstream commit: _\n"
+            "\nCommit authored by Packit automation (https://packit.dev/)\n",
+        ),
     ],
 )
 def test_get_default_commit_description(api_mock, resolved_bugs, result):
     assert (
         api_mock.get_default_commit_description("1.0.0", resolved_bugs=resolved_bugs)
         == result
     )
```

### Comparing `packitos-0.94.1/tests/unit/test_base_git.py` & `packitos-0.94.2/tests/unit/test_base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_cli.py` & `packitos-0.94.2/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_cli_utils.py` & `packitos-0.94.2/tests/unit/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_copr_helper.py` & `packitos-0.94.2/tests/unit/test_copr_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_dg.py` & `packitos-0.94.2/tests/unit/test_dg.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_dist_git_init.py` & `packitos-0.94.2/tests/unit/test_dist_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_image_builder.py` & `packitos-0.94.2/tests/unit/test_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_iterate_packages.py` & `packitos-0.94.2/tests/unit/test_iterate_packages.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_koji_build.py` & `packitos-0.94.2/tests/unit/test_koji_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_load_authentication.py` & `packitos-0.94.2/tests/unit/test_load_authentication.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_local_project.py` & `packitos-0.94.2/tests/unit/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_login_with_kerberos.py` & `packitos-0.94.2/tests/unit/test_login_with_kerberos.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_patches.py` & `packitos-0.94.2/tests/unit/test_patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_prepare_sources.py` & `packitos-0.94.2/tests/unit/test_prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_propose_downstream.py` & `packitos-0.94.2/tests/unit/test_propose_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_security.py` & `packitos-0.94.2/tests/unit/test_security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_specfile.py` & `packitos-0.94.2/tests/unit/test_specfile.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_status.py` & `packitos-0.94.2/tests/unit/test_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_sync.py` & `packitos-0.94.2/tests/unit/test_sync.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_upstream.py` & `packitos-0.94.2/tests/unit/test_upstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/test_utils.py` & `packitos-0.94.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/config/test_config.py` & `packitos-0.94.2/tests/unit/config/test_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/config/test_config_aliases.py` & `packitos-0.94.2/tests/unit/config/test_config_aliases.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/config/test_package_config.py` & `packitos-0.94.2/tests/unit/config/test_package_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/utils/test_changelog_helper.py` & `packitos-0.94.2/tests/unit/utils/test_changelog_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/utils/test_decorators.py` & `packitos-0.94.2/tests/unit/utils/test_decorators.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/utils/test_dist_git_instance.py` & `packitos-0.94.2/tests/unit/utils/test_dist_git_instance.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/utils/test_koji_helper.py` & `packitos-0.94.2/tests/unit/utils/test_koji_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/utils/test_lookaside.py` & `packitos-0.94.2/tests/unit/utils/test_lookaside.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/utils/test_repo.py` & `packitos-0.94.2/tests/unit/utils/test_repo.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/utils/test_source_script.py` & `packitos-0.94.2/tests/unit/utils/test_source_script.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/utils/test_upstream_version.py` & `packitos-0.94.2/tests/unit/utils/test_upstream_version.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests/unit/utils/test_versions.py` & `packitos-0.94.2/tests/unit/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/README.md` & `packitos-0.94.2/tests_recording/README.md`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_api.py` & `packitos-0.94.2/tests_recording/test_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_base_git.py` & `packitos-0.94.2/tests_recording/test_base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_image_builder.py` & `packitos-0.94.2/tests_recording/test_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_local_project.py` & `packitos-0.94.2/tests_recording/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_repository_cache.py` & `packitos-0.94.2/tests_recording/test_repository_cache.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_status.py` & `packitos-0.94.2/tests_recording/test_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/testbase.py` & `packitos-0.94.2/tests_recording/testbase.py`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml` & `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz` & `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz` & `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml` & `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz` & `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml` & `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz` & `packitos-0.94.2/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml` & `packitos-0.94.2/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml` & `packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml` & `packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml` & `packitos-0.94.2/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml` & `packitos-0.94.2/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml` & `packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml` & `packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml` & `packitos-0.94.2/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml` & `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml` & `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml` & `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml` & `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_status.yaml` & `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_status.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml` & `packitos-0.94.2/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/LICENSE` & `packitos-0.94.2/LICENSE`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/README.md` & `packitos-0.94.2/README.md`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/pyproject.toml` & `packitos-0.94.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packitos-0.94.1/PKG-INFO` & `packitos-0.94.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: packitos
-Version: 0.94.1
+Version: 0.94.2
 Summary: A set of tools to integrate upstream open source projects into Fedora operating system.
 Project-URL: Homepage, https://github.com/packit/packit
 Author-email: Red Hat <user-cont-team@redhat.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: dist-git,fedora,git,packaging,rpm
 Classifier: Development Status :: 4 - Beta
```

