# AgriFriend-Agriculture-Price-Prediction-Monitoring-on-APP
I have used data provided by open government site data.gov.in, which updates prices of the market daily.
## Working Interface Details:
I have provided user choice to see current market prices based on two choices: market-wise or commodity wise to increase accessibility options.
## Market wise:
The user has to provide the State, District, and Market name and then select a market-wise button. Then the user will be shown the prices of all the commodities present in the market in a graphical format so that he can analyze the rates on one scale. This feature is most helpful for a regular buyer to decide the choice of the commodity to buy. He is also given feature to download the data in a tabular format(CSV) for accurate analysis.
## Commodity Wise:
The user has to provide State, District and Commodity name and then select the Commodity wise button. Then the user will be shown the prices of all the markets present in the region with the commodity in a graphical format so that he can analyze the cheapest commodity rate. This feature is most helpful for wholesale buyers. He is also given feature to download the data in a tabular format(CSV) for accurate analysis.
## More Info.
On the first activity, the user is also given forecasting choice. It can be used to forecast the wholesale prices of various commodities at some later years. Regression techniques on time series data are used to predict future prices. Select the type of item and click the link for future predictions.

There are 3 java files Forecasts, DisplayGraphs, DisplayGraphs2 (in android code)..... Please change the localhost "server_name" at the time of testing as the server name changes each time a new server is made.
## Things Used:
I have used pandas, numpy, scikit learn, seaborn and matplotlib libraries for the same. The dataset is thoroughly analyzed using different functions available in pandas in my .iPynb file. Not just in-built functions are used but also many user-made functions are made to make the working smooth. Various graphs like point plot, heat-map, barplot, kdeplot, distplot, pair plot, strip plot, joint plot, regplot, etc are made and also deployed on the android app as well.
## To integrate the android app and machine learning analysis outputs
Used Flask to host my laptop as the server. I have a separate file for the Flask as server.py. Where all the necessary stuff of client request and server response have been dealt with. I have used npm package ngrok for tunneling purposes and hosting.
A different.iPynb file is used for the time series predictions using regression algorithms and would send the CSV file of prediction along with the graph to the android app when given a request.
This whole project was developed under a 36 hrs Hackathon.
