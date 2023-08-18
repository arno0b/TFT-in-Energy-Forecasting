# Temporal Fusion Transformers in Load Forecasting

A dynamic approach to load forecasting using Temporal Fusion Transformers (TFT). This project showcases the superiority of TFT in load forecasting against models like N-BEATS, NHITS and RNN models using data from PGCB, Bangladesh.

## Table of Contents

1. [Introduction](#introduction)
2. [Setup & Installation](#setup--installation)
3. [Usage](#usage)
4. [Results](#results)
5. [Dataset Source](#dataset-source)
6. [Acknowledgements](#acknowledgements)
7. [License](#license)

## Introduction

Electric load forecasting is a crucial component for efficient energy grid management. With the evolving nature of energy consumption patterns, a dynamic and adaptive forecasting method is paramount. This project employs Temporal Fusion Transformers to understand and adapt to concept drifts in load forecasting.

## Project Structure
```
TFT-in-Energy-Forecasting/
│
├── notebooks/
│ ├── combined tft.ipynb # tft notebook
| ├── combined nhits.ipynb # nhits notebook
| ├── combined nbeats.ipynb # nbeats notebook
| ├── RNN,LSTM.ipynb # RNN,LSTM notebook
| ├── energy EDA nhits.ipynb # Supplementary exploratory analyses
│ └── weather_EDA.ipynb # Supplementary exploratory analyses
│
├── data/
│ ├── raw/ # Raw, unprocessed data files
│ └── processed/ # Cleaned and pre-processed data
│
├── src/
│ └── visualization/ # Visualization scripts
│
├── results/
│ ├── figures/ # Graphs, plots for the final report
│ └── models/ # Trained model files
│
│
├── .gitignore
├── README.md
└── requirements.txt # Required python libraries
```

## Setup & Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/arno0b/TFT-in-Energy-Forecasting.git
   cd TFT-in-Energy-Forecasting

2. **Set Up a Virtual Environment (Recommended)**

    ```bash
    python -m venv env
    source env/bin/activate  # On Windows, use `env\Scripts\activate`
3. **Install Required Libraries**

    ```bash
    pip install -r requirements.txt
    
## Usage

1. **Data Exploration & Model Building**

Navigate to the `notebooks` directory and open the `combined tft.ipynb` in Jupyter Notebook:

      jupyter notebook notebooks/combined tft.ipynb
    
Run the cells sequentially to see the data analysis, model training, and evaluation processes.

2. **Supplementary Analyses**

The notebooks directory also contains other notebooks that delve into evaluations of other models.

## Results
The Temporal Fusion Transformer model achieved superior performance with a Mean Absolute Percentage Error (MAPE) of 1.15%, significantly outperforming other benchmarked models.


## Dataset Source
The dataset utilized in this project is sourced from Power Grid Company of Bangladesh (PGCB) which I scraped using Beautiful soup library. The raw data files, processed datasets used for modeling can be found under the data/raw, data/processed directory.


## Acknowledgements
1. Open-source libraries and frameworks used in the project.

## License
This project is licensed under the MIT License. See the `LICENSE.md` file for details.
