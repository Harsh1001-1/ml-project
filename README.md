# Uber Fare Analysis

A Jupyter Notebook project that explores Uber trip data, analyses fare and passenger patterns, visualises pickup and drop-off locations, and calculates trip distances as a feature for fare prediction experiments.

## What the notebook does

- Loads and explores an Uber trip dataset
- Extracts day, hour, day of week, month, and year from `pickup_datetime`
- Checks summary statistics and missing values
- Visualises fare amounts, passenger counts, trip-distance distribution, and drop-off locations
- Calculates trip distance from pickup and drop-off coordinates using the Haversine formula
- Creates an interactive pickup-location map with Folium
- Includes a prototype workflow for splitting data and experimenting with a prediction model

## Project file

| File | Description |
| --- | --- |
| `MLproject.ipynb` | Main Jupyter Notebook containing data analysis, visualisations, and modelling experiments |

## Requirements

- Python 3.9 or later
- Jupyter Notebook or VS Code with the Jupyter extension
- An Uber trip dataset CSV containing fields such as `pickup_datetime`, `pickup_latitude`, `pickup_longitude`, `dropoff_latitude`, `dropoff_longitude`, `passenger_count`, and `fare_amount`

Install the Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn folium jupyter
```

## How to run

1. Clone this repository:

   ```bash
   git clone https://github.com/Harsh1001-1/ml-project.git
   cd ml-project
   ```

2. Download the Uber trip CSV dataset and save it on your computer.

3. Open `MLproject.ipynb` in Jupyter Notebook or VS Code.

4. Update the `pd.read_csv(...)` paths in the notebook so they point to your downloaded CSV file.

5. Run the notebook cells from top to bottom.

## Dataset

The dataset itself is not included in this repository. Ensure your CSV includes the columns required by the notebook before running it.

## Output

The notebook produces descriptive statistics, plots of fares and passengers, geographic scatter plots, an interactive pickup-location map, and distance-based feature calculations for further fare-prediction work.
