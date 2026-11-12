# Mark Fredrickson

Senior data engineer working with healthcare data: payer claims ingestion, person matching
(master patient indexes), and the data quality and pipelines around them. M.P.H., Health
Informatics.

My public projects use fully synthetic data, and each one checks itself against known-correct
results (answer keys or ground truth), not just against "it ran".

| Project | What it shows |
|---|---|
| [person-matching-pipeline](https://github.com/fredr171/person-matching-pipeline) | Rule-based entity resolution that builds an MPI with stable person IDs. dbt + DuckDB and PySpark implementations agree exactly across 27 million rows; precision 0.992 against ground truth, with its limits measured. |
| [claims-lakehouse-dbt-duckdb](https://github.com/fredr171/claims-lakehouse-dbt-duckdb) | Event-driven claims ETL on AWS (S3, Lambda, EventBridge, SQS FIFO) with dbt: immutable bronze, stop vs warn gating, a payer registry, and GitHub-issue alerts that close themselves. |
| [claims-lakehouse-databricks-azure](https://github.com/fredr171/claims-lakehouse-databricks-azure) | The same spec on Azure and Databricks: Lakeflow, Auto Loader, AUTO CDC, Unity Catalog masks and Terraform, verified live against the same answer keys. |
| [synthetic-payer-files](https://github.com/fredr171/synthetic-payer-files) | Seeded CMS CCLF and Medicare Advantage delivery files with answer keys, shared by both lakehouses. |
| [wisconsin-lake-ranking](https://github.com/fredr171/wisconsin-lake-ranking) | A side project: five public data sources, cached and scored with explicit guardrails for missing data. I used it to choose where to buy land. |

**Stack:** SQL (SQL Server, Snowflake), dbt, Python, PySpark and Databricks, AWS, Azure,
Terraform, GitHub Actions.

These projects were built with Claude Code as an AI pair programmer; each README says how.
