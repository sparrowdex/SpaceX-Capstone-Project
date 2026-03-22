# SpaceX Falcon 9 First Stage Landing Prediction

This project analyzes SpaceX Falcon 9 launch data to predict whether the first stage will land successfully. The project includes data collection, data wrangling, exploratory data analysis, interactive visualizations, and the development of a machine learning model to predict landing outcomes.

## Project Structure

- **`data/`**: Contains the datasets used in this project, including data collected from the SpaceX API and web scraping.
- **`notebooks/`**: Contains Jupyter notebooks detailing the entire process from data collection to predictive analysis.
- **`images/`**: Contains images generated from the EDA and mapping notebooks.
- **`presentations/`**: Intended for project presentations (currently empty).
- **`spacex-dash-app.py`**: A Plotly Dash application for interactively exploring the launch data.
- **`requirements.txt`**: Lists the Python dependencies for this project.

## Data Sources

The data for this project was collected from two main sources:
1.  **SpaceX API**: For detailed information about past launches.
2.  **Wikipedia**: For a comprehensive list of Falcon 9 and Falcon Heavy launches.

## Methodology

The project is divided into several stages:

1.  **Data Collection**: Data is collected from the SpaceX API and by scraping a Wikipedia page.
2.  **Data Wrangling**: The collected data is cleaned, processed, and prepared for analysis.
3.  **Exploratory Data Analysis (EDA)**: EDA is performed using SQL queries and data visualization libraries like `matplotlib` and `seaborn`.
4.  **Interactive Visual Analytics**: Interactive maps are created using `folium`, and an interactive dashboard is built with `plotly-dash`.
5.  **Predictive Analysis**: A machine learning pipeline is built to predict landing success. Several classification models are trained and evaluated, with the best-performing model being identified.

## Installation

To run this project, you need to have Python installed. You can then install the required dependencies using pip:

```bash
pip install -r requirements.txt
```

If the `requirements.txt` file is not populated, you can install the necessary libraries manually:

```bash
pip install pandas numpy requests beautifulsoup4 folium plotly dash scikit-learn seaborn matplotlib
```

## Usage

### Jupyter Notebooks

The notebooks in the `notebooks/` directory should be run in the following order:

1.  `Data_Collection.ipynb`
2.  `Webscraping.ipynb`
3.  `Data_Wrangling.ipynb`
4.  `EDA_with_SQL.ipynb`
5.  `Data_Visualization_EDA.ipynb`
6.  `Interactive_Maps_with_Folium.ipynb`
7.  `Predictive_Analysis.ipynb`

### Interactive Dashboard

To run the interactive dashboard, execute the following command in your terminal:

```bash
python spacex-dash-app.py
```

This will start a local web server, and you can access the dashboard by navigating to the URL provided in the terminal (usually `http://127.0.0.1:8050/`).

## Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
- BeautifulSoup
- Plotly Dash
- Folium
- Matplotlib
- Seaborn

## Results

The predictive analysis showed that it is possible to predict the landing success of the Falcon 9 first stage with a good degree of accuracy. The **Logistic Regression** model was found to be the best-performing model on the test data.
