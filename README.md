# Sports Viewership Time Series Analysis

## Project Overview
This project analyzes the impact of COVID-19 on the viewership of major American sports leagues (NFL, NBA, MLB, NHL) using double exponential smoothing. We aim to understand how viewership trends have evolved post-pandemic and whether each league has returned to pre-pandemic levels.

## Software and Platform

### Software:
- **Python 3.x**: Used for data analysis and model implementation.
- **Pandas**: For data manipulation.
- **Numpy**: For numerical computations.
- **Matplotlib**/**Seaborn**: For creating visualizations.
- **Statsmodels**: To implement the double exponential smoothing model.
- **Jupyter Notebook**: For running and documenting the analysis.

### Platform:
- The project was developed and run on **MacOS** but should be compatible with **Windows** and **Linux** systems as well.

## Folder Structure
```plaintext
├── README.md               # This file
├── LICENSE.md              # License file (MIT License)
├── SCRIPTS/                # Contains all the Python scripts
│   ├── data_preprocessing.py    # Script for data cleaning and preprocessing
│   ├── model_implementation.py  # Script for fitting the double exponential smoothing model
│   └── evaluation.py            # Script for evaluating the model performance
├── DATA/                   # Contains datasets used in the project
│   ├── viewership_data.csv      # The main dataset with sports viewership data (1990-2024)
│   └── processed_data.csv       # Cleaned and processed data ready for analysis
├── OUTPUT/                 # Contains output figures and tables generated by the project
│   ├── viewership_trends.png    # Visualization of viewership trends pre- and post-COVID
│   └── model_evaluation.txt     # Performance evaluation metrics (MSE, R-squared)
└── DATA_APPENDIX.pdf       # Document explaining each dataset and variable used
```
## Instructions for Reproducing Results

1. **Clone the repository**:
   ```bash
   git clone https://github.com/bwillow1222/ds4003MI3P2.git
   cd project
2. **Install the required packages**
   ```bash
   pip install -r requirements.txt
3. **Run data preprocessing**
   ```bash
   python SCRIPTS/data_preprocessing.py
4. **Model implementation**
   ```bash
   python SCRIPTS/model_implementation.py
5. **Evaluation**
   ```bash
   python SCRIPTS/evaluation.py
6. **Check the results:**
   View the visualizations and performance metrics in the `OUTPUT/` folder.