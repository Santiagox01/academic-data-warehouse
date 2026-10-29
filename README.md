# Academic Data Warehouse | Student Performance Analytics

A dimensional data warehouse project built with **Python, SQL, and DuckDB** to analyze academic performance, course approval rates, and student persistence indicators using synthetic enrollment data.

## Project Overview

This project develops an academic Data Warehouse using a **star schema** to transform operational enrollment records into an analytical data model.

The dataset simulates student enrollments across six academic periods, from 2022-1 to 2024-2. The project explores how dimensional modeling, ETL processes, and analytical SQL queries can support institutional decision-making.

> **Data disclaimer:** All records are synthetically generated for educational purposes. The results do not represent actual institutional statistics.

## Objectives

- Design a dimensional model for academic data analysis.
- Build a star-schema Data Warehouse.
- Implement an ETL process using Python and DuckDB.
- Analyze academic performance and course approval rates.
- Explore patterns related to student persistence and academic risk.
- Generate visualizations and interpret analytical results.

## Tech Stack

- **Python** — data generation, transformation, and analysis.
- **Pandas** — data manipulation.
- **NumPy** — synthetic data generation.
- **DuckDB** — analytical database and SQL queries.
- **SQL** — dimensional modeling, ETL, and OLAP analysis.
- **Matplotlib & Seaborn** — data visualization.
- **Jupyter Notebook** — development and documentation.

## Data Warehouse Design

The warehouse follows a star-schema approach, organized around academic performance.

### Fact table

`hechos_rendimiento_academico`

Stores enrollment-level measures and academic outcomes.

### Dimension tables

- `dim_estudiante` — student attributes, including socioeconomic stratum and study schedule.
- `dim_asignatura` — course information, knowledge area, and credits.
- `dim_periodo` — academic period attributes.
- `dim_programa` — academic program information.

**Granularity:** Each fact record represents one student's enrollment in one course during one academic period.

## Analytical Queries

The project includes SQL analyses focused on:

1. Academic performance by program and academic period.
2. Courses with the highest number of failing grades in 2024.
3. Approval rates and earned credits by semester, socioeconomic stratum, and schedule.
4. Credit efficiency by academic program.
5. Academic risk patterns by knowledge area.

The notebook also includes visualizations and an institutional persistence analysis based on the generated data.

## Project Structure

```text
academic-data-warehouse/
├── README.md
├── Taller_Dimensional_DW_Jaramillo_Valencia.ipynb
└── dw_academico.duckdb  # Generated database, if exported
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/academic-data-warehouse.git
cd academic-data-warehouse
```

### 2. Install dependencies

```bash
pip install numpy pandas duckdb matplotlib seaborn jupyter
```

### 3. Run the notebook

```bash
jupyter notebook Taller_Dimensional_DW_Jaramillo_Valencia.ipynb
```

Run the cells in order to generate the synthetic enrollment data, build the Data Warehouse, execute analytical queries, and create visualizations.

## Key Concepts

- Dimensional modeling
- Star schema
- Fact and dimension tables
- Surrogate keys
- ETL pipelines
- SQL analytical queries and OLAP
- Data quality and integrity validation
- Academic performance analytics

## Limitations

The data is simulated, and the observed patterns depend on the assumptions used to generate it. The findings should not be interpreted as evidence about real students or institutions.

## Author

**Santiago Jaramillo Valencia**

Data Science Engineering Student  
Instituto Tecnológico Metropolitano (ITM)

---

*Academic project developed for the Advanced Topics in Databases course.*
