Testing

Run project dan generate table/views dll berdasarkan dbt_project.yml
dbt run 

Generate documentation
dbt docs generate

mart vs staging
mart: isinya table, lambat di awal saat run, namun ketika query lebih cepat
staging: isinya views, lambat untuk query, hanya sementara dan jarang untuk dipanggil. Tidak langsung memanggil table karena dapat mengurangi resource

Setting up project
https://github.com/rafifas/dbt-test/blob/demo-dbt/dbt_project.yml 
Create dim customers
https://github.com/rafifas/dbt-test/blob/demo-dbt/models/dim_customers.sql 
Create stg_customers
https://github.com/rafifas/dbt-test/blob/demo-dbt/models/staging/stg_customers.sql 
Create stg_orders
https://github.com/rafifas/dbt-test/blob/demo-dbt/models/staging/stg_orders.sql 
Create new_dim_customers
https://github.com/rafifas/dbt-test/blob/demo-dbt/models/mart/new_dim_customers.sql 
Create docs
dbt docs generate 
