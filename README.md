# Crypto Predictions

- Download github repository
 - https://github.com/c1im4cu5/Crypto_Predictions

```
git clone https://github.com/c1im4cu5/Crypto_Predictions
```

## R Squared Mean Machine Learning Algorithm - Flask API

API is designed to receive a single input for cryptocurrency trading pair from Coinbase. Any traded pair on Coinbase can be queried. Example Pairs:

- BTC-USD
- DOGE-USD
- ETH-USD
- ATOM-USD
- WBTC-BTC

# Using Postman:
GET and POST can be found @ /prediction

form-data<br>
Form Field = pair

# Details
Queries will be placed for a "day" interval. Predictions will be closing values.<p>

Algorithm will need to load tensorflow; which will take some time. Furthermore, user will need to wait for epochs to run. Total run time could exceed ten minutes. <p>

# Example API <br>
API was recently shut down (5-3-22) after being run on GCP Cloud Run for a few months.<p>
 
# Contributing <br>
Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to added/altered.
