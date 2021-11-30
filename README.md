# MUSA508_Final

https://www.kaggle.com/pranavbadami/nj-transit-amtrak-nec-performance?select=2018_11.csv

## Questions
#### What is the use case? 

Trying to develop a plugin tool (Chrome extension?) that shows users who are planning to buy tickets whether their line/station has a higher likelihood of being delayed (over 20 minutes).

#### How could data make a difference in answering this question? Do you have a sense for the business as usual decision making?

OpenData is the basis of our tool; transit companies and agencies likely have more intricate data that they use to predict delays and decide how to internally optimize departures. 

#### What datasets have you identified to help you answer this question?

We are mainly using a dataset from Kaggle, which scrapes its data from the NJ Transit DepartureVision Real Time Train Status service. We are also using weather data from the RIEM R package.

#### What kind of model would you build and what is the dependent variable?

The model is a regression model, with delay being the dependent variable. 

#### How will you validate this model (cross-validation & goodness of fit metrics that relate to the business process)?

We will validate this model through cross-validation, because we are mostly predicting categorically for different brackets of time, and our data is continuous numeric data.

#### How do you think that stakeholders would want to consume this data?

Our first stakeholders, customers, would use this data to inform their ticket purchasing decisions. If transit agencies or companies become interested in our product, it could also be used for internal predictions and management.

#### What are the use cases for your app and what should the app do?

The app will be a plugin or pop-up on ticket purchasing sites for NJ Transit and Amtrak for different lines and times of day, showing the likelihood of delay and how long delay might be for that stop or train.

## Resources/Data

https://njogis-newjersey.opendata.arcgis.com/

NJ Transit rail station: https://njogis-newjersey.opendata.arcgis.com/datasets/NJTRANSIT::rail-stations-of-nj-transit/about

NJ Transit light rail station: https://njogis-newjersey.opendata.arcgis.com/datasets/NJTRANSIT::light-rail-stations-of-nj-transit/about


Amtrak Station: https://geo.dot.gov/server/rest/services/NTAD/Amtrak_Stations/MapServer/0


## Inspiration by the dataset owner:
Lots of interesting, high-impact projects could be driven by this data:

Robust prediction: This data could be used to derive a system-level prediction system for the NJ Transit network. Such a system could provide intelligent, targeted advance warnings of delays or cancellations for millions of riders.
Combining datasets: Weather data and service alert data could be incorporated to look at the effect of weather events and analyze the impacts of specific kinds of service interruptions.
Data visualization: Visualizing this data could provide robust insight into the system-level mechanics of the NJ Transit rail network, as well as more engaging reporting on NJ Transit.

For some more inspiration, you can check out Medium articles written by Michael Zhang and me with this data:

The 5 Stages of a System Breakdown on NJ Transit
What are the chances that NJ Transit will cause you to miss the Dinky?
How data can help fix NJ Transit


