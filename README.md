# Sight and Sound 2012 Poll Notebooks
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dn480000/sight-and-sound-notebooks/master)

The project lets you easily scrape Sight and Sound 2012 Poll and recommed films using Personalized PageRank with Jupyter notebooks. 

You should first use `scrape.ipynb` to scape the poll data and save it in `/data`. You can use `recommend.ipynb` to study some basic characteristics of the votes data and then apply an implemtation of Personalized PageRank.

## Run Jupyter Notebooks
You can run the notebooks in your browser with [binder](https://mybinder.org/v2/gh/dn480000/sight-and-sound-notebooks/master). 


You can also install Jupyter Notebook with Conda and run the notebooks locally.

[Guide to install Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)

[Guide to install Jupyter Notebook](https://jupyter.org/install)

You can run the notebooks locally with the terminal command `jupyter notebook` in the project directory.

## Scraped Data
After the you run `scrape.ipynb`, the data are saved as JSON files in `/data` by default. The films are saved as an array of film objects of name, year (possibly null), director, country and url (possibly null). The voters are saved in VOTERS_PATH as an array of voter objects of name, role, country, gender and url. The votes are saved in VOTES_PATH as an array of pairs of voter index and film index. Each pair denotes a vote. The comments are saved in COMMENTS_PATH as an array of strings, in the same order as the voters. If a voter does not provide a comment, an empty string is saved.