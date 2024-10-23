# Sports Viewership Time Series Analysis

## Project Overview
This project analyzes the impact of COVID-19 on the viewership of major American sports leagues (NFL, NBA, MLB, NHL) using double exponential smoothing. We aim to understand how viewership trends have evolved post-pandemic and whether each league has returned to pre-pandemic levels.

## Software and Platform

### Software:
- **Python 3.8 or higher**

### Required Packages
- **Pandas**: For data manipulation.
- **Numpy**: For numerical computations.
- **Matplotlib**/**Seaborn**: For creating visualizations.
- **Statsmodels**: To implement the double exponential smoothing model.
- **Jupyter Notebook**: For running and documenting the analysis.

### Platform:
- The project was developed and run on **MacOS** but should be compatible with **Windows** and **Linux** systems as well.

## Map of Repository Structure
```plaintext
├── README.md               # This file
├── LICENSE.md              # License file (MIT License)
├── SCRIPTS/                # Contains all the Python scripts
│   ├── DataVisualizations.ipynb    # Script for data frequencies, distributions, and statistics
│   ├── Preprocess.ipynb            # Script for data cleaning and preprocessing
│   ├── ResidualsPlot.ipynb            # Script for creating the double exponential smoothing residuals plot
│   ├── ViewershipModeling.ipynb    # Script for fitting the double exponential smoothing model
├── DATA/                   # Contains datasets used in the project
│   ├── NFL.csv      # Imported NFL championship viewership data
│   ├── NBA.csv      # Imported NBA championship viewership data
│   ├── MLB.csv      # Imported MLB championship viewership data
│   ├── NHL.csv      # Imported NHL championship viewership data
│   └── Data_Appendix.pdf       # Document explaining each dataset and variable used
├── OUTPUT/                 # Contains output figures and tables generated by the project
│   ├── csv/
│   │   ├── nfl_viewership_forecast_vs_actual.csv    # Table output comparing NFL forecast to measured for post-COVID
│   │   ├── nba_viewership_forecast_vs_actual.csv    # Table output comparing NBA forecast to measured for post-COVID
│   │   ├── mlb_viewership_forecast_vs_actual.csv    # Table output comparing MLB forecast to measured for post-COVID
│   │   ├── nhl_viewership_forecast_vs_actual.csv    # Table output comparing NHL forecast to measured for post-COVID
│   ├── visualizations     # Performance evaluation metrics (MSE, R-squared)
│   │   ├── NFLplot.png      # Plotted NFL championship data with model and forecast
│   │   ├── NBAplot.png      # Plotted NBA championship data with model and forecast
│   │   ├── MLBplot.png      # Plotted MLB championship data with model and forecast
│   │   ├── NHLplot.png      # Plotted NHL championship data with model and forecast
│   │   ├── residualPlot.png       # Residual plot between actual and forecasted viewership
│   │   ├── sportsViewership.png   # Histograms of viewership across sports
└──  -  └── yearFrequency.png      # Stacked bar chart of entries per year by sport

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
   python SCRIPTS/Preprocess.ipynb
4. **Model implementation**
   ```bash
   python SCRIPTS/ViewershipModeling.ipynb
5. **Check the results:**
   View the visualizations and performance metrics in the `OUTPUT/` folder.
