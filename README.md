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
## b. Duplicates
# 3. Descriptive Statistics
## a. Insight 1: Global Cost of Living Comparison: Africa Highest, Asia Lowest Across Continents (2000 - 2023)
## b. Insight 2: Uncovering Income Gaps: A Closer Look at Monthly Earnings in Asia (2000 - 2023)

