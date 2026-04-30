🛒 AI-Powered Demand Forecasting System — Indian E-Commerce

An intelligent demand forecasting and inventory decision-support system built for the Indian e-commerce market, covering 6 cities, 20 product categories, and 100 SKUs over a 10-year period (2015–2024).


📌 Problem Statement

Businesses in the Indian e-commerce sector suffer significant revenue losses due to inaccurate demand predictions — leading to either overstocking (capital tied up in unsold inventory) or stockouts (lost sales and poor customer experience). Traditional forecasting models fail to account for India-specific factors like festivals, regional demand patterns, and macro-economic events.

💡 Our Approach

We built a context-aware, AI-powered forecasting system that goes beyond simple prediction — acting as a virtual AI Store Manager that provides actionable inventory decisions.

✨ Key Features

📊 Context-Aware Forecasting
Unlike traditional models, our system considers:

Indian festival calendar (Diwali, Holi, Independence Day, etc.)
Macro-economic market events (Demonetisation 2016, GST rollout 2017, COVID lockdowns 2020–21, Quick Commerce Era 2023+)
Seasonal & temperature effects on category-specific demand
City-level demand multipliers across Delhi, Mumbai, Bangalore, Chandigarh, Jaipur, Lucknow

🤖 AI Store Manager (In Development)
The system doesn't just predict demand — it provides actionable recommendations:

How much stock to order
Whether to apply discounts
Optimal restock timing per SKU

⚠️ Smart Risk Scoring Engine
For every product-city-week combination, the system computes:

Stockout Risk — probability that current stock won't meet demand
Overstock Risk — probability of excess unsold inventory
Combined Risk Score — helping businesses prioritize which SKUs need immediate attention

📦 Product-Level Granularity

20 categories × 5 SKUs each = 100 unique products
Individual SKU tracking with price, units sold, discount, and stock levels
Spike detection for sudden demand surges

🔁 Time-Series Feature Engineering

Lag features: lag_1, lag_4, lag_52 (captures weekly, monthly, yearly patterns)
Rolling averages: 4-week and 12-week windows
Trend indicators derived from lag differences


🗂️ Dataset Overview
PropertyDetailsTime Range2015–2024 (weekly data)CitiesDelhi, Mumbai, Bangalore, Chandigarh, Jaipur, LucknowCategories20 (Electronics, Clothing, Groceries, Mobiles, etc.)Products100 SKUsFeatures30+ columns including risk scores, lag features, market eventsKey Columnsunits_sold, sales, discount, current_stock, stockout_risk, overstock_risk, risk_score

🧠 Tech Stack
LayerToolsLanguagePythonML ModelsXGBoost, Random ForestData ProcessingPandas, NumPyFeature EngineeringLag features, rolling stats, spike detectionVisualization(Dashboard — In Progress)AI ChatbotGrok API (system prompt-based assistant for inventory queries)

📁 Project Structure
demand-forecasting/
│
├── data/
│   └── final_indian_ecommerce_dataset.csv   # Generated dataset
│
├── notebooks/
│   └── Forecast_Demand.ipynb                # Main notebook (EDA + Feature Engineering)
│
├── models/
│   └── xgboost_model.pkl
│
├── dashboard/
│   └── app.py
│
└── README.md

✅ What the System Delivers

✔️ XGBoost/Random Forest model training & evaluation
✔️ AI Store Manager — actionable restocking recommendations
✔️ Risk scoring engine for stockout & overstock decisions
✔️ Multi-city, multi-category demand analysis
✔️ AI Chatbot (Grok API) for natural language inventory queries
✔️ Logistics-aware demand adjustment

Author 
jaspreet kaur | BE CSE AIML
