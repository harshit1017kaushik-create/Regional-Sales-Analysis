# Regional Sales Analysis | 2022–2025

An end-to-end sales analytics project combining **Python, Pandas, Scikit-learn, AI-generated insights, and Power BI** to explore revenue, profitability, product performance, customer behavior, and regional sales trends.

**Live Website:** https://harshit1017kaushik-create.github.io/Regional-Sales-Analysis/
---

## Project Overview

This project analyzes regional sales data from January 2022 through February 2025, covering 175 customers, 30 products, and four US regions.

The workflow includes data preparation, exploratory data analysis, feature engineering, machine-learning experiments, AI-generated summaries, and interactive Power BI reporting.

The objective is to understand what drives sales and profitability, identify differences across regions and channels, and evaluate whether contextual business features can help predict high-margin orders.

## Project Objectives

- Analyze total revenue, profit, order volume, and profit margins.
- Compare sales performance across four US regions.
- Identify top-performing products and customers.
- Evaluate revenue and profitability by sales channel.
- Explore relationships between revenue, cost, profit, and margin.
- Build and compare machine-learning models for margin classification.
- Generate AI-assisted business summaries and recommendations.
- Present findings through an interactive Power BI dashboard and portfolio website.

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Data processing and analysis |
| Pandas | Data cleaning, transformation, and aggregation |
| NumPy | Numerical operations |
| Matplotlib and Seaborn | Exploratory data visualization |
| Scikit-learn | Machine-learning model development and evaluation |
| Jupyter Notebook | Analysis and experiment documentation |
| Power BI | Interactive dashboards and business reporting |
| AI-generated insights | Summarizing analytical findings |
| HTML, CSS, JavaScript | Portfolio website |

## Dataset

The project uses a regional sales dataset covering orders, customers, products, regions, and related business information.

### Main files

- `Regional_Sales_Dataset_2022_25.xlsx` — original dataset.
- `Sales_data_Regional_Sales_Final.csv` — cleaned and prepared dataset.
- `Sales_Regional_Analysis.ipynb` — sales data analysis and exploratory analysis.
- `ML_Sales.ipynb` — machine-learning experiments.
- `AI_Insights_Sales.ipynb` — AI-assisted business insights.
- `Sales_Analysis.pbix` — editable Power BI report, if included.

## Business Analysis Workflow

### 1. Data Preparation

The project uses Python to prepare sales data for analysis, combining relevant sales, customer, product, and regional information and creating additional analytical fields.

Key financial metrics include:

- Revenue
- Total cost
- Profit
- Profit margin percentage
- Order month and related time-based fields

### 2. Exploratory Data Analysis

The analysis examines sales performance from multiple perspectives:

- Revenue and profit by region
- Revenue by sales channel
- Top products by revenue and profit
- Product-level profit margins
- Customer revenue and profitability
- State-level sales performance
- Monthly revenue trends
- Revenue and profit relationships

### 3. Machine Learning: Predicting High-Margin Orders

The modeling experiment investigates whether an order can be classified as high margin using a 40% margin threshold.

The website reports the following model results:

| Experiment | Accuracy |
|---|---:|
| Logistic regression with price and cost features | 98.99% |
| Logistic regression using contextual features | 56.85% |
| Majority-class baseline | 55.04% |
| Decision tree using contextual features | 55.6% |

The contextual features include channel, region, product, customer, and timing information.

**Key interpretation:** Price and cost directly determine profit margin, so the 98.99% accuracy result is not evidence of strong predictive power from independent business context. Removing those features reduces accuracy to 56.85%, only modestly above the 55.04% majority-class baseline.

The website also reports that the contextual decision tree has only 1.9% recall for the high-margin class. These results suggest that contextual features alone provide limited predictive value in this experiment.

### 4. AI-Generated Insights

The project includes an AI insights notebook and a portfolio website presenting summarized findings about:

- Regional revenue concentration
- Channel-level sales and margin differences
- Product revenue versus profitability
- Customer-level performance
- Implications of the margin classification experiments

AI-generated summaries support interpretation of the analysis; business decisions should still be based on validated underlying data.

### 5. Power BI Dashboard

The Power BI report contains three main analytical pages.

**Page 1 — Regional Sales Overview**
- Total revenue, profit, quantity sold, orders, and average profit margin
- Top products by revenue
- Revenue by region and channel
- Monthly revenue trend

**Page 2 — Product & Profitability Analysis**
- Top customers by revenue
- Top products by profit
- Product revenue versus profit
- Profit by channel and region
- Products with the highest profit margins

**Page 3 — Geographic & Customer Analysis**
- State-level revenue performance
- Customer revenue and margin comparisons
- Quantity sold by region
- Profit margin by region
- State revenue versus profit

## Key Performance Indicators

The following values are displayed on the existing website and Power BI report.

| KPI | Reported value |
|---|---:|
| Total revenue | $1.24 billion |
| Total profit | $461.74 million |
| Average profit margin | 37.36% |
| Total orders | 10,684 |
| Units sold | 541,134 |
| Customers | 175 |
| Products | 30 |
| Regions | 4 |

### Selected Business Findings

**Regional performance**
- The West generates approximately $372.1M in revenue, or 30.1% of the total.
- The South contributes approximately $335.1M, followed by the Midwest at $320.3M.
- The Northeast contributes approximately $208.4M.

**Sales channels**
- Wholesale contributes approximately $668.2M in revenue and is the largest channel.
- Distributor revenue is approximately $387.1M.
- Export revenue is approximately $180.6M, while its reported average profit margin is the highest at 37.93%.

**Product performance**
- Product 26 leads with approximately $117.3M in revenue.
- Product 25 follows with approximately $109.4M.
- Product 9 has the highest reported average product margin at 39.90%.

**Customer performance**
- Aibox Company is the highest-revenue customer shown, with approximately $12.64M.
- Organon Corp has a reported customer profit margin of approximately 40.5%.

**Modeling**
- Contextual features alone provide limited improvement over the majority-class baseline.
- The experiment highlights the importance of separating directly derived financial variables from genuinely predictive business information.

These findings reproduce figures displayed by the existing project. They have not been independently recalculated for this README.

## Important Analytical Notes

- The state-level revenue-versus-profit visualization uses estimated profit based on the overall 37.36% average margin, as explained on the website. It should not be interpreted as actual state-level profit.
- High model accuracy when using price and cost may reflect information directly embedded in the target calculation.
- Model performance should be assessed using class-specific precision, recall, and suitable validation procedures, not accuracy alone.
- Descriptive patterns and correlations do not establish causation.

## Repository Structure

```text
Regional-Sales-Analysis/
├── README.md
├── Regional_Sales_Dataset_2022_25.xlsx
├── Sales_Regional_Analysis.ipynb
├── ML_Sales.ipynb
├── AI_Insights_Sales.ipynb
├── Sales_data_Regional_Sales_Final.csv
├── Sales_Analysis.pbix
└── regional-sales-analysis-site.html 
```

## How to Run the Project

1. Clone or download the repository.
2. Install Python and Jupyter Notebook.
3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn openpyxl jupyter
   ```

4. Open the notebooks in Jupyter Notebook.
5. Make sure the dataset paths match the location of your downloaded files.
6. Run the analysis notebook, followed by the machine-learning and AI-insights notebooks as needed.
7. Open `Sales_Analysis.pdf` to review the report or use Power BI Desktop to open `Sales_Analysis.pbix` if included.

## Project Deliverables

- Original Excel dataset
- Cleaned regional sales CSV
- Sales analysis notebook
- Machine-learning notebook
- AI-insights notebook
- Power BI report in PDF format
- Optional editable Power BI report
- Interactive portfolio website

## Author

**Harshit Kaushik**

B.Tech — Computer Science & Engineering

Interested in Data Analytics, Business Intelligence, Python, SQL, Machine Learning, and Power BI.

**GitHub:** https://github.com/harshit1017kaushik-create  
**Live Website:** https://harshit1017kaushik-create.github.io/Regional-Sales-Analysis/
