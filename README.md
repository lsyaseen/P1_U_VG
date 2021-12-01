## Analysis on the Video Game data set for the Udacity Data Science project

The dataset was downloaded from Kaggle: https://www.kaggle.com/ashaheedq/video-games-sales-2019

## Project tools, libraries and techniques

#### Programming Languages
The project was developed using *Python* using the Jupyter Notebook IDE.

#### Python Libraries Used
* *Pandas* Pandas is the main library used for this project, with the help of this library I managed to read in the CSV file, create a dataframe, and perform various cleaning and wrangling practices provided by pandas such as dropping and merging data.
* *Matplotlib* the main usage for matplotlib was to create the charts to deliver a visual aspect of the findings.

#### Project Objective and Data Wrangling Techniques
* Business understanding
  The objective of this project was to understand how the *Video Game* industry grew in the past decade with regards to the genres developed and the industry's targeted audience and customers, we present the following questions in the analysis approach.
  - What kind of video games developers usually develop that are suitable for children?
  - What are some of the emerging video games genres?
  - Do diffirent companies produce games for diffirent target audeicnes?


* Data Understanding
  The data acquired in this project was from Kaggle. It is a dataset of more than 50k records of video game sales scraped from vgchartz.com, which means that the data might lack structure and include missing elements that require proper cleaning before performing the analysis.
  
* Prepare the Data
  - The data did have several columns that included over 80% of missing data, these columns were insignifact to the objective which made it easy for me to choose to drop them to create a lighter version of the Data Frame.
  - The data did have several columns that included over 80% of missing data; these columns were insignificant to the objective, making it easy for me to drop them to create a lighter version of the Data Frame.
  - I also performed some simple type conversion and renamed some columns for consistency. I eventually created a cleaner copy of the data set to work with named `df_main`.
  - One more column was created for the new clean data frame named `Audience.` It stored some binary data of the type of audience based on other categorial columns.

* Question 1 - What kind of video games developers usually develop that are suitable for children?
  - Analyse: I used the genre and the rating columns to determine if there is correlation between both data sets.
  - Visualize: I created two Pie Charts and a Stacked Bar Chart to support the analysis.
  - Explanation: The two Pie Charts included the high-level segregation showing the games suitable for children or not, and the other is categorized into the different ratings provided by the `ESRB_RATING` column and the Stacked Bat Chart showed a breakdown of genres for each ESRB Rating.

* Question 2 - What are some of the emerging video games genres?
  - Analyse: The video games genres vary into 20 different categories in this data set, but how was the evolution of these genres based on the number of companies produced over the past decade?
  - Visualize: I created a line-graph that shows a time-series analysis of the genres.
  - Explanation: The chart shows that games such as `Action` , `Shooting` and `Fighting` were emerging in the past decade.

* Question 3 - Do diffirent companies produce games for diffirent target audiencnes?
  - Analyse: Is there a way to identify companies that might be targeting a certain group age? a question that we can answer by looking at the number of games produced by each companies and looking at the ESRB rating to create a profile of some of these companies.
  - Visualize: I created a Bar Chart that shows the % of games that are deemed for children based on the `Audience` column for every company and filtered them by the top companies that produce higher than 90% of games for kids.
  - Explanation: The Data shows the top companies that produce games for children compared to other ratings, this helps us identify companies that will "Most Likely" create games appropriate for kids.
 
 * Evaluation
 I managed to utilize the 50k+ records of video game production data to determine a profile of companies that will most likely produce video games appropriate for children. This was achieved by answering the core three questions proposed to derive the relevant information.


##### Here are some information about the fields in the data

- Rank - Ranking of overall sales
- Name - Name of the game
- Platform - Platform of the game (i.e. PC, PS4, XOne, etc.)
- Genre - Genre of the game
- ESRB Rating - ESRB Rating of the game
- Publisher - Publisher of the game
- Developer - Developer of the game
- Critic Score - Critic score of the game from 10
- User Score - Users score the game from 10
- Total Shipped - Total shipped copies of the game
- Global_Sales - Total worldwide sales (in millions)
- NA_Sales - Sales in North America (in millions)
- PAL_Sales - Sales in Europe (in millions)
- JP_Sales - Sales in Japan (in millions)
- Other_Sales - Sales in the rest of the world (in millions)
- Year - Year of release of the game

## Here is the blog post created for the project
### Video games, NOT Made For Children
https://medium.com/@lsyaseens/video-games-not-made-for-children-68b7570bb13

#### Here is a link to the GitHub Repo
https://github.com/lsyaseen/P1_U_VG.git
