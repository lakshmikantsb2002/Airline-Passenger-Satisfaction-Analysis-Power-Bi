# Airline-Passenger-Satisfaction-Report
Airline Passenger Satisfaction Report using Power BI
I have done this Airline Pasenger Satisfaction Report using Power BI while i was doing an  Data Analytics Internship at DharwadHubballiTutor Company.

Introduction


Most people don’t know it but the aviation industry is very competitive. In this competitive environment, distinctive factors could make an airline stand out from the others. A very good example of such factor is customer’s satisfaction. Customer’s satisfaction is very crucial in the aviation industry. Passengers are the primary focus in this industry as airlines rely on them for their operations to function effectively. Hence, airlines need to understand the needs and wants of their customers in order to provide unique experiences. A passenger’s journey encompasses the entirety of their travel experience, beginning from the initial stages of trip planning to the moment they arrive at their destination. As a Data-analyst, I have been brought in to analyze an airline’s data and find the key areas to focus on that could help improve passenger’s satisfaction rate.

Data

Data Description

For this particular case study, I analyzed the dataset which was obtained from Kaggle. The dataset provides a complete summary of how satisfied passengers are when travelling by our airline. The data was collated on a spreadsheet (Microsoft Excel) and it includes additional information about each passenger, their experience on the flight, type of travel as well as evaluation of other different factors such as cleanliness, comfort and their satisfaction level from 1 (lowest) to 5 (highest) etc.

Data Cleaning and transformation

The first stage of every data analysis process involves verifying the quality and reliability of the data. Therefore, cleaning of the dataset was necessary and this was carried out using Microsoft Excel. Upon examining the dataset, it was discovered that there weren’t many cleaning tasks required. The dataset was then imported into Power BI using the “Get Data” option and transformed using power query for cleaning. While studying the dataset, I made the choice to categorize the “Age” column into five “Age_categories” for better understanding and analysis. This process involved utilizing the “conditional column” feature and “IF” statements were employed during the execution of this task.


Sneak peek showing the IF statements on Power BI
The same procedure was applied to the “Flight distance” column. I opted to classify the “Flight distance” column into three “Miles_categories” to enhance the analysis process.


While in Power BI, I utilized DAX functions such as “COUNT”, “SUM”, and “CALCULATE” to create measures in Power BI. Later on, I incorporated these measures into a dashboard to enhance analytical insights. Some of which include:

Using the “COUNT” function to find the total number of unique passengers recorded in the datase
No of Customers = COUNTROWS(train)

Also, I proceeded to compute the Percentage of Arrivaldelay of Airplane who have expressed unsatisfaction with our airline services up to this point.
Percentage Arrivaldelay1 = CALCULATE(train([Number of Arrivaldelay1]/[total customers])

The process was repeated to determine the of passengers Percentage of Departuredelayof Airline are either neutral or dissatisfied with our airline services.
Percentage Departuredelay = CALCULATE(train([Number of Departuredelay]/[total customers])

Lastly, similar procedures were carried-out to compute the average age of our passengers and the average distance traveled by our airline so far.



Questions / Insights

After the cleaning in Excel and Power BI, the following questions were asked in order to derive insights:

How do specific groups respond to our airline services?

Upon examining the dataset, I discovered that passengers can be categorized based on gender and customer type. In terms of gender, I figured there doesn’t seem to be a particular gender that exhibits a consistently higher propensity for overall satisfaction with their travel experience with our airline.


Based on the chart, it can be inferred that gender does not influence passengers’ travel experiences with our airline services. Both genders display similar levels of satisfaction with our services, although a larger proportion of females express dissatisfaction compared to the other group.

Additionally, another group to consider in assessing responses to our airline service is the “customer type” category. This column describes the type of passenger, distinguishing between returning passengers and new passengers using our airline.


From my analysis, I discovered that returning passengers have equal level of satisfaction with our services while a greater percentage of new passengers express their dissatisfaction towards our services. This situation is very concerning to our business because new customers typically contribute more revenue and have the potential to refer others. If they are significantly unhappy with our services, it could overtime result in revenue loss for our airline.

How do passengers’ purpose of travel align with our airline services?

This question seeks to examine how passengers’ reasons for travelling affect their perceptions of our airline services. The column labelled “type of travel” describes the purpose of the passenger’s journey, distinguishing between flights for business purposes and those for personal reasons.


From my findings, I found that among approximately 89,000 passengers travelling for business purposes, 52,000 were satisfied with our airline services. However, a larger proportion of passengers travelling for personal reasons expressed dissatisfaction with our services.

Do factors such as travel class impact passengers’ satisfaction?


The data shows that passengers who travelled in business class expressed higher satisfaction with our services compared to those in economy and economy plus classes.

How does passengers’ satisfaction vary with age?

This question explores how passengers’ satisfaction might differ based on their age. Based on my research, I noticed that the “Adult group” (between 40 and 64) exhibits the highest level of dissatisfaction. Another interesting observation is that satisfaction rate rises with increasing age groups.


Creating interactive dashboards in Power BI involves designing visuals and adding interactive elements like slicers, filters and KPIs. These charts were put together on Power BI to make the dashboard as seen below:


Explore dashboard
Recommendations

● Contributing factors such as in-flight Wi-Fi services, cleanliness, online boarding, seat comfort etc. demand thorough attention, as these factors have a significant role in influencing passengers’ satisfaction levels. It is crucial to prioritize these factors and ensure they meet passengers’ expectations effectively.

● Identifying and giving priority to first-time passengers is essential as it serves as a strategy to boost our airline’s reputation through word-of-mouth referrals, ultimately leading to increased revenue.

● Online booking procedures should be improved on by making the user interface more friendly to accommodate both younger and older users, or alternatively, supplementing the process with additional instructions to facilitate a smoother booking experience.

● Consistently gather and assess feedback from passengers to pinpoint areas needing enhancement and evaluate the impact of implemented improvements. Utilize surveys and engage with passengers proactively to stay attuned to their changing preferences and requirements.

● Conduct thorough research on competitor airlines to identify key areas for improvement, enabling our airline to maintain a leading position and effectively compete within the industry.
