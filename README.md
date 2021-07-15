# Wine Analysis
The goal of this project is to predict if a wine will be red or white based off of a variety of different factors.

## Red vs White

![Sulphates and Fixed Acidity](https://user-images.githubusercontent.com/87451665/125705290-872c786d-922e-497d-bea9-f5016db0b738.JPG)

As we can see in the graph above, some factors such as Sulphates and Fixed Acidity differe substantially between red and white wines.
Below we can see that all of the factors included in the initial dataset are significant in a linear model to predict if a wine will be red or white.

![Significance Levels](https://user-images.githubusercontent.com/87451665/125705807-619827d4-7b2c-4899-8b99-ed164e540ef3.JPG)

Additionally, according to VIF (Variance Inflation Factors) density is the only variable that coudl possibly have significant multicolliniarity.

## Modeling

Using the lm function to predict we are presented with the following confusion matrix.  All data in the bottom left or top right of the table is misidentified.  As we can see there are 8 misidentified datapoints out of 1625.

![Model1](https://user-images.githubusercontent.com/87451665/125710997-e7669045-927f-40f5-8090-72e316cbd772.JPG)

Utilizing the SuperLearner package to do the same linear model, but with SuperLearner's optimizations we are presented the following confusion matrix with 0 misidentified datapoints.

![Model2](https://user-images.githubusercontent.com/87451665/125711042-2adfc554-a3f2-4831-b8b1-c0064f73267e.JPG)
