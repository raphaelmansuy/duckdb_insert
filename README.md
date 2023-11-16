# DuckDB Insert

This repository contains a Python program for ingesting data from various database sources and writing it to Parquet files, with optional AWS S3 support.

## Overview

The `duckdb_insert` program allows for efficient extraction of data from MySQL, PostgreSQL, and SQLite databases, and saving it in the Parquet format. This is particularly useful for data transformation and storage optimization tasks. It also supports uploading the Parquet files to AWS S3.

## Features

- **Multiple Database Support**: Compatible with MySQL, PostgreSQL, and SQLite.
- **Parquet File Generation**: Converts database data into Parquet file format for efficient storage and access.
- **AWS S3 Integration**: Option to upload Parquet files directly to an S3 bucket.
- **Batch Processing**: Supports reading data in batches for optimized performance.
- **Flexible Date Filtering**: Allows filtering of database records based on a specified date range.

## Installation

Install the necessary dependencies using:

```bash
pip install -r requirements.txt
```

## Usage

The script can be executed via the command line with various options for database connectivity, data filtering, and target file specification.

### Basic Usage

```bash
python duckdb_insert.py --db_type [mysql/postgres/sqlite] --host [host] --port [port] --user [username] --password [password] --database [dbname] --table_name [tablename] --target_path [path/to/save/parquet/files]
```

### Advanced Options

- AWS S3 support
- Date range filtering
- Batch size specification
- Automatic deletion of target files

For a detailed list of all options, use:

```bash
python duckdb_insert.py --help
```

## Contributing

Contributions are welcome. Please follow the guidelines in the repository for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
