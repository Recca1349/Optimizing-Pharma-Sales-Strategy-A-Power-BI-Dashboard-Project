# Pharmaceutical Sales Performance Analysis with Power BI
![pharmacy image](https://github.com/user-attachments/assets/ec2bdb17-e35e-45cd-8eca-7c4fb0c01348)


**Disclaimer**⚠️: All datasets, slides and reports do not contain real proprietary, confidential, or sensitive information from any company, institution, or individual mention. All info are dummy and design to demonstrate my capabilities of using PowerBI to perform advance analysis on healthcare dataset

## Table of Content
- [Description](#description)  
- [Business Introduction](#business-introduction)  
- [Problem Statement](#problem-statement)  
- [Aim of the Project](#aim-of-the-project)  
- [Processes / Methodologies Used](#processes--methodologies-used)  
- [Data Modeling](#data-modeling)  
- [Visualization](#visualization)   
  - [KPIs](#kpis)
  - [Matrix](#matrix)  
  - [Pie Chart](#pie-chart)  
  - [Line Charts](#line-charts)  
  - [Donut Chart](#donut-chart)  
  - [Map](#map)  
  - [Clustered Column Charts](#clustered-column-charts)  
- [Dashboard Review](#dashboard-review)  
- [Key Insights](#key-insights)  
- [Recommendations](#recommendations)  
- [Thank You](#thank-you)

## Description
This Power BI dashboard analyzes NovaMed Solutions’ sales data (2022–2026), highlighting trends in revenue, profit, top/bottom drug performance, and customer demographics. It supports data-driven decisions in sales strategy, inventory planning, and market targeting.
## Business Introduction
NovaMed Solutions is a leading pharmaceutical distributor committed to ensuring the timely delivery of essential medications to healthcare providers across diverse markets. With a focus on operational excellence, NovaMed bridges the gap between manufacturers and medical institutions by offering reliable distribution, strategic inventory management, and responsive customer service. The company leverages data-driven practices to optimize supply chain performance, meet dynamic market demands, and support better health outcomes through consistent access to high-quality pharmaceutical products.
## Problem Statement
NovaMed Solutions faced challenges in optimizing its sales performance and customer engagement due to limited visibility into product-level trends, inefficient demand forecasting, and fragmented customer insights. These issues led to suboptimal inventory management, missed revenue opportunities, and difficulty in identifying key growth areas. The business needed a centralized, data-driven approach to monitor performance, understand customer behavior, and make informed strategic decisions.
## Aim of the Project
The primary objectives of this project are as follows:
- Provide a centralized, interactive Power BI dashboard for sales analysis
- Track revenue, profit, and cost trends across products and time
- Identify top and bottom-performing drugs using dynamic ranking
- Analyze customer demographics by age, gender, and country
- Support data-driven decisions in sales strategy and inventory planning
- Enhance visibility into market performance and customer behavior
## Processes / Methodologies Used
**Business Understanding:** Defined the project objective to analyze NovaMed Solutions’ sales performance, product profitability, and customer demographics in order to uncover trends, reduce inefficiencies, and support data-driven decisions.

**KPI Development:** Defined and implemented core KPIs, including Revenue, Profit, Profit Margin, Quantity Sold, COGS, and Average Revenue per Customer. Created dynamic DAX measures to support month-over-month (MoM) trend analysis and top/bottom performance ranking.

**Data Understanding:** Explored and reviewed sales, product, and customer datasets (2022–2026) to understand key variables such as revenue, profit, quantity sold, buyer types, and demographic distributions.

**ETL Process:** Extracted the raw data, transformed it using Power Query (e.g., removing duplicates, changing data types, creating time columns), and loaded the cleaned data into Power BI for modeling and analysis.

**Data Modeling:** Created a star schema with fact and dimension tables, established relationships, and built calculated columns and DAX measures for dynamic KPI calculations and rankings.

**Visualization & Insight Generation:** Designed interactive dashboards to display top/bottom product performance, month-over-month sales trends, and customer insights by gender, age, and region. Enabled user exploration through filters and slicers.
## Data Modeling
The data modeling for this project adopts a star schema architecture to ensure efficient and scalable analysis within Power BI. The central Fact Table contains transactional sales data, including key metrics such as Revenue, Quantity Sold, Cost of Goods Sold (COGS), and Profit, alongside buyer type, sales date, drug names, drug IDs, sales IDs and customer IDs. This Fact Table is linked to multiple Dimension Tables through unique identifiers, including:

**Customer Dimension:** Contains attributes such as customer name, customer IDs, gender, age group, buyer type, and country.

**Product/Drug Dimension:** Contains information on the drugs such as drug IDs, names, their unit sales price, unit cost of production price and their treatment details.

**Calendar Dimension:** Includes hierarchical time data (Year, Quarter, Month) to support time-series and month-over-month analysis.

This relational model enables advanced filtering, slicing, and drill-down functionality across dashboards. It also allows for accurate aggregation and comparison of KPIs across customer segments, product types, and time periods, enhancing data exploration and business insight generation.

<img width="1920" height="962" alt="Novamed Model Screenshot" src="https://github.com/user-attachments/assets/b21508ac-aa2c-46ff-8453-eda0b1c1ea33" />

## Visualization

- KPIs
- Matrix
- Line Charts
- Pie Chart
- Donut Chart
- Map
- Clustered Column Charts

## Data Analysis
### KPIs
This dashboard presents key performance indicators (KPIs) for Total Revenue, Total Profit, Cost of Goods Sold (COGS), Profit Margin, and other critical sales metrics for NovaMed Solutions. Between 2022 and 2026, Total Revenue reached $71.31 million, with a Total Profit of $58.45 million, and COGS amounting to $12.85 million. The overall Profit Margin stood at a strong 81.97%, highlighting operational efficiency and pricing effectiveness. Over the same period, NovaMed served 200 customers, sold 269,470 units of pharmaceuticals, and tracked performance across 40 distinct drug products. These KPIs reflect NovaMed’s robust sales performance, cost management, and expanding market presence over the five-year period.

<img width="1172" height="142" alt="Screenshot Novamed KPIs" src="https://github.com/user-attachments/assets/de30d877-913d-4da8-bfa1-9471bc70fe30" />

<img width="1172" height="141" alt="Screenshot KPI2" src="https://github.com/user-attachments/assets/11ea526d-da65-4b44-b21d-cdda523d3a82" />

<img width="1172" height="143" alt="Screenshot kpi3" src="https://github.com/user-attachments/assets/8950f68e-9d4f-43cd-b1f8-003e0a4865ae" />

### Matrix
#### **1. Top & Bottom 10 Drugs by Revenue (Matrix Tables)**
   
This matrix highlights the top and bottom 5 performing drugs based on total revenue. It provides a clear side-by-side view of drug names alongside their respective revenue values, making it easy to identify high earners like Doxycycline and Ergocalciferol, as well as underperformers such as Montelukast and Warfarin. The table enables quick ranking and comparison, supporting evidence-based inventory and sales strategy decisions.

<img width="446" height="305" alt="topbottom1" src="https://github.com/user-attachments/assets/731e8f35-0b5d-4efb-be19-e8b0ae954ab4" />

<img width="445" height="305" alt="topbottom2" src="https://github.com/user-attachments/assets/4a021e24-6bab-4a59-8745-bed3d9528c5d" />


#### **2. Top & Bottom 10 Drugs by Profit (Matrix Tables)**

Similar to the revenue matrix, this visual ranks drugs by profit to spotlight products that are both financially valuable and cost-effective. Doxycycline again ranks highest in profitability, reinforcing its strong market position, while drugs with low or negative margins highlight cost or pricing concerns. This matrix is crucial for identifying which products contribute most to NovaMed’s bottom line.

<img width="446" height="306" alt="bottom profit2" src="https://github.com/user-attachments/assets/34daed49-c358-4016-9585-89b0afa4e108" />

<img width="446" height="307" alt="bottom3" src="https://github.com/user-attachments/assets/b64832c6-e4f0-4424-80d8-bfdf7c46057b" />


#### **3. Top 5 Performing Customers (Matrix Table)**

This matrix showcases NovaMed’s top 5 customers, ranked by total revenue, profit, and quantity sold. Leading the list is David Johnson, who alone contributed nearly $3.9M in revenue, followed by other high-value clients such as Bob Williams and Bob Smith. The table provides critical insight into the company's most profitable relationships, supporting efforts in customer retention, personalized service, and strategic upselling, particularly among the highest spenders.

<img width="392" height="193" alt="customer shot1" src="https://github.com/user-attachments/assets/3e7f8547-b343-47dd-9c37-61f6cc3491f2" />


#### **4. Bottom 5 Performing Customers (Matrix Table)**

This matrix identifies the lowest performing customers based on revenue, profit, and units purchased. These clients show minimal contribution to sales despite being active in the system. The visual is essential for spotting engagement gaps, reevaluating account strategies, and determining whether these customers require targeted sales support, reactivation campaigns, or should be deprioritized to allocate resources more efficiently.

<img width="392" height="193" alt="customer shot2" src="https://github.com/user-attachments/assets/e53405a5-3f53-4d21-8b56-a12f029b3de2" />


#### **5. Revenue by Country and Customer Type (Matrix Table)**

This table provides a combined view of revenue distribution by country and buyer type (User vs. Seller), offering insights into geographic and customer segment performance. Canada leads with the highest revenue, followed by Australia and the Germany, indicating strong market penetration in these regions. Additionally, the split between Users and Sellers highlights behavioral differences in purchasing patterns across locations. This visual is instrumental in shaping regional sales strategies, identifying high-value markets, and tailoring engagement approaches based on buyer roles and geographic trends.

<img width="377" height="356" alt="country revenue shot" src="https://github.com/user-attachments/assets/52196554-e22f-4d41-920a-9ea9f5df72e5" />


### Pie Chart
#### **Top 5 Drugs by Quantity Sold (Pie Chart)**

This pie chart illustrates the percentage share of total quantity sold by NovaMed’s top 5 performing drugs. Lisinopril leads with 25.4%, followed by Prednisone, Gabapentin, Clonazepam, and Atorvastatin, reflecting strong demand concentrations. The visual emphasizes how a small subset of drugs accounts for a significant portion of overall sales volume. While these high-volume drugs drive operational activity, the chart also invites a deeper look into whether their profit margins align with their demand, supporting decisions around pricing, inventory prioritization, and promotional efforts.

<img width="677" height="307" alt="Screenshot qty sold1" src="https://github.com/user-attachments/assets/cfadfde1-1a39-4f79-ab9c-ff9326075737" />


### Line Charts
#### **1. Revenue by Month Analysis**

This line chart displays monthly revenue trends from 2022 to 2026, helping NovaMed identify patterns, growth spikes, and slowdowns in sales performance. A notable peak in January ($6.8M) indicates strong early-year performance, while dips in February and August may point to operational lags, seasonal demand changes, or distribution gaps. By visualizing revenue movement over time, the chart supports better forecasting, budgeting, and strategic planning, enabling the business to replicate high-performing periods and mitigate downturns proactively.

<img width="1143" height="218" alt="line chart shot1" src="https://github.com/user-attachments/assets/b69e3e5e-1f24-4540-9278-7ea296aeca1c" />

#### **2. Profit by Month Analysis**

This line chart tracks monthly profit trends from 2022 to 2026, highlighting how NovaMed’s profitability fluctuates over time. The peak occurs in January with $5.6M in profit, indicating a strong start to the year, while February and August show notable declines, potentially due to reduced sales activity or operational inefficiencies. This visualization supports financial planning by helping stakeholders identify consistent profit drivers, assess the impact of seasonality, and develop strategies to improve underperforming periods.

<img width="1142" height="220" alt="line chart shot2" src="https://github.com/user-attachments/assets/162d911d-ed8f-409e-ba28-9e9df48eb496" />


### Donut Chart
#### **Gender Customer Base**

This donut chart visualizes the gender distribution of NovaMed’s customer base, with 47% identifying as male, 33% as female, and 21% as other. The breakdown offers valuable insight into customer diversity and supports the development of inclusive, gender-sensitive marketing strategies. By understanding demographic representation, NovaMed can better align product offerings, communication styles, and engagement efforts to meet the needs of all customer segments effectively.

<img width="317" height="192" alt="gender shot" src="https://github.com/user-attachments/assets/69d6e923-c27c-4ded-a3b5-1ee55e8dfbf7" />


### Map
#### **Revenue by Country (Map Visualization)**

This map visualization displays revenue distribution by country, highlighting Canada as the leading contributor, followed by Australia. These two countries together account for a significant portion of NovaMed’s sales, indicating strong market presence and customer engagement. The visual supports geographic performance tracking and helps inform decisions on regional investments, marketing focus, and resource allocation to strengthen NovaMed’s position in its top-performing territories.

<img width="610" height="328" alt="country revenue shot2" src="https://github.com/user-attachments/assets/77c9c2ca-d8cc-4a3d-8315-70c6ed559a8d" />


### Clustered Column Charts
#### **1. Age Distribution of Customer Base**

This clustered column chart displays the number of customers across different age groups, highlighting that the 40–59 age group leads with 74 customers, followed by 60+ with 63 customers. This visualization identifies NovaMed’s most engaged customer segments, enabling the company to align outreach, product development, and service offerings with the age demographics that represent the bulk of its client base.

<img width="327" height="210" alt="age customer base shot" src="https://github.com/user-attachments/assets/1f52f740-9490-4fed-bf3f-1d5a8088cbd3" />

#### **2. Revenue by Age Group || Gender**

This clustered column chart illustrates total revenue by gender across each age group, offering deep insight into customer value segmentation. The most significant contribution comes from males aged 60+, generating $11.2M in revenue, highlighting them as a key revenue-driving demographic. This visual helps NovaMed focus its sales, marketing, and product personalization efforts on the highest-yield customer segments.

<img width="776" height="310" alt="revenueage shot" src="https://github.com/user-attachments/assets/9c96e3fb-98fa-4c3f-ad7d-117daf2580aa" />

#### **3. Customer Base by Country**

This clustered column chart displays the number of customers by country, revealing that Canada leads with 86 customers, followed by Australia (46) and the Germany (19). The visualization highlights where NovaMed’s customer presence is most concentrated, offering valuable insights for regional market prioritization, customer engagement planning, and resource allocation. This view enables decision-makers to focus retention and expansion strategies in countries with strong existing demand.

<img width="402" height="210" alt="countrybase shot" src="https://github.com/user-attachments/assets/81cdf813-dda3-434a-bd76-fe80bc9735af" />

## Dashboard Review

The four interactive dashboards provide a comprehensive view of NovaMed Solutions’ sales performance from 2022 to 2026. They uncover trends in revenue, profit, and quantity sold across top and bottom-performing drugs, highlight monthly fluctuations, and offer demographic and geographic insights into the customer base. From identifying high-value drugs like Doxycycline and key customer segments by age, gender, and country, to tracking sales by buyer type and visualizing profit trends over time, the dashboards empower data-driven decision-making across marketing, inventory management, and strategic planning. Together, they serve as a dynamic tool for uncovering opportunities, reducing inefficiencies, and optimizing commercial performance.

### **1. Top/Bottom Analysis 1**

<img width="1331" height="751" alt="Novamed TopBottom Dashoboard1" src="https://github.com/user-attachments/assets/56d464a8-7a3d-42e2-91f7-a266c33fcc43" />

### **2. Top/Bottom Analysis 2**

<img width="1331" height="752" alt="Novamed TopBottom Dashoboard2" src="https://github.com/user-attachments/assets/ce0d3c53-0dc5-412e-ad30-f4987a28b618" />

### **3. Customer Analysis 1**

<img width="1327" height="751" alt="Novamed TopBottom Dashoboard5" src="https://github.com/user-attachments/assets/815dfa96-ffb8-41a0-9ae9-c72414a067ac" />

### **4. Customer Analysis 2**

<img width="1331" height="750" alt="Novamed TopBottom Dashoboard6" src="https://github.com/user-attachments/assets/55c1e3d6-6765-4aa6-b293-dce217a1fd29" />

## Key Insights

- Doxycycline leads as the top-performing drug, generating the highest revenue and profit, making it a crucial product for business growth.

- Top 5 drugs account for a significant share of total revenue, while several underperforming drugs contribute minimal returns, highlighting an opportunity to streamline the product portfolio.

- January consistently shows peak revenue and profit, suggesting strong seasonal performance early in the year, whereas February and August show noticeable drops that may require further analysis.

- High-value customers such as David Johnson and Bob Williams contribute millions in revenue, emphasizing the importance of customer retention and personalized engagement.

- Canada leads with 86 customers and the highest revenue, followed by Australia and the U.S., positioning them as NovaMed’s strongest geographic markets.

- Customers aged 40–50 and 60+ dominate the customer base, accounting for the largest share of purchases. These age groups are also key contributors to revenue.

- Males represent 47% of the customer base, and males aged 60+ alone generate $11.2M in revenue, identifying them as a high-value demographic segment.

- Buyers identified as “Users” outnumber “Sellers”, providing insight into purchasing behavior and the need for distinct strategies for each group.

- NovaMed achieved a profit margin of 81.97%, indicating strong operational efficiency and pricing strategy across most product lines.

- Total Revenue across the period (2022–2026) reached $71.31M, with a total of 200 customers and 269.47K units sold, reflecting solid overall performance and growth potential.

## Recommendations

Here are some recommendations to help stakeholders at NovaMed Solutions enhance sales performance, customer engagement, and operational efficiency based on insights drawn from the Power BI dashboards:

**Focus on Top-Selling Drugs:** Strengthen promotion and distribution of high-performing drugs like Doxycycline and Ergocalciferol, which contribute significantly to total revenue and profit. Ensuring adequate stock and continued visibility will maximize returns.

**Review Underperforming Products:** Investigate low-revenue and low-profit drugs such as Warfarin and Montelukast to understand challenges in demand, pricing, or positioning. Consider product optimization, rebranding, or potential phase-out.

**Leverage Monthly Sales Trends:** Monitor month-over-month revenue and profit trends closely. For example, capitalize on strong performance in January, and proactively plan for historically slower months like February and August by adjusting marketing and inventory strategies.

**Prioritize High-Value Customers:** Engage and retain top customers like David Johnson. Tailored communication, loyalty incentives, and account-based support can help maximize their lifetime value.

**Expand in Leading Markets:** Focus strategic expansion and marketing efforts on Canada and Australia, which lead in customer count and revenue. These regions present strong growth potential and should be prioritized for future campaigns.

**Target Key Demographics:** Develop age-specific marketing and service strategies focused on the 40–50 and 60+ age groups, which represent the largest share of the customer base.

**Design Inclusive Campaigns:** Use gender and buyer type insights (e.g., 47% male, 33% female, 21% other) to create personalized and inclusive messaging, ensuring relevance and stronger engagement across diverse customer segments.

**Track and Act on KPIs:** Continue monitoring key performance indicators like total revenue ($71.31M), profit margin (81.97%), and total quantity sold (269.47K) to guide sales strategy, pricing models, and operational improvements.

## Thank You
For more information, you can contact me
<img width="1010" height="251" alt="Contact shot" src="https://github.com/user-attachments/assets/c5d89cc2-7697-44cb-80d1-e7e456700bfd" />

