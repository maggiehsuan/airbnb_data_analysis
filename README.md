# Airbnb Boston and Seattle Data Analysis

## Airbnb Boston and Seattle Data Analysis

### Motivation

For this project, I want to explore the Boston and Seattle Airbnb dataset and find out the answer for my three business questions of interest by using descriptive analysis, inferential statistics, and machine learning:

**Question 1:**
How does price and availability of airbnb listings in Seattle and Boston change over time? Are there any seasonal patterns? 

**Question 2:**
Do the amenities provided by the host have impact on price and review ratings? This may help hosts improve their listings to increace price and revenue.

**Question 3:**
What key feautures impact the listings price the most? Can we predict the listing price well with LinearRegression Model? Can we have a better prediction by using other Model? 


### Installation

This project requires Python 3.x and the following Python libraries installed:

- NumPy 
- Pandas
- statsmodels
- scikit-learn 
- [catboost](https://catboost.ai/docs/concepts/python-installation.html)
- [plotly](https://plotly.com/python/getting-started/)

You will also need to have software installed to run and execute an iPython Notebook

Install Anaconda, a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.

### File Descriptions

For each city, the dataset is composed of three CSV files:<br>
- listings.csv   -    all detailed informations about listings<br>
- calendar.csv    -    availability and price information by day<br>
- reviews.csv   -   reviews for each listing
 

### Results

**Answer to Question 1:**

The rates in Seattle are significantly lower than in Boston, also the rates are higher on Friday and Saturday and at the lowest on Tuesdays in both cities. By comparing the rates plots with the availability plots we can identify a slight opposite trends of availability towards the rates, for example in September and October in Boston are the vacancies at only about 30 percent and the daily rates quite expensive at about 190$. The availabilities of the listings do not differ by weekday in both cities.

**Answer to Question 2:**

Price is most correlated to the following amenities: Air Conditioning, Cable TV, Family-/Kid Friendliness, TV, and Doorman. The amenities with the highest negative correlation to review ratings are: translation missing, gym, smoking allowed, pool, washer/dryer. On average amenities leads to higher price and less high to review score ratings. Expensive rates tend to result in reviews with lower ratings.

**Answer to Question 3:**

The following features are significant values to listing price as result of Catboost Model: "accommodates", "extra_people", "weekly_price", "number of bedrooms", which is different from the results of Linear Regression. 
As result of Linear Model the neighborhood area and frequency of calendar updates are highly related to price. 


### Licensing, Authors, Acknowledgements

Links for the data on Kaggle: [Boston](https://www.kaggle.com/airbnb/boston) and [Seattle](https://www.kaggle.com/airbnb/seattle/data).
