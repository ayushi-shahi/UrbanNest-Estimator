<!DOCTYPE html>
<html>
<head>
    <title>UrbanNest Estimator</title>
</head>
<body>

<h1>UrbanNest Estimator</h1>

<p><strong>UrbanNest Estimator</strong> is a machine learning project focused on predicting real estate prices. Designed specifically for urban markets, the model utilizes key features such as location, size, number of bedrooms, and amenities to provide accurate property price predictions.</p>

<h2>Table of Contents</h2>
<ol>
    <li><a href="#introduction">Introduction</a></li>
    <li><a href="#dataset">Dataset</a></li>
    <li><a href="#data-preprocessing">Data Preprocessing</a></li>
    <li><a href="#feature-engineering">Feature Engineering</a></li>
    <li><a href="#models-used">Models Used</a></li>
    <li><a href="#evaluation-metrics">Evaluation Metrics</a></li>
    <li><a href="#results">Results</a></li>
    <li><a href="#conclusion">Conclusion</a></li>
    <li><a href="#future-work">Future Work</a></li>
    <li><a href="#references">References</a></li>
</ol>

<h2 id="introduction">Introduction</h2>
<p>The <strong>Bangalore House Price Prediction</strong> project aims to predict the prices of houses in Bangalore using various regression models. This project involves data preprocessing, feature engineering, model training, evaluation, and comparison to identify the most effective model for predicting house prices.</p>

<h2 id="dataset">Dataset</h2>
<p>The dataset used in this project is sourced from <a href="https://www.kaggle.com">Kaggle</a>: Bengaluru House Price Data. It contains various features such as:</p>
<ul>
    <li>Area type</li>
    <li>Location</li>
    <li>Size</li>
    <li>Total square feet</li>
    <li>Number of bathrooms</li>
    <li>Balcony count</li>
    <li>Price of the house</li>
</ul>

<h2 id="data-preprocessing">Data Preprocessing</h2>
<p>Data preprocessing steps include:</p>
<ul>
    <li><strong>Handling missing values</strong>: Dropping columns with a high percentage of missing data and filling missing values in columns with low percentages.</li>
    <li><strong>Converting categorical features</strong> to numeric using techniques such as one-hot encoding.</li>
    <li><strong>Scaling features</strong> using Min-Max scaling.</li>
    <li><strong>Detecting and removing outliers</strong> using methods like Z-score.</li>
</ul>

<h2 id="feature-engineering">Feature Engineering</h2>
<p>Feature engineering involves:</p>
<ul>
    <li>Converting the 'total_sqft' feature to a numeric format by handling ranges and non-numeric entries.</li>
    <li>Extracting the number of bedrooms (BHK) from the 'size' feature.</li>
    <li>Creating new features to enhance the predictive power of the models.</li>
</ul>

<h2 id="models-used">Models Used</h2>
<p>Seven regression models were used in this project:</p>
<ol>
    <li><strong>Linear Regression</strong>: A basic regression model assuming a linear relationship.</li>
    <li><strong>Lasso Regression</strong>: Uses L1 regularization to prevent overfitting.</li>
    <li><strong>Ridge Regression</strong>: Similar to Lasso but uses L2 regularization.</li>
    <li><strong>Random Forest Regression</strong>: An ensemble model averaging multiple decision trees.</li>
    <li><strong>Gradient Boosting Regression</strong>: Builds trees sequentially to correct errors.</li>
    <li><strong>Support Vector Machine</strong>: Adapts hyperplanes for regression purposes.</li>
    <li><strong>XGBoost</strong>: Optimized gradient boosting for large datasets.</li>
</ol>

<h2 id="evaluation-metrics">Evaluation Metrics</h2>
<p>Performance of the models was evaluated using:</p>
<ul>
    <li><strong>Root Mean Squared Error (RMSE)</strong>: Measures the square root of average squared differences.</li>
    <li><strong>R-squared (R²) Score</strong>: Represents the proportion of variance explained by input features.</li>
</ul>

<h2 id="results">Results</h2>
<p>Model performances on the test set:</p>
<table border="1">
    <tr>
        <th>Model</th>
        <th>RMSE</th>
        <th>R²</th>
    </tr>
    <tr>
        <td>Linear Regression</td>
        <td>64.90</td>
        <td>79.03%</td>
    </tr>
    <tr>
        <td>Lasso Regression</td>
        <td>62.81</td>
        <td>80.36%</td>
    </tr>
    <tr>
        <td>Ridge Regression</td>
        <td>64.86</td>
        <td>79.05%</td>
    </tr>
    <tr>
        <td>Random Forest Regression</td>
        <td>44.20</td>
        <td>90.27%</td>
    </tr>
    <tr>
        <td>Gradient Boosting Regression</td>
        <td>46.92</td>
        <td>89.04%</td>
    </tr>
    <tr>
        <td>Support Vector Machine</td>
        <td>126.27</td>
        <td>20.63%</td>
    </tr>
    <tr>
        <td>XGBoost</td>
        <td>48.87</td>
        <td>88.11%</td>
    </tr>
</table>

<h2 id="conclusion">Conclusion</h2>
<p>The <strong>Random Forest Regression</strong> model provided the best performance, making it the most suitable model for predicting house prices in Bangalore. Ensemble methods outperformed linear models, while Support Vector Machine showed the least predictive power for this dataset.</p>

<h2 id="future-work">Future Work</h2>
<p>Future improvements could include:</p>
<ul>
    <li>Further hyperparameter tuning for all models.</li>
    <li>Exploring other advanced regression techniques.</li>
    <li>Incorporating additional features or external datasets.</li>
    <li>Implementing cross-validation for better robustness.</li>
</ul>

<h2 id="references">References</h2>
<ul>
    <li><a href="https://www.kaggle.com">Kaggle Dataset: Bengaluru House Price Data</a></li>
    <li><a href="https://scikit-learn.org/stable/">Scikit-learn Documentation</a></li>
    <li><a href="https://xgboost.readthedocs.io">XGBoost Documentation</a></li>
</ul>

</body>
</html>
