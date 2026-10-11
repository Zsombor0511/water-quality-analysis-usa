# Water Quality Analysis – USA

University Python course project (ELTE): exploratory data analysis and machine learning on a US water quality dataset (412 records).

> The notebook itself is written in Hungarian (course assignment), this README is in English.

## What the notebook does

- **Data loading and preprocessing** with pandas: data types, date conversion, missing values, column renaming, descriptive statistics
- **Exploratory data analysis** with Matplotlib and Seaborn: nitrogen and phosphorus distributions (histograms with KDE), geographic scatter plots, frequency chart of sewage system states, Pearson correlation heatmap
- **Interactive map** with Folium: phosphorus levels shown as colour-coded markers at the GPS coordinates
- **Feature engineering:** total pollution (N+P), quality categories with `apply()`, group sizes with `groupby()`, categorical encoding with `LabelEncoder`
- **Decision Tree classifier** (scikit-learn) predicting the state of the sewage system: 80/20 train-test split, tree visualization, accuracy, classification report, confusion matrix
- **Linear Regression** relating population to pollution level (R² ≈ 0.92)

## How to run

1. Make sure `data.csv` is in the same folder as the notebook (it is included in this repository)
2. Install the dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Start Jupyter and open the notebook:
   ```
   jupyter notebook water_quality_usa.ipynb
   ```

## Tech

Python, pandas, NumPy, Matplotlib, Seaborn, Folium, scikit-learn, Jupyter

## Data

`data.csv` (412 records, provided in the course) contains water quality measurements with these columns: latitude and longitude, state of the sewage system, sampling date, nitrogen (mg/L), phosphorus (mg/L) and population.
