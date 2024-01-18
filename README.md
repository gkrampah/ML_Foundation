# Intro to AI and ML
Two of the biggest breakthroughs in the history of artificial intelligence are an image classification and machine translation (from one language to another). Deep learning (DL) is a subset of machine learning (ML) and ML is also a subset of AI. AI is any program that sense, reason, act and adapt. Ml are algorithms whose perfamance improve as they are exposed to more data over time. They are not explicitly programmed but learn patterns as they are exposed to more data. DL is a subset of ML in which its multilayered neral networks learn fromvast amounts of data

## History of AI 
AI has experienced cycles of AI winters and AI booms. 

AI solutions include speech recognition, computer vision, assisted medical diagnosis, robotics, and others.   

## Modern AI 
Factors that have contributed to the current state of Machine Learning are: bigger data sets, faster computers, open source packages, and a wide range of neural network architectures.   

## Machine Learning Workflow 
The machine learning workflow consists of: 

- Problem statement

- Data collection

- Data exploration and preprocessing

- Modeling

- Validation

- Decision Making and Deployment

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

## Estimation and Inference and Hypothesis testing

A statistical inference is about finding the underlying data generating process of our data, then the statistical model is going to be a set of the possible distributions or even reggressions that that data can take. Now, a parametric model is a particular type of statistical model. What differentiates a parametric model? Some of the major characteristics, or that a parametric model is constrained to a finite number of parameters, and that'll rely on some strict assumptions made about the distributions from which that data is pulled. Now, non-parametric models, on the other hand, will mean that our inference will not rely on as many assumptions, such as it will not have to rely on the data being pulled from a particular distribution, it'll be a distribution free inference.


Now, when we're doing parametric modeling, the most common way of estimating parameters and a parametric model is through the Maximum Likelihood estimate. The likelihood function is related to probability and is a function of the parameters of the model. 