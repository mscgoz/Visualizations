# Data Visualization PRojects
Repo for all of my Visualization projects

1. Candy Dataset - Tableau
2. OECD Secondary School Graduation Rates - Tableau
3. Loan Analysis - Amazon Quicksight
4. SaaS Sales Analysis - Amazon Quicksight
5. Flight Cancellation Analysis - Amazon Quicksight

## 1. Candy Dataset Visual Analysis

### 1.1. Introduction

The essence of Halloween is straightforward: provide satisfying treats to those in costumes or face potential late-night tricks from unhappy visitors. To help avoid such mishaps and to guide your candy-buying decisions this season, an experiment was designed to determine the most favored Halloween candies. By setting numerous fun-sized candy varieties against one another, the collective preference of participants was used to rank them.

Though the exact identities of voters remain unknown, data reveals that 8,371 unique IP addresses participated in approximately 269,000 randomized matchups. While this doesn’t qualify as a scientific survey, it offers a reasonable glimpse into popular candy preferences (Hickey, Laskowski, Chow, & Scherer, 2017).


### 1.2. Data Dictionary

| **Header**          | **Description**                                                                 |
|----------------------|---------------------------------------------------------------------------------|
| **chocolate**        | Indicates whether the candy contains chocolate.                                |
| **fruity**           | Specifies if the candy is fruit-flavored.                                      |
| **caramel**          | Denotes the presence of caramel in the candy.                                  |
| **peanut_almondy**    | Indicates if the candy contains peanuts, peanut butter, or almonds.            |
| **nougat**           | Specifies whether the candy includes nougat.                                   |
| **crisped_ricewafer** | Highlights if the candy has crisped rice, wafers, or cookie elements.          |
| **hard**             | Identifies whether the candy is classified as hard candy.                      |
| **bar**              | Specifies if the candy is a bar-style product.                                 |
| **pluribus**         | Indicates if the candy is sold as part of a bag or box with multiple pieces.   |
| **sugar_percent**     | Represents the sugar content percentile within the dataset.                    |
| **price_percent**     | Denotes the unit price percentile compared to all candies in the dataset.      |
| **win_percent**       | Reflects the candy's win percentage based on 269,000 head-to-head matchups.    |

### 1.3. Data Visualizations - Tableau Links


### 1.4. Source:

Reference: 
Hickey, W., Laskowski, C., Chow, T., & Scherer, E. (2017, October 27). The Ultimate Halloween Candy Power Ranking. FiveThirtyEight. Retrieved from https://fivethirtyeight.com/videos/the-ultimate-halloween-candy-power-ranking/

Dataset:
https://github.com/fivethirtyeight/data/tree/master/candy-power-ranking

## 2. OECD Secondary School Visual Analysis

### 2.1. Introduction

The secondary graduation rate refers to the projected proportion of individuals expected to complete secondary education during their lifetime. The data is categorized by gender and presented for both upper-secondary and post-secondary, non-tertiary education levels (Organisation for Economic Co-operation and Development, n.d.).

### 2.2. Data Dictionary

grad rate sheet:

| **Header**          | **Description**                                                                 |
|----------------------|---------------------------------------------------------------------------------|
| **Location**  | Displays a 3-letter country code representing the country (e.g., CZE).         |
| **Indicator**  | Contains a single value, "gradrate," meaning "graduation rate"; included only to maintain consistency across OECD datasets. |
| **Subject**    | Specifies the subcategory of data, divided by gender and school level.     |
| **Measure**    | Indicates the unit of measurement: **PC** for percentage or **A** for annual count. |
| **Frequency**  | Shows how often the data is reported; the only value is **A** (annual).     |
| **Time**       | Represents the year the data was collected (e.g., 2010, 2011, etc.).       |
| **Value**      | Displays the graduation rate.                                              |
| **Flag Codes** | Identifies potential errors in the data; the only flag is **M** (missing data). |

enrollment sheet:

| **Header**            | **Description**                                                                 |
|------------------------|---------------------------------------------------------------------------------|
| **Location**           | Displays a 3-letter country code representing the country (e.g., CZE).  |
| **Indicator**          | Contains a single value, "enrollment," which stands for the enrollment rate.   |
| **Subject**            | Represents data categories split by age groups: **AGE_17**, **AGE_18**, and **AGE_19**. |
| **Measure**            | Indicates the unit of measurement, specifically a percentage: **PC_AGE**.      |
| **Frequency**  | Shows how often the data is reported; the only value is **A** (annual).     |
| **Time**       | Represents the year the data was collected (e.g., 2010, 2011, etc.).       |
| **Value**      | Displays the graduation rate.                                              |
| **Flag Codes** | Identifies potential errors in the data; the only flag is **M** (missing data). |

### 2.3. Data Visualizations - Tableau Links

https://public.tableau.com/views/Graduation_Rates_Deutschland/Sheet1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

https://public.tableau.com/views/EnrollmentRateDeutscland/Sheet1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

### 2.4. Source:

Reference: 
Organisation for Economic Co-operation and Development. (2024). Secondary graduation rate. https://www.oecd.org/en/data/indicators/secondary-graduation-rate.html

Dataset:
https://www.oecd.org/en/data/indicators/secondary-graduation-rate.html#indicator-chart

## 3. Loan Analysis

### 3.1. Introduction

In this project, I explored the [LoanData.csv] dataset to understand credit behavior, borrower purposes, and loan performance outcomes through interactive visualizations. The primary goal was to interpret how loan purposes relate to final loan status — whether loans are paid, defaulted, or currently active.

Using Amazon QuickSight, I built a Sankey Diagram to map the flow between Loan Status and Purpose fields. This format clearly shows which loan purposes are most common, and how they correlate with repayment success.

### 3.2. Data Dictionary


| **Header**          | **Description**                                                                |
| ------------------- | ------------------------------------------------------------------------------ |
| **id**              | Unique identifier for each loan application or record.                         |
| **loan\_amnt**      | Total loan amount requested by the borrower.                                   |
| **term**            | Duration of the loan, typically in months (e.g., 36 or 60 months).             |
| **int\_rate**       | Annual interest rate charged on the loan, expressed as a percentage.           |
| **installment**     | Monthly payment amount the borrower agrees to pay.                             |
| **grade**           | Credit risk grade assigned to the loan (ranging from A to G).                  |
| **emp\_length**     | Number of years the borrower has been employed (e.g., "10+ years", "<1 year"). |
| **home\_ownership** | Borrower's home ownership status (e.g., RENT, OWN, MORTGAGE).                  |
| **annual\_inc**     | Annual income reported by the borrower.                                        |
| **purpose**         | Reason for taking the loan (e.g., debt consolidation, credit card, medical).   |
| **loan\_status**    | Final status of the loan (e.g., fully paid, charged off, current).             |
| **addr\_state**     | U.S. state abbreviation where the borrower resides (e.g., CA, NY, TX).         |


### 3.3. Data Visualizations 

[📄 View Full Report (PDF)](./loan_report.pdf)

### 3.4. Source:

Reference: 
Exploring the Generative Business Intelligence Features in Amazon QuickSight (2025). https://explore.skillbuilder.aws/learn/courses/21647/lab-exploring-the-generative-business-intelligence-features-in-amazon-quicksight

Dataset:
https://explore.skillbuilder.aws/learn/courses/21647/lab-exploring-the-generative-business-intelligence-features-in-amazon-quicksight

## 4. SaaS Sales Analysis

### 4.1. Introduction

In this project, I analyzed the SaaS-Sales.csv dataset to uncover sales performance trends across time, industries, customer segments, and geographic locations. The objective was to evaluate growth behavior, detect high-performing markets, and identify strategic areas for improvement.

Using Amazon QuickSight, I built interactive visuals such as time series charts, donut breakdowns, Sankey diagrams, and geospatial maps to capture a multi-dimensional understanding of sales dynamics.

### 4.2. Data Dictionary


| **Header**       | **Description**                                                        |
| ---------------- | ---------------------------------------------------------------------- |
| **City**         | Name of the city where the order was placed.                           |
| **Contact Name** | Name of the customer contact person.                                   |
| **Country**      | Country in which the transaction occurred.                             |
| **Customer**     | Name of the customer or organization.                                  |
| **Customer ID**  | Unique identifier for each customer.                                   |
| **Date Key**     | Date value for joining or filtering time-based data.                   |
| **Discount**     | Discount rate applied to the order, expressed as a percentage.         |
| **Industry**     | Industry sector associated with the customer (e.g., Tech, Healthcare). |
| **License**      | Type of SaaS license purchased.                                        |
| **Order Date**   | Date on which the order was placed.                                    |
| **Order ID**     | Unique identifier for each transaction.                                |
| **Product**      | Name of the SaaS product sold.                                         |
| **Profit**       | Net profit generated from the transaction.                             |
| **Quantity**     | Number of product licenses or units sold.                              |
| **Region**       | Broad geographic region (e.g., EMEA, AMER, APJ).                       |
| **Row ID**       | Row identifier for internal tracking.                                  |
| **Sales**        | Total sales amount generated.                                          |
| **Segment**      | Customer classification: SMB, Enterprise, or Strategic.                |
| **Subregion**    | More specific location grouping under each region.                     |



### 4.3. Data Visualizations 

[📄 View Full Report (PDF)](./saas_report.pdf)

### 4.4. Source:

Reference: 
Creating Interactive Dashboards with Amazon QuickSight (2025). https://explore.skillbuilder.aws/learn/course/internal/view/elearning/22329/lab-create-interactive-dashboards-with-amazon-quicksight

Dataset:
https://explore.skillbuilder.aws/learn/course/internal/view/elearning/22329/lab-create-interactive-dashboards-with-amazon-quicksight

## 5. Flight Cancellation Analysis 


### 5.1. Introduction

I analyzed a dataset containing over 12 million flight records that involved US airports as either departure or arrival points. Within this dataset, approximately 250,000 flights were marked as cancelled between 2020 and 2022. I conducted an exploratory analysis to uncover patterns behind these cancellations, with a focus on potential correlations between cancellation reasons, airline carriers, and airport-specific trends.

### 5.2. Data Dictionary

cancelled flight table 

| **Header**                         | **Description**                                                               |
| ---------------------------------- | ----------------------------------------------------------------------------- |
| **FLIGHT\_DATE**                   | Date of the flight (YYYY-MM-DD format).                                       |
| **DAY\_OF\_WEEK**                  | Day of the week on which the flight was scheduled.                            |
| **OP\_CARRIER**                    | Two-letter code representing the operating carrier.                           |
| **CARRIER\_NAME**                  | Full name of the airline carrier operating the flight.                        |
| **OP\_CARRIER\_FL\_NUM**           | Carrier-specific flight number.                                               |
| **ORIGIN**                         | Three-letter IATA code of the origin airport.                                 |
| **DISPLAY\_AIRPORT\_NAME\_ORIGIN** | Full name of the origin airport.                                              |
| **DEST**                           | Three-letter IATA code of the destination airport.                            |
| **DISPLAY\_AIRPORT\_NAME\_DEST**   | Full name of the destination airport.                                         |
| **CANCELLATION\_CODE**             | Reason for cancellation (if cancelled).                                       |
| **NUMBER\_OF\_FLIGHTS**            | Number of scheduled flights (usually 1 per row).                              |
| **LATITUDE\_ORIGIN**               | Geographic latitude of the origin airport.                                    |
| **LONGITUDE\_ORIGIN**              | Geographic longitude of the origin airport.                                   |
| **LATITUDE\_DEST**                 | Geographic latitude of the destination airport.                               |
| **LONGITUDE\_DEST**                | Geographic longitude of the destination airport.                              |
| **DISTANCE\_LEGEND**               | Categorized flight distance (e.g. "2500 Miles and Greater", "Less Than 250"). |


cancellation codes table

| **Header** | **Description**     |
| ---------- | ------------------- |
| **A**      | Carrier             |
| **B**      | Weather             |
| **C**      | National Air System |
| **D**      | Security            |


### 5.3. Data Visualizations 

[📄 View Full Report (PDF)](./flight_report.pdf)

### 5.4. Source:

Reference: 
Building BI Dashboards with Amazon QuickSight (2025). https://explore.skillbuilder.aws/learn/course/internal/view/elearning/16904/building-bi-dashboards-with-amazon-quicksight

Dataset:
https://us-west-2-tcprod.s3.amazonaws.com/courses/SPL-TF-100-ANQSDB/v1.0.8.prod-9fb9b762/scripts/all-cancelled-flights.csv
https://us-west-2-tcprod.s3.amazonaws.com/courses/SPL-TF-100-ANQSDB/v1.0.8.prod-9fb9b762/scripts/cancellation-codes.csv
