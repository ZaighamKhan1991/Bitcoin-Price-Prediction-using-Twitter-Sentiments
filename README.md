# Project : The Effect of News and Tweets on the Price of Bitcoin

### [Project Description](doc/project2_desc.md)

![screenshot](doc/figs/Restuarants.PNG)

Cryptocurrency is the talk of the town in today’s world. It is essentially a form of digital
currency, which any government or financial institution does not govern. It has gained rapid
popularity in recent years, which has further led to many applications accepting cryptocurrency.
Bitcoin was the first cryptocurrency to be launched in 2009, after which many more have been
launched in the market. However, bitcoin remains the most popular cryptocurrency in use.
Bitcoins transactions primarily occur using peer-to-peer technology, replacing the need for a
third party, such as a central bank. Bitcoins are a highly volatile currency due to being controlled
directly by people rather than any government intermediary. Previous studies by Kristoufek and
American Institute for Economic Research (AIER) show the fluctuations in cryptocurrency
coinciding with dramatic events over the world and the price of such currencies being driven by
news sentiment (Kristoufek, 2015). We will take a deeper look at how these price fluctuations
are correlated with news and Twitter sentiments.
The **objective** of this project are to find out:

- Do the sentiments of tweets and news influence the price of Bitcoin?
- Does the value of the S&P 500 Index influence the price of Bitcoin?
- Which predictive model is the most optimal for predicting the price of the Bitcoin?
- 
## Project Title: The Effect of News and Tweets on the Price of Bitcoin

+ Team members
	+ Ning Ding,, , Biyu Wang, and Anna Yass
	+ Khan, Zaigham
	+ Miao, Chelsea
	+ Wang, Biyu
	+ Yass, Anna

+ **Data Collection**: This project uses four data files: Twitter tweets, news articles from New York Times,
S&P 500 Index intraday prices, and bitcoin prices between January 1, 2022, to February 22,
2022. It was decided to use hourly intervals from all datasets to capture the most detailed
fluctuations for all four datasets. To merge the four files together, a master sheet of blank time
series was created between January 1, 2022 to February 22, 2022 in hourly intervals 

+ **Project summary**: This study used four analytical techniques: Linear Regression, Random Forest, Time
Series and Neural Network. We started with Linear Regression to examine the relationship
between the price of bitcoin and sentiments of tweets and news. This regression model shows the
correlation between Twitter and news sentiments and the price of bitcoin. The p-value in the
Linear Regression examines the statistical significance of this correlation.
However, Linear Regression models can only examine linear relations between
dependent and independent variables. Therefore, other models that take nonlinearity into
consideration were also used. In general, Trees based and Random Forest are the best models to
use for such cases. We used Random Forest to show the most important predictor of the price of
bitcoin. However, Random Forests do not take historical data into consideration. Since the best
predictor of the price of bitcoin today is the price of bitcoin yesterday, we had to use Time Series
models. Time Series models allow us to consider the historical information, such as the prices
from a previous date and time. To generate a better RMSE, historical information from both the
price of the S&P 500 Index and the price of bitcoin were used. To do this, we used a Multivariate
Time Series model in our analysis. Finally, we used Neural Network as the last model to
benchmark our results. Neural Network uses a mesh of learning layers for prediction and
evaluation. In this study, we used the ‘nnet’ and ‘neuralnet’ package to create a basic Neural
Network to predict the price of bitcoin.

+ **Contribution statement**: ([default](doc/a_note_on_contributions.md)) All team members contributed equally in all stages of this project. All team members approve our work presented in this GitHub repository including this contributions statement.

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── app/
├── lib/
├── data/
├── doc/
└── output/
```

Please see each subfolder for a README file.

