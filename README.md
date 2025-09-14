# 🛍️ Customer Segmentation with RFM Analysis -- Olist E-commerce

## 📌 Project Overview

This project applies **RFM (Recency, Frequency, Monetary) Analysis** to
the **Olist e-commerce dataset** to uncover customer segments and
generate actionable business insights.\
By segmenting customers into groups such as **Champions, Loyal, At-Risk,
and Lost**, the analysis supports data-driven strategies for **customer
retention, re-engagement, and revenue growth**.

------------------------------------------------------------------------

## 📂 Dataset

We used three datasets from Olist: - **Customers Dataset
(`olist_customers_dataset.csv`)** -- Customer IDs and location info\
- **Orders Dataset (`olist_orders_dataset.csv`)** -- Order lifecycle and
timestamps\
- **Payments Dataset (`olist_order_payments_dataset.csv`)** -- Payment
details including amounts

After merging, the data covered **\~100,000 unique customers** with
transaction history.

------------------------------------------------------------------------

## ⚙️ Methodology

1.  **Data Preparation**
    -   Merged customers, orders, and payments data\
    -   Cleaned missing values and ensured timestamp parsing
2.  **Feature Engineering**
    -   Defined **Recency**: days since last purchase\
    -   Defined **Frequency**: number of unique orders\
    -   Defined **Monetary**: total spend
3.  **RFM Scoring**
    -   Applied quintile-based scoring (1--5 scale)\
    -   Constructed composite **RFM_Score**\
    -   Mapped scores to descriptive **segments** using regex rules
4.  **Visualization & Insights**
    -   Customer distribution by segment\
    -   **Recency vs Frequency heatmap**\
    -   **Pareto revenue analysis** (80/20 rule)\
    -   Monetary spread by segment (boxplots)

------------------------------------------------------------------------

## 📊 Key Findings

-   The **top 20% of customers contributed \~78% of total revenue**
    (Pareto principle).\
-   **Champions & Loyal Customers** are the primary revenue drivers and
    should be nurtured with loyalty rewards.\
-   **At-Risk & Hibernating Customers** represent reactivation
    opportunities via targeted marketing.\
-   A large portion of customers fall under **Lost**, highlighting the
    importance of improving retention.

------------------------------------------------------------------------

## 📈 Visualizations

*(Add chart images here after running the notebook and saving plots to
`visuals/`)*

-   Segment distribution bar chart\
-   Recency--Frequency heatmap\
-   Pareto chart of revenue contribution\
-   Boxplot of Monetary value by segment

------------------------------------------------------------------------

## 🚀 How to Run

1.  Clone the repository:

    ``` bash
    git clone https://github.com/yourusername/RFM-Customer-Segmentation.git
    cd RFM-Customer-Segmentation
    ```

2.  Install dependencies:

    ``` bash
    pip install -r requirements.txt
    ```

3.  Open and run the notebook:

    ``` bash
    jupyter notebook notebooks/RFM_Analysis_enhanced.ipynb
    ```

------------------------------------------------------------------------

## 📌 Business Recommendations

-   **Retention:** Offer loyalty rewards & VIP experiences to
    Champions.\
-   **Upsell:** Promote bundles or premium products to Loyal Customers.\
-   **Reactivation:** Send discounts or personalized offers to At-Risk
    customers.\
-   **Prevention:** Improve onboarding and engagement to reduce Lost
    segment size.

------------------------------------------------------------------------

## 🧰 Tech Stack

-   **Python** (Pandas, NumPy, Matplotlib, Seaborn)\
-   **Jupyter Notebook** for analysis and reporting

------------------------------------------------------------------------

## 📄 License

This project is open-source and available under the MIT License.
