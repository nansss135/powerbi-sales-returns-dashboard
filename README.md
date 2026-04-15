#  Sales & Returns Performance Dashboard (Power BI)


##  Project Overview

This project presents a comprehensive **Sales and Returns Analysis Dashboard** developed using **Power BI and DAX**. The dashboard provides insights into sales performance, profitability, customer behavior, and return trends across different regions, segments, and time periods.

The objective of this project is to transform raw data into meaningful insights using **data modeling, DAX calculations, and interactive visualizations**.



##  Dataset Description

The dataset consists of the following tables:

###  Fact Tables

* **Sales_Fact** – Contains transactional sales data (Sales Amount, Cost, Quantity, CustomerID, ProductID, DateKey, RegionID)
* **Returns_Fact** – Contains returned order data linked via SalesID

###  Dimension Tables

* **Customer_Dim** – Customer details (First Name, Last Name, Full Name)
* **Product_Dim** – Product information and categories
* **Date_Dim** – Date hierarchy (Year, Month, Quarter, Weekday)
* **Region_Dim** – Region details (Central, East, North, South, West)



##  Data Model Architecture

The project follows a **Star Schema Model**:

* Sales_Fact is the central table
* Connected to all dimension tables using **Many-to-One relationships**
* Returns_Fact is linked to Sales_Fact using **SalesID**
* Dimension tables act as filters for analysis

###  Key Features:

* Efficient data relationships
* Optimized filtering
* Scalable structure



##  Calculated Columns

The following calculated columns were created:

* **Profit** = Sales Amount - Cost
* **ReturnFlag** = Identifies whether a sale is returned or not
* **Full Name** = Concatenation of First Name and Last Name

---

##  DAX Measures & Calculations

A dedicated **Measure_Table** was created to store all DAX measures.

###  Basic Measures

* Total Sales
* Total Cost
* Total Profit
* Total Quantity
* Total Returns

###  Customer Metrics

* Unique Customers
* Average Sale

###  Return Analysis

* Return Rate
* Sales Returned

###  Advanced DAX Measures

* High Sales
* High Sales All Region
* Sales Of All Region

###  Time Intelligence

* Total Sales YoY%

###  DAX Functions Used

* SUM()
* COUNTROWS()
* DISTINCTCOUNT()
* DIVIDE()
* CALCULATE()
* FILTER()
* ALL()

---

##  Dashboard Visualizations

The dashboard includes a variety of interactive visuals:

###  KPI Cards

* Total Sales
* Total Profit
* Total Cost
* High Value Sales
* Average Sales
* Unique Customers
* Return Rate



###  Gauge Chart

* Displays **High Value Sales Performance vs Target**
* Helps track performance against a benchmark

---

###  Donut Chart

* Shows **Total Sales by Segment**
* Identifies top contributing segments

---

###  Funnel Chart

* Displays **Total Returns by Segment**
* Highlights return distribution

---

###  Line Chart

* Shows **Total Profit by Month**
* Helps analyze trends over time

---

###  Decomposition Tree

* Breaks down sales into:

  * Segment
  * Category
  * Region
* Helps identify key contributors


### 📌 Slicers

* Month filter
* Region filter
* Enable interactive dashboard exploration

---

##  Matrix-Based Analysis

The Matrix visual is the core analytical component.

###  Structure:

* Rows → Region
* Columns → Month
* Values → Multiple KPIs

###  Metrics Included:

* Total Sales
* Total Profit
* Return Rate
* Avg Sale
* Total Cost
* Total Quantity
* Unique Customers
* Total Returns
* High Sales
* Sales Of All Region
* Sales Returned

---

##  Key Insights

* Retail segment contributes the highest sales
* High value sales form a significant portion of revenue
* Return rate is relatively low (~10%)
* Sales and profit vary across regions and months
* West and North regions show strong performance

---

##  Tools & Technologies

* **Power BI Desktop**
* **DAX (Data Analysis Expressions)**
* Data Modeling (Star Schema)
* Interactive Visualizations



##  Conclusion

This project demonstrates how Power BI can be used to:

* Build efficient data models
* Perform advanced DAX calculations
* Create interactive dashboards
* Generate actionable business insights

The dashboard provides a **complete analytical view of sales and returns**, making it useful for business decision-making.



##  Future Enhancements

* Add forecasting models
* Include more granular location data
* Improve UI/UX design
* Integrate real-time data sources


##  Author

**Nandani Rajput**
B.Tech CSE Student | Power BI Learner



