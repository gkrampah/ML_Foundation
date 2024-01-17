# Reading data for ML

A few common Structured Query Language (SQL) databases used with Python include:

- Microsoft SQL Server
- Postgres
- MySQL
- AWS Redshift
- AWS Aurora
- Oracle DB
- Terradata
- Db2 Family
- Many, many others

connection packages use to connect to the databases include:

- `sqlite3`
- `SQLAlchemy` (most common)
- `psycopg2`
- `MySQLdb`

NoSQL databases are not relational and vary more in structure. Most of NoSQL databases store data in JSON format. Eg:
- Document databases: mongoDB, couchDB
- key-value stores: Riak, Voldemort, Redis
- Graph databases: Neo4j, HyperGraph
- Wide-column stores: Cassandra, HBase

## Data Cleaning

### How data gets messy
- Duplicate and unnecessary data
- inconsistent test or typos
- missing data
- outliers
- data source issues:
    - multiple systems 
    - different database types
    - on premise, in cloud etc

### Handling missing data
* remove the data: remove rows compleletly
* Impute the data: replace the substituted values. replace the missing data with the most common value, average value etc
* mask the data: create a category for the missing values

### Outliers
1. Statistics: calculate interquater range and use that to determine what an outlier is
2. Residuals- difference between the actual and the predicted values of the outcome variable: 
    - standardized: residual divided by the standard error
    - Deleted: residual from fitting model on all data excluding current observation
    - Studentized: Deleted residuals divided by residual standard error

Handling outliers

* Remove the outlier 
* or assign the mean or median value, 
* transform the variable or 
* predict what the value should be using regression or using similar observations


