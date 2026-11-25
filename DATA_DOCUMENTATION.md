# source
The dataset was compiled from historical UFC event records sourced from public MMA databases on Kaggle (UFC Datasets 1994–2026) the raw fight.csv and event.csv tables were merged into data.csv and filtered to isolate modern ppv events from 2023+ to focus on recent data

# size
there are 705 rows and 10 columns / features

# features
fight_id - unique string identifier for each individual fight
event_name - title + card number
date - the  date when the event took place in YYYY-MM-DD
weight_class - the weight division for the match
title_fight - binary indicator (1 if its a title fight, 0 if not)
referee - name of the referee who reffed the fight
winner_id - unique identifier corresponding to the winning fighter
result_status - the outcome status of the match
method - the  method by which the fight ended
round - the round in which the fight ended

# issues
missing values - in winner_id i dont think all cases are accounted for, eg draw, no contest (no winner or loser), overturned decision, etc
lack of direct foul metrics - no column that tracks unpunished fouls (eg eye pokes or back of the head shots) therefore, analysis of reffing errors relies on related indicators such as fights ending in disqualifications (dq), no contest (nc), etc
time limitation - filtering the dataset to events from 2023+ restricts the sample size to 705 bouts, which focuses on recent years (where there have been the most controversies and mistakes) but limits historical comparisons
