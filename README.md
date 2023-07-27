# AlcoholSalesAR-Forecast

Alcohol Sales Forecasting with Autoregression (Time Series Analysis)

<p>
  <img src="https://cdn.stocksnap.io/img-thumbs/960w/whiskey-glass_NBCKWLMBGX.jpg" width="350" alt="alcohol image">
</p>

## Context

Alcohol, a timeless and captivating drink, has influenced societies for ages. Its global trade and diverse appeal make predicting prices crucial. Autoregression models analyze historical data to forecast trends, guiding producers, distributors, and consumers. From wines to beers and spirits, alcohol's allure transcends borders, captivating enthusiasts worldwide.

## Autoregression

Autoregressive (AR) models are a subset of time series models, which can be used to predict future values based on previous observations. AR models use regression techniques and rely on autocorrelation in order to make accurate predictions. Autoregressive is made of the word, Auto and Regressive which represents the linear regression on itself (auto). In the context of time-series forecasting, autoregressive modeling will mean creating the model where the response variable Y will depend upon the **previous values of Y** at a pre-determined **constant time lag**. The time lag can be daily (or 2, 3, 4… days), weekly, monthly, etc. [0]

A time series is a sequence of measurements of the same variable(s) made over time. Usually, the measurements are made at evenly spaced times - for example, monthly or yearly. Let us first consider the problem in which we have a y-variable measured as a time series.
In this context, we might have **_y_** a measure of the gold price, with measurements observed every 3 months. To emphasize that we have measured values over time, we use **_t_** as a subscript rather than the usual "**i**," i.e., means **_y_** measured in time period **_t_**. The $\epsilon$ is the error term (typically normally distributed). [1]

An autoregressive model is when a value from a time series is regressed on previous values from that same time series. for example,
$y_{t}$ on $y_{t-1}$ [1]:

$y_t = \beta_0 + \beta_{1} y_{t-1} + \epsilon_t$

## Data

Data from FRED with a CC0 licence. [2]

File CSV has 377 rows, and the last date is 2023-04-01.

## Implementation

The implementation of gold price forecasting is done in a Jupyter Notebook. Inspiration by [4].

Sources:

0. Ajitesh Kumar, "Autoregressive (AR) models with Python examples", https://vitalflux.com/autoregressive-ar-models-with-python-examples/
1. The Pennsylvania State University, "Autoregressive Models", T.2.1, https://online.stat.psu.edu/stat501/book/export/html/996
2. St. Louis Fed's Federal Reserve Economic Data, "Merchant Wholesalers, Except Manufacturers' Sales Branches and Offices: Nondurable Goods: Beer, Wine, and Distilled Alcoholic Beverages Sales", https://fred.stlouisfed.org/series/S4248SM144NCEN
3. Photo by PublicDomainPictures: https://pixabay.com/photos/gold-bars-wealth-finance-gold-bars-163519/
4. Egor Howell, "How To Forecast Time-Series Using Autoregression", https://towardsdatascience.com/how-to-forecast-time-series-using-autoregression-1d45db71683
