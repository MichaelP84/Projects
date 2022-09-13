# Sentiment Analysis + Stock Data LSTM Model


### Description

This project involves combining sentiment analysis connotations with stock data in an attempt to create a model that can account for complicated fluctuations in a stock price that result from popular opinion (or changes in the value of the company that are reflected in popular opinion).


### Libraries Used

The Long Shot Term Memory Model is implemented using tensorflow, the parameters of the model are tuned using a grid-serach, and the model is set to converge multiple times, recording the best local optimum, using tf.keras.models.model_to_json and is loaded using tf.keras.models.model_from_json. The training time of the model is optimized using Tensorflow early stopping, and Pandas and numpy are used for data manipulation and formatting. keras.preprocessing.sequence.TimeseriesGenerator is used to format the data into a time series format.


### Challenges faced

The biggest problem that this project faces is its inability to perform better than the baseline. This is largely due to the fact that the model has low variance but lacks a substantial amount of data to learn from. A more substantial amount of data is required because of the complicated patterns the model must learn between two already complicated series: stock prices and people's tweets.

While the mean absolute error had made great improvments through many tweaks of the model, a different approach or larger scale model should be implemented if this were to be tried again.
