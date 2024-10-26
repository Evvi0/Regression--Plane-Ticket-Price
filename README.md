# Regression--Plane-Ticket-Price

## Summary
Airline_Clean_Dataset.csv displays a dataframe of 12 columns that describe specific flight details. These details will be used to create a regression model, that predicts the price of a ticket for that specific airline, flight time etc. If applied, a model sich as this can pose very useful for knwoing how much a flight will cost you. This works well outside the scope of normal plane ticket purhcasing because it allows for creating flights that would not exist on an airline's website, making it easy to know the price of a flight without having to wait for a flight with those specifics to come about.

## Visual
A histogram that shows the log of price creates a more normalized graph to display plane tickets at each price.

![image](https://github.com/user-attachments/assets/fc75b963-7449-41df-b8d1-82f7167f2bbd)


## Techniques
Most columns in this dataset contain numerical features in different ranges than others. Some has categorical features. These two probelsm were fixed by simple use of a MinMaxScaler, and a target encoder. For the model, I used XGBRegressor with some parameters like early stopping rounds and n estimators.

![image](https://github.com/user-attachments/assets/23100516-c4ce-4479-84d9-c73b1bbeddf2)


## Evaluation
To see how my model did, I used RMSE.

![image](https://github.com/user-attachments/assets/7c1e8b65-f49e-4319-a0c2-988b17927a2f)
