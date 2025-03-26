# House Price Prediction

This project aims to predict house prices using machine learning techniques. By analyzing various features of houses, such as size, location, and number of rooms, the model provides valuable insights for potential buyers or sellers in estimating housing prices.

## Project Overview

The objective of this project is to develop a model that accurately estimates house prices based on specific features. This prediction task is significant in real estate and finance, enabling informed decision-making for buyers, sellers, and investors. By employing machine learning algorithms and a curated dataset, this project provides a powerful tool for estimating house prices.

## Key Features

- **Data Collection and Processing:** The project utilizes a dataset containing features such as house age, number of rooms, location, and other relevant attributes. Using Pandas, the data is processed and transformed to ensure it is suitable for analysis.

- **Model Development:** The machine learning model is implemented using algorithms like Linear Regression, Decision Trees, or more advanced techniques like XGBoost. The trained model is evaluated for accuracy and reliability.

- **Web Application:** The project incorporates a web application, providing a user-friendly interface for predicting house prices. Users can input details such as the number of bedrooms, bathrooms, house size, and location to receive a price prediction.


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>House Price Prediction</title>
    <link rel="stylesheet" href="app.css">
</head>
<body>
    <div class="container">
        <h1>🏡 House Price Predictor</h1>
        <p>Enter the details below to estimate the price.</p>

        <div class="input-group">
            <label for="location">📍 Location:</label>
            <select id="location"></select>
        </div>

        <div class="input-group">
            <label for="sqft">📏 Total Sqft:</label>
            <input type="number" id="sqft" placeholder="Enter total square feet">
        </div>

        <div class="input-group">
            <label for="bhk">🛏️ BHK:</label>
            <input type="number" id="bhk" placeholder="Number of bedrooms">
        </div>

        <div class="input-group">
            <label for="bath">🚿 Bathrooms:</label>
            <input type="number" id="bath" placeholder="Number of bathrooms">
        </div>

        <button onclick="predictPrice()">💰 Predict Price</button>

        <h2 id="result">Estimated Price: <span>---</span></h2>
    </div>

    <script src="app.js"></script>
</body>
</html>
