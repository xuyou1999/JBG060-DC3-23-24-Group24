
# Code Description and Execution Order
This repository, forked from the course JBG060, features a range of computational notebooks and scripts focused on data analysis and modeling. The primary components include topic modeling, IPC estimation, data merging, and time-series forecasting. The sequence of execution for these notebooks is as follows:
1. `topic_discovery.ipynb` - Topic discovery using BERTopic and GPT API.
2. `Ida_model.ipynb`
3. `IPC estimation.ipynb` - Interpolation of IPC data.
4. `merge_article_food.ipynb` - Merging datasets geospatially.
5. `Time-series.ipynb` - Time-series forecasting.

## Detailed Workflow
### Topic Modeling
- `topic_discovery.ipynb`: Analyzes the relativity of topics to articles using BERTopic and GPT API. Results are stored in the `data` folder. Note: API key is hidden for security reasons, and you will need your own to replicate the process.

### Geodata Information
- New geodata is derived using `conties_and_regions_for_articles.ipynb`, `counties_and_regions_for_food_crises_clean.ipynb`, and `regions_for_articles.ipynb`, located in the `geodata` folder.
- Utilizes `ss_county_boundaries.geojson` for South Sudan's geopolitical information.
- The outputs, including new district information, are stored in `geodata/results`.

### IPC Estimation and Data Integration
- `IPC estimation.ipynb`: Performs IPC interpolation.
- `merge_article_food.ipynb`: Merges the topic modeling and IPC interpolation datasets geospatially into "food_crises_interpol_news.csv".

### Time-Series Forecasting
- `Time-series.ipynb`: Utilizes the merged data for forecasting.

## Requirements and Troubleshooting
- Python version: 3.9.16.
- Required libraries: bertopic (0.15.0), pandas (1.4.4), geopandas (0.13.2), matplotlib (3.7.2), seaborn (0.12.2), statsmodels (0.14.0).
- Installation: Run `pip install -r requirements.txt` in Terminal (macOS)/Command Prompt (Windows). PyCharm users will see an installation prompt in a new environment.
- Troubleshooting:
  - Ensure all necessary libraries are installed and are the correct versions.
  - Check the Python version. If issues persist, create a virtual environment with Python 3.9.16.
