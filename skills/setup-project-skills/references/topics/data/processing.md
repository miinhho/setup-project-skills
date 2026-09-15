# Data processing and orchestration

| Skill | Install source | Use when |
| --- | --- | --- |
| `pandas-pro` | `Jeffallan/claude-skills` | Pandas joins, reshaping, missing data, time series, or DataFrame transformations recur. |
| `polars` | `k-dense-ai/scientific-agent-skills` | Polars expressions, lazy execution, streaming, Arrow interoperability, or pandas migration recurs. |
| `dask` | `k-dense-ai/scientific-agent-skills` | Pandas or NumPy workloads must scale beyond one machine's memory. |
| `spark-engineer` | `Jeffallan/claude-skills` | Spark DataFrames, SQL, structured streaming, or distributed job implementation recurs. |
| `spark-optimization` | `wshobson/agents` | Measured Spark shuffle, partition, caching, skew, or memory bottlenecks recur. |
| `airflow` | `astronomer/agents` | Airflow project structure, configuration, or operation recurs. |
| `authoring-dags` | `astronomer/agents` | Airflow DAG authoring recurs. |
| `testing-dags` | `astronomer/agents` | Airflow DAG validation and tests recur. |
| `airflow-state-store` | `astronomer/agents` | Airflow 3.3+ tasks need crash-safe state across retries or external-job polling. |
| `dagster-expert` | [Dagster plugin][dagster-plugin] | Dagster assets, components, definitions, materialization, schedules, sensors, tests, or `dg` CLI work recurs. |
| `beam-concepts` | `apache/beam` | Apache Beam's PCollection, PTransform, window, trigger, or portability model needs explanation. |
| `runners` | `apache/beam` | A Beam pipeline moves among Direct, Dataflow, Flink, Spark, or other runners. |
| `flink` | `gordonmurray/data-engineering-skills` | Apache Flink SQL, Table API, DataStream, state, checkpoints, savepoints, upgrades, or backpressure recur. |
| `confluent-cloud-flink-sql` | `confluentinc/agent-skills` | Flink SQL runs on Confluent Cloud and must respect its dialect and compute-pool behavior. |
| `flink-udf` | `confluentinc/agent-skills` | Java UDF, UDTF, or PTF code deploys to Confluent Cloud Flink. |
| `confluent-cloud-cdc-tableflow` | `confluentinc/agent-skills` | A Confluent Cloud CDC pipeline writes Tableflow Iceberg or Delta Lake tables. |
| `iceberg` | `gordonmurray/data-engineering-skills` | Apache Iceberg schema, partitions, snapshots, v2/v3 compatibility, compaction, or multi-engine operation recurs. |
| `paimon` | `gordonmurray/data-engineering-skills` | Apache Paimon streaming tables, changelog production, compaction, or Flink CDC integration recur. |
| `fluss` | `gordonmurray/data-engineering-skills` | Apache Fluss streaming storage, tiering, log or primary-key tables, or lakehouse integration recurs. |
| `iggy` | `gordonmurray/data-engineering-skills` | Apache Iggy deployment, streams, topics, retention, transports, or SDK clients recur. |

[dagster-plugin]: https://github.com/dagster-io/skills/tree/master/plugins/dagster
