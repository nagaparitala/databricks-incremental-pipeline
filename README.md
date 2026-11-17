# Databricks Incremental Orders Pipeline

A Databricks practice project using sample order CSVs, Auto Loader, PySpark and Delta Lake. The notebooks walk from Unity Catalog setup through incremental Bronze ingestion, Silver deduplication and merges, schema evolution, data quality, recovery and job orchestration.

1. Start with [01 Project setup](01_project_setup.ipynb), then review Steps 02–06 in order as the sample pipeline evolves.
2. For Step 7, import the three job notebooks into Databricks and configure their dependencies using the [Lakeflow job diagram](lakeflow-job.md).
3. Adjust the catalog, schema and volume references for your workspace. The Step 7 notebooks use `workspace.incremental_project` and expect the tables and cleaned input prepared by the earlier notebooks.

The repository contains notebook exports with execution outputs and workspace metadata removed, not a deployed Lakeflow job or a Databricks bundle.
