# Big Query COVID-19
There are multiple datawarehouseing options now a days. Amazon has Redshift, Microsoft has Azure SQL Data Warehouse and Google has BigQuery. There are several components which make each service worthy of using, it depends on the need of your business like frequency and size of each queries done during the day. 

## Motivation
This project was done with the idea of trying BigQuery and integrate it with the BI tool named Data Studio, both are part of the Google Cloud Platform enviroment so integration between both is very fluent. BigQuery is a serverless Datawarehousing service, they give a 12 month free of charge period (subject to a maximum of 300 GB of querying capacity). This means that you can either run out of credits before reaching the first 12 months or reach the due date beforehand. Queriess are done using standard SQL so the project also has the motivation of practicing SQL querying skills.

## Project
The project was developed using BigQuery public datasets regarding COVID-19. The tables architecure used can be seen in Tables.ipynb and the SQL queries used can be done inspecting SQL.ipynb.

The querying operations where tested in the BigQuery console in order to make sure we are using the intended data and it is structured appropriately. Once the queries where validated, we created a new report in Data Studio alongside 2 Data Sources which used the already tested customed SQL code in order to extract the data from the BigQuery covid-19 dataset.

## Dashboard
The data set found was very interesting. We have seen many dashboards indicating COVID-19 main statistichs such as total cases, total deaths, daily cases, etc. This Dashboard includes those usual statistichs but the core of the report includes policies made by each government through time. The data used has its source in this url: https://www.bsg.ox.ac.uk/research/research-projects/coronavirus-government-response-tracker. The University of Oxford's School of Management developed a dataset that keeps track of governments policies regarding restrictions in multiple areas summarying their policies restrictiveness as "Stringency Index", more about this information can be found in Tables.ipynb. The dashboard provides a global view of government restrictiveness and its effects on the COVID-19 daily cases and deaths within a user friendly interface. Data is filtered by country and dates for the user's specific needs. 

## Why Data Studio?
Several reasons. Now a days the offer for BI tools its the highest its ever been. The market is dominated by heavy use Business Intelligence tools such as Power BI and Tableau, both very flexible and powerful in their own way. Although these BI tools can be also used in this use case, we wanted to try the more lightweight BI Tool called Data Studio provided by Google. The reasons are the following.
 - **Its free**: Data Studio is a very powerful tool which is free of use, compared to the mentiones tools which are not.
 - **Easy and pleasing design**: Data Studio offers the same capabilities when it comes to designing visuals or layouts as Power BI or Tableau. It lets the user customize the dashboard seemlessly. 
 - **Natural Integration with Big Query**: As we where working with Big Query, the natural option for visualizing our data fast and easy is using Data Studio, both are tools within the Google Cloud Platform. 
 
## Conclusions
BigQuery is a fantastic option when it comes to datawarehousing. Its ideal for businesses that do heavy big size queries few times a day for analysis. Due to the fact that Google Big Query charges you for computational resources when querying as well as storage the client doesnt have to pay any fee upfront,  it can save a lot of money compared to a service as Amazon Redshift that charges a monthly fee with unlimited querying capabilities. 

Its fast and uses standard SQL language. Lifetime SQL analysists can use this tool with ease in order to perform their Dashboards and reports. 

Data Studio performed the same tasks as a Power BI would have done. Having enough Power BI experience myself, the natural integration between Data Studio and Big Query using SQL made the task very comfortable when it came to importing the data to the dashboard. This BO Tool has almost every feature as the other BI tools as far as developing visuals and flexibility of use when it comes to data integration. 
