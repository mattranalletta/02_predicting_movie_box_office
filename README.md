# Project 2: Regression
## Predicting international movie box office revenue

The main goal of this project was to 

### Variables

**Target variable (y)**: International box office revenue

**Original features (X)**: </br>
year; budget; release month; runtime; ratings (yes or no): G, PG, PG-13, R; genre (yes or no): action, adventure, animation, biography, comedy, crime, documentary, drama, family, fantasy, history, horror, music, musical, mystery, romance, sci-fi, sport, thriller, war, western

**Final model features, pared down by Lasso regression**: </br>
Positive correlation: year; budget; runtime; G rating (yes or no); genre (yes or no): adventure, animation, comedy </br>
Negative correlation: release month; genre (yes or no): action, biography, crime

### Data
Box Office Mojo: [Top 1000 movies by worldwide gross](https://www.boxofficemojo.com/chart/top_lifetime_gross/?area=XWW)

### Tools
Python packages: BeautifulSoup, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

### Possible impacts
