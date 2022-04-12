# Compute@Edge google bigquery connector starter kit for Rust

This starter kit is to connect google bigquery. you can use data maniplulation language (DML) since this uses [jobs.query of bigquery API](https://cloud.google.com/bigquery/docs/reference/rest/v2/jobs/query). The reason why this uses jobs.query to insert data rather than [streaming insert api](https://cloud.google.com/bigquery/docs/reference/rest/v2/tabledata/insertAll) is to allow to modify the inserted data immediately.

## Configuration

Please put your gcp project information in the [bigquery] section of the [config.toml](src/config.toml) file. We need [a service account](https://cloud.google.com/iam/docs/service-accounts) of your project to connect bigquery.

## Security issues

Please see [SECURITY.md](SECURITY.md) for guidance on reporting security-related issues.
