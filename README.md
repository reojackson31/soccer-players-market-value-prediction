# Predicting Market Value of Soccer Players based on their attributes

## 1. Problem Statement

In the dynamic and financially significant world of professional soccer, accurately estimating a player's market value is crucial for clubs during transfer windows. The transfer market value of a player is influenced by a variety of factors like their age, contract duration, physical attributes, and playing abilities. The objective of this project is to develop a regression model that can predict the transfer market value of soccer players using available data on the attributes of players. This model can assist soccer clubs, sports analysts, and market stakeholders in making informed decisions during player signings and sales.

## 2. Data Source

For this project, the dataset from EA Sports FC (FIFA) 2024 is used. The dataset contains detailed attributes of over 18,000 players who are currently playing in top-tier leagues globally. The dataset has details about the physical attributes of players (age, height, weight), their current club and contract details, and ratings for their playing attributes, including speed, passing, shooting, and work rate, among others. The current market value (in EUR) for these players is used as the target variable for regression.

## 3. Model Selection

Among the models tested (refer to the notebook), the Random Forest model is selected due to its significantly lower Mean Squared Error (MSE), indicating a higher accuracy in prediction compared to the other models. While Random Forest models are relatively simple to implement, they also offer a degree of explainability through options like feature importance scores, making it easier to interpret how different predictors influence the model's predictions. This balance of high accuracy, simplicity, and interpretability makes the Random Forest model a preferred choice for this project.

## 4. Interpretation of Results

The feature importance scores from the random forest model reveal that 'overall' player rating is the most influential factor in determining a player's market value. Attributes such as 'dribbling', 'passing', 'defending', and 'shooting' are also relevant, highlighting the importance of technical skills in valuing players. Interestingly, physical attributes like 'age', 'height_cm', and 'weight_kg', along with contract duration ('rem_contract_yrs'), have lesser but still significant impacts, suggesting a balanced consideration of skills, physicality, and potential future contribution in the market value of a player.

## 5. Conclusions

The insights derived from the model provide an initial framework for clubs and agents to assess the market value of players based on key attributes, ensuring that negotiations for buying or selling players are backed by data-driven valuations. By understanding the factors that most significantly impact a player's market value, such as overall rating, technical skills, and physical attributes, stakeholders can make informed decisions that align with the financial and strategic goals of their clubs. This model allows stakeholders to determine optimal asking prices for players they wish to sell and establish fair price points for potential acquisitions, thereby optimizing their investment in the transfer market and creating a more transparent and rational player valuation process.

## 6. Next Steps

In this model, we have only considered the dataset containing the physical attributes of players, their current club and contract details, and their playing attributes. For next steps, expanding the dataset to include historical performance stats of players such as minutes played, goals scored, assists, and clean sheets can improve the model's accuracy since these factors are also critical in deciding the market value of a player. Adding these additional predictors will allow for a more detailed understanding of a player's value, taking into account their direct contributions to matches, thereby improving the model's capability to predict market value with greater accuracy.
