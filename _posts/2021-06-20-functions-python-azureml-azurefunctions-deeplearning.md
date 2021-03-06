---
title:  "Training a Model with AzureML and Azure Functions"
metadate: "hide"
categories: [ Functions, Github, ML]
image: "https://github.com/Azure-Samples/functions-python-azureml-azurefunctions-deeplearning/raw/master/images/arch_diagram.png"
visit: "https://github.com/Azure-Samples/functions-python-azureml-azurefunctions-deeplearning/"
---
Automating the training of new ML model given code updates and/or new data with labels provided by a data scientist, can pose a challenge in the context of the dev ops or app development process due to the manual nature of data science work. One solution would be to use a training script (written by the data scientist) with the Azure Machine Learning SDK for Python (Azure ML Python SDK) run with a lightweight Azure Function that sends a training script to larger compute (process managed by the dev ops professional) to train an ML model (automatically performed when new data appears). This, then, triggers the build and release of an intelligent application (managed by the app developer).


The intent of this repository is to communicate the process of training a model using a Python-based Azure Function and the Azure ML Python SDK, as well as, to provide a code sample for doing so. Training a model with the Azure ML Python SDK involves utilizing an Azure Compute option (e.g. an N-Series AML Compute) - the model is not trained within the Azure Function Consumption Plan. Triggers for the Azure Function could be HTTP Requests, an Event Grid or some other trigger.