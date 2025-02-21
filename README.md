# 🚀 Customer Sales ETL Pipeline

## 🌟 Project Overview
This project implements an **automated ETL pipeline** for **customer sales data**, enabling efficient **data extraction, transformation, and loading (ETL)** for business insights. The pipeline processes data from multiple CSV files, cleans and aggregates it, and loads it into a **MySQL database** for analysis. **Apache Airflow** is used to schedule and manage the workflow.

## 🔥 Key Features
- 📥 **Data Extraction**: Extracts and consolidates sales data from multiple CSV files.
- 🔄 **Data Transformation**: Cleans missing values, standardizes formats, and performs feature engineering.
- 🏦 **Data Storage**: Loads the transformed data into a **MySQL** database.
- 🎯 **Orchestration**: Manages the entire ETL process using **Apache Airflow**.
- 📊 **Scalability**: Designed for easy expansion and cloud integration.

## 🛠️ Technologies Used
- 🐍 Python
- 🌬️ Apache Airflow
- 🐼 Pandas
- 🛢️ MySQL
- 🐳 Docker *(optional for Airflow setup)*

## 📂 Project Structure
```
📦 customer-sales-etl
├── dags/          # Airflow DAG definitions
├── scripts/       # Python scripts for extraction, transformation, and loading
├── data/          # Sample sales data in CSV format
├── requirements.txt  # Required Python packages
└── README.md
```

## 🚀 How to Run the Project
### Prerequisites
- Install **Python 3.8+**, **MySQL**, and **Apache Airflow**.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/customer-sales-etl.git
   cd customer-sales-etl
   ```
2. Set up a virtual environment:
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Configure MySQL connection in `load.py`.
5. Start Apache Airflow:
   ```bash
   airflow db init
   airflow scheduler & airflow webserver
   ```
6. Trigger the ETL pipeline via Airflow.

## 📈 Conclusion
This project demonstrates a **complete ETL pipeline** for sales data processing, with automation and scheduling using **Apache Airflow**. It provides a scalable framework that can be adapted for real-world **data analytics** use cases.

## 🤝 Contributing
Contributions are welcome! Feel free to **fork the repo**, submit **pull requests**, or **open issues**.
