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

* <code>dbt test</code><br>
testing models/schema following schema.yml. option to test unique column/no null. <br>


* <code>dbt docs generate</code><br>
generate docs/data dictionary, will reside under target folder

* <code>dbt docs serve</code><br>
ui to navigate dbt docs generated beforehand, hosted local