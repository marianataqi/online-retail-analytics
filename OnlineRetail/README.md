\# 📊 Online Retail Analytics Project



\## 📂 Project Overview

End-to-end analysis of the \*\*Online Retail\*\* dataset to design a star schema, compute business KPIs, segment customers (RFM/CLTV), and forecast sales with an LSTM model.  

Data is stored/queried in \*\*PostgreSQL\*\* and analyzed in \*\*Python\*\* (pandas, SQLAlchemy/psycopg2, matplotlib, seaborn) via Jupyter Notebooks.



---



\## 🧰 Tools \& Technologies

\- \*\*Database:\*\* PostgreSQL

\- \*\*Data Access:\*\* psycopg2, SQLAlchemy

\- \*\*Analysis \& Viz:\*\* Python (pandas, matplotlib, seaborn), Jupyter

\- \*\*ML:\*\* TensorFlow/Keras (for LSTM)



---



\## 📑 Notebooks



\### 1️⃣ Star Schema Modeling – 01 (`online\_retail\_starschema-01.ipynb`)

\- Clean \& transform raw dataset

\- Design \*\*Star Schema\*\* (Fact + Dimension tables)

\- Load into PostgreSQL for efficient querying



\### 2️⃣ Basic Sales Analysis \& KPIs – 02 (`online\_retail\_basic sales analysis \& KPIs-02.ipynb`)

\- \*\*Top 10 Customers by Spending\*\* → find high-value customers  

\- \*\*Top 10 Best-Selling Products\*\* → optimize product strategy  

\- \*\*Sales by Country\*\* → identify top markets  

\- \*\*Daily Sales Trend \& AOV\*\* → seasonality \& behavior  

\*\*Insights:\*\* revenue concentrated in few customers/products; UK dominates; seasonality suggests need for forecasting.



\### 3️⃣ RFM \& CLTV Analysis – 03 (`online\_retail\_RFM\_CLTV-Customer Segmentation-03.ipynb`)

\- Compute \*\*RFM\*\* metrics (Recency, Frequency, Monetary) via SQL

\- Segment customers (Champions, Loyal, At Risk, Lost)

\- Estimate \*\*CLTV\*\* (e.g., Monetary × Frequency) and tier via percentiles

\*\*Impact:\*\* prioritize high-value customers; targeted retention/marketing; base for predictive CLTV/churn.



\### 4️⃣ Sales Forecasting with LSTM – 04 (`online\_retail\_sales\_forecasting\_LSTM.ipynb`)

\- Aggregate \*\*daily sales\*\*, scale with MinMaxScaler

\- Create 30-day sequences → next-day prediction

\- Model: \*\*LSTM(50)\*\* → \*\*Dense(1)\*\*, loss \*\*MSE\*\*, optimizer \*\*Adam\*\*

\- \*\*Train/Test split ~85/15\*\*, evaluate with \*\*MAE\*\*

\- Generate \*\*14-day forecast\*\* and plot \*Actual vs Forecast\*



---



\## ▶️ How to Run

1\. Create a Python env and install requirements (pandas, numpy, matplotlib, seaborn, psycopg2, SQLAlchemy, tensorflow).  

2\. Ensure PostgreSQL is running; set connection string in notebooks if needed.  

3\. Open notebooks in Jupyter and run cells in order (01 → 04).



> Dataset: \*\*UCI Online Retail\*\* (2010–2011).



---



