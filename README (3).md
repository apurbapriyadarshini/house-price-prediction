# House Price Prediction

**Internship Project | CodTech IT Solutions**

## Objective
Predict the price of a house based on features such as area, number of bedrooms, bathrooms, stories, and amenities (air conditioning, parking, furnishing status, etc.). This is a supervised **regression** problem.

## Dataset
`Housing.csv` — 545 houses with the following columns:
- `price` — target variable
- `area`, `bedrooms`, `bathrooms`, `stories`, `parking` — numeric features
- `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `prefarea` — yes/no features
- `furnishingstatus` — furnished / semi-furnished / unfurnished

## Approach
1. Exploratory Data Analysis (price distribution, area vs price, correlation heatmap)
2. Data preprocessing (encoding yes/no columns, one-hot encoding furnishing status)
3. Model training using **Linear Regression**
4. Evaluation using MAE, RMSE, and R2 score
5. Feature coefficient analysis
6. **Interactive demo** — enter a house's details and get a live price prediction

## How to Run
1. Install dependencies: `pip install -r requirements.txt`
2. Open `House_Price_Prediction.ipynb` in Jupyter Notebook or VS Code
3. Run all cells in order
4. In the last cell, enter house details when prompted to get a live price prediction

## Results
The Linear Regression model achieves an R2 score of around 0.95 on the test set, meaning it explains most of the variation in house prices. Area, air conditioning, and preferred location turned out to be the strongest price drivers.
