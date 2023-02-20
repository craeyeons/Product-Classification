# Product-Classification

## Why

With the number of choices and brands in supermarkets multiplying, it would take great effort to manually sort through items one by one. Hence this project aims to help sort supermarket items by its brand and type. 

Ideally this can lead to more ambitious projects such as automated checkout systems, item management systems, product recommendation, or even pricing and discounts to help maximize profit.

## How

We shall begin by collecting our own data set of brands which we wish to identify. In this case, we have a group of 10 brands.
To collect our own set of images, Selenium is utilised to implement a simple web scraper.

Then, we simply train a Convoluted Neural Network (CNN) model to perform the classification. In particular, mini batch gradient descent with the Adam optimiser is utilised.

Finally, we analyse our data using captum and matplotlib. With this, we can clearly visualise what our model is focusing to come up with its decision. 
