# Forage Quantium Data Analytics Virtual Experience Program
My submission of this program's 3 tasks: 
- Data preparation and customer analytics,
- Experimentation and uplift testing, and
- Analytics and commercial application.

## Dependencies
Language: Python 3.8 \
Packages: pandas, matplotlib, mlxtend, datetime, sklearn, scipy

## Project Overview and Task Insights 
This virtual experience program involves analysing chip purchases at supermarkets.
The aim of this project was to evaluate different customers' purchasing behaviours and the performance of trial stores with a new layout to provide insights of customer preferences to the client 
and a recommendation of whether the trial has been successful. 

### Task 1: Data Preparation and Customer Analytics
Files: QVI_task1.ipynb, reads QVI_purchase_behaviour.csv and QVI_transaction_data.xlsx
- Data cleaning: changed the date from integer format to datetime data type, removed salsas and outliers 
- Analysed purchase behaviours of different customers (total sales, grouped by:
  - LIFESTAGE: customer attribute that identifies whether a customer has a family or not and what point in life they are at
  - MEMBER_TYPE: customer segmentation used to differentiate shoppers by the price point of products they buy and the types of products they buy. It is used to identify whether customers may spend more for quality or brand or whether they will purchase the cheapest options.
- A deeper dive into the Mainstream Young Singles/Couples segment to determine their preferences (chip brand and packet size) over other segments

Insights:
- The three highest contributing segments to total sales are: 1. Budget older families, 2. Mainstream young singles/couples, 3. Mainstream retirees
- Older families have largest avg no of packets purchased per customer, while the mainstream young singles/couples have the largest population
- Across most segments, Kettles chips and 175g packets are the most purchased
- Minstream young singles/couple are 28% more likely to purchase Tyrells chips than other segments, and 32% more likely to purchase 270g chip packets which are Twisties chips

### Task 2: Experimentation and Uplift Testing
Files: QVI_task2.ipynb, reads QVI_data.csv
- Three stores (77, 86, 88) undergo a new store layout with the trial period in Feb-Apr 2019
- Used the total sales and number of customers metric to generate a combined score to compare the trial and potential control stores with using Pearson correlations and magnitude distances
- Determined if difference in performance of those metrics of the control stores (stores with the highest score) compared to the trial store is significant using hypothesis testing 

Insights:
- Control and trial store pairs are:
  - 77 and 233
  - 86 and 155
  - 88 and 40
- For the total sales, store 77 saw a statistically significant increase (above the 95% control threshold) in Mar and Apr while store 86 saw an increase in Mar
- For the number of customers, both stores 77 and 86 saw significant increases in at least 2 months
- No significant change in performance due to the trial in store 88

### Task 3: Analytics and commercial application
- Prepared a report in Powerpoint highlighting key insights from Tasks 1 and 2 using the Pyramid Principle


