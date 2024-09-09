- by default, Spark will assume all columns are strings

  - if you want it to guess column types, in `.csv()` set `inferSchema=True`

- to select a specific column by name you can do
  - df.select('col_name')
  - this returns a pyspark.sql.dataframe.DataFrame
  - you can also do df['col_name']
    - this returns a Column data type
    - you can use this for vectorized transformations
