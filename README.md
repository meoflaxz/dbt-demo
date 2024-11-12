* <code>pip install dbt-bigquery</code><br>
install dbt with bigquer connector

* <code>dbt --version</code><br>
check dbt version

* <code>dbt init XXX</code><br>
initialized dbt project

* <code>dbt debug</code><br>
validating connection<br>
should be in the project file before write dbt debug otherwise dbt will not found dbt_project.yml

* <code>dbt run</code><br>
build all table/run, will run entire table config <br>

* <code>dbt run --full-refresh</code><br>
dbt run, but with table dropping <br>

* by default data is materialized following what we defined in <code>dbt_projects.yml</code>. Override using <code>{{ config(materialized='table') }}</code> in the model folder<br>

* <code>dbt seed</code><br>
load CSV file into project/warehouse <br>

