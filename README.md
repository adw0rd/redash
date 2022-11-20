<p align="center">
  <img title="Redash" src='https://redash.io/assets/images/logo.png' width="200px"/>
</p>

Redash is designed to enable anyone, regardless of the level of technical sophistication, to harness the power of data big and small. SQL users leverage Redash to explore, query, visualize, and share data from any data sources. Their work in turn enables anybody in their organization to use the data. Every day, millions of users at thousands of organizations around the world use Redash to develop insights and make data-driven decisions.

Redash features:

1. **Browser-based**: Everything in your browser, with a shareable URL.
2. **Ease-of-use**: Become immediately productive with data without the need to master complex software.
3. **Query editor**: Quickly compose SQL and NoSQL queries with a schema browser and auto-complete.
4. **Visualization and dashboards**: Create [beautiful visualizations](https://redash.io/help/user-guide/visualizations/visualization-types) with drag and drop, and combine them into a single dashboard.
5. **Sharing**: Collaborate easily by sharing visualizations and their associated queries, enabling peer review of reports and queries.
6. **Schedule refreshes**: Automatically update your charts and dashboards at regular intervals you define.
7. **Alerts**: Define conditions and be alerted instantly when your data changes.
8. **REST API**: Everything that can be done in the UI is also available through REST API.
9. **Broad support for data sources**: Extensible data source API with native support for a long list of common databases and platforms.

<img src="https://raw.githubusercontent.com/getredash/website/8e820cd02c73a8ddf4f946a9d293c54fd3fb08b9/website/_assets/images/redash-anim.gif" width="80%"/>

## Getting Started

* [Setting up Redash instance](https://redash.io/help/open-source/setup) (includes links to ready-made AWS/GCE images).
* [Documentation](https://redash.io/help/).

- Amazon Athena
- Amazon CloudWatch / Insights
- Amazon DynamoDB
- Amazon Redshift
- ArangoDB
- Axibase Time Series Database
- Apache Cassandra
- ClickHouse
- CockroachDB
- Couchbase
- CSV
- Databricks
- DB2 by IBM
- Dgraph
- Apache Drill
- Apache Druid
- Eccenca Corporate Memory
- Elasticsearch
- Exasol
- Microsoft Excel
- Firebolt
- Google Analytics
- Google BigQuery
- Google Spreadsheets
- Graphite
- Greenplum
- Apache Hive
- Apache Impala
- InfluxDB
- IBM Netezza Performance Server
- JIRA (JQL)
- JSON
- Apache Kylin
- OmniSciDB (Formerly MapD)
- MariaDB
- MemSQL
- Microsoft Azure Data Warehouse / Synapse
- Microsoft Azure SQL Database
- Microsoft Azure Data Explorer / Kusto
- Microsoft SQL Server
- MongoDB
- MySQL
- Oracle
- Apache Phoenix
- Apache Pinot
- PostgreSQL
- Presto
- Prometheus
- Python
- Qubole
- Rockset
- Salesforce
- ScyllaDB
- Shell Scripts
- Snowflake
- SPARQL
- SQLite
- TiDB
- TreasureData
- Trino
- Uptycs
- Vertica
- Yandex AppMetrrica
- Yandex Metrica

## Запуск

Создайте в корне файл `.env`:

    REDASH_COOKIE_SECRET=aigaey8Iez8xeeghahsh4iC9aneech

И запустите Redash:

    docker-compose up -d

И перейдите по ссылке http://localhost:5050/

## Решение пробемы: relation "organizations" does not exist

Нужно выполнить миграции:

    docker-compose run --rm server create_db

## Frontend

Так можно запустить вотчер для обновления ассетов:

    docker-compose run webpack yarn watch

Подробности в `webpack.config.js` и `package.json`

