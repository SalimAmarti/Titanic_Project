Titanic project - Kaggle
=======

<img src="https://img5.goodfon.com/wallpaper/nbig/e/c9/zhivopis-art-titanik-tiianic-liudi-parokhod.jpg" width="60%">

Motivations
-------

As a data lover for a few years now, I long waited for the moment when I would be able to tackle the famous Titanic project!

I took the leap, learned more about Data Science and Machine Learning and eventually worked on this project.

Sources
-------

I used Kaggle's Titanic dataset.

*https://www.kaggle.com/c/titanic/data*

Executive Summary
-------

As it is my first project, I took an extensive time exploring the data. Then I went through the features during EDA to find helpful insights for the next steps of the analysis.
I spent some time cleaning the data and tried several Machine Learning models to best predict the survivors.

The best model was **Gradient Boosting** as I reached a score of **0.78947**.

I was able to reach the **top 17%** of the Kaggle leaderboard!

<img src="Kaggle_leaderboard.png" width="30%">


Exploratory Data Analysis (EDA)
-------

| Variable | Definition | Key |
| --- | --- | --- |
| survival | Survival | 0 = No, 1 = Yes |
| pclass | Ticket class	| 1 = 1st, 2 = 2nd, 3 = 3rd |
| sex | Sex |	
| Age |	Age in years |	
| sibsp | # of siblings / spouses aboard the Titanic |
| parch | # of parents / children aboard the Titanic |	
| ticket | Ticket number |	
| fare | Passenger fare	|
| cabin | Cabin number |	
| embarked | Port of Embarkation | C = Cherbourg, Q = Queenstown, S = Southampton |

I looked at the distributions for the various numerical and categorical variables. Below are a few highlights of the interesting insights:

Data cleaning
-------

- Removed 'PassengerId' which I didn't think would be of any use
- Removed 'Name' even if I believe it would be interesting to perform some NLP here (let's put this as potential model improvement/exploration)
- Performed one-hot encoding for 'Sex' as models need to be fed with numerical features
- Created 'Family Size' and removed 'SibSp' and 'Parch'
- Removed 'Ticket' even if we could maybe do something with that feature (let's keep that in mind for future improvements)
- Performed one-hot encoding for 'Embarked'

Model Building
-------

Next steps / Improvements
-------
