---
title:  "Big Data Processing: Serverless MapReduce on Azure"
metadate: "hide"
categories: [ Durable Functions, Github, Big Data]
image: "https://github.com/Azure-Samples/durablefunctions-mapreduce-dotnet/raw/main/images/MapReduceArchitecture.png"
visit: "https://github.com/Azure-Samples/durablefunctions-mapreduce-dotnet/"
---
In this sample you will find handful of Azure Functions comprising a Mapper and Reducer to determine the average speed of New York Yellow taxi trips, per day over all of 2017.

You will use Durable Functions - specifically the Fan-out/Fan-in pattern - to distribute the workload across multiple instances of the Mapper then coordinate the outputs in to the Reducer and finally return the computed values for each day.

The source data you will be using for this MapReduce implementation can be found here: http://www.nyc.gov/html/tlc/html/about/trip_record_data.shtml and contains 12 CSV files of roughly 800MB each (Yellow dataset) you need to make available in Azure Blob storage - total size is ~9.6GB.