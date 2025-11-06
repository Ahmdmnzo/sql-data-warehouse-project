## 📋 Data Warehouse Project

A production-grade data warehouse built with SQL Server, implementing the Medallion Architecture to integrate data from multiple source systems (ERP and CRM). This project demonstrates end-to-end data engineering capabilities including ETL pipeline development, dimensional modeling, and data quality management.

## 🏗️ Architecture

**Medallion Architecture - Three-Layer Design:**
- **Bronze Layer**: Raw data staging from ERP and CRM sources
- **Silver Layer**: Cleaned, validated, and conformed data
- **Gold Layer**: Star schema dimensional model (future implementation)

## 🛠️ Tech Stack

- **Database**: SQL Server Express
- **ETL**: SQL stored procedures and scripts
- **Design**: Star schema data modeling
- **Tools**: SSMS, Draw.io for architecture diagrams

## 💡 Key Features

- **Multi-source integration**: Combined ERP and CRM data into unified warehouse
- **Automated ETL pipeline**: Stored procedures for bronze and silver layer loads
- **Data standardization**: Cleansed and conformed data from disparate sources
- **Comprehensive documentation**: Data catalog, naming conventions, and architecture diagrams
- **Scalable design**: Layered architecture supports future enhancements

## 📁 Project Structure

```
data-warehouse-project/
├── datasets/
│   ├── source_crm/              # CRM system data
│   │   ├── cust_info.csv
│   │   ├── prd_info.csv
│   │   └── sales_details.csv
│   └── source_erp/              # ERP system data
│       ├── CUST_AZ12.csv
│       ├── LOC_A101.csv
│       └── PX_CAT_G1V2.csv
│
├── docs/
│   ├── data_architecture.png    # Overall DW architecture
│   ├── data_flow.png            # ETL flow diagrams
│   ├── data_integration.png     # Source integration design
│   ├── data_model.png           # Dimensional model design
│   ├── data_catalog.md          # Data dictionary
│   └── naming_conventions.md    # Naming standards
│
├── scripts/
│   ├── init_database.sql        # Database initialization
│   ├── bronze/
│   │   ├── ddl_bronze.sql       # Bronze layer table definitions
│   │   └── proc_load_bronze.sql # Bronze layer ETL procedures
│   └── silver/
│       ├── ddl_silver.sql       # Silver layer table definitions
│       └── proc_load_silver.sql # Silver layer ETL procedures
│
└── tests/                       # Test scripts and validation
```

## 🎓 Skills Demonstrated

- **ETL Development**: Built automated data pipelines using SQL stored procedures
- **Data Integration**: Combined multiple source systems with different schemas
- **SQL Development**: DDL, stored procedures, and data transformation logic
- **Data Architecture**: Implemented industry-standard Medallion Architecture
- **Documentation**: Created comprehensive technical documentation and diagrams
- **Data Modeling**: Designed scalable warehouse structure
