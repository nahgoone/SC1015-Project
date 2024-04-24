# SC1015-Project
![alt text](https://github.com/nahgoone/SC1015-Project/blob/main/Steam.png "Steam")
### FCSE Group 6 Members
- [Ngo Zong Han](https://github.com/nahgoone)
- [Rochelle Tan Tyen Xyn](https://github.com/Rosheru)

## Our Motivation
- The gaming industry has always been saturated with games and between 2010 and 2020, annual game industry revenue grew from $78 billion to $137 billion — more than either Hollywood or the American music industry.
- Steam was 1 such platform that was able to benefit from this trend, having a huge increase in influx of users from 8.4 million in 2015 to 33 million in 2023
- More people and developers are trying to capitalize on this trend, however, the average time to create a game, not to mention a successful one is difficult.
- One might need to take a few months, years, or even a decade to create a playable game. Creating a successful one is even more difficult. As a computer science student who’s also interested in developing games, this problem would be interesting to solve

## Project Goal
- Our project aims to maximize profits when producing Steam Games by predicting the 'success' probability before developing the game.

## Datasets Used
- All of the [Data](https://drive.google.com/drive/folders/1pe-xQLG2WaZTIf8NbjC5G2nqP5fd9vBy) we have collected and used are in a Google Drive.

## Juypter NoteBooks:
1. [Data Collection](https://github.com/nahgoone/SC1015-Project/blob/main/Steam%20Data%20Collection.ipynb)
2. [Steam Spy Cleaning](https://github.com/nahgoone/SC1015-Project/blob/main/Steam%20Spy%20Cleaning.ipynb)
3. [Steam App Cleaning](https://github.com/nahgoone/SC1015-Project/blob/main/Steam%20App%20Cleaning.ipynb)
4. [Steam EDA](https://github.com/nahgoone/SC1015-Project/blob/main/Steam%20EDA.ipynb)
5. [Classification](https://github.com/nahgoone/SC1015-Project/blob/main/Classification.ipynb)
6. [Binary Classification](https://github.com/nahgoone/SC1015-Project/blob/main/Binary%20Classification.ipynb)
7. [Hierarchal Clustering](https://github.com/nahgoone/SC1015-Project/blob/main/Hierarchal%20Clustering.ipynb)
8. [Linear Regression](https://github.com/nahgoone/SC1015-Project/blob/main/Linear%20Regression.ipynb)

## Slide Deck: 
1. [Slides](https://github.com/nahgoone/SC1015-Project/blob/main/SC1015%20PPT%20Slides.pdf)


## Summary of our project:
**1. Data Collection**
- Used JSON with 2 Web APIs (SteamSpy and Steam Web) to extract and store all data into [excel sheets](https://drive.google.com/drive/folders/1pe-xQLG2WaZTIf8NbjC5G2nqP5fd9vBy)

**2. Data Cleaning**
1. Identify NULL Values and Missing Data
2. Removing duplicated and irrelevant columns
3. Preprocessing of data
4. Combining and exporting datasets

**3. EDA**

**Description of the Steam Dataset:**
> `appid`: Unique ID for each game <br>
> `name`: Name of each game <br>
> `release_date`: Total games released, releases by year, highest daily releases <br>
> `english`: Indicates (0 or 1) whether the game supports English <br>
> `developer`: Developers that released the game <br>
> `publisher`: Publishers that released game <br>
> `platforms`: Operating systems the game can be played on <br>
> `categories`: Categories of the games set by Steam <br>
> `genres`: Most popular genres <br>
> `steamspy_tags`: The top 3 most tags Steam users associate the game with <br>
> `positive_ratings`: Number of positive reviews by Steam users <br>
> `negative_ratings`: Number of negative reviews by Steam users <br>
> `average_playtime`: Average playtime since March 2009 in minutes. <br>
> `median_playtime`: Median playtime since March 2009 in minutes. <br>
> `owners`: Total number of owners per game, distribution range of game owners <br>
> `price`: Price of the game in SGD <be>

2. Platforms
- As expected games mostly support running on Windows Operating system followed Mac OS and Linux OS

3. Categories
- Top 5 most popular categories set by Steam are `Single-player`, `Family Sharing`, `Steam Achievements`, `Steam Cloud` and `Full controller support`

4. Owners
- The majority of games sold less than 20,000 copies
- A small but noteworthy portion of games have sold over 2 million copies
- Some games have immense popularity exceeding 100 million copies sold
- The top 8 Games with the most copies sold are, Dota, Counter-Strike 2, Palworld,

5. Genres
- Top 5 most popular genres among all games are, Indie, Action, Casual, Adventure, Simulation
- Massively Multiplayer seems to be the most own genre followed by RPG, Action and Strategy
- Surprisingly although Indie is tagged in most games, it has a low average number of users

6. Release Dates
- Increasing trend in number of games released since 2014
- Majority if not all games released in 2014 and earlier have less than 20,000 copies sold
- Comparing each year after 2014, there are more games with over 20,000 copies sold each year than games with less than 20,00 copies sold

7. Categories
- Top 5 Developers with most games: Choice of Games, Creobit, Laush Dimitriy Sergeevich, KOEI TECMO GAMES CO., LTD, Hosted Games
- Top 5 Publishers with most games: Big Fish Games, 8floor, Conglomerate 5, Choice of Games, HH-Games

8. Numeric
- Top 5 Games with highest `positive_ratings`: Counter-Strike 2, Dota 2, PUBG: BATTLEGROUNDS, Terraria, Rainbow Six® Siege
- Top 5 Games with the highest `negative_ratings`: Counter-Strike 2, PUBG: BATTLEGROUNDS, Dota 2, War Thunder Rainbow Six® Siege


**4. Machine Learning**
**4.1 Regression:**
- Measured variables against average playtime
- Gradient Boosting Regressor is important as it was used to improve the accuracy of the linear regression model. It can handle missing values and outliers in the data which lowers Variance and MSE. This leads to more stable and reliable predictions.
- In summary, model 3 was the best.

**4.2 Classification**
- Learning how to do One Hot Encoding and Binary for Classification
- Learning how to use different metrics to determine the best model to predict the success of a game
  1. Out Of Box Score
  2. F1 Score (Precision + Recall)
  3. ROC and AUC

**5. Learning Outcomes**
**Data Collection:**
- Gathering Data using JSON and Web APIs

**Data Cleaning:**
- Handling multiple Data formats in Excel
- Processing different data using python

**Data Visualisation & Analysis:**
- Applying course knowledge
- Learning new visualisation techniques

**Machine Learning:**
1. Models:
   - Clustering, Linear Regression, Gradient Boosting Regressor
2. One Hot Encoding Classification:
   - F1 Score, Accuracy
   - random forest classifier
3. Binary Classification
   - using random forest classifier
   - learned to binarise categorical features
   - using ROC cure (AUC-ROC) to access the performance of the model

**6. Conclusion**
- Rather than trying to target a genre segment, developers should focus on ensuring their game is accessible, e.g. cheap/affordable, cross-platform, and popular via marketing and high perceived quality.
- Future works: Analyze various player demographics and preferences and make games catered to their targetted audience. 

## Key Takeaways: 
**Owners and Average Playtime:** 
- Games with a larger number of owners tend to have higher average playtimes. 

**Overall Reviews and Average Playtime**: 
- Games with more overall reviews, which can be indicative of popularity or player engagement, tend to have higher average playtimes. 
- Positive reviews might encourage more players to try the game, leading to longer play sessions or more frequent play. Conversely, negative reviews might deter players, resulting in shorter playtimes. 

**Price and Average Playtime**: 
- The relationship between price and average playtime can vary. 
- Generally, lower-priced games may attract more players due to affordability, potentially resulting in longer playtimes.  
- On the other hand, higher-priced games may have dedicated fan bases or offer premium content, leading to longer play sessions despite the higher cost. 
- Players may perceive higher-priced games as having higher value, motivating them to spend more time playing to justify the investment.

**Diverse Player Preferences**: 
- Video game genres cater to a wide range of player preferences and gaming experiences. 
- Some players may prefer short, intense sessions offered by action-packed games, while others may enjoy the immersive storytelling of role-playing games (RPGs) that lead to longer playtimes. 
- The diversity in player preferences leads to varying average playtimes across different genres, resulting in a weaker correlation between genre and playtime.

# Contributions:
1. **Data Collection:** Zong Han
2. **Data Cleaning and Preprocessing:** Rochelle
3. **EDA and Visualisation:** Zong Han & Rochelle
4. **Binary Classification, Hierarchical Clustering, Linear Regression:** Rochelle
5. **OHE Classification:** Zong Han
6. **Slides:** Zong Han & Rochelle
7. **GitHub:** Zong Han

# References:
**APIs:**
- https://partner.steamgames.com/doc/webapi_overview
- https://steamspy.com/api.php
- https://steamspy.com/

**Motivation:** 
- https://www.channelnewsasia.com/singapore/skull-and-bones-video-game-pirates-ubisoft-singapore-ps5-xbox-pc-4126386
- https://www.washingtonpost.com/video-games/esports/2020/01/28/2010s-were-banner-decade-big-money-tech-esports-reaped-rewards/
- https://www.statista.com/statistics/1330211/steam-peak-concurrent-players/

**People:** 
- https://nik-davis.github.io/posts/2019/steam-data-collection/
- https://aldenyuan.medium.com/exploratory-data-analysis-on-steam-store-games-dataset-f4ff06da44eb
- https://medium.com/all-things-ai/in-depth-parameter-tuning-for-random-forest-d67bb7e920d

