# 🛒 User Funnel & Revenue Analytics Dashboard

> An end-to-end data analytics project analyzing **20,000 user sessions** using **Python** and **Pandas** to uncover conversion bottlenecks, revenue patterns, and channel performance. Identified a **59.62%** checkout drop-off rate and built an interactive **Power BI** dashboard segmenting revenue by channel, region, device, and product category to surface actionable growth insights.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)

---

## 📌 Problem Statement

E-commerce and fintech platforms lose a majority of users between browsing and purchase. Without granular funnel data, product teams are flying blind on **where** users drop off and **why** revenue is being left on the table.

This project answers:
- Where exactly in the user journey are we losing customers?
- Which marketing channels drive the most revenue?
- Which product categories and regions generate the highest returns?
- Does device type affect conversion or session behavior?

---

## 🏗️ Project Architecture

<img width="590" height="1295" alt="Untitled design" src="https://github.com/user-attachments/assets/2e1b6a0a-78d6-4e25-8673-586a868b5f7b" />

## 📊 Dataset Overview

| Property | Details |
|---|---|
| **Total Records** | 20,000 user sessions |
| **Key Columns** | Session_ID, User_ID, Event, Device, Channel, Region, Product_Category, Revenue, Day |
| **Funnel Stages** | Browse → Add to Cart → Checkout → Purchase |
| **Channels** | Email, Google Ads, Social Media, Organic |
| **Regions** | East, West, North, South |
| **Devices** | Mobile, Tablet, Desktop |
| **Product Categories** | Electronics, Fashion, Home, Sports, Beauty |

---

## 🔍 Key Findings

### 1. Funnel Drop-Off Analysis
The most critical insight of the entire project:

| Stage | Sessions | Conversion Rate | Drop-Off Rate |
|---|---|---|---|
| Browse | 12,500 | 100.00% | 0.00% |
| Add to Cart | 5,200 | 41.60% | **58.40%** |
| Checkout | 2,100 | 16.80% | **59.62%** |
| Purchase | 950 | 7.60% | **54.76%** |

**Critical Insight:** Only **7.6% of users** who browse actually complete a purchase. The steepest drop-off happens at **Add to Cart → Checkout (59.62%)**, indicating friction in the checkout experience — likely UX issues, unexpected costs, or lack of trust signals.

**Business Recommendation:** Prioritize checkout UX optimization, add trust badges, and implement cart abandonment email flows targeting the 58.4% drop-off at Add to Cart.

---

### 2. Revenue by Marketing Channel

| Channel | Revenue Share | Insight |
|---|---|---|
| Email | Highest (~0.3M) | Best ROI channel |
| Google Ads | Second (~0.3M) | High spend, high return |
| Social Media | Third (~0.28M) | Strong mid-funnel |
| Organic | Lowest (~0.25M) | Needs SEO investment |

**Insight:** Email drives the highest revenue — suggesting that retargeting and lifecycle email campaigns should be scaled aggressively.

---

### 3. Revenue by Region

| Region | Revenue | Share |
|---|---|---|
| East | 312.15K | 26.53% |
| South | 304.29K | 25.87% |
| West | 283.26K | 24.08% |
| North | 276.71K | 23.52% |

**Insight:** Revenue is relatively evenly distributed across regions, but **East leads at 26.53%** — making it a priority market for targeted campaigns.

---

### 4. Device Distribution
Sessions are almost equally split across devices:
- Mobile: 33.36%
- Desktop: 33.36%
- Tablet: 33.28%

**Insight:** Uniform device distribution means the platform must be **fully optimized across all three device types** — no single device can be deprioritized.

---

### 5. Revenue by Product Category
Electronics leads revenue followed closely by Fashion, Home, Sports, and Beauty — indicating a **balanced product portfolio** with no single category dominating.

---

### 6. Daily Revenue Trend
Revenue peaks around **Day 5 (~50K)** and maintains between 30K-50K through mid-month before declining toward Day 30 (~18K).

**Insight:** End-of-month revenue dip suggests opportunity for flash sales or promotional campaigns in the final week of each month.

---

## 🛠️ Tech Stack & Why

| Tool | Purpose | Why chosen |
|---|---|---|
| **Python** | Data cleaning, preprocessing, drop-off calculations | Fast manipulation of 20K row datasets |
| **Pandas** | Aggregation, groupby, funnel stage mapping | Industry standard for tabular data analysis |
| **Power BI** | Interactive dashboard creation | Best-in-class for business stakeholder reporting |
| **Excel** | Funnel summary table, quick pivots | Universal format for sharing insights with non-technical teams |

---

## 📈 Dashboard Screenshots

### Funnel Analysis + Channel Revenue + Region Revenue
<img width="1167" height="632" alt="Screenshot 2026-06-27 165845" src="https://github.com/user-attachments/assets/850741c3-28b9-4943-ae83-ddd36bba0c91" />

### Revenue Treemap + Daily Trend + Device Sessions
<img width="1120" height="587" alt="Screenshot 2026-06-27 165927" src="https://github.com/user-attachments/assets/ff715983-8eb0-4600-afb3-8e98262e5e29" />

### Device Distribution + Product Category Revenue + Daily Sessions
<img width="1163" height="636" alt="Screenshot 2026-06-27 165944" src="https://github.com/user-attachments/assets/43152135-3628-459a-a049-63a9a9a0aaf0" />

### Funnel Drop-Off Summary Table
<img width="671" height="130" alt="Screenshot 2026-06-27 170008" src="https://github.com/user-attachments/assets/f597e482-ca94-43cc-a1fa-a4acea2a031a" />

---

## 💡 Business Impact

If the **Add to Cart → Checkout drop-off** (59.62%) were reduced by just 10%:
- ~520 additional users reach checkout per cohort
- At current checkout→purchase rate (45.2%), that's ~235 additional purchases
- At average order value, this represents **significant incremental revenue per campaign cycle**

This kind of analysis is used to **prioritize engineering sprints and marketing budgets.**

---

## 🔮 Future Scope

- [ ] **Cohort Analysis** — track how conversion rates change for users acquired in different months
- [ ] **A/B Test Framework** — simulate impact of UI changes on funnel drop-off
- [ ] **Predictive Model** — use logistic regression to predict which users are likely to purchase
- [ ] **Real-time Dashboard** — connect to live data via API instead of static dataset
- [ ] **Customer Segmentation** — RFM (Recency, Frequency, Monetary) analysis for targeted campaigns

---

