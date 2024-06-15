- 120203054 Ayşe Kocavelioğlu
- 120203009 Beril Polat
- 120203068 İlayda Aslan
- 120203039 Sinem Yontar
- 120203058 Şevval Yavaş
  
# The Goal of This Project

This project's goal is to examine three separate datasets from Spotify, Taylor Swift, and TikTok that provide data about music. In order to obtain insight into music preferences, trends, and features across many platforms, the goal is to use machine learning algorithms to find patterns, similarities, and correlations between these datasets. 

Our goal is to create robust machine learning models that can accurately evaluate and predict Taylor Swift's song features, music trends on various platforms, release date, song order and preferences for her new album. We also expect to gain insightful information about the variables that influence song popularity and engagement that Taylor Swift, her producer, and music platforms can apply to their decision-making and content development processes.
From these perspectives, the project can provide insightful information about user behavior, content preferences and market dynamics in the music industry. Ultimately, this will help artists, producers, platforms, and other stakeholders make better decisions and develop more effective strategies.

At the end of our analysis, we will determine if Taylor Swift wants to make a new song, what features should be in this song.  

# Research Questions and Their Aims
1) How do the genres of music used on different platforms affect their popularity?
This analysis aims to provide insight into how musical elements influence viral trends on social media platforms. By comparing data from Spotify and TikTok, we can identify trends in music consumption and popularity across different platforms. This information can help guide advertising campaigns for Taylor Swift. Analyzing TikTok's most popular genres can reveal insights into the preferences of younger audiences, which can be useful for targeting niches in the music industry. This approach to genre classification can help improve machine learning algorithms in music analysis.

2) What makes a song popular?
The music industry is constantly evolving, with digital streaming platforms reshaping the way songs are discovered, consumed and popularized. This analysis aims to measure various musical features and their impact on listeners' perception in order to predict the success of Taylor Swift's new song. This project aims to delve into this area to reveal music popularity over the internet using data science techniques.

3) What are the criteria for numbering the tracks on Taylor Swift’s album?
The purpose of this research is to ensure that the order of the songs in Taylor's new album contributes to a consistent artistic expression. Whether based on emotional or musical dynamics, a thoughtful track numbering strategy can improve the listener's overall listening experience. A well-structured album of sequences can be more memorable and effective. It increases its popularity by leaving a mark on the listeners

4) Can the popularity of Taylor Swift’s songs be determined by the season in which they were released? 
The purpose of this research question is to ensure that Taylor can strategically determine the release date of her album to maximize its impact by utilizing analysis of seasonal trends. Releasing songs during seasons or times of year when they have historically been more popular can increase their visibility and attract audience attention. In this way, with its knowledge of seasonal preferences, it can shape its marketing and promotional activities accordingly.

## Inputs
- Spotify Songs Dataset (spotify_songs.csv)
- Taylor Swift Dataset (taylorswift-Features.csv and taylorswift-Tracks.csv)
- TikTok Dataset

## Outputs
- Identification of common patterns: Determine if there are common trends or patterns across the three datasets, such as preferred genres, popular tracks, or characteristic audio features.
- Genre classification: Develop a machine learning model to classify songs into genres based on their audio features. Evaluate the model's performance using cross-validation techniques.
- Predictive modeling: Build predictive models to forecast track popularity or engagement on platforms like Spotify and TikTok based on audio features, artist, and album information.
- Feature importance analysis: Determine which audio features contribute most to track popularity or engagement on different platforms, providing insights for artists and producers.

## Preprocessing Steps
The 'preprocessData' function in Python is designed to prepare a music track dataset for machine learning by extracting and engineering various features. It begins by copying the original DataFrame and then extracting seasonal information from the release dates, converting months to seasons, and mapping these seasons to numerical values. Additionally, it extracts the month, weekday, and year from the release dates. The function calculates the first release date for each album and determines the days since the previous album's release, incorporating this information back into the DataFrame. It counts the number of tracks per album and adds this count as a new feature. To capture interactions between key audio features, polynomial features are generated and merged with the main DataFrame. Finally, the function drops unnecessary columns, retains only numerical data, and splits the dataset into features (X) and the target variable (y), readying it for machine learning modeling.

# About The Next Steps and Gantt Chart
First of all, as we did the preprocessing of the data, we will develop a model for our case which is suitable. Then, we will validate our model and implement it. After these steps are completed, we will test the model and evaluate this model to see if the chosen model is the best or not. As a consequence, after completing final review, it will be available for us to give impressive insight based on our analysis.

    

```mermaid

gantt
    dateFormat  YYYY-MM-DD
    title IE 423 Project Timeline

    
    section Initiation
    Considering Datasets               : done,    p1, 2024-03-01, 2024-03-03
    Finding Extra Dataset              : done,    p2, 2024-03-01, 2024-03-03
    Writing Research Question          : done,    p3, 2024-03-03, 2024-03-16

    section Preprocessing of The Data
    Writing Proposal                   : done,   p4, 2024-03-16, 2024-04-30
    Importing Necessary Libraries      : done,   p5, 2024-04-20, 2024-04-22
    Data Cleaning                      : done,   p6, 2024-04-22, 2024-04-30
    Data Reduction                     : done,   p7, 2024-04-22, 2024-04-30

    section Modelling
    Model Development                  : active, p8, 2024-05-01, 2024-05-15
    Model Validation                   : active, p9, 2024-05-15, 2024-05-21
    Model Implementation               : active, p10, 2024-05-21, 2024-05-30
    
    section Model Testing
    Model Testing                      : active, p11, 2024-06-01, 2024-06-07
    Model Evaluation                   : active, p12, 2024-06-07, 2024-06-14

    section Reporting
    Final Review                       : active, p13, 2024-06-14, 2024-06-19
    Giving Impressive Insights         : active, p14, 2024-06-14, 2024-06-19


