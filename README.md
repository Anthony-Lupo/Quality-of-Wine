Predicting The Wine Quality


![20190430_195732](https://user-images.githubusercontent.com/94997866/155644786-516ce884-cf78-40e0-821d-7aa363d7350e.jpg)

Sommeliers are able to tell the quality of wine by taste, smell, sight and mouth feel. What if you aren't a Sommelier and you want to make wine? How do you decide what is a good wine?

I have been tasked with predicting the quality of wine based off of 11 different features. These are chemical properties of wine, that can be quantified by anybody.

The qualities are as follows:

For more information, read [Cortez et al., 2009].
Input variables (based on physicochemical tests):
1. volatile acidity :   Volatile acidity is the gaseous acids present in wine.
2. fixed acidity :   Primary fixed acids found in wine are tartaric, succinic, citric, and malic
3. residual sugar :   Amount of sugar left after fermentation.
4. citric acid :    It is weak organic acid, found in citrus fruits naturally.
5. chlorides :   Amount of salt present in wine.
6. free sulfur dioxide :   So2 is used for prevention of wine by oxidation and microbial spoilage.
7. total sulfur dioxide 
8. pH :   In wine pH is used for checking acidity
9. density 
10. sulphates :    Added sulfites preserve freshness and protect wine from oxidation, and bacteria.
11. alcohol :   Percent of alcohol present in wine.
Output variable (based on sensory data):
12 - quality (score between 3 and 8)


This is a regression Problem, that will be analyzed by different regression models to help determine the best evaluation of the predictions.

---------------------------------------------------------------------
After Exploring the data, there were multiple correlations discovered
---------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/94997866/155646645-619916d8-0145-42c1-97c6-787cd936a260.png)


There seems to minimal correlation between alcohol and quality, at 0.48, making it the strongest of the correlations between a feature and the target.

There seems to be a strong correlation between:

density and fixed acidity (0.67)
citric acid and fixed acidity (0.67)
pH and fixed acidity (0.69)
There is a negative correlation between:

fixed acidity & volatile acidity (-0.26)
fixed acidity & free sulfur dioxide (-0.14)
fixed acidity & total sulfur dioxide (-0.1)
fixed acidity & pH (-0.69), this is a strong negative correlation
fixed acidity & alcohol (-0.062)
volatile acidity & citric acide (-0.55) strong
citric acid & pH (-0.55) strong!
alcohol & density (-0.5)

![image](https://user-images.githubusercontent.com/94997866/155646868-05c1c4dd-f9a3-4465-8a85-0f4909b4879c.png)
![image](https://user-images.githubusercontent.com/94997866/155646907-a0e84c2a-2f36-4660-b064-110266592b4f.png)
![image](https://user-images.githubusercontent.com/94997866/155646922-b79a3483-aef7-4958-990c-102410e45ccf.png)

