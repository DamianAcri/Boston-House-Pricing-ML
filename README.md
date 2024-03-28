# Boston-House-Pricing-ML

## Software and requirements

1.  [Github Account](https://www.github.com)
2.  [Heroku Account](https://heroku.com)
3.  [Visual Studio Code IDE](https://code.visualstudio.com)
4.  [GIT CLI](https://git-scm.com/book/en/v2/Getting-Started-The-Command-Line)


### Create new enviroment

```
conda create -p venv python==3.7 -y
```
### Dataset Description
The dataset used for this project contains the following variables:

CRIM: Per capita crime rate by town
ZN: Proportion of residential land zoned for lots over 25,000 sq.ft.
INDUS: Proportion of non-retail business acres per town
CHAS: Charles River dummy variable (1 if tract bounds river, 0 otherwise)
NOX: Nitric oxides concentration (parts per 10 million)
RM: Average number of rooms per dwelling
AGE: Proportion of owner-occupied units built prior to 1940
DIS: Weighted distances to five Boston employment centers
RAD: Index of accessibility to radial highways
TAX: Full-value property-tax rate per $10,000
PTRATIO: Pupil-teacher ratio by town
B: 1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town
LSTAT: Percentage lower status of the population

### Model Development
The machine learning model is built using Flask, a web framework for Python. The model is trained using a regression algorithm to predict house prices based on the provided features. Two files are used in the model: regmodel.pkl, which contains the trained regression model, and scaling.pkl, which contains the scaling parameters used for data preprocessing.

### Usage
The user can interact with the model through a web interface. Upon entering the relevant features of a property, the model predicts the price of the house.
The model can also be accessed programmatically via an API (/predict_api endpoint) by sending a JSON request with the necessary data.
Deployment
The Flask application is deployed locally with debugging enabled for easy development and testing. It listens on port 5000 by default and can be accessed through a web browser or programmatically.

### Files
regmodel.pkl: Pickle file containing the trained regression model.
scaling.pkl: Pickle file containing the scaling parameters used for data preprocessing.
home.html: HTML template for the user interface.

Contributors
Damián Acri

Acknowledgments:
Krish Naik for all the info provided

Disclaimer: This project is intended for educational purposes only. The house price predictions should not be considered as financial advice or used for any commercial purposes.

