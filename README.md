Part 1: Data Analysis and Insight
1. Data Overview

The dataset titled "Cost of Living" provides comprehensive information on the average living expenses for monthly income across different countries, making it a valuable resource for comparing economic conditions worldwide. 

It includes 202 rows and 5 columns: Country, Year, Average Monthly Income, Cost of Living, and Region.
  
  - The Country lists the name of each country included (South Africa, China, India, Japan, France, Germany, Russia, Canada, Mexico, United States, Australia, Brazil) in the dataset. 
 
  - The Year (2000-2023) indicates when the data was collected. Average_Monthly_Income shows the average income earned per person per month. 
  
  - Cost_of_Living reflects the estimated average monthly expenses in each country. 
 
  - The Region categorizes each country into a broader geographical area such as Asia, Africa, Europe, North America, Oceania and South America. 

![image](https://github.com/user-attachments/assets/5fc374d6-1a80-4641-9174-323a5e395eb2)

Although the exact source of the data is not specified in the file, it likely draws from a combination of reputable global databases such as Numbeo, World Bank, International Labour Organization (ILO), International Monetary Fund (IMF) or from the government. This is because these organizations are commonly known for publishing the types of data like this for research or study. 

This dataset is useful for analyzing income-to-cost-of-living ratios, comparing economic well-being across countries and regions, and understanding global disparities in affordability and quality of life. 

2. Data Cleaning

![image](https://github.com/user-attachments/assets/7639dca2-e3b5-4480-93b3-f48bcd9aa4bf)

The missing values are in the column C (Avarage_Monthly_Income), at the rows 160 and 176. They are missing the Avarage_Monthly_Income. 

![image](https://github.com/user-attachments/assets/bfd183b0-13d4-47d8-a98f-3ef91b3887a2)

I chose to use the median as a measure of central tendency because it provides a more accurate representation of the typical country in the dataset. The average (mean) income can be skewed by a few very high-income countries, which inflates the overall figure and may not reflect the economic reality of most countries.
In contrast, the median represents the middle value in the distribution, ensuring that outliers (either very high or very low incomes) do not distort the result. This makes the median a more reliable indicator when analyzing global datasets with significant variation in income levels.

![image](https://github.com/user-attachments/assets/cb00b1bd-a01b-443c-88f2-a5d803ded27a)

The missing values are in the column D (Region), at rows 26 and 38. They are missing the Region name. 

![image](https://github.com/user-attachments/assets/f95178b8-c752-4e20-b838-569ae1ab7b6d)

In the dataset, the "Region" column is blank in these rows. To fill in the missing region, I examined other entries in the dataset and found that Mexico belongs to "North America". Assigning "North America" ensures consistency and accuracy. This approach also avoids data fragmentation and helps maintain clean, standardized categories for regional analysis.
 
 ![image](https://github.com/user-attachments/assets/e3001f81-5087-4047-a034-a5b8e117c7e2)

2 duplicate values: Data and Remove duplicate.
I chose to remove duplicate values in the Excel file because they could cause inaccuracies in the analysis. According to the notification, 2 duplicate rows were found and removed, leaving 200 unique entries. 
Keeping duplicates would have affected the summary statistics, visualizations, and overall interpretation of the data. Each country-year observation is only represented once, which improves the validity and clarity of the results. 

3. Descriptive Statistics
   
 ![image](https://github.com/user-attachments/assets/f6b8d4fc-8aee-427a-9b75-6d37d5f01880)

The average monthly income across countries is $4,244, while the average cost of living is $3,705. Although income is generally higher than living costs, both variables show high variation (with large ranges and standard deviations), suggesting strong economic disparities between countries. 
This indicates that while some countries (South Africa, China, India, Japan, France, Germany, Russia, Canada, Mexico, United States, Australia, Brazil) offer a comfortable balance between income and expenses, others may face challenges where cost of living is disproportionately high or income is very low.

Insight 1: The Relationship Between Income and Cost of Living

![image](https://github.com/user-attachments/assets/781108e5-c5ae-4622-9db6-b08f737d8043)

 
The scatter plot displays the relationship between average monthly income (y-axis) and cost of living (x-axis) across various data points (likely representing countries or regions). The points are widely scattered without forming a clear upward or downward pattern. This means there's no correlation between income and cost of living. Some countries with high costs of living do not always have high incomes, and some countries with low costs of living might still have high incomes. This weak relationship suggests that cost of living and income levels vary independently in many places.

Insight 2: Income and Living Cost Distribution Across Countries.

 ![image](https://github.com/user-attachments/assets/46f0c138-dc5f-4163-80a3-a8db6a1b379b)

Based on the chart, Europe and Asia have the highest total income and cost of living, indicating they contain many countries with high economic activity. However, North America stands out for having its total income almost equal to its total cost of living, suggesting that people in this region may have less disposable income compared to those in Europe or Asia. This highlights potential differences in financial comfort and savings potential across regions.


