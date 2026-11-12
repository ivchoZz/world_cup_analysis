# FIFA World Cup matches analysis

An exploratory analysis of 900 FIFA World Cup matches (1930-2018), made to practice cleaning, transforming and visualizing data with pandas, NumPy and matplotlib.

**Data:** `world_cup_matches1.csv` (source: https://www.kaggle.com/datasets/abhijitdahatonde/fifa-world-cup-all-dataset/discussion?sort=recent-comments)

## Questions and findings

1. **Do matches have more or fewer goals over the years?**
   Average goals per match were high in the early tournaments (about 3.9 to 5.4 from 1930 to 1954) and fell to roughly 2.2 to 3.0 from 1962 onwards.

2. **Do host teams have an advantage?**
   When the Home Team is the tournament host it wins 63.6% of matches (75 of 118), versus 54.7% (428 of 782) otherwise. The host sample is small and hosts are often strong teams, so the data does not support a firm conclusion.

3. **Which teams are the most successful?**
   By win rate (teams with at least 20 matches), Brazil is first with 67.0% of 109 matches, followed by Germany (61.5%). Win rate and total wins give different top 10 lists: Croatia, Poland and Hungary rank high by rate but have far fewer matches.

## Limitations

- Teams that no longer exist (for example Yugoslavia and Czechoslovakia) are counted separately from their successors.
- Penalty shootouts are not recorded, so knockout matches that ended level count as draws.
- The 20-match threshold in question 3 is my own choice.

## How to run

python -m pip install -r requirements.txt
jupyter notebook

Then open `world_cup_analysis.ipynb` and run all cells.