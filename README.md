
# Largest Countries Analysis (Power BI Dashboard)

### Dashboard File : The dashboard can be simply downloaded from the files section above.

## Project Overview

This project is a data analysis dashboard that provides insights into some of the largest countries in the world by area: USA, Russia, India, China, Australia, and Canada. The dashboard allows users to explore, compare, and analyze key metrics related to these countries, including their geographical, demographic, economic, and environmental characteristics.

## Dashboard View (Power BI Desktop)

The dashboard consists of two pages that you can see below.

### Page 1: 

![page1](https://github.com/user-attachments/assets/c0789b32-6ec2-4ecf-b6e0-0df6c48ae4e7)

### Page 2:

![page2](https://github.com/user-attachments/assets/bf76cd45-8b9b-4da0-80df-b5cc95af5002)

## Steps followed 

- Step 1 : Load data into Power BI Desktop (from csv file). The full dataset is available here: 
https://www.kaggle.com/datasets/waqi786/country-comparison-dataset-usa-and-more

- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution" and "column quality" options.

- Step 3 : It was observed that in none of the columns errors & empty values were present. It says that the dataset is clean and is ready to making charts. 

- Step 4 : Some columns were removed from the dataset because their information was not relevant.

- Step 5 : The theme of the Dashboard was created manually. At the top of the dashboard, there is a main bar with filters. What's more, each visualization is enclosed in a gray frame.

- Step 6 : Vizualizations used in the dashboard:
a) Card (New) - visualization of average values (Page 1: Population, GDP, HDI; Page 2: Number of crimes, Military expenditure, Agricultural Land) 

b) Stacked Column Chart - visualization of avarage comparison for: 
(Page 1: Tourism Revenue, International Visitors; Page 2: Number of Airports)

c) Stacked Bar Chart - comparison of average Crime Rate for each country (Page 2). To show it in % I had to create New Metric named % Crime Rate. I used DAX expression below:
        
        % Crime Rate = AVERAGE(country_comparison_large_dataset[Crime Rate (per 100,000)]) / 100000

d) Line Chart - to show trends for Unemployment Rate and Population (Page 1)

e) Filled Map - to represent data in shaded areas. It was used for visualizing values across different countries. Maps were created for: Forest Coverage (Page 1) and Agricultural Land (Page 2)

f) Slicers - to filter the charts/plots by different categories (Year and Country)



# Insights

The dashboard was created in Power BI Desktop. This two-page report allows you to compare the specific countries (USA, Russia, China, Canada, India and Australia) by some geographical, demographic and economic metrics.

Following example inferences can be drawn from the dashboard:

### With no filters (from 2000 to 2023, for all countries)

#### From Page 1:
 - The highest Tourism Revenue is noticed in the USA = 221 B

![tr](https://github.com/user-attachments/assets/db728bb0-8187-46f2-a781-e2b8d3814e03)

 - The highest Forest Coverage is in Russia = almost 50 %

![forest](https://github.com/user-attachments/assets/a098bb05-69c9-417c-b0f5-d9edd9150710)

 - The average HDI in the world is 0.84 (India, Russia, China got HDI between 0,6 - 0,8 and USA, Canada, Australia got HDI over 0,9)

![hdi](https://github.com/user-attachments/assets/deb9db88-0145-4631-9271-ee1a47a8bf41)

- The lowest Population in the world was noticed in 2019

![pop](https://github.com/user-attachments/assets/b06554cd-4f05-48a8-a003-ec643f3dc2b6)

#### From Page 2:

- The highest Crime Rate is Australia (0,9 %) and the lowest in China (0,1 %)

![crime](https://github.com/user-attachments/assets/350ef133-25a1-4610-9872-efcfc3e54efc)

- The Literacy Rate in India is very low (74 %) comparing to other big countries

![literacy](https://github.com/user-attachments/assets/573e3d61-8453-46fc-bdea-ac0a2264c308)

- Number of Airports in USA is very high = 13,6 K

![airports](https://github.com/user-attachments/assets/aa87178d-f21a-45e4-9c15-1ee2a813fc07)











