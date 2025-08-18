# Using Machine Learning to Predict NFL Spreads
### Synopsis

In this project, I will attempt to use a calibration-incentivized machine learning algorithm to beat Vegas betting lines, specifically the spread. To do this, I will feed in historical data currently dating back to 2018 (though I may pull older statistics). These statistics are pulled from Pro Football Reference (PFR) and stored in the directory "Stats."

Included in these statistics are the Vegas betting lines, a game’s weather and temperature, playing surface, as well as the actual game statistics. For example, I store each team’s offensive passing yards, rushing yards, first downs, third-down conversion rate, and all types of turnovers, etc. Furthermore, I also store the offensive stats of a given team’s opponent as an indictment of the team of interest’s defense.

I will evaluate the effectiveness of this algorithm by simulating betting conditions for the 2024 season. Ideally, we hope to reach a success rate of 52.4%, which accounts for Vegas’ standard 10% vigorish. If we find success, and if the timing works, I will then implement this algorithm on the 2025 NFL season with a real-world bankroll.

This README will change throughout the project but will serve as a record of my changing goals and ideas as I go through the process.

#
### Relevant Programs and Files

ScrapeStats.ipynb - Python script to scrape statistics off of PFR and store them in the corrosponding directory.

Stats/  - Directory containing the stats of every game played by every team for all seasons between 2018 and 2023.

#
### Current Research

Beyond general background reading, two research papers, in particular, have been especially useful:

> Brandon, Daniel. (2024). Predicting NFL Point Spreads via Machine Learning. International Journal of Data Analytics. 5. 1-18. 10.4018/IJDA.342851.

> Conor Walsh, Alok Joshi. Machine Learning for Sports Betting: Should Model Selection Be Based on Accuracy or Calibration? Machine Learning with Applications, Volume 16, 2024, 100539, ISSN 2666-8270.
