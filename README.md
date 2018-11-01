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
- numpy: https://docs.scipy.org/doc/numpy-1.15.1/reference/
- pandas: https://pandas.pydata.org
- scikit-learn: http://scikit-learn.org/stable/
  * The code in this report will use scikit-learn's `KMeans()` class to perform clustering on countries by data (see notebook for explanation). (http://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)
- requests: http://docs.python-requests.org/en/master/
- json: https://docs.python.org/3/library/json.html
- csv: https://docs.python.org/3/library/csv.html

## Files Created
This notebook creates CSV files of data extracted and compiled as part of this analysis.

1. `page_data.csv`: Data from data source (1) comprising of articles about politicians, their article "revision_ids" and associated country. 
2. `WPDS_2018_data.csv`: Data from source (2) comprising of population data for each country
3. `predictions_data.csv`: This file is generated in the Jupyter notebook. It consists of (revision/article ID, ORES prediction) pairs, obtained from the ORES API calls. It is saved here for convenience of not having to recreate it. 
4 `master_data.csv`: This file is the master data file as required by the assignment. It is a table with schema: 
  - *(article-name,	  country	rev_id,  	prediction,	  Country,	  population)* 
             

## Code

Code and Python project contained in the jupyter notebook `hcds-512-a2.ipynb`

## Visualizations Created

As requested by the assignment, 4 visualizations are created, along with two others used in the analysis section. These are tables consisting of countries ranked by the "article-percentage" and "good-article-percentage" fields (see Jupyter Notebook/assignment link). 

In addition, two analogous tables are created for the statistical analysis section on bias. 

All tables were saved to .png files, and can be found in this repository. 

## License

This assignment code is released under an MIT License. 

The data sources are licensed under a CC-BY-SA 4.0 license. 
