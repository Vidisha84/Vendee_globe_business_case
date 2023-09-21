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

https://github.com/Vidisha84/Vendee_globe_business_case/blob/main/lambda.png

To complete this business case, we need to do the following steps:

1.Create a Lambda Architecture in Azure with a real-time path and a batch-processing path. Our architecture should include an Event Hub, a Stream Analytics Job, and an output to PowerBI. The batch-processing path can use any data storage service you prefer: a Data Lake, a SQL Database, a Cosmos database, or a Synapse Analytics Workspace.
2.Create a PowerBI dashboard that displays a world map with the current location of each racing team, and a table with the teams ranked by position in the race.
3.Download the Python race simulation app to your local computer. Configure the app to send data to your EventHub.
4.Start the Python app. Every 60 seconds, the telemetry of the simulated racing boats will be sent to your Azure cloud.

 You will have completed the business case if your PowerBI dashboard correctly shows the position and ranking of each sailing team in the 
 race.

 ## Getting started
 To help us get started, guided instructions were provided to build the first piece of the Lambda Architecture which consisted of an Event Hub and instructions to get the Python sailing simulator up and running.
