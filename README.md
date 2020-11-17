﻿Bitcoin Price Notification
Overview
As we all know that the Bitcoin price rises or falls gradually several times within minutes.This python based application will allow us to keep a track of the price.As soon as the price reaches a threshold ,it’ll send notifications or alerts on the Telegram Application.
Specifications
Coinmarketcap API
The coinmarket api provides the latest price.We import the requests module and define the bitcoin_api_url variable which contains the Coinmarketcap API URL for Bitcoin.
IFTTT Applet
IFTTT is a popular automation website. IFTTT (“if this, then that”) is a web service that bridges the gap between different apps and devices..
Concepts Used
* Oops to write clean modular extensible code
* WebHooks(IFTTT) and python package
* requests in python(GET, POST) using the requests library


Extra Features
1. A graph demonstrating the price curve.
2. Price prediction and plotting
3. Displaying the results for various currencies






Requirements
* download pip
* download requests module for python3 using command => $ python3 -m pip install requests
* Install requests by using the command pip install requests
* Install pandas by using the command pip install pandas
* Install numpy by using the command pip install numpy
* Install sklearn by using the command pip install sklearn
* Install matplotlib by using the command pip install matplotlib
* Create a ifttt applet by following this link https://ifttt.com/create/
Steps Involved


* Create an account on coinmarketcap api and get the api key
* Create a ifttt applet
1. Choose the “webhooks” service and select the “Receive a web request” trigger
2. For the action select the “Notifications” service and select the “Send a rich notification from the IFTTT app” action
3. Set the message to Bitcoin price is at ${{Value1}
4. Create the action and finish setting up the applet
* Regular price updates applet:
1. Again choose the “webhooks” service and select the “Receive a web request” trigger
2. For the action select the “Telegram” service and select the “Send message” action
3. Set the message text to: Latest bitcoin prices:<br>{{Value1}}
4. Create the action and finish with the applet
* Once you’re done doing this use the get request to get the data from the coinmarket Api and convert it to json format 
* Convert the timestamp according to your system
* Then use the threshold value to compare the price and send the notification on the Telegram app using the ifttt applet
* Store the value of the date and price as (x,y) and plot it
* Split the data into test and train dataset in the 1:4 ratio
* Feed the data to the model
* Calculate the accuracy
* Print the predicted values finally
* Plot the predicted value on the previous graph