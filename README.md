# Repository forked from the course JBG060 

## Code description
The work done includes (INSERT TOPIC MODELLING PARTS), and the interpolation of IPC ("IPC estimation.ipynb"). The topic modelling and IPC interpolation each generate a data set, merged geospatially ("merge_article_food.ipynb") into "food_crises_interpol_news.csv". This data is then used for time-series forecasting ("Time-series.ipynb").

## Order of code execution
1) "topic_discovery.ipynb"
2) "Ida_model.ipynb"
3) "IPC estimation.ipynb"
4) "merge_article_food.ipynb"
5) "Time-series.ipynb"

## Requirements and troubleshooting
To install the requirements open Terminal (macOS)/Command Prompt (Windows) and run pip install -r requirements.txt. If you create a new environment in PyCharm, an icon should appear to install requirements. The code runs with Python 3.9.16.

Required libraries:
- bertopic == 0.15.0 
- pandas == 1.4.4 
- geopandas == 0.13.2 
- matplotlib == 3.7.2 
- seaborn == 0.12.2
- statsmodels == 0.14.0 

If you encounter any issues while running the notebooks, try the following:
- check that you have all the necessary libraries installed and the correct versions of them
- check your Python version. In principle, the code should work with any Python versions higher than 3.9.16. If this is not the case, create a virtual environment that uses Python 3.9.16.
