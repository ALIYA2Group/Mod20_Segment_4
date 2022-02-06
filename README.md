# Mod20_Segment_4
# Final Presentation 
![P1](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P1.jpg)

The team members are Amber, Ayram, Leo, Leslie, deliver the presentation in 2 min equal proportions. The live presentation is scheduled for 7pm Friday, February 9th, 2022. 

Includes the following:
•	Demonstrates the interactivity of the dashboard in real time 
•	Includes speaker notes within README.md

# Presentation Speaker Notes (2 Minutes)

Our selected topic is analyzing and forcasting scientific data on the Arctic Poles melting and shrinking ice over time due to seasonal variance and other features. Based on past features of science exploration and calculation on melting and atmosphere changes we extracted, transformed and loaded the selected trends to show the sea-ice diminishing from 2003-2020 to try and predict future  size of the arctic sea ice extent.
We selected this topic becuase we wanted to predict at what point in time would the sea ice shrink. The source data was from the National Snow and Ice Data Center (NSIDC) and Climate Data Store. Source data was originally 15.5 Million rows. 

We explored Seasonal Variance, Surface pressure,Total column ozone, Average atmospheric carbon dixide (XCO2), Average atmospheric carbon dioxide (CO2) sea ice extent (Artic), 2m temperature, Sea-ice cover, Snow albedo, Snowmelt. These were the selected features of data as it pertains to melting sea ice and climate change; 

![P2](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P2.PNG)

The big data exploration phase of the project included analysis of climate change features from live daily stalite and station montitoring data that ae cloud synced ensuring long-term monitoring is possible. We extracted data to analyze from National Snow & Ice Data Center (NSIDC) and Climate Data Store. Loaded into Cloud services that allowed for more scalability and performance. And used supervised Machine Learning Regression Models. Using the following Technologies, languages, tools, and algorithms.

# Github 
## [AliyaGroup2 Github](https://github.com/ALIYA2Group)

# Google Slides
## [AliyaGroup2 Google Slides Presentation](https://docs.google.com/presentation/d/e/2PACX-1vTcX9jJk6ygnS3amtgkJ-ByMINvXs98Os4At5uzAr8ARsh10iMweahxc6NGSYjBHSQ_T0KmloQUrV55/pub?start=true&loop=true&delayms=3000)

# Final 
## [AliyaGroup2 Final](https://seaiceanalysis.appspot.com/)

# Machine Learning Model Speaker Notes(2 Minutes)

*	Result of the analysis
*	Recommendation for future analysis
*	Anything the team would have done differently
Slides
Presentations are finalized in Google Slides and should include:
*	Slides are primarily images or graphics (rather than primarily text).
*	Images are clear, in high-definition, and directly illustrative of subject matter.

Working code for machine learning model, as well as the following:
*	Description of data preprocessing
*	Description of feature engineering and the feature selection, including the decision-making process
*	Description of how data was split into training and testing sets
*	Explanation of model choice, including limitations and benefits
*	Explanation of changes in model choice (if changes occurred between the Segment 2 and Segment 3 deliverables)
*	Description of how the model was trained (or retrained, if the team is using an existing model)
*	Description and explanation of model's confusion matrix, including final accuracy score


# Model addresses the question and problem the team is solving, which Yes, we can montitor melting, and we can forcast variables, but we can not extract an exact date. 

IMPORTANT
If statistical analysis is not included as part of the current analysis, the team should describe how it would be included in the next phases of the project.

# Database Integration Speaker Notes (2 Minutes)
•	Result of the analysis
•	Recommendation for future analysis
•	Anything the team would have done differently

Live Presentation
The team members deliver the presentation in equal proportions. The live presentation should include the following:
•	Demonstrates the interactivity of the dashboard in real time
•	Adheres to the time limits provided by instructor
•	Includes speaker notes, flashcards, or a video of the presentation rehearsal

Students will be expected to present a final project with a fully integrated database.
•	Database stores static data for use during the project
•	Database interfaces with the project in some format (e.g., scraping updates the database)
•	Includes at least two tables (or collections, if using MongoDB)
•	Includes at least one join using the database language (not including any joins in Pandas)
•	Includes at least one connection string (using SQLAlchemy or PyMongo)
IMPORTANT
If you use a SQL database, you must provide your ERD with relationships.

# Dashboard and Website Speaker Notes(2 Minutes)
•	Result of the analysis
•	Recommendation for future analysis
•	Anything the team would have done differently

Live Presentation
The team members deliver the presentation in equal proportions. The live presentation should include the following:
•	Demonstrates the interactivity of the dashboard in real time
•	Adheres to the time limits provided by instructor
•	Includes speaker notes, flashcards, or a video of the presentation rehearsal

1. Using" beautiful soup" and "splinter" to scrap the news from idc website.
2. We put the scraping script in the "Google app engine Cron task" and it will automatically do the scraping everyday.
3. Store the data into MongoDB.
4. Deploy the web page to "Google app engine".
5. The website is using "Flask" and "pymongo" to show and read the data from MongoDB.


##Q&A:

1. Can you summarize the Project?  

We created the foundation for the final project. By defining roles between team members and establishing a communication structure. We wanted to see if we could predict the melting of Artic Sea Ice. We create a repository for the project and invite the other team members. We made great strides in building the different pieces of the project. The analysis come along nicely, and we worked on the machine learning model, and the databases were transitioned into an operational, data-holding tool. All of the individual pieces we've been building come together. We assembled these pieces, putting the final touches on the repository. Working on the README.md to fully describe the project and its purpose. The repository would be ready to be added to your portfolio. The team’s final task is to practice the presentation. Each of us will participate in the presentation over Zoom. Record it. There were slow spots, and sections to clarity. All loose ends that have been lingering were tied up especially anything related to the machine learning model, dashboard, or even the analysis. It was a short few weeks to perform ELT, MLT and Dashboard, and we were successful.  Based on past features of science exploration and calculation on melting and atmosphere changes we extracted, transformed and loaded the selected trends to  show the sea-ice diminishing from 2003-2020 to try and predict future  size of the arctic sea ice extent.
