# Deep-Learning-Based-Quantitative-Trading-Program

This program uses a 40-parameter 4-layer linear neural network with an LSTM to predict the stock market of a company based on Twitter sentiment analysis. In this setting, the sample testing company is Microsoft.

The program consists of three sections:

The first section is a simple 20-parameter 4-layer linear neural network with an LSTM that takes in past data of 20 days from Microsoft stock and trains itself.
The second section takes into account Twitter sentiment of Microsoft for the past 20 days and trains a 40-parameter 4-layer linear neural network with an LSTM to predict the future stock.
The third section splits the training data set into two fractions: when the stock is going up or when the stock is going down. It then trains two 40-parameter 4 layer neural network, each with an LSTM, to understand the correlation bewteen Twitter sentiment and up-down trends. It then implements a policy search algorithm to determine whether the stock goes up or down with a threshold calculated by taking the median of the Twitter sentiments with the respective data in the up and down fractions. Finally, it predicts the stock market trends of Microsoft.
