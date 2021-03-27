## Stock market APIs

We will use the [yfinance](https://pypi.org/project/yfinance/) because Yahoo decommissioned their official API on May 15th 2017. In order to fetch the tickers for all possible stock market products we will use [Yahoo ticker downloader](https://github.com/Benny-/Yahoo-ticker-symbol-downloader). There are other possible APIs to use, for example [yahooquery](https://github.com/dpguthrie/yahooquery). 

## Data analysis

Ideas to analyse stock data:

- Fit a linear regression to data and see if the R coefficient is good enough to approximate the data as linear
- SARIMAX models
- RNN with LSTM cells combined with attention mechanism. Similar to Seq2seq but just taking the encoder part. Take the output of the encoder (which will be a vector) to asses probability that stock price will increase by a predefined amount in a given amount of time, e.g. the price will go up *50%* in the next *6 months*. See [this](https://levelup.gitconnected.com/building-seq2seq-lstm-with-luong-attention-in-keras-for-time-series-forecasting-1ee00958decb) for a possible starting point.
