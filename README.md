# Vendor_performance_analysis

"""
Vendor Performance Analysis Project

This Python notebook is designed to analyze vendor performance using sales summary data.
It performs the following key steps:

1. **Library Imports**:
   - Loads essential libraries like `pandas`, `sqlalchemy`, `sqlite3`, `matplotlib`, and `scipy.stats`.

2. **Logging and Database Setup**:
   - Configures logging to track data ingestion steps.
   - Establishes a connection to a local SQLite database (`inventory.db`) using SQLAlchemy.

3. **Data Ingestion Functions**:
   - `ingest_db(df, table_name, engine)`: Saves a DataFrame to a database table.
   - `load_raw_data()`: Automatically reads all CSV files from a `/data` directory, loads them into DataFrames, and writes them to the database. The process is logged and timed.

4. **Main Execution Block**:
   - When the script is run directly, it triggers `load_raw_data()` to ingest data into the database.

5. **Data Loading and Analysis**:
   - Connects to the database using `sqlite3`.
   - Loads data from the `vendor_sales_summary` table into a DataFrame.
   - Displays the first few rows and summary statistics for exploration.

The rest of the notebook likely includes visual analysis and statistical testing (e.g., t-tests) for vendor performance evaluation.
"""
