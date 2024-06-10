# iceberg-spark-gcs-compatibility
script to download compatible iceberg spark and gcs connectors with nessie catalogue

need to match versions between:

- pyspark
- python3.X
- iceberg-spark-runtime
- spark
- hadoop
- gcs-connector
- nessie 
- java requirements
  - java 11+


## Dependency
```
gcs-connector -> hadoop-version 
hadoop-version <-> spark-version
iceberg-spark-runtime <-> spark-version <-> nessie
```


## Resources

https://community.cloudera.com/t5/Community-Articles/Spark-Python-Supportability-Matrix/ta-p/379144
  - python compatibility matrix

https://spark.apache.org/downloads.html
  - indicates spark:3.5.1 requires hadoop:3.3 or later

https://github.com/GoogleCloudDataproc/hadoop-connectors/issues/1099
  - shows you need to download hadoop on the machine too

https://community.cloudera.com/t5/Community-Articles/Spark-Python-Supportability-Matrix/ta-p/379144
  - install pyspark with specific hadoop version


