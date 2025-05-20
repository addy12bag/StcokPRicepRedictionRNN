# StcokPRicepRedictionRNN
This project aims to predict future stock prices using a Recurrent Neural Network (RNN) architecture, specifically a Stacked Long Short-Term Memory (LSTM) model. LSTMs are a type of RNN that are highly effective for time series forecasting due to their ability to learn long-term dependencies in sequential data.

The dataset used contains historical stock prices, typically including features like Open, High, Low, Close prices, and Volume. The data is preprocessed by normalizing it and converting it into a supervised learning format using sliding time windows.

The core of the model is a Stacked LSTM architecture, which consists of multiple LSTM layers stacked on top of each other. This deep structure allows the model to learn more abstract representations of patterns in stock price movements, leading to improved prediction performance. Dropout layers are added between LSTM layers to prevent overfitting, and the final Dense layer outputs the predicted stock price.

The model is trained on historical data using Mean Squared Error (MSE) as the loss function and Adam optimizer. The trained model is then evaluated on unseen test data and visualized through plots comparing predicted and actual stock prices.
