## Metis Project 2: Regression
### Predicting international movie box office revenue

by [Matt Ranalletta](https://www.linkedin.com/in/matthewranalletta/)

### Summary

The main goal of this project was to come up with a model to predict the international box office revenue of a movie based off a number of known data. A model like this could be useful for production companies or studios to decide what kinds of movies to make, for distributors to estimate how much money to dedicate to marketing, or for cinemas to know more about the types of movies that make the most money.

The requirements for the project were to scrape HTML from a website using Beautiful Soup or Selenium, and then perform regression analysis on the data using Python packages from Scikit-learn or StatsModels.

In the end, the r-squared value for my model ended up being about .29, indicating that only 29% of the variance for international box office revenue was due to the features in my model.

---
### Deliverables
- `movies_scraping.ipynb`- scraping data from site, basic cleaning
- `top1000.pkl` - pickled dataframe after scraping
- `movies_regression.ipynb` - regularization, validation, regression analyses, feature engineering

---
### Data
Box Office Mojo: [Top 1000 movies by worldwide gross](https://www.boxofficemojo.com/chart/top_lifetime_gross/?area=XWW)

---
### Tools
Python packages: BeautifulSoup, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

---
### Variables

**Target variable**: International box office revenue

**Original features**: </br>
- year
- budget
- release month
- runtime
- ratings (yes or no): G, PG, PG-13, R
- genre (yes or no): action, adventure, animation, biography, comedy, crime, documentary, drama, family, fantasy, history, horror, music, musical, mystery, romance, sci-fi, sport, thriller, war, western

**Final features, pared down by Lasso regression**: </br>
- Positive correlation: 
  - year
  - budget
  - runtime
  - G rating
  - genres: adventure, animation, comedy </br>
- Negative correlation: 
  - release month
  - genres: action, biography, crime
