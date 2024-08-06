# Titanic Data Analysis

This repository contains a Python script for analyzing the Titanic dataset. The script performs data cleaning, exploratory data analysis, and visualizations. It demonstrates basic data manipulation techniques and provides insights into the dataset.

## Features

- **Data Cleaning**: Handles missing values, converts categorical variables to numerical values, and removes unnecessary columns.
- **Exploratory Data Analysis (EDA)**: Includes summary statistics and basic statistics about the dataset.
- **Visualizations**: Generates plots to visualize the distribution of ages, survival rates by sex, and survival rates by embarkation port.
- **File Output**: Saves the cleaned dataset and visualizations to files.

## Requirements

- Python 3.x
- pandas
- matplotlib
- seaborn
- kaggle

## Installation

1. Install the necessary Python packages:

    ```bash
    pip install pandas matplotlib seaborn kaggle
    ```

2. Upload your `kaggle.json` file to the Colab environment.

## Usage

1. **Install Kaggle API and Download the Dataset**:
    ```python
    !pip install kaggle

    import os
    os.makedirs('/root/.kaggle', exist_ok=True)
    !mv kaggle.json /root/.kaggle/
    !chmod 600 /root/.kaggle/kaggle.json

    !kaggle competitions download -c titanic -f train.csv
    !unzip train.csv.zip
    ```

2. **Run the Analysis Script**:
    Save the script as `analyse_train.py` and run it to perform the analysis:

    ```bash
    python analyse_train.py
    ```

3. **Check Output**:
    - The cleaned data will be saved to `analyzed_train.csv`.
    - Plots will be saved as `age_distribution.png`, `survival_rate_by_sex.png`, and `survival_rate_by_embarked.png`.

## Script Details

The `analyse_train.py` script performs the following steps:
1. **Load the Dataset**: Reads the Titanic dataset from a CSV file.
2. **Clean the Dataset**: Handles missing values, converts categorical variables, and drops unnecessary columns.
3. **Save Cleaned Data**: Outputs the cleaned dataset to `analyzed_train.csv`.
4. **Analyze and Visualize**: Generates and saves visualizations to understand the distribution and survival rates.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Kaggle for providing the Titanic dataset.
- Python libraries such as pandas, matplotlib, and seaborn for data manipulation and visualization.

