# Call Duration and Sales Insights

Data analysis project exploring the relationship between call duration and sales conversion in a real-world call center operation.

## 🧩 Business Context

In a sales call center operation, each call represents a revenue opportunity. However, while an agent is engaged in a call, they are unable to attend new incoming customers.

When multiple calls extend in duration, operational capacity decreases and service levels begin to deteriorate.

This creates a natural operational tension: Should call duration be reduced to improve service levels, or should conversations be extended to increase the probability of closing a sale?

---

## ❓ Analytical Question

**Is there a relationship between call duration and the probability of closing a sale?**

---

## 🗂️ Data Source

This analysis was built using two independent systems:

- Call management system (operational data)  
- Sales tracking system (commercial data)  

Both datasets were linked using a composite key based on:
Date + Customer Phone Number + Agent ID

⚠️ **Note:**  
All data has been anonymized. No real customer or sensitive information is included.

---

## 🧹 Data Processing

The analytical dataset was constructed through a multi-step cleaning and validation process:

- Filtering connected calls with assigned agents  
- Removing records without confirmed sales  
- Validating customer phone consistency  
- Identifying and handling duplicates  
- Excluding records with operational inconsistencies  

The final dataset represents **valid customer interactions with confirmed sales outcomes**.

---

## 📈 Exploratory Analysis

The analysis included:

- Call duration histograms  
- Sales distribution across time intervals  
- Comparison between sales and renewals  
- Agent-level performance analysis (scatter plot)  
- Relationship between call volume and probability of sale  

---

## 🔍 Key Findings

- **65.6% of sales occur between 15 and 35 minutes**  
- The **probability of closing a sale increases with call duration**  
- Call volume drops significantly after 35 minutes  
- Top-performing agents operate between **17 and 25 minutes**  
- Three behavioral zones were identified:
  - Exploration (< 15 min)
  - Commercial conversation (15–35 min)
  - Extended negotiation (> 35 min)

---

## 💡 Key Insight

> Longer calls do not necessarily represent operational inefficiency. In many cases, they reflect ongoing negotiations with a higher probability of closing a sale.

---

## ⚖️ Business Implication

A strategy focused solely on reducing average call duration may negatively impact sales conversion.

This highlights a structural trade-off between **operational efficiency** and **commercial performance**.

---

## 🚀 Future Analysis

- How many interactions are required before a customer converts?  
- Behavioral analysis of non-converted calls  
- Early detection of high-potential long calls  
- Agent performance patterns  

---

## 📄 Full Report

The complete analysis report is available in Spanish:

[Download full report](./report/portafolio.pdf)

---

## 📁 Repository Structure
├── report/ │   └── portafolio.pdf │ ├── data/ │   └── dataset_anonymized.xlsx │ ├── analysis/ │   └── analysis_file.xlsx ├── images/ └── charts.png

---

## 🛠️ Tools Used

- Excel (data analysis, pivot tables, visualization)  
- Composite key data modeling  
- Exploratory data analysis techniques  

---

## 👤 Author

Alfredo Andres Gutierrez Vivius. B.Sc. Electronics Engineering.  M.Sc. Mechanical Engineering

This project was developed as an applied data analysis case based on a real-world sales operation.


