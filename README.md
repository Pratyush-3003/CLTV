# 🧮 Customer Lifetime Value (CLTV) Prediction

## 📌 Project Overview

This project aims to predict Customer Lifetime Value (CLTV) using past purchase behavior. CLTV is a crucial metric for businesses to understand the total revenue a customer is expected to generate over their relationship with the company. The project leverages statistical models and machine learning techniques to make accurate predictions.

## 🔍 Features

- **Data Preprocessing**: Cleaning and transforming raw transaction data.
  
- **Feature Engineering**: Extracting meaningful features from customer purchase history.
  
- **CLTV Calculation**: Implementing traditional statistical formulas.
  
- **Machine Learning Models**: Using regression techniques to predict CLTV.
  
- **Visualization**: Analyzing customer spending patterns using charts.
  
- **Streamlit GUI**: A user-friendly web app to upload CSVs, run the prediction models, and visualize CLTV results interactively.

## 📲 Streamlit Web App

We developed a **Streamlit-based GUI** to make the CLTV prediction tool accessible to non-programmers:

- Upload transaction data in `.csv` format.
  
- Automatically computes frequency, recency, T (customer age), and monetary value.
  
- Fits probabilistic models (`BG/NBD` and `Gamma-Gamma`) using the `lifetimes` library.
  
- Predicts number of future purchases and average transaction value.
  
- Displays CLTV prediction table and visualizes CLTV distribution using histograms.

✅ Hosted using **ngrok** for public sharing (ideal for testing and demos in Colab).

## 📂 Dataset

The dataset consists of transactional records with fields such as:

- `InvoiceNo`: Unique invoice identifier
  
- `StockCode`: Product code
  
- `Description`: Product description
  
- `Quantity`: Number of units purchased
  
- `InvoiceDate`: Date of purchase
  
- `UnitPrice`: Price per unit
  
- `CustomerID`: Unique customer identifier
  
- `Country`: Country of transaction

## ⚙️ Technologies Used

- **Python**: Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
  
- **Statistical Modeling**: `lifetimes` library for BG/NBD and Gamma-Gamma models
  
- **Machine Learning**: Linear Regression, Decision Trees (optional model-based extension)
  
- **GUI**: Streamlit for interactive web interface
  
- **Visualization**: Matplotlib, Seaborn
  
- **Platform**: Google Colab for development, Pyngrok for sharing
