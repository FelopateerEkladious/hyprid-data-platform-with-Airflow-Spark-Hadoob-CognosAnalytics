# Data Platform for retail data analytics
## Overview
The data infrastructure is a mix of on-premises and cloud-based systems.
Tools and Technologies Used:

**OLTP Database**: MySQL
**NoSQL Database**: MongoDB
**Main Data Warehouse**: IBM DB2 (Cloud)
**Staging Warehouse**: PostgreSQL
**Big Data Framework**: Hadoop
**Analytics Platform**: Apache Spark
**Business Intelligence**: IBM Cognos Analytics
**Data Workflows**: Apache Airflow

## Workflow
* SoftCart’s business is conducted primarily through its website, accessible via desktop, mobile, and tablet devices.
* Product information is kept in a NoSQL MongoDB database.
* Sales and inventory transactions are handled through a MySQL database.
* These databases are the backbone of the website’s operations.
* Data from the MySQL and MongoDB databases is regularly moved into a staging warehouse powered by PostgreSQL.
* The primary data warehouse operates on IBM’s cloud-based DB2 server.
* The BI team uses IBM DB2 to generate performance dashboards with IBM Cognos Analytics.
* SoftCart leverages a Hadoop ecosystem for storing all analytics data.
* Apache Spark processes and analyzes data on the Hadoop platform.
* Apache Airflow manages ETL workflows to transfer data between OLTP systems, the NoSQL database, and the data warehouses.
