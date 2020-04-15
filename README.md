# COVID-19 Challenge Topics Modeling on Reddit texts

## Objective: 

This project performs LDA topics modeling based on reddit submissions and comments to see what COVID-19 related topics are the most popular and what we could do to bring real social impact under the prevalence of coronvirus. 


## Dataset: 
1. Data Collection Method: Pushshift API for Reddit
2. Data Format: csv
3. Data Type: mainly texts 
4. Timeframe: March 1st, 2020 - April 11th, 2020
5. Data: 
  - [redsub.csv](https://drive.google.com/drive/folders/1xnHpzweXw1APN3v_kOZHX9CyAS1tt5zs?usp=sharing): 566951 submissions from Reddit 
  - [redcom.csv](https://drive.google.com/drive/folders/1xnHpzweXw1APN3v_kOZHX9CyAS1tt5zs?usp=sharing): 1069748 comments from Reddit
  - subred_covid_submis.csv: 18965 submissions from Reddit r/Coronvirus subreddit
6. Features:
  - redsub.csv / subred_covid_submis.csv: PostID, Title, Url, Author, Postdate, Score, TotalComments, Permalink (subreddit), and Flair
  - redcom.csv: CommentID, Author, Comment, Score, PublishDate, Subreddit, Permalink

## Machine learning techniques: 
1. It is assumed that the semantics of our document are actually being governed by some hidden, or “latent,” variables that we are not observing. Several Machine Learning methods are compared in the following table. Considering interpretability and accuracy, the Latent Dirichlet Allocation (LDA) Topics Model is used to clutser texts into distinct categories.
2. The code is included in Reddit_TopicsModel.ipynb

![alt text](https://github.com/Freiheit77/COVID-19-Topics-Model/blob/master/ML%20comparison%20for%20topics%20modeling.png)

## Results: 
1. submission_vis: topics modelling interactive visualization based on data from redsub.csv
[submission topics visualization](https://freiheit77.github.io/COVID-19-Topics-Model/submission_vis.html)
2. covid_sub_vis.html: topics modelling interactive visualization based on data from subred_covid_submis.csv
[r/Coronvirus topics visualization](https://freiheit77.github.io/COVID-19-Topics-Model/covid_sub_vis.html)
3. comment_vis.html: topics modelling interactive visualization based on data from redcom.csv
[comment topics visualization](https://freiheit77.github.io/COVID-19-Topics-Modelling/comment_vis.html)
4. Topics summarized: 
![alt text](https://github.com/Freiheit77/COVID-19-Topics-Model/blob/master/Screenshot%202020-04-15%20at%2012.53.52%20AM.png)

## Recommendation 
Based on the analysis of COVID-19 related discussions in Reddit community, the following suggestions are proposed to Reddit executives to take social responsibility, make contributions to COVID-19, and improve brand image.

From the within-community perspective: 
    1) Reddit should increase the number and exposure of prevention discussions through intervention of moderators (similar to community manager who are responsible for maintenance).
    2) Reddit could create “prevention” and “mutual help” post type (flair) and encourage discussions within these types. 

From the community-wide perspective:
    1) Encourage more moderators from various communities to post and pin covid-related prevention topics in their communities.
    2) For new users, Reddit could automatically subscribe them to COVID-19 related communities.     
    3) Reddit could put more prevention-related topics on trending today or Popular posts to increase COVID-19 news exposure.

