**Data Warehousing Concepts**

### **1\. OLTP (Online Transaction Processing)**

* **Purpose**: Manages real-time business transactions.

* **Features**:

  * Handles large number of short, simple queries.

  * Frequent INSERT, UPDATE, DELETE operations.

  * Data is **highly normalized** to reduce redundancy.

  * Ensures **consistency, concurrency, and speed**.

* **Use Cases**: Banking systems, retail POS, reservation systems.

---

### **2\. OLAP (Online Analytical Processing)**

* **Purpose**: Supports business analysis and decision-making.

* **Features**:

  * Works on **historical data** stored in a Data Warehouse.

  * Executes complex queries with **aggregation and summarization**.

  * Data is often **denormalized** (Star/Snowflake schema) for faster retrieval.

  * Optimized for **read-heavy** operations.

* **Types**:

  * **ROLAP** – Uses relational DBs.

  * **MOLAP** – Uses multidimensional cubes.

  * **HOLAP** – Hybrid approach.

* **Use Cases**: Sales analysis, customer behavior, forecasting.

---

### **3\. Dimensional Modeling**

* **Definition**: A design methodology for structuring data in a Data Warehouse to make analysis easier.

* **Key Components**:

  * **Fact Table**: Central table with measurable data (e.g., sales amount, revenue).

  * **Dimension Tables**: Surrounding tables with descriptive attributes (e.g., product, time, location, customer).

* **Schemas**:

  * **Star Schema** – Simple, fact table linked directly to dimensions.

  * **Snowflake Schema** – Normalized dimensions (more complex).

  * **Galaxy Schema** – Multiple fact tables sharing dimensions.

* **Goal**: Provide a clear, intuitive structure that improves query performance and supports OLAP analysis.

---

