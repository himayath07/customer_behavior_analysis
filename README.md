# 🛍️ Customer Shopping Behavior — Data Analytics Project


## 📖 Overview

This project analyzes **customer shopping behavior** to uncover patterns in purchasing habits, spending trends, and product preferences. The full data analytics pipeline is demonstrated — from data loading and cleaning in Python, SQL analysis, and interactive visualization in Power BI to a final report and presentation using Gamma.

## 🎯 Objectives

- Understand customer demographics and shopping patterns
- Identify top-performing product categories and shopping malls
- Analyze spending trends across different segments
- Provide actionable business insights for marketing and sales strategies
- Create an interactive dashboard for stakeholder decision-making

## 🗂️ Dataset

| Property | Details |
|----------|---------|
| **File Name** | `customer_shopping_behavior.csv` |
| **Source** | Public dataset on retail and e-commerce shopping data |
| **Description** | Transaction-level details about customers, demographics, shopping preferences, and product categories |

### Key Columns

- `customer_id` — Unique customer identifier
- `age`, `gender`, `location` — Demographic attributes
- `category`, `product`, `quantity`, `price` — Purchase details
- `date` — Transaction date
- `payment_method`, `shopping_mall` — Purchase context

## 🛠️ Tools & Technologies

| Category | Tools Used |
|----------|------------|
| **Programming** | Python (Pandas, NumPy, Matplotlib, Seaborn) |
| **Database** | PostgreSQL / MySQL / SQL Server |
| **Visualization** | Power BI |
| **Presentation** | Gamma |
| **IDE** | Jupyter Notebook / VS Code |

## 📁 Project Structure

```
customer-shopping-behavior/
│
├── data/
│   ├── customer_shopping_behavior.csv    # Raw dataset
│   └── cleaned_data.csv                   # Processed dataset
│
├── notebooks/
│   ├── customer_behavior.ipynb            # Main analysis notebook
│   └── EDA_and_Cleaning.ipynb             # Data exploration & cleaning
│
├── sql/
│   └── sql_queries.sql                    # SQL analytical queries
│
├── powerbi/
│   └── dashboard.pbix                     # Power BI dashboard file
│
├── reports/
│   ├── insights_report.pdf                # Written report
│   └── presentation.pdf                   # Gamma presentation
│
├── visualizations/
│   └── *.png                              # Saved charts and graphs
│
├── requirements.txt                       # Python dependencies
└── README.md                              # Project documentation
```

## ⚙️ Project Workflow

### 1. 📥 Data Loading

- Loaded the dataset into Python using Pandas
- Explored data structure, types, and missing values
- Generated initial data quality report

### 2. 🔍 Exploratory Data Analysis (EDA)

- Generated summary statistics for numerical and categorical columns
- Visualized distributions, spending trends, and category preferences using Matplotlib and Seaborn
- Identified seasonal trends and customer segments
- Analyzed correlations between variables

### 3. 🧹 Data Cleaning

- Removed duplicates and handled missing or inconsistent values
- Standardized categorical data (e.g., payment method names, location formatting)
- Created derived fields such as `total_spent = quantity × price`
- Validated data integrity and consistency

### 4. 💾 SQL Analysis

- Imported the cleaned data into a SQL database (PostgreSQL/MySQL/SQL Server)
- Executed analytical queries such as:
  - Top 5 product categories by total revenue
  - Monthly sales trend by region
  - Gender-wise average spending comparison
  - Customer retention rate using repeat purchases
  - RFM (Recency, Frequency, Monetary) analysis
- Exported SQL results for visualization

### 5. 📊 Power BI Dashboard

- Connected Power BI to the SQL database
- Designed an interactive dashboard showing:
  - **Total Revenue and Orders**
  - **Top Product Categories and Shopping Malls**
  - **Age Group Spending Distribution**
  - **Regional Sales and Payment Preferences**
  - **Time-series trends and seasonality**
- Added filters for date range, category, and gender to allow deep analysis

### 6. 📝 Reporting & Presentation

- Compiled insights and business recommendations in a written report
- Created a Gamma presentation summarizing:
  - Project objectives
  - Key findings and metrics
  - Data-driven insights & recommendations
  - Dashboard highlights and demo

## 💡 Key Insights & Results

### Customer Behavior

- 📈 **Top Customers**: The top 10% of customers contribute ~40% of total revenue
- 👥 **Customer Segments**: Identified 4 distinct customer segments based on spending patterns

### Product & Category Insights

- 🏆 **Popular Categories**: Electronics and Clothing are the most popular purchase categories
- 💰 **Revenue Drivers**: Premium products in Electronics generate highest margins

### Spending Trends

- 📅 **Peak Shopping Days**: Average spending peaks during weekends and festive seasons
- 🎉 **Seasonal Patterns**: Q4 shows 35% higher sales compared to other quarters

### Demographics

- 👩 **Gender Distribution**: Female customers show higher average basket value
- 🎂 **Age Groups**: 25-34 age group contributes the highest transaction volume

### Payment & Location

- 💳 **Preferred Payment**: Credit card usage dominates urban regions (65%)
- 🏢 **Top Malls**: Downtown shopping malls generate 2x more revenue than suburban locations

## 📈 Dashboard Preview

> 📸 *Add Power BI dashboard screenshots here*

**Dashboard Features:**
- Real-time KPI tracking
- Interactive filters and slicers
- Drill-down capabilities
- Mobile-responsive design

## ▶️ How to Run

### Prerequisites

- Python 3.8+
- Power BI Desktop
- SQL Database (PostgreSQL / MySQL / SQL Server)
- Git

### Installation

1. **Clone this repository:**
   ```bash
   git clone [https://github.com/himayath07/customer-shopping-behavior.git](https://github.com/himayath07/customer_behavior_analysis.git)
   cd customer-shopping-behavior
   ```

2. **Install Python dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up your SQL database:**
   - Create a new database
   - Update connection credentials in the configuration file

### Running the Analysis

1. **Data Exploration & Cleaning:**
   ```bash
   jupyter notebook notebooks/EDA_and_Cleaning.ipynb
   ```
   Or open `customer_behavior.ipynb` in VS Code

2. **Execute SQL Analysis:**
   - Import the cleaned data into your SQL database
   - Execute the queries from `sql/sql_queries.sql`
   - Export results as needed

3. **Power BI Dashboard:**
   - Open `powerbi/dashboard.pbix` in Power BI Desktop
   - Configure database connection
   - Refresh data and explore visuals

4. **View Reports:**
   - Check the `reports/` folder for final documentation and presentation

## 📦 Dependencies

```txt
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
seaborn>=0.12.0
sqlalchemy>=2.0.0
psycopg2-binary>=2.9.0  # For PostgreSQL
pymysql>=1.0.0          # For MySQL
jupyter>=1.0.0
openpyxl>=3.0.0
```

## 🔮 Future Enhancements

- [ ] Implement machine learning models for customer churn prediction
- [ ] Add predictive analytics for sales forecasting
- [ ] Create customer recommendation engine
- [ ] Automate ETL pipeline with Apache Airflow
- [ ] Deploy dashboard to Power BI Service
- [ ] Integrate real-time data streaming

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Your Name**

- GitHub: [@himayath07](https://github.com/himayath07)
- LinkedIn: [Mohammed Himayath Ali](https://www.linkedin.com/in/mohammed-himayath-ali-6a7757244/)

## 🙏 Acknowledgments

- Dataset source and contributors
- Open-source community for amazing tools
- Power BI community for dashboard inspiration

---

⭐ **If you found this project helpful, please consider giving it a star!**

*Last Updated: November 2025*
