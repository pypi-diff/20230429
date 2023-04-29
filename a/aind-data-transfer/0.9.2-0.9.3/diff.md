# Comparing `tmp/aind-data-transfer-0.9.2.tar.gz` & `tmp/aind-data-transfer-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-data-transfer-0.9.2.tar", last modified: Tue Mar 14 22:34:55 2023, max compression
+gzip compressed data, was "aind-data-transfer-0.9.3.tar", last modified: Wed Mar 15 21:04:26 2023, max compression
```

## Comparing `aind-data-transfer-0.9.2.tar` & `aind-data-transfer-0.9.3.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.014859 aind-data-transfer-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.982860 aind-data-transfer-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.990860 aind-data-transfer-0.9.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.990860 aind-data-transfer-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-03-14 22:34:55.014859 aind-data-transfer-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.990860 aind-data-transfer-0.9.2/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/conf/ephys_upload_job_configs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/conf/smartspim_upload_job_configs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/conf/transcode_job_configs.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/post_install.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.990860 aind-data-transfer-0.9.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.990860 aind-data-transfer-0.9.2/scripts/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/bin/openephys_job.sh
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/bin/transcode_job.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.990860 aind-data-transfer-0.9.2/scripts/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/cluster/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/cluster/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/create_neuroglancer_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/gcs_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/make_mips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/run_openephys_jobs_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/smartspim_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/validate_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/scripts/write_ome_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 22:34:55.014859 aind-data-transfer-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.982860 aind-data-transfer-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.990860 aind-data-transfer-0.9.2/src/aind_data_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-14 22:34:34.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.994860 aind-data-transfer-0.9.2/src/aind_data_transfer/config_loader/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/config_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/config_loader/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/config_loader/ephys_configuration_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/config_loader/imaging_configuration_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.994860 aind-data-transfer-0.9.2/src/aind_data_transfer/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/jobs/openephys_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/jobs/s3_upload_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/jobs/transcode_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.994860 aind-data-transfer-0.9.2/src/aind_data_transfer/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/readers/ephys_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/readers/imaging_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.994860 aind-data-transfer-0.9.2/src/aind_data_transfer/transcode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/transcode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/transcode/ome_zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.994860 aind-data-transfer-0.9.2/src/aind_data_transfer/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/transformations/ephys_compressors.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/transformations/imaging_compressors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/transformations/metadata_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/transformations/video_compressors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.994860 aind-data-transfer-0.9.2/src/aind_data_transfer/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/util/chunk_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/util/dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/util/env_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/util/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/util/npopto_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/util/s3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.994860 aind-data-transfer-0.9.2/src/aind_data_transfer/writers/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/writers/ephys_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/src/aind_data_transfer/writers/imaging_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.994860 aind-data-transfer-0.9.2/src/aind_data_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-03-14 22:34:54.000000 aind-data-transfer-0.9.2/src/aind_data_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-03-14 22:34:54.000000 aind-data-transfer-0.9.2/src/aind_data_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 22:34:54.000000 aind-data-transfer-0.9.2/src/aind_data_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-14 22:34:54.000000 aind-data-transfer-0.9.2/src/aind_data_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-14 22:34:54.000000 aind-data-transfer-0.9.2/src/aind_data_transfer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.994860 aind-data-transfer-0.9.2/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/templates/queue_slurm_job.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.998860 aind-data-transfer-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/imaging/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.998860 aind-data-transfer-0.9.2/tests/resources/imaging/12345-random-sample/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/12345-random-sample/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/12345-random-sample/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/12345-random-sample/README
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/12345-random-sample/dataset_description.json
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/12345-random-sample/instrument.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.998860 aind-data-transfer-0.9.2/tests/resources/imaging/12345-random-sample/micr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/12345-random-sample/micr/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/12345-random-sample/procedures.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/12345-random-sample/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.998860 aind-data-transfer-0.9.2/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/README
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/dataset_description.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.998860 aind-data-transfer-0.9.2/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/exaSPIM/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/exaSPIM/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/instrument.json
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/procedures.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.002859 aind-data-transfer-0.9.2/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/README
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/dataset_description.json
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/instrument.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.002859 aind-data-transfer-0.9.2/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/mesoSPIM/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/mesoSPIM/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/procedures.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.002859 aind-data-transfer-0.9.2/tests/resources/test_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/test_configs/ephys_upload_job_test_configs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/test_configs/example_configs_src_pattern1.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/test_configs/example_configs_src_pattern2.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.002859 aind-data-transfer-0.9.2/tests/resources/test_configs/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/test_configs/imaging/transcode_job_test_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/test_configs/jobs_list.csv
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/test_configs/jobs_list_2.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.002859 aind-data-transfer-0.9.2/tests/resources/test_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/test_metadata/data_description.json
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/test_metadata/processing.json
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/test_metadata/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.002859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.002859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.002859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/continuous.dat
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.002859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/
--rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.002859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/
--rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.002859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/MessageCenter/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/MessageCenter/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/MessageCenter/text.npy
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/MessageCenter/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.006859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/
--rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy
--rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy
--rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.006859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.006859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy
--rw-r--r--   0 runner    (1001) docker     (123)   223851 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/structure.oebin
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/sync_messages.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.006859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.006859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/continuous.dat
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.006859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/
--rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.006859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/
--rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.006859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/MessageCenter/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/MessageCenter/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/MessageCenter/text.npy
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/MessageCenter/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.006859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/
--rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy
--rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy
--rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.010859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.010859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy
--rw-r--r--   0 runner    (1001) docker     (123)   223851 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/structure.oebin
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/sync_messages.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.010859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.010859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/continuous.dat
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.010859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/
--rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.010859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/
--rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.010859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/MessageCenter/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/MessageCenter/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/MessageCenter/text.npy
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/MessageCenter/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.010859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/
--rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy
--rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy
--rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.010859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/
--rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy
--rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy
--rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:54.986860 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.010859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/
--rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy
--rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy
--rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy
--rw-r--r--   0 runner    (1001) docker     (123)   223851 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/structure.oebin
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/sync_messages.txt
--rw-r--r--   0 runner    (1001) docker     (123)    59324 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)    59324 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings_3.xml
--rw-r--r--   0 runner    (1001) docker     (123)    59324 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings_6.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:34:55.014859 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Videos/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Videos/a_video_file.avi
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Videos/another_video_file.avi
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Videos/video_ref.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_chunk_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_compressors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_ephys_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_ephys_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_gcs_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_generic_upload_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_imaging_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_imaging_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_metadata_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_ome_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-14 22:34:33.000000 aind-data-transfer-0.9.2/tests/test_s3_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.417736 aind-data-transfer-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.373736 aind-data-transfer-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.393736 aind-data-transfer-0.9.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.393736 aind-data-transfer-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-03-15 21:04:26.413736 aind-data-transfer-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.393736 aind-data-transfer-0.9.3/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/conf/ephys_upload_job_configs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/conf/smartspim_upload_job_configs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/conf/transcode_job_configs.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/post_install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.393736 aind-data-transfer-0.9.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.393736 aind-data-transfer-0.9.3/scripts/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/bin/openephys_job.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/bin/transcode_job.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.393736 aind-data-transfer-0.9.3/scripts/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/cluster/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/cluster/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/create_neuroglancer_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/gcs_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/make_mips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/run_openephys_jobs_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/smartspim_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/validate_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/scripts/write_ome_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 21:04:26.417736 aind-data-transfer-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.377736 aind-data-transfer-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.393736 aind-data-transfer-0.9.3/src/aind_data_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-15 21:04:10.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.393736 aind-data-transfer-0.9.3/src/aind_data_transfer/config_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/config_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/config_loader/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/config_loader/ephys_configuration_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/config_loader/imaging_configuration_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.397736 aind-data-transfer-0.9.3/src/aind_data_transfer/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/jobs/openephys_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/jobs/s3_upload_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/jobs/transcode_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.397736 aind-data-transfer-0.9.3/src/aind_data_transfer/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/readers/ephys_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/readers/imaging_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.397736 aind-data-transfer-0.9.3/src/aind_data_transfer/transcode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/transcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/transcode/ome_zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.397736 aind-data-transfer-0.9.3/src/aind_data_transfer/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/transformations/ephys_compressors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/transformations/imaging_compressors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/transformations/metadata_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/transformations/video_compressors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.397736 aind-data-transfer-0.9.3/src/aind_data_transfer/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/util/chunk_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/util/dask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/util/env_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/util/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/util/npopto_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/util/s3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.397736 aind-data-transfer-0.9.3/src/aind_data_transfer/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/writers/ephys_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/src/aind_data_transfer/writers/imaging_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.393736 aind-data-transfer-0.9.3/src/aind_data_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-03-15 21:04:26.000000 aind-data-transfer-0.9.3/src/aind_data_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-03-15 21:04:26.000000 aind-data-transfer-0.9.3/src/aind_data_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 21:04:26.000000 aind-data-transfer-0.9.3/src/aind_data_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-15 21:04:26.000000 aind-data-transfer-0.9.3/src/aind_data_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-15 21:04:26.000000 aind-data-transfer-0.9.3/src/aind_data_transfer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.397736 aind-data-transfer-0.9.3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/templates/queue_slurm_job.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.401736 aind-data-transfer-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.381736 aind-data-transfer-0.9.3/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.381736 aind-data-transfer-0.9.3/tests/resources/imaging/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.401736 aind-data-transfer-0.9.3/tests/resources/imaging/12345-random-sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/12345-random-sample/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/12345-random-sample/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/12345-random-sample/README
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/12345-random-sample/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/12345-random-sample/instrument.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.401736 aind-data-transfer-0.9.3/tests/resources/imaging/12345-random-sample/micr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/12345-random-sample/micr/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/12345-random-sample/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/12345-random-sample/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.401736 aind-data-transfer-0.9.3/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/README
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.401736 aind-data-transfer-0.9.3/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/exaSPIM/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/exaSPIM/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/instrument.json
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.401736 aind-data-transfer-0.9.3/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/README
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/instrument.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.401736 aind-data-transfer-0.9.3/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/mesoSPIM/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/mesoSPIM/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.401736 aind-data-transfer-0.9.3/tests/resources/test_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/test_configs/ephys_upload_job_test_configs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/test_configs/example_configs_src_pattern1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/test_configs/example_configs_src_pattern2.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.405736 aind-data-transfer-0.9.3/tests/resources/test_configs/imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/test_configs/imaging/transcode_job_test_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/test_configs/jobs_list.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/test_configs/jobs_list_2.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.405736 aind-data-transfer-0.9.3/tests/resources/test_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/test_metadata/data_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/test_metadata/processing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/test_metadata/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.389736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.405736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.381736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.405736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.385736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.405736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/continuous.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.405736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/
+-rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.405736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/
+-rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.385736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.405736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/MessageCenter/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/MessageCenter/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/MessageCenter/text.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/MessageCenter/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.385736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.405736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/
+-rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.385736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.405736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.385736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.409736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy
+-rw-r--r--   0 runner    (1001) docker     (123)   223851 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/structure.oebin
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/sync_messages.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.385736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.409736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.385736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.409736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/continuous.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.409736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/
+-rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.409736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/
+-rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.389736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.409736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/MessageCenter/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/MessageCenter/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/MessageCenter/text.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/MessageCenter/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.389736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.409736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/
+-rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.389736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.409736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.389736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.409736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy
+-rw-r--r--   0 runner    (1001) docker     (123)   223851 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/structure.oebin
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/sync_messages.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.389736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.413736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.389736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.413736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/continuous.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.413736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/
+-rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.413736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/
+-rw-r--r--   0 runner    (1001) docker     (123)    76800 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.389736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.413736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/MessageCenter/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/MessageCenter/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/MessageCenter/text.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/MessageCenter/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.389736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.413736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/
+-rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.389736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.413736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/
+-rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.389736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.413736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/
+-rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy
+-rw-r--r--   0 runner    (1001) docker     (123)   223851 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/structure.oebin
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/sync_messages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    59324 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    59324 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings_3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    59324 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings_6.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:04:26.413736 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Videos/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Videos/a_video_file.avi
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Videos/another_video_file.avi
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Videos/video_ref.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_chunk_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_compressors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_ephys_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_ephys_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_gcs_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_generic_upload_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_imaging_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_imaging_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_metadata_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_ome_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-15 21:04:09.000000 aind-data-transfer-0.9.3/tests/test_s3_transfer.py
```

### Comparing `aind-data-transfer-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aind-data-transfer-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aind-data-transfer-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/.github/ISSUE_TEMPLATE/user-story.md` & `aind-data-transfer-0.9.3/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/.github/workflows/ci.yml` & `aind-data-transfer-0.9.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/.github/workflows/tag_and_publish.yml` & `aind-data-transfer-0.9.3/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/.gitignore` & `aind-data-transfer-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/LICENSE` & `aind-data-transfer-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/PKG-INFO` & `aind-data-transfer-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-transfer
-Version: 0.9.2
+Version: 0.9.3
 Summary: Services for compression and transfer of aind-data to the cloud
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ephys
```

### Comparing `aind-data-transfer-0.9.2/README.md` & `aind-data-transfer-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/conf/ephys_upload_job_configs.yml` & `aind-data-transfer-0.9.3/conf/ephys_upload_job_configs.yml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/conf/smartspim_upload_job_configs.yml` & `aind-data-transfer-0.9.3/conf/smartspim_upload_job_configs.yml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/conf/transcode_job_configs.yml` & `aind-data-transfer-0.9.3/conf/transcode_job_configs.yml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/pyproject.toml` & `aind-data-transfer-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/scripts/README.md` & `aind-data-transfer-0.9.3/scripts/README.md`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/scripts/cluster/submit.py` & `aind-data-transfer-0.9.3/scripts/cluster/submit.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/scripts/create_neuroglancer_links.py` & `aind-data-transfer-0.9.3/scripts/create_neuroglancer_links.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/scripts/gcs_upload.py` & `aind-data-transfer-0.9.3/scripts/gcs_upload.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/scripts/make_mips.py` & `aind-data-transfer-0.9.3/scripts/make_mips.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/scripts/run_openephys_jobs_template.py` & `aind-data-transfer-0.9.3/scripts/run_openephys_jobs_template.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/scripts/s3_upload.py` & `aind-data-transfer-0.9.3/scripts/s3_upload.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/scripts/smartspim_job.py` & `aind-data-transfer-0.9.3/scripts/smartspim_job.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/scripts/validate_datasets.py` & `aind-data-transfer-0.9.3/scripts/validate_datasets.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/scripts/write_ome_zarr.py` & `aind-data-transfer-0.9.3/scripts/write_ome_zarr.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/config_loader/base_config.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/config_loader/base_config.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/config_loader/ephys_configuration_loader.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/config_loader/ephys_configuration_loader.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/config_loader/imaging_configuration_loader.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/config_loader/imaging_configuration_loader.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/gcs.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/gcs.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/jobs/openephys_job.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/jobs/openephys_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             output_location = gcp_dest
         else:
             output_location = dest_data_dir
 
         code_url = job_configs["endpoints"]["code_repo_location"]
         parameters = job_configs
         processing_instance = ProcessingMetadata.from_inputs(
-            process_name=ProcessName.EPHYS_PREPROCESSING,
+            process_name=ProcessName.EPHYS_PREPROCESSING.value,
             start_date_time=start_date_time,
             end_date_time=end_date_time,
             input_location=str(input_location),
             output_location=output_location,
             code_url=code_url,
             parameters=parameters,
             notes=None,
```

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/jobs/s3_upload_job.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/jobs/s3_upload_job.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/jobs/transcode_job.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/jobs/transcode_job.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/readers/ephys_readers.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/readers/ephys_readers.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/readers/imaging_readers.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/readers/imaging_readers.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/s3.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/s3.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/transcode/ome_zarr.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/transcode/ome_zarr.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/transformations/ephys_compressors.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/transformations/ephys_compressors.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/transformations/imaging_compressors.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/transformations/imaging_compressors.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/transformations/metadata_creation.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/transformations/metadata_creation.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/transformations/video_compressors.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/transformations/video_compressors.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/util/chunk_utils.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/util/chunk_utils.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/util/dask_utils.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/util/dask_utils.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/util/env_utils.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/util/env_utils.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/util/file_utils.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/util/io_utils.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/util/io_utils.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/util/npopto_correction.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/util/npopto_correction.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/util/s3_utils.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/util/s3_utils.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/writers/ephys_writers.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/writers/ephys_writers.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer/writers/imaging_writers.py` & `aind-data-transfer-0.9.3/src/aind_data_transfer/writers/imaging_writers.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer.egg-info/PKG-INFO` & `aind-data-transfer-0.9.3/src/aind_data_transfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-transfer
-Version: 0.9.2
+Version: 0.9.3
 Summary: Services for compression and transfer of aind-data to the cloud
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ephys
```

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer.egg-info/SOURCES.txt` & `aind-data-transfer-0.9.3/src/aind_data_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/src/aind_data_transfer.egg-info/requires.txt` & `aind-data-transfer-0.9.3/src/aind_data_transfer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/templates/queue_slurm_job.sh` & `aind-data-transfer-0.9.3/templates/queue_slurm_job.sh`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/imaging/12345-random-sample/LICENSE` & `aind-data-transfer-0.9.3/tests/resources/imaging/12345-random-sample/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/LICENSE` & `aind-data-transfer-0.9.3/tests/resources/imaging/exaSPIM_125L_2022-08-05_17-25-36/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/LICENSE` & `aind-data-transfer-0.9.3/tests/resources/imaging/mesoSPIM_125L_2022-08-18_17-05-00/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/test_configs/ephys_upload_job_test_configs.yml` & `aind-data-transfer-0.9.3/tests/resources/test_configs/ephys_upload_job_test_configs.yml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/test_configs/example_configs_src_pattern1.yml` & `aind-data-transfer-0.9.3/tests/resources/test_configs/example_configs_src_pattern1.yml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/test_configs/example_configs_src_pattern2.yml` & `aind-data-transfer-0.9.3/tests/resources/test_configs/example_configs_src_pattern2.yml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/test_configs/imaging/transcode_job_test_config.yml` & `aind-data-transfer-0.9.3/tests/resources/test_configs/imaging/transcode_job_test_config.yml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/test_metadata/data_description.json` & `aind-data-transfer-0.9.3/tests/resources/test_metadata/data_description.json`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/test_metadata/processing.json` & `aind-data-transfer-0.9.3/tests/resources/test_metadata/processing.json`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/test_metadata/subject.json` & `aind-data-transfer-0.9.3/tests/resources/test_metadata/subject.json`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/structure.oebin` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment1/recording1/structure.oebin`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/structure.oebin` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment3/recording1/structure.oebin`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/NI-DAQmx-103.PXIe-6341/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/continuous.dat`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeB/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/continuous.dat`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/continuous/Neuropix-PXI-100.ProbeC/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/full_words.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/states.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/NI-DAQmx-103.PXIe-6341/TTL/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/full_words.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/states.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeB/TTL/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/full_words.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/sample_numbers.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/states.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/events/Neuropix-PXI-100.ProbeC/TTL/timestamps.npy`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/structure.oebin` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/experiment6/recording1/structure.oebin`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings.xml` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings.xml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings_3.xml` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings_3.xml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings_6.xml` & `aind-data-transfer-0.9.3/tests/resources/v0.6.x_neuropixels_multiexp_multistream/Record Node 101/settings_6.xml`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_base_config.py` & `aind-data-transfer-0.9.3/tests/test_base_config.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_chunk_utils.py` & `aind-data-transfer-0.9.3/tests/test_chunk_utils.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_compressors.py` & `aind-data-transfer-0.9.3/tests/test_compressors.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_ephys_config_loader.py` & `aind-data-transfer-0.9.3/tests/test_ephys_config_loader.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_ephys_readers.py` & `aind-data-transfer-0.9.3/tests/test_ephys_readers.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_gcs_uploader.py` & `aind-data-transfer-0.9.3/tests/test_gcs_uploader.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_generic_upload_job.py` & `aind-data-transfer-0.9.3/tests/test_generic_upload_job.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_imaging_config_loader.py` & `aind-data-transfer-0.9.3/tests/test_imaging_config_loader.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_imaging_readers.py` & `aind-data-transfer-0.9.3/tests/test_imaging_readers.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_io_utils.py` & `aind-data-transfer-0.9.3/tests/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_metadata_creation.py` & `aind-data-transfer-0.9.3/tests/test_metadata_creation.py`

 * *Files identical despite different names*

### Comparing `aind-data-transfer-0.9.2/tests/test_ome_zarr.py` & `aind-data-transfer-0.9.3/tests/test_ome_zarr.py`

 * *Files identical despite different names*

