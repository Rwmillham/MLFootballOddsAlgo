# Using Data Science and Machine Learning to Predict NFL Spreads

### Most Recent Update
After a long first semester of my senior year, I am getting back to work on this project. Currently, I have retrieved game statistics and information from thousands of games across eight seasons. Furthermore, I have analyzed the statistics and identified several key metrics that correlate with performance against the spread. For example, teams that convert a higher percentage of their third-down attempts tend to perform much better against the spread than Vegas predicts.

For my final semester of college, I have enrolled in two machine learning courses: _Introduction to Machine Learning_ and _Bayesian Methods for Machine Learning_ (course descriptions below). I plan to bridge the gap between my academic coursework and this project by applying these concepts directly to my analysis. Finally, I have one or two remaining validation checks to complete to ensure the accuracy of the collected statistics.

Next Steps: 

1. Validate and test the data collection process to ensure accurate statistics.
2. Fix a bug in the database architecture that retrieves incorrect data when parsed by programs.
3. Become more familiar with machine learning algorithms through coursework and implement the lessons learned when developing the predictive machine learning model.

### Synopsis
In this project, I will attempt to use a calibration-incentivized machine learning algorithm to beat Vegas betting lines, specifically the spread. To do this, I will feed in historical data currently dating back to 2017 (though I may pull older statistics). These statistics are pulled from Pro Football Reference (PFR) and stored in the directory "Stats."

Included in these statistics are the Vegas betting lines, a game’s weather and temperature, playing surface, as well as the actual game statistics. For example, I store each team’s offensive passing yards, rushing yards, first downs, third-down conversion rate, and all types of turnovers, etc. Furthermore, I also store the offensive stats of a given team’s opponent as an indictment of the team of interest’s defense.

I will evaluate the effectiveness of this algorithm by simulating betting conditions for the 2024 season. Ideally, we hope to reach a success rate of 52.4%, which accounts for Vegas’ standard 10% vigorish. If we find success, and if the timing works, I will then implement this algorithm on the 2025 NFL season with a real-world bankroll.

This README will change throughout the project but will serve as a record of my changing goals and ideas as I go through the process.

#
### Relevant Programs and Files

ScrapeStats.ipynb - Python script to scrape statistics off of PFR and store them in the corrosponding directory.

UniversalFunctions.ipynb - Function that are consistantly used to pull from a database, and parse relavant data.

Stats/  - Directory containing the stats of every game played by every team for all seasons between 2018 and 2023.

FootballTester.ipynb - Program to work on whatever project I am currently attacking, before formal file is created once finished
#
### Current Research

Beyond general background reading, two research papers, in particular, have been especially useful:

> Brandon, Daniel. (2024). Predicting NFL Point Spreads via Machine Learning. International Journal of Data Analytics. 5. 1-18. 10.4018/IJDA.342851.

> Conor Walsh, Alok Joshi. Machine Learning for Sports Betting: Should Model Selection Be Based on Accuracy or Calibration? Machine Learning with Applications, Volume 16, 2024, 100539, ISSN 2666-8270.

### Releavent Course Listings with Description:

EECS 445. Introduction to Machine Learning: 

>Theory and implementation of state-of-the-art machine learning algorithms for large-scale real-world applications. Topics include supervised learning (regression, classification, kernel methods, neural networks, and regularization) and unsupervised learning (clustering, density estimation, and dimensionality reduction). For each topic, mathematical principles, key algorithmic ideas, and implementation will be highlighted


EECS 498-009. Bayesian Methods for Machine Learning

>This course will cover modern machine learning techniques from a Bayesian probabilistic perspective. Bayesian probability allows us to quantify, model and reason about all types of uncertainty. The result is a powerful, internally-consistent framework for approaching many problems that arise in machine learning, including parameter estimation, model comparison, and decision making.