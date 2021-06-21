---
title:  "Serverless Hack: Build a Computer Vision enabled App"
metadate: "hide"
categories: [ Functions, Github, ML, Event Grid, CosmosDB]
image: "https://github.com/microsoft/WhatTheHack/raw/master/015-Serverless/images/preferred-solution.png"
visit: "https://github.com/microsoft/WhatTheHack/blob/master/015-Serverless/README.md"
---
In this hack, you will be solving the business problem of event driven scale for the Tollbooth Application.

Provision an Azure Storage Blob Container to store vehicle photos.
Set up Azure Functions to process the vehicle photos leveraging Event Grid.
Use Cognitive Services Computer Vision API OCR to comprehend the license plate data from the vehicle photos.
Store the license plate data in Azure Cosmos DB.
Provision a Logic App for obtaining the stored license plate data from Cosmos DB and exporting it to a new CSV file saved to Blob storage.
Use Application Insights to monitor the Azure Functions in real-time as data is being processed through the serverless architecture.