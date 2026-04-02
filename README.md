# Assignment 2 – Clickstream Analytics with Azure Event Hubs
**Student Name**: Faiza Boudehane
**Student ID**: 041273470
**Semester**: Winter 2026

---ChatGpt was used in this lab

## Demo Video

🎥 [Watch Demo Video](https://youtu.be/seIHIOQA9Sc)

## Architecture
<img width="1012" height="336" alt="image" src="https://github.com/user-attachments/assets/5c46bffd-ff3d-42ac-998d-db2eafe56dec" />

## Design decisions
To enrich the events with devices information we needed to include it in the client webpage as the javascript function is defined there, this function get information and prepare the data payload to send to the Endpoint of events.
For the connection of the Stream analytics output to dashboard I opted for the use of a HTTP trigger function that send the newly queried result and event to the /api/events that already exists, then I had to update the Dashboard page by adding the device information to the output on the page, but this didn't work till now!
## Setup instructions
I used the local App and created on Azure the event hub namespace with one event hub and one function App that is based on HTTP trigger.
```
