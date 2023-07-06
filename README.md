Welcome to tw-campaign-finance

### Getting started

Install dbt:

```
python3 -m venv venv
source venv/bin/activate

pip install dbt-duckdb
```

Prepare an empty database:

```
mkdir -p tmp && python -c "import duckdb; duckdb.connect('tmp/duckdb.db').close()"
```

### Using the project

Download the incomes & expenditures csv under the path `data/` 
* https://lydata.ronny-s3.click/incomes.csv
* https://lydata.ronny-s3.click/expenditures.csv

Try running the following commands:
- dbt seed
- dbt run
- dbt test

The resulting parquet files will be available under `target/`.


Data source could be found at: https://g0v.hackmd.io/gGGUBDEXQOKGL_feUpPekg

###

See also `vgplot/` directory for yaml spec for interactive exploration with [mosaic](https://uwdata.github.io/mosaic/)

### License

MIT
