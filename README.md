# Product-Classification

## Why

With the number of choices and brands in supermarkets multiplying, it would take great effort to manually sort through items one by one. Hence this project aims to help sort supermarket items by its brand and type. 

Ideally this can lead to more ambitious projects such as automated checkout systems, item management systems, product recommendation, or even pricing and discounts to help maximize profit.

## How

We shall begin by collecting our own data set of brands which we wish to identify. In this case, we have a group of 10 brands.
To collect our own set of images, Selenium is utilised to implement a simple web scraper.

Then, we simply train a Convoluted Neural Network (CNN) model to perform the classification. In particular, mini batch gradient descent with the Adam optimiser is utilised.

Finally, we analyse our data using captum and matplotlib. With this, we can clearly visualise what our model is focusing to come up with its decision.

## Results

At 15 epochs, the results are as follow:

final training set error: 12.952%
final test set error: 17.280%

With further investigation using captum and matplotlib, the results seem to be satisfactory, yet not mature for commercial use. 

<img width="791" alt="image" src="https://user-images.githubusercontent.com/42890150/220179296-b519b223-8de4-49b9-99bd-2d2bc12d2aeb.png">

<img width="558" alt="image" src="https://user-images.githubusercontent.com/42890150/220179369-5e825948-000e-4aae-b59d-50c84e0aeeec.png">

## Further Imporovements

1. The data set provided for this model is not particularly large. (~150 images * 4 rotations per class) Hence the model would greatly benefit with a larger data set.

2. The learning rate could be lowered/fined tuned to prevent overfitting towards the last few epochs. This could perhaps be achieved with a learning rate scheduler.

3. The model may benefit with a greater number of epochs.

4. The model may benefit more if images of greater resolution were utilised. The resolution of images in this model is greatly decreased to compensate for the lack of computing power.


