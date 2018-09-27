# Prophet

- https://facebook.github.io/prophet/
- [Quick Start](https://facebook.github.io/prophet/docs/quick_start.html)

## Forecasting at scale

Prophet is a forecasting procedure implemented in R and Python. It is fast and provided completely automated forecasts that can be tuned by hand by data scientists and analysts.

Prophet is a procedure for frecasting time series data based on an additive model where non-linear trends are fit with yearly, wekkly, and daily seasonality, plut holiday effect. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well.

Prophet is open source software released by Facebook's Core Data Science tema. It is available for download on CRAN an PyPI.

### Accurate and fast

Prophet is used in many applications across Facebook for producing reliable forecasts for planning and goal setting. We've found it to perform better than any other approach in the majority of cases. We fit models in [Stan](http://mc-stan.org/) so that you get forecasts in just a few seconds.

### Fully automatic

Get a reasonalble forecast on messy data with no manual effort. Prophet is robust to outliers, missing dta, and dramatic changes in your time series.

### Tunable forecasts

The Prophet procedure includes manyu possibilities for user to tweak and adjust forecasts. You can use human-interpretable parameters to imporove your forecast by adding your domain knowledge.

### Available in R or Python

We've implemented the Prophet procedure in R and Python, but they share the same underlying Stan code for fitting. Use whatever language you're comfortable with to get forecasts.

## Installation

### PyStan 설치

- https://pystan.readthedocs.io/en/latest/windows.html

```python
conda install numpy cython matplotlib scipy pandas pystan -c conda-forge
```

## Quick Start

### Python API

Prophet follows the `sklearn` model API. We create an instance of the `Prophet` class and then call its `fit` and `predict` methods.

The input to Prophet is always a dataframe with two columns: `ds` and `y`. The `ds`(datestamp) column should be of a format expected by Pandas, ideally YYYY-MM-DD for a date or YYYY-MM-DD HH:MM:SS for a tiemstamp. The `y` column must be numeric, and represents the measurement we wish to forecast.

As an example, let's look at a time series of the log daily page views for the Wikipedia page for [Peyton Manning](https://en.wikipedia.org/wiki/Peyton_Manning). We scraped this data using the [Wikipediatrend](https://cran.r-project.org/web/packages/wikipediatrend/vignettes/using-wikipediatrend.html) package in R. Peyton Manning provides a nice example because it illustrates some of Prophets' features, like multiple seaonality, changing growth rates, and the ability to model special days (such as Manning's playoff and superbowl appearances). The CSV is available [here](https://github.com/facebook/prophet/blob/master/examples/example_wp_log_peyton_manning.csv)

First we'll import the data:


"# prophet-quick-start"  git init git add README.md git commit -m "first commit" git remote add origin git@github.com:jacegem/prophet-quick-start.git git push -u origin master
"# prophet-quick-start"  git init git add README.md git commit -m "first commit" git remote add origin git@github.com:jacegem/prophet-quick-start.git git push -u origin master
"# prophet-quick-start" 
