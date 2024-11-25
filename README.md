# PCA Analysis and Data Transformation

This repository contains Jupyter notebooks and data files for performing PCA (Principal Component Analysis) and data transformation. The main components of this repository are:

- `ACP_VIz.ipynb`: A notebook for performing PCA analysis and visualizing the results.
- `Transform_Data.ipynb`: A notebook for transforming the data to match target statistics.
- `data/`: A directory containing the data files used in the analysis.

## Repository Structure

```plaintext
ACP_VIz.ipynb
data/
preprocessed_data/
ACP Data.csv
Indicators.csv
transformed_data.csv
README.md
Transform_Data.ipynb
```

## Notebooks

### `ACP_VIz.ipynb`

This notebook performs PCA analysis on the transformed data and visualizes the results. The steps include:

1. Loading and exploring the data.
2. Calculating statistical indicators.
3. Computing the correlation matrix.
4. Performing PCA computation.
5. Selecting two principal axes.
6. Creating an individuals table.
7. Plotting the correlation circle.
8. Analyzing the correlation between variables and principal components.

### `Transform_Data.ipynb`

This notebook transforms the data to match target statistics. The steps include:

1. Loading the original data and target statistics.
2. Transforming each variable to match the target statistics.
3. Ensuring the transformed data matches new ranges by capping to min/max values.
4. Exporting the transformed data to a CSV file.

## Data

The `data/` directory contains the following files:

- `preprocessed_data/ACP Data.csv`: The original data file used for PCA analysis.
- `preprocessed_data/Indicators.csv`: The file containing statistical indicators.
- `transformed_data.csv`: The transformed data file used in the PCA analysis.

## Usage

1. Open `Transform_Data.ipynb` and run all cells to transform the data and save it to `data/transformed_data.csv`.
2. Open `ACP_VIz.ipynb` and run all cells to perform PCA analysis and visualize the results.

## Requirements

- Python 3.x
- Jupyter Notebook
- pandas
- seaborn
- matplotlib
- scikit-learn

## Installation

To install the required packages, run:

```sh
pip install pandas seaborn matplotlib scikit-learn
```
