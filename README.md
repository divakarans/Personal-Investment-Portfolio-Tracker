# 📊 Personal Investment Portfolio Tracker – Power BI Project

This project is a single-page Power BI dashboard that tracks and analyzes personal investment data across multiple brokers and asset types. Designed and developed by **Divakaran S**, the dashboard offers a visual and interactive breakdown of asset distribution, broker contributions, and monthly investment trends.

---

## 📁 Project Overview

- Visualizes investment value across different brokers like Zerodha, Binance, and ICICI Direct.
- Shows allocation by asset type (Crypto, Bonds, Mutual Funds, ETFs, etc.).
- Analyzes trading behavior through monthly quantity and total value line charts.
- Displays detailed table of assets with quantity and value.

---

## 🛠️ Tools & Technologies

- **Power BI**
- **Power Query Editor**
- **DAX**
- Data Source: Structured CSV files

---

## 📊 Key Visuals

- **Bar Chart**: Total investment by broker
- **Donut Chart**: Asset type distribution
- **Line Chart**: Monthly investment trend
- **Table**: Detailed view by asset
- **Cards**: Total Investment, Quantity, Highest Asset Value, etc.

---

## 🧹 Power Query Steps

- Removed placeholder values like `"--"` from Broker column
- Converted data types for numeric fields
- Removed duplicates and blank records

---

## 📌 DAX Measures Used

```DAX
Total Investment = SUM(InvestmentTransactions[TotalValue])
Total Quantity = SUM(InvestmentTransactions[Quantity])
Average Price Per Unit = [Total Investment] / [Total Quantity]
Highest Asset Value = MAXX(VALUES(Assets[AssetName]), CALCULATE(SUM(InvestmentTransactions[TotalValue])))
```

---

## 📷 Screenshots

![Screenshot 2025-06-13 115959](https://github.com/user-attachments/assets/faf65aaa-a3d1-4624-85f3-effbd8b24eb1)


---

## 👤 Author

**Divakaran S**

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/divakarans99) or explore more projects in this repository.

