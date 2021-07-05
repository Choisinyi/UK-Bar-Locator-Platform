

# UK Bar Locator Platform

## Key takeaways: 
1. Chatbot
2. Recommendation System 
3. Streamlit Web app

## ![Screenshot (52)](https://user-images.githubusercontent.com/80455832/122505976-fd800d00-d02f-11eb-98a9-59ade9ff72b0.png)
# Table of Contents:

- Business Objectives
- AI Chatbot
- Recommendation system
          - Data Collection
          - Pre-Processing
          - Model Development & Predictions
- Limitations & Next steps


# Business Objectives
With people across the UK itching to get out from lockdown as a result of Covid-19 and understanding that pubs plays a significant role in English culture, this streamlit app is designed to recommend and help you find bars near you. By doing so, we hope to achieve the following:

- Help customers find new pubs
- Help local pubs find new potential customers
- Assist tourist that might be unfamiliar with the area looking to visit a pub

# Part A: AI Chatbot
Mainly using the Google dialogflow to build the AI Chatbot

Intents:
- 1. Suggest different types of pubs and drinks -> Pop up the result of high-ranked restaurants from website
- 2. Connect to Google Canledar API -> Help the users to markdown an appointment for drinks on their own Google Canledar automatically
- 3. Ask for the nearest pubs-> help guiding the users to Recommendation System -> Streamlit -> (direct to Part B)

![Screenshot (60)](https://user-images.githubusercontent.com/80455832/122524438-b3f0eb80-d04a-11eb-81fc-11c57e2f6d7a.png)

![Screenshot (61)](https://user-images.githubusercontent.com/80455832/122524425-b05d6480-d04a-11eb-91b4-3b53302ca45a.png)


# Part B: Recommendation System with Streamlit web app

![Screenshot (68)](https://user-images.githubusercontent.com/80455832/122540835-98daa780-d05b-11eb-8143-0fbeeffecfdd.png)
![Screenshot (78)](https://user-images.githubusercontent.com/80455832/122547040-30db8f80-d062-11eb-9c38-56d3edecde68.png)

## 1) Data collection
The data was collected using the open-source platform Kaggle on every pub within the UK

Link: https://www.kaggle.com/rtatman/every-pub-in-england

Overview: This dataset includes information on 51,566 pubs in the UK

Data Upload Year: 2017 (outdated but used for learning purpose)

Contents:

- fsa_id (int): Food Standard Agency's ID for this pub.
- name (string)L Name of the pub
- address (string): Address fields separated by commas.
- postcode (string): Postcode of the pub.
- easting (int)
- northing (int)
- latitude (decimal)
- longitude (decimal)
- local_authority (string): Local authority this pub falls under

## 2) Preprocessing & EDA

![Screenshot (79)](https://user-images.githubusercontent.com/80455832/122547050-33d68000-d062-11eb-885c-f78be433fe2b.png)
![Screenshot (81)](https://user-images.githubusercontent.com/80455832/122547091-3cc75180-d062-11eb-86c4-181d4eabae9c.png)

## 3) Model development-- K-Means
![Screenshot (82)](https://user-images.githubusercontent.com/80455832/122547102-3f29ab80-d062-11eb-85ac-637a4a811447.png)
![Screenshot (83)](https://user-images.githubusercontent.com/80455832/122547122-451f8c80-d062-11eb-974a-8c6c871fda67.png)
![Screenshot (84)](https://user-images.githubusercontent.com/80455832/122547126-481a7d00-d062-11eb-9413-b337677e33a0.png)
![Screenshot (85)](https://user-images.githubusercontent.com/80455832/122547136-4bae0400-d062-11eb-992b-5e69f9b65ae9.png)
## 4) Making Predictions
![Screenshot (86)](https://user-images.githubusercontent.com/80455832/122547143-4d77c780-d062-11eb-88ca-c15b5c43470b.png)
![Screenshot (87)](https://user-images.githubusercontent.com/80455832/122547150-4f418b00-d062-11eb-8579-db1874251ee4.png)

# Demo time for Streamlit web app!
step 1: select one of the landmarks in London

![122635299-99377900-d115-11eb-8ac3-cd2648090c09](https://user-images.githubusercontent.com/80455832/124442440-54ffd600-ddaf-11eb-90e0-b17fa73eee83.gif)

![122635531-10214180-d117-11eb-93e7-aed106b5ab0f](https://user-images.githubusercontent.com/80455832/124442453-57fac680-ddaf-11eb-9e16-d7400c6ae24e.gif)

![122635534-144d5f00-d117-11eb-9d0c-f7e25b68c5e7](https://user-images.githubusercontent.com/80455832/124442474-5af5b700-ddaf-11eb-8f67-867541d359f6.gif)





