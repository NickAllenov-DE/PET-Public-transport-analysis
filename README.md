# PET-Project:   
# Analysis of public transport accessibility 

## Project team:  
- Nikolai Allenov - Data Engineer (Data collection, Creating an ETL process and DWH)
- Dmitry Verkhovtsev - 


## The purpose of the project  
Evaluate the accessibility of public transport in Moscow, especially for people with disabilities, identify problems in the infrastructure and offer recommendations for improvement.  

## Methods  
• Data collection: Parsing data on transport routes, stops, travel time, from user reviews and from the API of city services.  
• Data analysis: Using classification and clustering techniques to analyze reviews and routes (NLP to analyze reviews).  
• Modeling: Building models to identify dependencies between transport accessibility and other factors (for example, distance from the center, waiting time).  
• Visualization: Create a dashboard to display the results of the analysis.  
• Model training: Using ML to classify routes by accessibility.  

## Practical application possibilities   
• Urban Services: Using recommendations to improve routes, stops and other aspects of transport infrastructure to make it more accessible.  
• Users: Improving the usability of transport for people with disabilities, through improved navigation and routes.  
• Transportation companies: Optimize routes and schedules to increase passenger satisfaction.  

## Value  
• Social significance: The project will help to increase the accessibility of transport for all categories of citizens, including people with disabilities.  
• Cost-effectiveness: Route optimization and infrastructure improvements can reduce transportation costs.  
• Technical contribution: The use of modern methods of parsing, data analysis and machine learning to solve applied problems.  

## Stages of the project:  
               
## 1. Data collection   
   • Parsing of data on routes, schedules and public transport stops (API of the city, OSM).  
   • Parsing passenger feedback on transport accessibility (social networks, feedback platforms).  
   • Collecting geodata on the location of stops and infrastructure facilities for people with disabilities.  

Tools:  
    • Moscow API (Transport API, OpenStreetMap API)  
    • Parsing: Python (BeautifulSoup, Scrapy)  
    • Database: PostgreSQL for storing data on routes, stops and reviews.   

## 2. Generation of text and features  
   • Generation of features based on reviews using NLP (tonality analysis, highlighting problematic topics).  
   • Generation of photos of stops and routes using computer vision (according to the queries "accessibility for people with disabilities").  
   • Tokenization and text processing of reviews to create categories of problems and suggestions.  

Tools:  
    • NLP: Python (spaCy, NLTK, Transformers)  
    • CV: OpenCV for analyzing photo stops (classification by accessibility)  
• Features: Pandas, NumPy for creating data tables.    

## 3. Uploading data to Yandex.Toloka  
   • Preparation of instructions for assessors to evaluate photos of stops for accessibility.  
   • Creation of a golden dataset and a honeypot to verify the accuracy of the assessors' work.  
   • Uploading data to Yandex Toloka to mark up images and check texts for compliance with a given topic.  

Tools:  
    • API Toloka  
    • Data preparation: Pandas, JSON  
    • Golden Dataset and Honeypot: manual configuration on the Toloka platform    

## 4. AB testing  
   • Conducting AB-testing, in which the instructions for assessors will be changed for different groups.  
   • Analysis of the result of AB tests based on the quality of the markup (in terms of accuracy and speed of execution).  

Tools:  
   • AB-tests: Python (SciPy, Statsmodels)  
   • Metrics: Precision, Recall, F1-Score  

## 5. Prediction by marking assessors  
  • Using NLP to analyze text reviews, predicting tonality and subject matter.  
  • Classification of images based on the marking of assessors (accessibility of stops, transport hubs).  
  • Clustering of stops by problem areas and places with high availability.  

Tools:  
    • NLP: Transformers (BERT, RoBERTa)  
    • ML models: Scikit-learn, TensorFlow (CNN for image analysis)  
    • Clustering: KMeans, DBSCAN  
               
## 6. Building a dashboard  
   • Data visualization: transport accessibility by area, problem points (heatmaps), routes, recommendations.  
   • Display of the analysis results on an interactive map.  

Tools:  
    • Visualization: Apache Superset, Power BI, Plotly Dash  
    • Map: Folium, Mapbox  

## 7. Creating an ETL process and DWH  
   • Creation of an ETL process for automatic updating of data from transport APIs and social networks.  
   • Building DWH to store historical data and prepare data marts for analysis.  

Tools:  
    • ETL: Apache Airflow for process automation  
    • DWH: ClickHouse for storing large amounts of data  
    • Data marts: SQLAlchemy, dbt for data transformation  


   ## Technology stack:  
   • Languages: Python, SQL  
   • Data parsing: BeautifulSoup, Scrapy, API  
   • Databases: PostgreSQL, ClickHouse  
   • NLP: SpaCy, NLTK, Transformers (BERT, RoBERTa)  
   • ML: Scikit-learn, TensorFlow, Keras  
   • AB-testing: Statsmodels, SciPy  
   • Markup tools: Yandex Toloka  
   • Orchestration: Apache Airflow  
   • Dashboards and visualization: Power BI, Apache Superset, Plotly, Folium  
   • DevOps: Docker for containerization, GitHub Actions for CI/CD. Perhaps Kubernetes?  


# Contacts:  
## Nikolai Allenov  
- Email: AllenovNS@gmail.com  
- Telegram: https://t.me/NickAllenov  
- Linkedin: https://linkedin.com/in/nickallenov-de

## Dmitry Verkhovtsev  
- Email: dimitry.verkhovtsev@gmail.com  
- Telegram: https://t.me/Gantt_bar  
- Linkedin:   
