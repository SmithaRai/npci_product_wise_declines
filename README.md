# npci product wise declines analysis 

NPCI, a key player in India's dynamic retail payment landscape, offers a variety of products. To ensure its continued success, it's crucial to analyze transaction volume and decline rates across these products. By delving into product-specific decline rates, we can gain valuable insights into the performance and growth of each offering. This analysis will empower us to develop actionable recommendations for improvement.

## **problem statement**
By analyzing decline data for each product, we can identify the root causes of these failures and develop strategies to improve success rates.

## **Outcomes**
Identify Products with High Decline Rates
Understand Reasons for Declines
Prioritize Improvement Strategies

## **Questions to ask**
decline rate experienced in each product
which decline type is high and in which product
what is the decline rate trend over time for each product(monthly, yearly)?
which issuer bank is facing tremendous decline issues and for which product
which year experienced increased and also low declines 
bottom 5 issuer banks based on the approved transaction value
top 5 issuer banks by technical declines

## **Dataset Description**
#### 1.**id** : Unique identifier for each row.
#### 2.**date** : date of transaction
#### 3.**product** : product used for transaction
#### 4.**issuer_bank** : Bank issuing the card to the customer.
#### 5.**total_volume** : transaction volume
#### 6.**approved_transaction_volume** : number of approved transactions for each issuer bank.
#### 7.**business_decline_transactions** : declines  due to factors related to the transaction itself or the customer for each issuer bank.
#### 8.**technical_decline_transactions** : declines due to issues with NPCI's infrastructure, bank systems, or network problems for each issuer bank.
#### 9.**month** : month wise transactions
#### 10.**year** : year wise transactions

### **Dataset Overview : Key Statistics and Shape**
  **Missing Values** :no missing values
  **Complete Data** : 2300 rows,10 columns

## **Analysis insights**

### **NFS Payments**

**Positive Trends**: Overall transaction volume (both total and approved) has shown steady year-over-year growth, indicating a healthy increase in NFS usage.
**Business Declines**: While business declines did increase in 2022, they recovered and decreased in the following year, suggesting a temporary disruption that was successfully addressed.
**Technical Declines**: Technical declines have been consistently decreasing year-on-year, demonstrating improvements in the system's reliability.
**Month-wise Trends**: Month-wise data doesn't reveal a clear pattern, indicating potential seasonal variations or other factors that require further investigation.

### **AEPS Payments**

**Volatile Performance**: Unlike NFS, AEPS transactions exhibited significant fluctuations. Total transactions saw a rise in 2022 followed by a decline the next year. Approved transactions also dropped after 2021, suggesting potential issues with user adoption or service disruptions.
**Business Declines**: Business declines for AEPS transactions were significantly higher compared to NFS, and they further increased in 2022 before showing a gradual decrease. This highlights potential challenges specific to AEPS that need to be addressed.
**Technical Declines**: AEPS experienced consistently higher technical declines compared to NFS, with a steeper increase in 2022 followed by a gradual decrease. This suggests that the AEPS system might require additional focus on technical improvements.
**Month-wise Anomaly**: Notably, the month-wise line chart revealed a concerning dip in approved transactions for December 2022 in AEPS, requiring immediate investigation to identify and rectify the cause.

### **Issuer Banks Analysis**

**Top Technical Decline Issuers**: The top five banks contributing to technical declines (Bank of Maharashtra, Indian Overseas Bank, Indian Bank, UCO Bank, and Andhra Pragathi Grameen Bank) warrant further investigation to pinpoint the root causes of these issues.
**Bottom Approved Transaction Value Issuers**: The bottom five banks based on approved transaction value (AGI, Jana Small Finance Bank, YES Bank Prepaid YP2, Karnataka Grameen Bank, and YES Bank Prepaid YP2) require attention to identify and address potential factors hindering their user adoption or transaction success rates.

## **recommendations**

**Fraud Mitigation**: The rise in AEPS fraud, as evidenced by recent cases and the Telangana police alert, highlights the need for robust Fraud Risk Management (FRM) solutions like those offered by the national financial switch. Implementing such solutions can help prevent fraudulent transactions and protect user funds.

**Infrastructure Improvements**:  Technical glitches in AEPS, which are prevalent especially in rural areas, can be attributed to limited high-speed internet infrastructure. Expanding fiber optic cable networks and improving overall network connectivity in these regions is crucial to ensure smooth and reliable transaction processing.

**Enhanced User Experience**: Slow transaction processing times due to poor network connectivity can deter users from adopting AEPS.  Infrastructure upgrades (as mentioned above) along with user interface improvements can streamline the transaction process and provide a more positive user experience.

**Rural Outreach and Awareness Programs**:  The overall drop in AEPS transactions might be linked to the limited availability of business correspondents, particularly in remote areas.  To address this, awareness campaigns should be conducted to educate users in rural areas about the benefits and functionalities of AEPS banking. Additionally, deploying micro ATMs in shops across these regions can provide users with convenient access to cash withdrawal and purchase capabilities.

## **PowerBI Dashboard**

1. **Slicers**: YEAR wise filters on chart , product wise filters on chart

2. **KPIs**: Total count of Issuer banks, Total number of transactions, total number of approved transactions,Total number of business declines and total number of technical declines metrics offer a quick overview of  transactions and declines behaviour.

## **Conclusion**

The analysis of NPCI product wise declines  data has provided valuable insights into customer behavior, declines reason, and transactions behaviour. By leveraging data-driven strategies, businesses can optimize their operations and enhance customer satisfaction, leading to improved  performance .

### **🚀Key Takeaways:**

- **Product Performance:** Assessed the overall health of NPCI products based on decline data.

- **Focus on Trends:** Analyzed variations in decline rates across different products.
