# AfriTech Brand Health & Product Risk Assessment  
*A Data-Driven Evaluation of Customer Experience, Product Performance & Market Perception*

🔗 **Power BI Dashboard:** _Coming Soon_  
Interactive analytics built using SQL insights, DAX modeling, and imported analytical tables.

---

## 📌 Table of Contents
- [Description](#description)
- [Business Introduction](#business-introduction)
- [Business Challenge](#business-challenge)
- [Aim](#aim)
- [Data Points for Analysis](#data-points-for-analysis)
- [Processes](#processes)
  - [1. SQL Data Preparation & Cleanup](#1-sql-data-preparation--cleanup)
  - [2. Power BI Modeling & Dashboard Development](#2-power-bi-modeling--dashboard-development)
- [Key Insights](#key-insights)
- [Recommendations](#recommendations)
- [Technology Stack](#technology-stack)

---

## Description
This project evaluates AfriTech Electronics’ brand perception, customer satisfaction, product reliability, and competitive positioning.

Using **SQL** and **Power BI**, this analysis uncovers how product recalls, customer service performance, and social media sentiment shape revenue, loyalty, and brand trust.

The project forms part of my job as a data consultant at **Amdari**, demonstrating end-to-end analytics from database structuring to BI storytelling.

---

## Business Introduction
AfriTech Electronics is a consumer electronics company serving **200 customers** across **49 regions**.  
The customer base represents a balanced demographic with:

- **Average Income:** 61.1K  
- **Average Age:** 44  
- **Customer Types:** New, Returning, VIP  

This analysis helps AfriTech understand key brand health drivers across sentiment, product performance, service quality, and customer behavior.

---

## Business Challenge

### 1. **Negative Social Media Buzz**
A surge in critical posts about product issues and slow customer service is harming brand sentiment and trust.

### 2. **Customer Complaints**
Defect, billing, and support-related complaints are increasing, with long response times accelerating customer frustration.

### 3. **Product Recalls**
Frequent recalls have created concern among customers and reduced confidence in product reliability.

### 4. **Competitive Pressure**
Competitors are gaining market share by positioning themselves as more reliable alternatives.

---

## Aim
- Analyze customer, transaction, and social media interaction data using SQL.  
- Build a Power BI dashboard summarizing brand health, sentiment, product performance, and service metrics.  
- Quantify recall risks, revenue exposure, and customer churn risk.  
- Provide strategic recommendations to help AfriTech rebuild trust, reduce recalls, and improve overall customer satisfaction.

---

## Data Points for Analysis

### **Customer Information**
- CustomerID  
- Customer Name  
- Region  
- Age  
- Income  
- CustomerType (New, Returning, VIP)

### **Transaction Information**
- Transaction Date  
- Transaction Year  
- Product Purchased (Smartphone, Laptop, Tablet, Smartwatch)  
- Purchase Amount  
- Product Recalled (True/False)  
- Competitor (if any)

### **Social Media Interaction Data**
- Interaction Date  
- Platform (Twitter, Facebook, Instagram, LinkedIn, TikTok)  
- Post Type (Text, Image, Video, Link, Story)  
- Likes, Shares, Comments  
- User Followers  
- Influencer Score  
- Brand Mention  
- Competitor Mention  
- Sentiment (Positive, Neutral, Negative)  
- Crisis Event Time  
- First Response Time  
- Resolution Status  
- NPS Response  

---

## Processes

---

### 1. SQL Data Preparation & Cleanup
- Removed blank fields and null values  
- Standardized and reformatted date types  
- Extracted **Transaction Year** for time-series analysis  
- Converted the raw dataset into **three normalized tables**:
  1. Customers  
  2. Transactions  
  3. Social Media Interactions  

### **SQL-Based Insights Extracted**
- Recall rates  
- Revenue at risk  
- NPS scoring  
- Churn risk model  
- Sentiment classification  
- Share of Voice analysis  
- Response time calculations  

Some outputs (NPS, SOV, sentiment) were imported **directly** from SQL into Power BI for accuracy.

---

### 2. Power BI Modeling & Dashboard Development

#### ✔ Created a Complete Date Table  
Enabled:
- Weekly, Monthly, Quarterly trends  
- Time intelligence (YoY, MoM)  
- Rolling periods  

#### ✔ Imported SQL Tables
- NPS scoring table  
- Sentiment model output  
- Competitor SOV table  

#### ✔ Developed DAX Measures
- Revenue at Risk  
- Avg Response Time (6.4 months)  
- Resolution Rate (48%)  
- CSAT (41%)  
- Sentiment distribution  
- Engagement metrics  
- Churn-risk segmentation  
- Customer type distribution  

#### ✔ Dashboard Views Included
- Customer Insights Overview  
- Sentiment Breakdown by Type  
- Age & Income Distribution  
- Geographic Spread of Customers  
- Churn Risk Dashboard  
- Highest-Value Customers  
- Product Recall Analysis  
- Share of Voice vs Competitors  

---

## Key Insights

### ⭐ **200 Customers Across 49 Regions**
A diverse customer base with strong potential for targeted support and engagement.

### ⭐ **Sentiment Mix**
- Positive: 41.01%  
- Neutral: 40.8%  
- Negative: 18.19%  

### ⭐ **High Churn Risk (64.59%)**
A large portion of customers fall under “Churn Risk.”

### ⭐ **Service Response Time is Extremely High**
Average: **6.4 months**, a major driver of dissatisfaction.

### ⭐ **Laptop Line Requires Urgent Attention**
It is both the **top-selling** and **most-recalled** product.

### ⭐ **Share of Voice**
- AfriTech: 50.6%  
- Competitors: 49.4%  

Volume is strong, but sentiment is weak.

---

## Recommendations

A multi-dimensional improvement strategy is required to reduce recall frequency, improve service delivery, and restore public confidence.

---

### **1. Prioritize and Fast-Track VIP Customers**
- Introduce a VIP-only support queue.  
- Assign dedicated account specialists.  
- Offer priority resolutions and post-resolution follow-ups.  

This will significantly reduce churn among the highest-value customers.

---

### **2. Reduce Recall Rates — Especially for the Laptop Line**
- Conduct root-cause failure analysis.  
- Strengthen manufacturing QA.  
- Provide firmware/hardware updates where needed.  
- Address usability complexity for older customers.  

The Laptop is both the revenue engine and the highest risk product.

---

### **3. Overhaul Customer Service and Reduce Response Times**
- Implement automated ticket triage.  
- Establish strict SLAs for response and resolution.  
- Expand support channels (WhatsApp, live chat, call-back).  
- Track performance daily for SLA compliance.  

Reducing response time will immediately improve CSAT and sentiment.

---

### **4. Monitor Critical KPIs Consistently**
#### **Service KPIs**
- Resolution Time    
- CSAT  
- Response Time 

#### **Brand Health KPIs**
- Share of Voice  
- Sentiment Category Trends    

#### **Operational KPIs**
- Recall rates by product  
- Repeat complaint volume  
- NPS trends  

Routine KPI monitoring provides early warning signals for retention and reputation risks.

---

### **5. Improve Recall Data Quality (Key Dataset Limitation)**
Most recall entries lacked a **reason for recall**, which prevents identifying root causes.

Recommend:  
- Adding a mandatory “Reason for Recall” field  
- Tagging recalls (Hardware, Software, Usability, Battery, Damage, etc.)  
- Logging detailed explanations for analytics  

This will help reduce future recall frequency through targeted fixes.

---

### **6. Support the 41+ Age Segment More Effectively**
The majority of customers — especially those experiencing Laptop recalls — are aged **41 and above**.

Recommended support:  
- Beginner-friendly setup guides  
- Clear illustrated manuals  
- Video tutorials  
- Senior support line  
- Optional virtual onboarding sessions  

This reduces usability-driven frustration and recall requests.

---

### **7. Improve Brand Sentiment Through Transparent Communication**
- Announce fixes to major product issues  
- Communicate improvements in response times  
- Publish educational content  
- Use influencer partnerships strategically  

Stronger sentiment builds trust and reduces churn.

---

### **8. Strengthen Engagement on High-Performing Social Platforms**
Focus on TikTok, Instagram, LinkedIn, and Twitter where engagement is highest.

Actions:  
- Targeted ads  
- Fast-response teams  
- Sentiment-driven campaigns  
- Educational product content  

Maintaining positive engagement strengthens AfriTech’s public brand voice.

---

### **9. Conduct Usability Testing for Key Product Lines**
Especially the Laptop, to ensure:  
- Accessibility  
- Simplicity  
- Compatibility with older demographics  

This ensures products align with customer needs.

---


This holistic program strengthens trust and long-term brand loyalty.

---

## Technology Stack

### **PostgreSQL**
- Data storage  
- SQL analysis  
- Views & stored procedures  
- Performance optimization  

### **Power BI**
- Data modeling  
- DAX calculations  
- Time series intelligence  
- Interactive dashboard development  

---
