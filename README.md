# Master
1️⃣ Create Raw Database
📌 Creates a raw database in Databricks and stores the ingested data as a table.

2️⃣ Create Config Table
📌 Generates a config table that stores the table names and their latest modified timestamps, enabling metadata tracking.

3️⃣ Update Config Table
📌 Updates the config table at the end of the workflow to reflect the latest changes.

4️⃣ Customer Dimension
📌 Defines the schema for the Customer Dimension, extracts customer data from the raw file, and performs upsert operations to ensure only the latest data is retained.

5️⃣ Product Dimension
📌 Defines the schema for the Product Dimension, extracts product data from the raw file, and performs upsert operations for accurate data representation.

6️⃣ ShipMode Dimension
📌 Defines the schema for the ShipMode Dimension, extracts shipping mode details, and ensures upsert operations for maintaining updated data.

7️⃣ Fact Sales Table
📌 Creates the Fact Sales Table, extracts transactional sales data from the raw file, and performs upsert operations for efficient reporting and analytics.

8️⃣ To_CSV Process
📌 Extracts changed records from all dimension and fact tables, converts them into CSV files, and stores them in Azure Storage for further processing.
