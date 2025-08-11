# 🛒 Sales Analytics & Customer Segmentation API

This project is a **Flask-based machine learning pipeline** designed to process sales datasets and generate:

- **Demand Segmentation** (High-demand & low-demand products)
- **Customer Segmentation** (VIP, Loyal, Lost, Occasional customers)
- **Market Basket Analysis (MBA)** with association rules (FP-Growth) and **Jaccard similarity** between products
- **Automated PDF Reports** with visualizations

It was originally built for the **AdventureWorks Sales Dataset**, but works for any dataset with the correct format.  
Sample reports are included in the `output_reports/` folder.

---

## 📂 Dataset Requirements

Sample sales dataset from AdventureWorks2019 is also added in output reports folder for reference. All the reports were generated on that dataset. 

Your input dataset must be a CSV file containing these columns:

| quantity | sale_date | product_id | unit_price | client_id | sale_id | total_price |
|----------|-----------|------------|------------|-----------|---------|-------------|
| 2        | 2024-01-05 | P001       | 15.5       | C101      | S001    | 31.0        |
| 1        | 2024-01-06 | P002       | 22.0       | C102      | S002    | 22.0        |

---

## ⚙️ Installation

```bash
git clone https://github.com/aribakhann2/flask_api.git
cd flask_api
python -m venv venv
source venv/bin/activate   # On Mac/Linux
venv\Scripts\activate      # On Windows
pip install -r requirements.txt
