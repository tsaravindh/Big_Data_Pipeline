# Big_Data_Pipeline
Chicago Crime Data Pipeline
# Chicago Crime Arrest Prediction 🚔

This project leverages the **Chicago Crimes Dataset (2001–Present)** published by the Chicago Police Department to build an end-to-end machine learning pipeline on **AWS**. The goal is to analyze crime patterns and predict the likelihood of an arrest for reported crimes using distributed data processing and classification models.

---

## Project Overview

- Cleaned and processed millions of crime records using **AWS EMR (Apache Spark)**
- Extracted temporal features (hour, day of week, month) for better trend analysis
- Performed **EDA** to identify top crimes, arrest patterns, and yearly trends
- Built **Logistic Regression** and **Decision Tree** models to predict arrests
- Visualized results and stored predictions and charts on **AWS S3**

---

## Dataset Information

- Source: [City of Chicago Data Portal](https://data.cityofchicago.org)
- Size: ~8 million rows
- Features include:
  - Crime Type, Location, Community Area
  - Date/Time, Year, Arrest (Target Variable)

---

## Architecture

The pipeline consists of:
- **AWS S3**: Data storage
- **AWS EMR**: Data preprocessing and model training using Spark
- **Amazon Athena**: Query cleaned data from S3
- **ML Models**: Logistic Regression, Decision Tree
- **S3 Output**: Stores visualizations and predictions

See architecture diagram in `images/`.

---

## Technologies Used

- Python (PySpark, Pandas, Matplotlib)
- AWS EMR, Athena, S3, Step Functions
- Scikit-learn (for comparison)
- Jupyter Notebook

---

## Results

- Logistic Regression Accuracy: ~76%
- Decision Tree Accuracy: ~74%
- Arrests are highly predictable for certain crime types like narcotics and prostitution

---

## How to Run

1. Clone the repo:
   ```
   git clone https://github.com/YOUR_USERNAME/chicago-crime-arrest-prediction.git
   ```
2. Open the notebook in `notebooks/Final_Project.ipynb`
3. Upload data or connect to S3 bucket
4. Run each step from preprocessing to modeling

---

## Author

**Aravindh Tiruchirapalli Seetharaman**  
[aravindtststs@gmail.com]

---

## License


