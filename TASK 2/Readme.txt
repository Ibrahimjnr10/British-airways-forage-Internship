# British-Airways
## Objective
The wrangling of data and analysis to understand the sentiment, behavior of passengers and flight pattern to uncover actionable insights to enhance service quality and operational efficiency for British Airways. via the means of Web Scraping, Sentiment and Exploratory Analysis 

## Overview
This repository contains three comprehensive projects analyzing British Airways' customer experience and operational data through web scraping, sentiment analysis, predictive modeling, and exploratory data analysis (EDA). The projects aim to uncover actionable insights to enhance service quality and operational efficiency for British Airways.

### Projects
Web Scraping and Sentiment Analysis,
Predictive Modeling for Customer Sentiment,
Exploratory Data Analysis (EDA) of Flight and Rating Data


## Dataset Descriptions

B_Airways_ratings.csv
- index: Index column
- date_flown: Date of the flight
- staff_service: Rating of the staff service (1-5)
- food: Rating of the food service (1-5)
- ground_service: Rating of the ground service (1-5)
- seat_comfort: Rating of the seat comfort (1-5)
- pricing: Rating of value for money (1-5)
- recommended: Whether the reviewer recommended the airline (Yes/No)

B_Airways_flight_info.csv
- index: Index column
- date_flown: Date of the flight
- travellers_type: Type of travelers (e.g., Business, Leisure)
- route: Flight route
- aircraft: Aircraft type
- Seat_type: Type of seat (e.g., Economy, Business)

reviews.csv: Scraped reviews dataset.
- title: title of review
- date: date reveiw was written
- country: country of reveiwer
- review: actual review/ remark

## Workflow:
Web Scraping --> Sentiment Analysis AND prediction --> Exploratory Data Analysis

## Web Scraping
Overview
This project involves scraping customer reviews of British Airways from a third party website https://bit.ly/3VUEG0Z to understand the sentiment towards the airline. Sentiment analysis is to be applied to categorize the reviews into positive, neutral, and negative sentiments.
and for further exploration


### Key Files
WebScraping.ipynb: Script for scraping reviews from websites.

### Steps
Request all pages. -->
Locating tags. -->
Extrating tag text -->
Handling irregularities and alignment of data. -->
Structuring data into DataFrame. -->
Storing Datasets -->


## Sentiment Analysis and prediction
Overview
This project focuses determining the sentiment of reviews and on building a predictive model to forecast customer sentiment based on review content. The model helps in identifying potential issues proactively.

### Key Files
sentiment_analysis.ipynb: Script for performing sentiment analysis on the scraped reviews.
reviews.csv: Dataset of reviews with sentiment labels.

### Steps
Loading the review data. -->
Tokenizing Lemmatizing review. -->
Detecting language using langdetect. -->
Extracting sentiments using TextBlob. -->
Preprocessing data by Creating Bag of Words (BOW) -->
Imputing missing data (most frequent strategy is used) -->
Build and train the predictive model. -->
Evaluate the model's performance. -->


## Exploratory Data Analysis (EDA) of Flight and Rating Data
Overview
This project involves EDA of flight and rating data from 2019 to 2024 to identify operational patterns and customer preferences.

### Key Files
eda.ipynb: Script for performing EDA on the flight and rating data.
B_Airways_flight_info.csv: Dataset containing flight information.
B_Airways_ratings.csv: Dataset containing flight ratings.

### Steps
Load and clean the datasets -->
Analyze and visualize patterns in flight data (e.g., most flown aircraft, popular routes). -->
Analyze and visualize customer ratings and service performance. -->
Identify areas for improvement and make recommendations. -->

### Challenges addressed:
I encountered several challenges during our analysis, including data imbalance and missing values. Addressing these required significant data cleaning efforts and balancing the sentiment data to ensure accurate predictions. Few dynamic approaches and functions were utilized to attain this. These approaches can be found on the GitHub repository notebook for further exploration


### Recommendations
General
1. Automated Data Cleaning: Implement automated scripts to clean and normalize the data, ensuring consistency and accuracy.
2. Incremental Scraping: Develop a system to incrementally scrape new reviews, keeping the dataset up-to-date without redundant data collection.
3. Enhance food and ground services to improve customer satisfaction.
4. Invest in more comfortable seating options for long-haul flights.
5. Explore new routes and increase frequencies to regions with growth potential.
6. Continue training programs for staff to maintain high service standards.
More recommendation upon exploration of project notebooks, presentaion and article
 


## Link to the slides
https://docs.google.com/presentation/d/1Za0fjvwVDgwUDtpbk0lDIM5AiD2BVfoKlikpKDLK8Pk/edit?usp=sharing

## Link to the documentation
https://medium.com/@abdulsalamibrahima017/unlocking-insights-a-deep-dive-into-british-airways-passenger-experience-f62e6cfff597

## Folders present in the project:
- Web scrape
- Sentiment Analysis
- EDA
  
Conclusion
By leveraging insights from these projects, British Airways can proactively address customer concerns, enhance service offerings, and explore new growth opportunities. This repository provides the necessary scripts and datasets for replicating the analysis and driving data-driven decisions in the aviation industry.

How to Run
Clone this repository.
Install the required dependencies.
Run the scripts for each project as described in their respective sections.
bash
Copy code
git clone <repository_url>
cd <repository_name>
pip install -r requirements.txt
python <script_name.py>

License
This repository is licensed under the MIT License. See the LICENSE file for more details.

Contact
For any questions or suggestions, please contact Ibrahim Abdulsalam at Abdulsalamibrahima017@gmail.com or chat up +2349131606400
