Incremental loading and merging using Hive and MySQL
PROBLEM:

A company ABC receives the data about the purchase made on their website by customers on a daily basis. To streamline the data collection and analysis, the company wishes to load all the data on a relational database system so that it can be accessible easily. Also, they need to maintain the data which is up-to –date i.e if there is any change made in the purchase order, it must overwrite the previous data reflect in the database.

APPROACH:

We follow a step-by-step process in achieving the solution for the above-mentioned problem:

Load the data from client's machine and create a table on MySQL.
Load the data into Hive Table.
Implement SCD-1 to keep the up-to-date data.
Load the data back into MySQL.
Create a backup table for reconciliation.
