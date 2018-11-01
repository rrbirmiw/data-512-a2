# Bias in Data
*Template for this README comes from https://github.com/Ironholds/data-512-a2* 
Name: Rahul Birmiwal 

Date: 11/1/18

## Goal
An exploratory data analysis of Wikipedia page data, seeking to determine if bias exists in Wikipedia page data about political leaders from all countries on earth. Such articles are scored (i.e. if an article is "featured" or "good," or not) using the Wikipedia ORES machine-learning service, Using a combination of those scores, and country population data, this project uses a quantitative measure of "good-article-percentages" as the "bias-proxy." A Jupyter Notebook and associated Python code walks through the procedures to create the analysis. 

The assignment description comes from https://wiki.communitydata.cc/Human_Centered_Data_Science_(Fall_2018)/Assignments#A2:_Data_curation

## Data sources used

Three main sources of data: 
1. Wikipedia Page Data: https://figshare.com/articles/Untitled_Item/5513449. Released under a CC-BY-SA 4.0 license.
2. Population Data: https://www.dropbox.com/s/5u7sy1xt7g0oi2c/WPDS_2018_data.csv?dl=0. Author of this population data is unknown at the time of this writing. 
3. ORES Data: The ORES data is accessed through the ORES API and pulled via the standard Python `requests` library. Information about ORES can be found here: https://www.mediawiki.org/wiki/ORES#API_usage

## Resources used
This analysis was prepared using Python 3.5 running in a Jupyter Notebook environment.  
Documentation for Python can be found here: https://docs.python.org/3.5/  
Documentation for Jupyter Notebook can be found here: http://jupyter-notebook.readthedocs.io/en/latest/  

## Dependencies: 
Following Python library dependencies are required to run the notebook: 
- numpy 
- pandas 
- scikit-learn
- requests
- json 
- csv

## Files Created
This notebook creates  CSV files of data extracted and compiled as part of this analysis.

The first file...

The Nth file...

## Visualizations Created

## License

This assignment code is released under...

The data sources are licensed under...
