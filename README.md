# Mod20_Segment_4
# Final Presentation 
![P1](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P1.jpeg)

# Presentation (2 Minutes)
Our selected topic is analyzing and forcasting scientific data on the Arctic Poles melting and shrinking ice over time due to seasonal variance and other features. 
We selected this topic becuase we wanted to predict at what point in time would the sea ice shrink. The source data was from the National Snow and Ice Data Center (NSIDC) and Climate Data Store.
•	Description of the source of data
Based on past features of science exploration and calculation on melting and atmosphere changes we extracted, transformed and loaded the selected trends to show the sea-ice diminishing from 2003-2020 to try and predict future  size of the arctic sea ice extent.
We explored the following features of data; 
![P2](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P2.PNG)

the data exploration phase of the project
•	Description of the analysis phase of the project
•	Technologies, languages, tools, and algorithms used throughout the project
•	Result of the analysis
•	Recommendation for future analysis
•	Anything the team would have done differently


# Github 
#AliyaGroup2 
## [AliyaGroup2 Github](https://github.com/ALIYA2Group)


# Machine Learning Model (2 Minutes)
Students will be expected to submit the working code for their machine learning model, as well as the following:
•	Description of data preprocessing
•	Description of feature engineering and the feature selection, including the decision-making process
•	Description of how data was split into training and testing sets
•	Explanation of model choice, including limitations and benefits
•	Explanation of changes in model choice (if changes occurred between the Segment 2 and Segment 3 deliverables)
•	Description of how the model was trained (or retrained, if the team is using an existing model)
•	Description and explanation of model's confusion matrix, including final accuracy score
Additionally, the model obviously addresses the question or problem the team is solving.
IMPORTANT
If statistical analysis is not included as part of the current analysis, the team should describe how it would be included in the next phases of the project.

# Database Integration (2 Minutes)
Students will be expected to present a final project with a fully integrated database.
•	Database stores static data for use during the project
•	Database interfaces with the project in some format (e.g., scraping updates the database)
•	Includes at least two tables (or collections, if using MongoDB)
•	Includes at least one join using the database language (not including any joins in Pandas)
•	Includes at least one connection string (using SQLAlchemy or PyMongo)
IMPORTANT
If you use a SQL database, you must provide your ERD with relationships.

# Dashboard and Website

[Final Preview](https://seaiceanalysis.appspot.com/)

1. Using" beautiful soup" and "splinter" to scrap the news from idc website.
2. We put the scraping script in the "Google app engine Cron task" and it will automatically do the scraping everyday.
3. Store the data into MongoDB.
4. Deploy the web page to "Google app engine".
5. The website is using "Flask" and "pymongo" to show and read the data from MongoDB.