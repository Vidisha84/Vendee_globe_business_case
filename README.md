# Vendee_globe_business_case
The Vendée Globe is a solo non-stop round the world sailboatrace founded by Philippe Jeantot in 1989. The race takes placeevery four years and is considered an extreme quest ofindividual endurance and the ultimate test in ocean racing.
The 9th edition of the Vendee Globe was held in 2020-2021and was won by French sailor Yannick Bestaven who tookslightly over 80 days to sail non-stop around the globe.
During the race, spectators could follow the action live on anonline racing dashboard. The technology for tracking the boatslive was provided by Nokia.

## Your Challenge
In this business case, you will assume the role of Nokia. You will build a cloud-based Lambda Architecture to process the telemetry data from the sailing boats. 
Your architecture should run in Azure and contain a real-time path for processing sailing boat data in real-time, and a batch-processing path
for collecting sailing boat data in batches and performing calculations on those batches.

The Lambda Architecture should send all boat data to a PowerBI dashboard. The dashboard should display a world map with the current position of each boat, and a table with a ranking of racing teams. The ranking table should be sorted by who is currently in the lead.

When I initially developed this project, there was no ongoing Vendee Globe race. To work around this, I utilized an application that simulates real-time data from Vendee Globe Race participants. This app was not developed by me, but I incorporated it into my project to provide the necessary information. You can access the app through this link: https://github.com/mdfarragher/TCS/blob/main/race_simulator.py

![Lambda architecture](https://github.com/Vidisha84/Vendee_globe_business_case/blob/main/lambda.png)


To complete this business case, we need to do the following steps:

1.Create a Lambda Architecture in Azure with a real-time path and a batch-processing path. Our architecture should include an Event Hub, a Stream Analytics Job, and an output to PowerBI. The batch-processing path can use any data storage service you prefer: a Data Lake, a SQL Database, a Cosmos database, or a Synapse Analytics Workspace.

2.Create a PowerBI dashboard that displays a world map with the current location of each racing team, and a table with the teams ranked by position in the race.

3.Download the Python race simulation app to your local computer. Configure the app to send data to your EventHub.

4.Start the Python app. Every 60 seconds, the telemetry of the simulated racing boats will be sent to your Azure cloud.

 You will have completed the business case if your PowerBI dashboard correctly shows the position and ranking of each sailing team in the 
 race.

 ## Getting started
 To help us get started, guided instructions were provided to build the first piece of the Lambda Architecture which consisted of an Event Hub and instructions to get the Python sailing simulator up and running.

To complete the business case, here's what needed to add:

1. The remaining pieces of the Lambda Architecture: a Stream Analytics Job, an output to PowerBI, and a second output to a data storage service of your choice.

2.A data storage service of your choice to store batch data: a Data Lake, a SQL Database, a Cosmos database, or a Synapse Analytics
Workspace.

3.A view or stored procedure or Synapse notebook to calculate the table of teams ranked by position in the race.

4.A PowerBI dashboard that displays a world map with the current location of each racing team,and a table with the teams ranked by position in the race.

## Challenges

During the business case, we need to address several challenges:

. The Python app occasionally produces garbled data. How are you going to ensure that only clean data arrives in the PowerBI dashboard?

. How are you going to calculate the ranked list of sailing teams? How will you calculate who is ahead in the race?

. Which data service are you going to use for the batch-processing path in the Lambda Architecture?

. How will you present your data in the PowerBI dashboard?

There are multiple solutions for each challenge

## To solve the challenges started with following steps
 
 ### Set up an Event hub
 
![image](https://github.com/Vidisha84/Vendee_globe_business_case/assets/145435974/bdf85d03-a5db-41a2-9cb6-3810d42c9aa6)



### Downloaded and Configure the python sailing simulator

![image](https://github.com/Vidisha84/Vendee_globe_business_case/assets/145435974/3ba50dd5-2178-4863-90bb-fb94cb144253)


### Connected Python stimulator with eventhub endpoints and name.It starts running

![image](https://github.com/Vidisha84/Vendee_globe_business_case/assets/145435974/34a32921-3379-4ec6-b017-bfbb087e327b)


### Set up Stream Analytics for streaming data
![image](https://github.com/Vidisha84/Vendee_globe_business_case/assets/145435974/1e18f3cf-a5a7-4593-9c5f-952065215b62)


### For batch data created Data lake storage Gen2
![image](https://github.com/Vidisha84/Vendee_globe_business_case/assets/145435974/802ccca3-8d41-4332-93f6-af251ff72c6d)


### Created Outputs

![image](https://github.com/Vidisha84/Vendee_globe_business_case/assets/145435974/9df8c4dc-bbeb-4567-b28e-283f314e791c)









