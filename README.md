# FEMA Flood Insurance Analysis using SQL Queries via DuckDB-Python 

This project analyzes large-scale FEMA National Flood Insurance Program (NFIP) datasets using **DuckDB** and **Python** to uncover insights on flood insurance policies and claims across the U.S.

---

## Project Objective

Flooding is the costliest natural disaster in the U.S., yet flood insurance coverage and affordability vary widely. This project aims to:

- Efficiently analyze FEMA's **NFIP Policies (70M records)** and **Claims (3M records)** datasets.
- Derive meaningful regional and temporal insights using SQL and Python.
- Demonstrate how **DuckDB** enables fast, in-memory querying of massive datasets — without the need for a full database server.

---
<p align="center">
  <img width="638" height="384" alt="image" src="https://github.com/user-attachments/assets/550bbaec-e8bd-455a-83b4-03606864a35a" width="45%"/> 
  <img width="638" height="384" alt="image" src="https://github.com/user-attachments/assets/ffdd96e3-790c-4538-8b8c-11457ca2e8e1" width="45%"/>
</p>

<Figure size 1400x700 with 8 Axes><img width="1095" height="563" alt="image" src="https://github.com/user-attachments/assets/9ed34d78-80ea-42f5-bcdb-a3af034404b7" />

## Tech Stack

| Tool        | Purpose                              |
|-------------|---------------------------------------|
| **DuckDB**  | SQL-based OLAP engine for big data analysis directly within Python |
| **Python**  | Data processing, scripting, and orchestration |
| **Pandas**  | Light transformation & data validation |
| **SQL**     | Complex analytics over large datasets |
| **Parquet** | Source data formats from FEMA |

---

## Dataset Overview

| Dataset        | Records | Description                           |
|----------------|---------|---------------------------------------|
| NFIP Policies  | ~70M    | Policy records across states, years, ZIP codes, with attributes like coverage, premiums, elevation, occupancy, etc. |
| NFIP Claims    | ~3M     | Flood insurance claim records with timing, location, and payout details |

Data source: Listed in jupyter notebooks for both the datasets

---

## Key Highlights

-  **Analyzed 70M+ rows** locally with DuckDB without memory errors.
-  Built SQL queries to:
  - Compare **policy coverage vs. claims trends** by ZIP and state
  - Identify **underinsured areas**
  - Evaluate **temporal patterns** in policy issuance and claims
-  Applied column filtering and narrowing to reduce compute load while maintaining insight quality.
-  Validated DuckDB results against PostgreSQL for consistency.

---

