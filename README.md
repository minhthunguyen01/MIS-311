# 1. Data overview
## a. Data Description
The dataset titled "Cost of Living" provides an overview of the average monthly income and estimated cost of living across various countries and regions from 2000 to 2023.


The primary objective of this dataset is to understand and compare economic affordability across different countries and regions. By analyzing average monthly income alongside the cost of living, we can uncover how financially comfortable people are in various parts of the world.  


This is a structured, cross-sectional dataset combining both numerical and categorical variables for comparative economic analysis across different countries and regions.  


While the exact source of the dataset is not mentioned in the Excel file, this type of dataset the contents it is about clearly show that it can be extracted from public global databases like Numbeo and World Bank.  
## b. Data Structure
The dataset has 202 rows and 5 columns. For each column:  
- Country (Categorical) – The name of the country where the data was collected (Australia, Brazil, Canada, China, France, Germany, India, Japan, Mexico, Russia, South Africa,  and the United States). Among them, Mexico was the most reported country.  
![image](https://github.com/user-attachments/assets/8632a521-988a-4086-96dd-0b4dbd0aef2d)
- Year (Numerical) – The specific year in which the data was recorded (2000 - 2023).
- Average Monthly Income (Numerical) – The average monthly earnings of individuals in that country for the given year.
- Cost of Living (Numerical) – The estimated monthly cost required to sustain a standard lifestyle in that country.
- Region (Categorical) – The broader geographical classification (e.g., Europe, Asia, North America, etc.).


Sample entry:  
![image](https://github.com/user-attachments/assets/8fd12e7e-0a57-4f6c-bc8f-ddc6d2308896)
# 2. Data Cleaning
## a. Missing Data
In the dataset, there are 2 missing values in the Average_Monthly_Income column (rows 162 and 178) and 2 missing entries in the Region column (rows 26 and 39) using Filter.  
![Screenshot 2025-05-14 122732](https://github.com/user-attachments/assets/e7e05530-2ec9-4c34-8f8e-21aebf4c3356)


![Screenshot 2025-05-14 122850](https://github.com/user-attachments/assets/8d320937-73c5-4e97-b7f4-877a74b7688b)  


The Median value is the most suitable method for filling in missing values in the Average_Monthly_Income column because it provides a more robust and accurate representation of typical income levels. Unlike the Average value, which can be significantly influenced by extreme values (outliers), the median selects the middle value in a sorted dataset, ensuring that unusually high or low income values do not distort the replacement value for missing entries.


The Descriptive Statistics tool in Excel’s Data Analysis Toolpak does indeed provide the median.
![Screenshot 2025-05-14 155405](https://github.com/user-attachments/assets/2f855b25-2608-4887-a5a7-11b4f25118df)


This result table shows that the Median of average monthly income equals 4270.4, so the value is filled in the two missing values in the Average_Monthly_Income column.
![Screenshot 2025-05-14 124147](https://github.com/user-attachments/assets/048c21d8-051e-4a7b-8fff-aad9edf55899)


In the Region column, handling missing data is easier because the countries are predefined. Therefore, based on the nations, the region will be determined. In both rows 26 and 39, the country is Mexico, so the region name used to fill the blanks is North America.
![Screenshot 2025-05-14 124206](https://github.com/user-attachments/assets/a347ec15-ebc1-40fe-a7aa-2440596f812a)
## b. Duplicates
Duplicates (rows 30 & 37, rows 42 & 45) were removed because they repeated the same data entries. Keeping them could distort analysis results or inflate counts. After removal, the dataset had 200 rows, accurate rows—ensuring reliable insights.
![Screenshot 2025-05-14 131525](https://github.com/user-attachments/assets/85a13926-36f3-4ef8-8f7f-6a0a7c5e1ab0)
# 3. Descriptive Statistics
![Screenshot 2025-05-14 155415](https://github.com/user-attachments/assets/b2d63428-f0f9-439a-a1eb-bb4a1dff1b76)


Living costs also fluctuate across countries and territories, influenced by market prices and economic policies. The data shows expenses range from $464.49 to $6,981.02, with an average of $3,705.13 and a median of $3,688.09. While the distribution is relatively balanced, the wide range ($6,516.53) highlights significant differences in living standards and spending habits among regions.


![Screenshot 2025-05-14 155405](https://github.com/user-attachments/assets/538c9af8-f1dc-44de-ab67-efb458fa1588)


The average monthly income across countries and territories varies significantly, reflecting differences in economic conditions. According to the data, incomes range from $534.74 to $7,976.56, with an average of $4,274.95. Although the median ($4,270.4) is close to the average, the high standard deviation ($2,139.82) indicates considerable disparities between regions, affecting living standards and development opportunities.
## a. Insight 1: Global Cost of Living Comparison: Africa Highest, Asia Lowest Across Continents (2000 - 2023)
![image](https://github.com/user-attachments/assets/02bcbc70-3923-40c4-8012-cfc29d42e360)


The average cost of living varies significantly across continents. Africa has the highest cost at $3963.17, while Asia has the lowest at $3645.29. North America ($3750.07) and Oceania ($3913.40) have relatively high costs, reflecting living standards and the prices of goods and services. Europe and South America have lower costs, at $3554.35 and $3585.02, respectively. These differences highlight the economic and social factors that influence living expenses worldwide.
## b. Insight 2: Uncovering Income Gaps: A Closer Look at Monthly Earnings in Asia (2000 - 2023)
![image](https://github.com/user-attachments/assets/6e1f019e-1d3e-494e-97b0-f877974904c9)


The chart presents the average monthly income for China, India, and Japan within the Asian region. India ranks highest with an average monthly income of $4,294.91, followed by Japan at $4,195.25, while China has the lowest at $4,041.26. Although the income gap between the countries is relatively small, India exceeds China by approximately $253.65 and Japan by $99.66, suggesting slight regional disparities in earnings that may reflect differences in economic structure, cost of living, or labor market conditions.


