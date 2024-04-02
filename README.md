This repo contains analysis of NBA statistics, particularly in relation to spread, the difference between the home team score and away team score.

The original data was obtained from Kaggle.

Team Summaries
csv file with end of season statistics from 1947 to present
https://www.kaggle.com/datasets/sumitrodatta/nba-aba-baa-stats
Sumitro Datta

Game Results (scores)
csv file for each year (1953-2021)
https://www.kaggle.com/datasets/amanuelwk/nba-regular-season-data
Amanuel Wolde-Kidan

These were combined into a single CSV file using using code not currently included here.  Team summaries represent end of season statistics for each of the 30 NBA teams.  Team scores are for that season, so the summaries represent later data that are being used to predict those scores.  In other words, the scores (spread) being predicted are contributing to the data being used to predict them.  To minimize this effect, only the latest matchup between two teams in a season is included in the data.  It would be great to have team summaries as they were right before each game, but I was unable to find that data.  If you are reading this, and you have ideas on where to look for better data, please message me.

Files:
* since_2005_data_with_scores.csv is the raw merged data described above
* STD_against_spread.csv is data manually pulled from (https://www.boydsbets.com/ats-margin-standard-deviations-by-point-spread/, accessed 04022024) to estimate avearge error of oddsmakers.  This is used to evaluate the performance of predictive models.
