# AzureChatBot-Covid-Data

## Project Overview
This repository contains the code and resources for a chatbot that provides answers to frequently asked questions about COVID-19 and vaccinations. The chatbot is built on Azure's Bot Service and Language Understanding (LUIS), leveraging the power of Azure AI to provide accurate, up-to-date information sourced from reputable health organizations.

## Features
- Respond to user inquiries about COVID-19 symptoms, prevention, and vaccine availability.
- Utilizes Azure Cognitive Services for natural language processing and understanding.
- Can be integrated into multiple platforms such as websites, messaging apps, and social media platforms.

## How It Works
The chatbot uses a pre-trained model on Azure LUIS to understand user intent and provide relevant answers. It pulls information from a knowledge base that includes data from the Centers for Disease Control and Prevention (CDC) and Penn Medicine (MD).

## Getting Started
To get started with the COVID-19 FAQ Chatbot, you'll need to set up a few Azure services:
1. Azure Bot Service: Create a new bot resource on Azure.
2. Language Understanding (LUIS): Import the pre-built LUIS application for intent recognition.
3. QnA Maker: Set up a QnA Maker service to manage your knowledge base.

### Prerequisites
- An Azure subscription (Free Tier works with this chatbot)
- Basic knowledge of bot framework and Azure services
- [Optional] Knowledge of REST APIs for custom integration

## Installation
Clone the repository to your local machine using:
## Setup
Follow these steps to configure the chatbot in Azure:

1. Navigate to portal.azure.com and select "Language Services"
![Language Services](https://github.com/AdamKnight02/AzureChatBot-Covid-Data/assets/158077970/f505de27-bd20-454d-9dc5-f7f27236f3c3)
2. Once at language services select "Custom question answering" and select "Continue to create your resource"
![Custom Question Answering](https://github.com/AdamKnight02/AzureChatBot-Covid-Data/assets/158077970/59788ab1-1239-49a5-8940-c0517d9a4e55)
3. Once you reach the next page select "create new" under the resource group and type in whatever you'd the group to be called
![Create New Resource](https://github.com/AdamKnight02/AzureChatBot-Covid-Data/assets/158077970/bd60c2e9-1bd0-407e-a8ee-294b39430cb8)
4. Next for the region in the US select East or West US since those are the only regions that allow for Language services.
![Select Region](https://github.com/AdamKnight02/AzureChatBot-Covid-Data/assets/158077970/c30d824b-833d-4f05-a351-1e75a988f0df)
5. Ensure the Azure search region is the same as the instance region, name the instance whatever you like.
![Review and Create](https://github.com/AdamKnight02/AzureChatBot-Covid-Data/assets/158077970/f4392377-fe0c-4af4-964e-c895f91a62c2)
6. Certify that you've read the terms and conditions, then proceed to select Review + Create
![Language Studio](https://github.com/AdamKnight02/AzureChatBot-Covid-Data/assets/158077970/f6200660-b3a2-4fce-9064-799ecf175381)
7. Once the deployment has succeeded proceed back to https://language.cognitive.azure.com/
8. Select "Create new"
![Manage Sources](https://github.com/AdamKnight02/AzureChatBot-Covid-Data/assets/158077970/d6ce5c1e-755c-4a06-80d2-1c2536230d61)
9. Once the dialog box has opened up the information available and your resource group will auto-populate the page and select "done"
10. After the dialog box disappears select "Custom Question Answering" at the bottom of the webpage
![Question Pairs](https://github.com/AdamKnight02/AzureChatBot-Covid-Data/assets/158077970/6beb2963-f22d-435c-8e25-84e470e8641d)
11. Select "Manage sources" and add the data you would like analyzed
![Deployment Scripts](https://github.com/AdamKnight02/AzureChatBot-Covid-Data/assets/158077970/ff3550f6-1f2f-47e7-bf4e-40739b65ed4c)
12. From here you can add files or URLs for the purpose of this project I just added URLs
13. Once the data has been transcribed into Azure the question pairs section will auto-populate, I recommend skimming through the answers to spot-check any errors
![Data Set](https://github.com/AdamKnight02/AzureChatBot-Covid-Data/assets/158077970/a40c4500-f2a3-40c0-a14f-a5486170f10a)
Example of how it is used and how you can edit the text bots parameters to answer questions on other things such as service now tickets.
![Example](https://github.com/AdamKnight02/AzureChatBot-Covid-Data/assets/158077970/30e29673-27c4-49f8-94b4-217837a80380)
