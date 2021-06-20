---
title:  "Serverless recipes with Azure Cosmos DB and Azure Functions"
metadate: "hide"
categories: [ CosmosDB, Github]
image: "https://www.bing.com/th?id=OIP.EgSPriuEnAtlIWJV8R_E1QHaGs&w=108&h=100&c=8&rs=1&qlt=90&o=6&dpr=2&pid=3.1&rm=2"
visit: "https://github.com/ealsur/serverless-recipes"
author: "yaya"
---

This repository acts as compendium of different recipes using Azure Cosmos DB and Azure Functions.

The content is distributed in different folders, each for a different scenario:

Cosmos DB Input Binding: Contains samples on how to use the Cosmos DB Input Binding to run queries and read data from your Cosmos DB containers.
Cosmos DB Output Binding: Contains samples on how to use the Cosmos DB Output Binding to save a single document or multiple documents to your Cosmos DB containers.
Client management: Contains samples on how to best use a custom Cosmos DB SDK client within Azure Functions optimizing for best performance and avoiding common pitfalls.
Cosmos DB Trigger: Contains a complete sample using Cosmos DB, Azure Cognitive Services, and Azure Signal R to create a flow of data analysis based on events happening in a Cosmos DB container.
Cosmos DB Trigger Scenarios: Contains scenario samples like sharing the leases container.
Custom ConnectionMode & Protocol: Contains a complete sample to customize the ConnectionMode and Protocol used in the internal DocumentClient instances for bindings and trigger.
Monitoring the Cosmos DB Trigger progress: Contains a sample to leverage the Remaining Work Estimator and send progress to App Insights.