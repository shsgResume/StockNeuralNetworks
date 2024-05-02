<h1>Requirements</h1>
The packages can be installed easily via Miniconda. The packages required are

> [!NOTE]
> Python &ge; 3.11 & < 3.12 <br>
> Numpy <br>
> Pandas <br>
> Tensorflow and Keras <br>
> Seaborn <br>
> yfinance <br>
> Matplotlib <br>

<h1>About</h1>
This repository is a roject that utilizes a Recurrent Neural Network (RNN) to predict the stock prices of companies in the NYSE. Options prices and visualizations are also shown in the Jupyter notebook. 
The data and analysis can be used to make informed decisions for investors.

The stock prices can be pulled form the package yfinance. To predict the stock prices, an RNN of type Long Short Term Memory (LSTM) is used. LSTM is suitable for time series analysis,which is what stock prices pretty much are.


Some companies (Microsoft, Micron and Nvidia; tickers MSFT, MU, NVDA) are chosen here to investigate there correlations. An sns (using the Seaborn package) plot can be created to visualize the correlations of the stock prices.
![image](https://github.com/shsgResume/StockNeuralNetworks/assets/167844966/23345cd8-d5d2-46ec-a55f-f71b1a37f7e3)


Afterwards, to predict stock prices (or just for understanding), moving averages of the stock prices can be made manually on the data using the efficient Pandas library.

![image](https://github.com/shsgResume/StockNeuralNetworks/assets/167844966/b4fb5458-5ee2-44f0-a719-1142ce2bc887)



The intial prices for a 10 year window (this was replotted on 1 May 2024) was made and can be seen below.

![image](https://github.com/shsgResume/StockNeuralNetworks/assets/167844966/0231f41d-c609-4152-b8fb-4788d5c13d20)

Using this information, it is possible to train an RNN, with some of the data as the training data. Shown here is when the RNN was trained with 80% of the 10 year data as the training data.

![image](https://github.com/shsgResume/StockNeuralNetworks/assets/167844966/9dd899f3-d15f-4110-bde1-21a045767c0a)
![image](https://github.com/shsgResume/StockNeuralNetworks/assets/167844966/2b1e677b-720d-4d8a-a365-c22bba0803f8)
![image](https://github.com/shsgResume/StockNeuralNetworks/assets/167844966/b74f6e80-4b6f-4dce-ba4c-8219f32f75d0)

Options prices are also included in th eJupyter notebook for traders interested in that instead.

<h1>References</h1>

The idea to create this was inspired from fares-ds 's work [link](https://github.com/fares-ds/Predicting-the-closing-stock-price-of-APPLE-using-LSTM)





