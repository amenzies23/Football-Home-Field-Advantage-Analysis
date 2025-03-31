# CMPT353-FinalProject
Final Project for the MoneyBall Group for SFU's FALL 2024 CMPT 353 class

This was a group project with two other students, but our work was independent of each other. So the work in this repository was fully completed by myself.
## Project Structure (to be updated)
```bash
repository
├── performanceData
│   ├── EPL_2015_matchsheets.csv
│   ├── ...
├── performancePlots
│   ├── boxPlots
│   ├── histograms
│   ├── scatterplots
│   ├── stackedBarPlots
├── analysePerformance.py
├── gatherPerformanceData.ipynb
```

## Libraries required


soccerdata

pandas

numpy

scipy

matplotlib

seaborn

If any of these librarys are not yet installed:
```bash
pip install <library>
```

## Performance Metrics

### `gatherPerformanceData.ipynb`
Uses the library SoccerData to scrape data from ESPN to obtain information about each match for a specified league and season.

### `analysePerformanceData.py`
Program to analyse all metrics gathered from gatherPerformanceData.ipynb. It will first take in a directory of csv files containing match data across a season for a specified league. It will append all csv files into one dataframe, and performance a statistical analysis and plot diagrams for each metric in the dataframe. The statistical tests used will be either a T-Test, or Mann-Whitney U-Test based on if the data passes the conditions for a regular T-Test. All results will be visualized in corresponding hstograms, satterplots, bxplots, and stacked bar plots.

## Running the analysis function
```bash
python3 performance/analysePerformance.py performance/performanceData
```
Inside `analysePerformance.py`, the function calls for generating the plots are currently commented out since the plots exist in the corresponding plots folder already. 
