
<h1>Seattle House Prices Analysis</h1>
<p>This repository contains the analysis and visualization of the King County house sales dataset. The aim is to clean the data, perform exploratory data analysis (EDA), and derive insights from the dataset.</p>

<h2>Table of Contents</h2>
<ul>
    <li><a href="#overview">Overview</a></li>
    <li><a href="#dataset">Dataset</a></li>
    <li><a href="#data-cleaning">Data Cleaning</a></li>
    <li><a href="#exploratory-data-analysis">Exploratory Data Analysis</a></li>
    <li><a href="#visualizations">Visualizations</a></li>
    <li><a href="#dependencies">Dependencies</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#results">Results</a></li>
    <li><a href="#license">License</a></li>
</ul>

<h2 id="overview">Overview</h2>
<p>This project involves analyzing house prices in King County, which includes Seattle. The analysis covers various aspects such as identifying duplicate entries, handling missing values, identifying and removing outliers, and visualizing important features affecting house prices.</p>

<h2 id="dataset">Dataset</h2>
<p>The dataset used is <code>kc_house_data.csv</code>, which includes the following columns:</p>
<ul>
    <li><b>id</b>: Unique identifier for a house</li>
    <li><b>date</b>: Date of the house sale</li>
    <li><b>price</b>: Price of the house</li>
    <li><b>bedrooms</b>: Number of bedrooms</li>
    <li><b>bathrooms</b>: Number of bathrooms</li>
    <li><b>sqft_living</b>: Square footage of the living space</li>
    <li><b>sqft_lot</b>: Square footage of the lot</li>
    <li><b>floors</b>: Number of floors</li>
    <li><b>waterfront</b>: Binary indicator for waterfront property</li>
    <li><b>view</b>: Quality of the view</li>
    <li><b>condition</b>: Condition of the house</li>
    <li><b>grade</b>: Overall grade of the house based on King County grading system</li>
    <li><b>sqft_basement</b>: Square footage of the basement</li>
    <li><b>lat</b>: Latitude coordinate</li>
    <li><b>long</b>: Longitude coordinate</li>
    <li><b>sqft_living15</b>: Square footage of living space in 2015</li>
    <li><b>sqft_lot15</b>: Square footage of the lot in 2015</li>
</ul>

<h2 id="data-cleaning">Data Cleaning</h2>
<h3>Removing Duplicates</h3>
<ul>
    <li>Identified and removed duplicate entries based on the <code>id</code> column.</li>
    <li>Retained entries with the latest valuation date and highest price for duplicates.</li>
</ul>

<h3>Handling Missing Values</h3>
<ul>
    <li>Checked for and addressed missing values in the dataset.</li>
</ul>

<h3>Removing Outliers</h3>
<ul>
    <li>Used Interquartile Range (IQR) to identify and remove outliers in <code>price</code>, <code>bedrooms</code>, <code>bathrooms</code>, <code>sqft_living</code>, and <code>sqft_living15</code>.</li>
</ul>

<h2 id="exploratory-data-analysis">Exploratory Data Analysis</h2>
<p>Performed various analyses to understand the distribution and relationships between different features:</p>
<h3>Box Plots</h3>
<ul>
    <li>Generated box plots for numerical columns to identify outliers and understand data distribution.</li>
</ul>

<h3>Scatter Plots</h3>
<ul>
    <li>Created scatter plots to visualize relationships between features like <code>sqft_living</code>, <code>floors</code>, <code>bedrooms</code>, and <code>bathrooms</code>.</li>
</ul>

<h3>Correlation Analysis</h3>
<ul>
    <li>Computed and visualized the correlation matrix to identify significant features affecting the house prices.</li>
</ul>

<h3>Yearly Valuation Analysis</h3>
<ul>
    <li>Analyzed properties valued in 2014 and 2015, identifying properties with price changes.</li>
</ul>

<h2 id="visualizations">Visualizations</h2>
<h3>Box Plot Comparisons</h3>
<ul>
    <li>Comparison of initial and subsequent valuations for properties.</li>
</ul>

<h3>Heatmap</h3>
<ul>
    <li>Heatmap to visualize the density of high and low-priced properties based on their geographical coordinates.</li>
</ul>

<h3>Distribution Plots</h3>
<ul>
    <li>Distribution of prices, grades, and views for high and low-priced properties.</li>
</ul>

<h2 id="dependencies">Dependencies</h2>
<p>The project requires the following Python libraries:</p>
<ul>
    <li>pandas</li>
    <li>numpy</li>
    <li>matplotlib</li>
    <li>seaborn</li>
    <li>folium</li>
    <li>scikit-learn</li>
</ul>

<h2 id="usage">Usage</h2>
<ol>
    <li>Clone the repository:
        <pre><code>git clone https://github.com/sailikhitha07/House_Price_Prediction_and_EDA.git
cd House_Price_Prediction_and_EDA</code></pre>
    </li>
    <li>Install the required dependencies:
        <pre><code>pip install -r requirements.txt</code></pre>
    </li>
    <li>Run the analysis:
        <p>Open the Jupyter notebook <code>House_Price_Prediction.ipynb</code> and run the cells to execute the analysis step-by-step.</p>
    </li>
</ol>

<h2 id="results">Results</h2>
<p>Key findings from the analysis:</p>
<h3>Duplicate Handling</h3>
<ul>
    <li>Successfully identified and handled duplicate entries.</li>
</ul>

<h3>Outlier Removal</h3>
<ul>
    <li>Removed significant outliers to improve data quality.</li>
</ul>

<h3>Correlation Analysis</h3>
<ul>
    <li>Identified significant features influencing house prices such as <code>sqft_living</code>, <code>grade</code>, and <code>bathrooms</code>.</li>
</ul>

<h3>Price Distribution</h3>
<ul>
    <li>Visualized the distribution of house prices and other related features.</li>
</ul>

<h3>Geospatial Analysis</h3>
<ul>
    <li>Heatmap visualization of high and low-priced properties.</li>
</ul>

<h2 id="license">License</h2>
<p>This project is licensed under the MIT License. Please feel free to use, modify, and distribute it according to the terms of the license.</p>
