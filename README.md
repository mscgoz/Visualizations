# Tableau_Public_Projects
Repo for all of my Tableau Public projects

1. Candy Dataset
2. OECD Secondary School Graduation Rates
3. ...
4. ...

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
| **Location**           | Displays a 3-letter country abbreviation representing the country (e.g., CZE). |
| **Indicator**          | Contains a single value, "enrollment," which stands for the enrollment rate.   |
| **Subject**            | Represents data categories split by age groups: **AGE_17**, **AGE_18**, and **AGE_19**. |
| **Measure**            | Indicates the unit of measurement, specifically a percentage: **PC_AGE**.      |
| **Frequency**          | Describes the reporting frequency of the data; it has one value: **A** (annual). |
| **Time**               | Refers to the year the data was collected (e.g., 2010, 2011, etc.).            |
| **Value**              | Represents the enrollment rate.                                                |
| **Flag Codes**         | Identifies potential errors in the data; the only flag is **M**, meaning "missing data." |

### 2.3. Data Visualizations - Tableau Links

https://public.tableau.com/views/Graduation_Rates_Deutschland/Sheet1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

https://public.tableau.com/views/EnrollmentRateDeutscland/Sheet1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

### 2.4. Source:

Reference: 
Organisation for Economic Co-operation and Development. (2024). Secondary graduation rate. https://www.oecd.org/en/data/indicators/secondary-graduation-rate.html

Dataset:
https://www.oecd.org/en/data/indicators/secondary-graduation-rate.html#indicator-chart
