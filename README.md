# csv_to_postgresql
A script that I wrote to load CSV into PostgreSQL while analyzing the Brazilian Ecommerce data olist
Automatically scans the current directory to find .csv files,
Converts them into a pandas dataframe,
Creates the necessary tables on PostgreSQL,
Loads the dataframe and the index to PostgreSQL. Then, depending on the table, the indices have been either removed or set to be the PK as some tables lacked PK's.
Tables that have a PK assigned later on SQL have the format "column_name_PK" in the ERD diagram

The SQL ERD:

![olistERD](https://github.com/seyf97/csv_to_postgresql/assets/111386377/eb2c17eb-e27a-4321-b8d7-0e9947b9c2f8)
