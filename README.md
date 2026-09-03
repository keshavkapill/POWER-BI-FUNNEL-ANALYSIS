# 📊 SQL + Power BI Funnel & Revenue Analysis

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,14,16,18&height=220&section=header&text=Funnel%20%26%20Revenue%20Analysis&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=35"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/SQL-SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white"/>
  <img src="https://img.shields.io/badge/Power%20BI-Data%20Visualization-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
  <img src="https://img.shields.io/badge/DAX-Analytics-512BD4?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Analytics-Funnel%20Analysis-6A5ACD?style=for-the-badge"/>
</p>

<p align="center">
  <b>Turning raw user-event data into actionable funnel, revenue, and customer insights.</b>
</p>

---

## 🚀 Project Overview

This project analyzes an e-commerce customer journey using **SQL and Power BI**.

The analysis focuses on understanding how users move through the funnel:

```text
Browse → Add to Cart → Checkout → Purchase
```

The project combines:

* 🗄️ **SQLite** for data storage and SQL analysis
* 🔎 **SQL** for extracting and transforming data
* 📊 **Power BI** for interactive visualization
* 🧮 **DAX** for calculated metrics
* 📈 **Business Analytics** for identifying trends and opportunities

The goal is to understand **user behavior, conversion performance, revenue generation, traffic sources, and customer drop-offs**.

---

## 🎯 Business Objectives

The analysis aims to answer questions such as:

* How many users are entering the funnel?
* How many users reach each funnel stage?
* Where is the largest drop-off occurring?
* What percentage of users complete a purchase?
* Which traffic sources generate the most revenue?
* Which devices generate better revenue performance?
* What events contribute most to the customer journey?
* How can conversion rates be improved?

---

## 🧰 Tech Stack

| Technology                | Purpose                   |
| ------------------------- | ------------------------- |
| 🗄️ SQLite                | Database management       |
| 💻 SQL                    | Data querying & analysis  |
| 📊 Power BI               | Dashboard & visualization |
| 🧮 DAX                    | Calculated metrics        |
| 🐍 Python                 | Supporting data analysis  |
| 📁 CSV                    | Source dataset            |
| 🖥️ DB Browser for SQLite | Database exploration      |

---

## 📂 Project Structure

```text
Funnel-Revenue-Analysis/
│
├── client_site_dataset.csv
│
├── funnel_analysis.db
│
├── funnel_analysis.sqbpro
│
├── sql/
│   └── funnel_analysis_queries.sql
│
├── PowerBI/
│   └── Funnel_Revenue_Analysis.pbix
│
├── screenshots/
│   ├── dashboard.png
│   ├── funnel.png
│   └── revenue_analysis.png
│
└── README.md
```

---

# 📊 Dataset

The project uses an event-based customer interaction dataset:

```text
client_site_dataset.csv
```

The dataset contains information related to:

* Users
* Sessions
* Events
* Devices
* Traffic sources
* Products
* Revenue
* Customer journey stages

The database created from the dataset is:

```text
funnel_analysis.db
```

---

# 🗄️ Database

SQLite is used as the project's relational database.

The database can be opened using:

**DB Browser for SQLite**

The project database file is:

```text
funnel_analysis.db
```

The SQLite project file is:

```text
funnel_analysis.sqbpro
```

---

# 🔎 SQL Analysis

SQL is used to extract meaningful insights from the raw event data.

The main SQL queries are available inside:

```text
sql/funnel_analysis_queries.sql
```

### SQL concepts used

* `SELECT`
* `WHERE`
* `GROUP BY`
* `ORDER BY`
* `HAVING`
* `JOIN`
* `COUNT`
* `SUM`
* `AVG`
* `CASE`
* `DISTINCT`
* Subqueries
* Aggregations
* Conditional calculations

---

# 🔄 Customer Funnel

The customer journey is analyzed using four major stages:

```text
┌───────────────┐
│    BROWSE     │
└───────┬───────┘
        ↓
┌───────────────┐
│  ADD TO CART  │
└───────┬───────┘
        ↓
┌───────────────┐
│   CHECKOUT    │
└───────┬───────┘
        ↓
┌───────────────┐
│   PURCHASE    │
└───────────────┘
```

This allows the business to identify exactly where customers leave the purchasing journey.

---

# 📈 Key Metrics

The analysis contains approximately:

| Metric             |       Value |
| ------------------ | ----------: |
| 👥 Unique Users    |      10,000 |
| 🔄 Unique Sessions |      10,000 |
| 🖱️ Total Events   |      21,409 |
| 💰 Total Revenue   | $277,323.06 |

---

# 🚨 Funnel Drop-Off Analysis

One of the major findings is the significant drop between:

```text
Checkout → Purchase
```

The approximate drop-off at this stage is:

### 🔻 ~70.9%

This indicates that a large percentage of users who reach checkout do not complete their purchase.

### Possible business considerations

* Improve checkout experience
* Reduce checkout friction
* Simplify payment process
* Investigate payment failures
* Improve trust signals
* Optimize page performance
* Provide clearer pricing information

---

# 💰 Revenue Analysis

Revenue was analyzed across multiple dimensions.

### Traffic Source

The analysis indicates that:

> **Google Ads contributes the highest revenue among the analyzed traffic sources.**

This can help determine where marketing investment is generating the strongest financial return.

---

# 💻 Device Analysis

Device-level analysis was performed to understand differences in customer behavior.

The analysis indicates:

> **Desktop users generate the highest revenue per event.**

This can be useful when prioritizing optimization efforts across different device experiences.

---

# 📊 Power BI Dashboard

Power BI is used to transform the SQL analysis into an interactive dashboard.

The dashboard focuses on:

### 📌 Funnel Performance

* Users at each stage
* Conversion rates
* Drop-off rates
* Funnel visualization

### 💰 Revenue Performance

* Total revenue
* Revenue by source
* Revenue by device
* Revenue trends

### 👥 User Behavior

* User activity
* Session activity
* Event distribution
* Customer journey

### 📈 Business Insights

* Highest-performing channels
* Highest-performing devices
* Funnel bottlenecks
* Revenue opportunities

---

# 🧮 DAX

DAX is used within Power BI to create calculated metrics and measures.

Examples include:

```text
Total Revenue
Total Users
Total Sessions
Conversion Rate
Drop-off Rate
Revenue per Event
```

DAX allows the dashboard to dynamically calculate and visualize business metrics.

---

# 🔄 Project Workflow

```text
             RAW CSV DATA
                  │
                  ▼
        ┌──────────────────┐
        │  SQLite Database  │
        └────────┬─────────┘
                 │
                 ▼
          SQL DATA ANALYSIS
                 │
                 ▼
       ┌────────────────────┐
       │ Business Metrics   │
       │ & Insights         │
       └─────────┬──────────┘
                 │
                 ▼
            POWER BI
                 │
                 ▼
       INTERACTIVE DASHBOARD
                 │
                 ▼
         BUSINESS DECISIONS
```

---

# 🛠️ How to Use

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/keshavkapill/REPOSITORY-NAME.git
```

```bash
cd REPOSITORY-NAME
```

Replace `REPOSITORY-NAME` with the actual name of your GitHub repository.

---

## 2️⃣ Open the Database

Open:

```text
funnel_analysis.db
```

using **DB Browser for SQLite**.

---

## 3️⃣ Run SQL Queries

Open:

```text
sql/funnel_analysis_queries.sql
```

Execute the queries inside SQLite to reproduce the analysis.

---

## 4️⃣ Open Power BI

Open:

```text
Funnel_Revenue_Analysis.pbix
```

using Microsoft Power BI Desktop.

---

# 🖼️ Dashboard Preview

> Keep your existing project screenshots/images here.

```text
screenshots/
├── dashboard.png
├── funnel.png
└── revenue_analysis.png
```

If your original README already contains image links, **keep those exact image lines** instead of replacing them.

---

# 💡 Business Recommendations

Based on the analysis, the following improvements can be considered:

### 1. Optimize Checkout

The Checkout → Purchase stage shows the largest funnel drop-off.

### 2. Improve Payment Experience

Investigate unsuccessful transactions and simplify payment flows.

### 3. Focus on High-Revenue Channels

Google Ads demonstrates strong revenue contribution and can be analyzed further for campaign-level optimization.

### 4. Optimize Desktop Experience

Since desktop users show strong revenue per event, maintaining a smooth desktop experience can support revenue performance.

### 5. Monitor Funnel Conversion

Track conversion rates continuously to identify changes in customer behavior.

---

# 🧠 Challenges

During the project, several analytical challenges were addressed:

* Understanding event-based customer data
* Converting raw events into funnel stages
* Calculating meaningful conversion metrics
* Handling aggregations in SQL
* Connecting SQL analysis with Power BI
* Creating meaningful DAX measures
* Identifying actionable business insights
* Designing a dashboard that communicates findings clearly

---

# 📚 Learning Outcomes

Through this project, I strengthened my understanding of:

* SQL
* SQLite
* Data Cleaning
* Data Transformation
* Funnel Analysis
* Revenue Analysis
* Power BI
* DAX
* Data Visualization
* Business Intelligence
* Customer Journey Analytics
* Data-driven Decision Making

---

# 🚀 Future Improvements

Potential improvements include:

* Real-time dashboard integration
* More advanced customer segmentation
* Cohort analysis
* Customer lifetime value analysis
* Marketing campaign ROI analysis
* Time-based funnel analysis
* Automated reporting
* Predictive conversion modeling
* Advanced Power BI dashboards

---

# 👨‍💻 About Me

### Keshav Kapil

BTech CSE student interested in:

* 💻 Software Development
* 📊 Data Analytics
* ☁️ Cloud Computing
* 🧠 Data Structures & Algorithms
* 🌐 Full Stack Development

---

# 🤝 Connect With Me

<p align="center">

<a href="https://github.com/keshavkapill">
<img src="https://img.shields.io/badge/GitHub-Keshav%20Kapil-181717?style=for-the-badge&logo=github"/>
</a>

<a href="https://www.linkedin.com/in/keshavkapil15/">
<img src="https://img.shields.io/badge/LinkedIn-Keshav%20Kapil-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

</p>

---

<p align="center">
  ⭐ If you found this project useful, consider giving it a star!
</p>
