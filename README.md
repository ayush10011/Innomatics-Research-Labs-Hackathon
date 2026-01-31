# Innomatics-Research-Labs-Hackathon
Innomatics Research Labs | Advanced GenAI Internship | Entrance Test | Hackathon

# 🍔 Food Delivery Data Analytics Project

## 📌 Overview
This project simulates a **real-world food delivery platform** by integrating data from multiple sources and performing analytics to extract meaningful business insights.

The final merged dataset serves as the **single source of truth** for all analysis performed in this hackathon.

---

## 📂 Datasets Used
The project combines **three different data formats**, commonly found in production systems:

1. **orders.csv**  
   - Transactional data  
   - Order details, order amount, timestamps  

2. **users.json**  
   - User master data  
   - User details, city, membership type (Gold / Regular)  

3. **restaurants.sql**  
   - Restaurant master data  
   - Restaurant ID, city, cuisine type  

---

## 🔄 Data Integration Process
The datasets are merged using **LEFT JOINs** to ensure all orders are retained.

### Join Keys:
- `orders.user_id → users.user_id`
- `orders.restaurant_id → restaurants.restaurant_id`

### Final Output:
📁 **final_food_delivery_dataset.csv**

This final dataset is used for **all analysis and insights**.

---

## 📊 Analysis Performed
Using the final dataset, the following insights are derived:

-  Order trends over time  
-  User behavior patterns  
-  City-wise performance analysis  
-  Cuisine-wise revenue contribution  
-  Impact of Gold vs Regular membership  
-  Revenue distribution and seasonality  

---

## 🧠 Key Business Questions Answered
- Which city generates the highest revenue from Gold members?
- How does membership impact user spending?
- Which cuisines perform best in each city?
- What are peak ordering periods?

---

## 🛠️ Tools & Technologies
- Python (Pandas, JSON, SQL parsing)
- CSV, JSON, SQL data formats
- Jupyter Notebook / VS Code
- Git & GitHub

---

## 📁 Repository Structure
├── data/
│ ├── orders.csv
│ ├── users.json
│ └── restaurants.sql
├── final_food_delivery_dataset.csv
├── analysis.ipynb
└── README.md
