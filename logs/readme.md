# logs

## Info

This directory stores logs from the pipeline executions.

The Makefile in the [crf-data-mgmt](https://github.com/crowdfightcovid19/crf-data-mgmt) repository contains `MAIN_TARGETS` that save logs here.

## Directory structure

    .
    ├── readme.md
    ├── download_YYYYMMDD-HHMMSS.log            # Generated by `make download`
    ├── preprocess_YYYYMMDD-HHMMSS.log          # Generated by `make preprocess`
    ├── archive_YYYYMMDD-HHMMSS.log             # Generated by `make archive`
    ├── clean_YYYYMMDD-HHMMSS.log               # Generated by `make clean`
    └── distclean_YYYYMMDD-HHMMSS.log           # Generated by `make distclean`

