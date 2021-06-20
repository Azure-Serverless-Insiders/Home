---
title:  "Real-time Speech-to-Text and Translation with Cognitive Services, Azure Functions, and SignalR Service"
metadate: "hide"
categories: [ Functions, ML]
image: "https://anthonychu.ca/post-assets/2019-03-26/architecture.png"
visit: "https://anthonychu.ca/post/realtime-captioning-translation-cognitive-services-signalr-azure-functions/"
---
The app consists of two projects:

A Vue.js app that is our main interface. It uses the Microsoft Azure Cognitive Services Speech SDK to listen to the device's microphone and perform real-time speech-to-text and translations.

An Azure Function app providing serverless HTTP APIs that the user interface will call to broadcast translated captions to connected devices using Azure SignalR Service.