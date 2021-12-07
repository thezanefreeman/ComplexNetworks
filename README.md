# Networks & Dynamics of Political Discussion Python Analysis

During our research, we decided to focus on a politically-charged time. With that being said, we analyzed the months surrounding the 2012 US Presidential Election. Specifially, we analyzed Reddit comment data from September, October, and November. 

## Installation

The notebooks included in this repository rely on the Reddit comment data extracted from the [PushShift Dataset](https://files.pushshift.io/reddit/comments/). Before using the notebooks, please download and unzip the files entitled [RC_2012-09.bz2](https://files.pushshift.io/reddit/comments/RC_2012-09.bz2), [RC_2012-10.bz2](https://files.pushshift.io/reddit/comments/RC_2012-10.bz2), and [RC_2012-10.bz2](https://files.pushshift.io/reddit/comments/RC_2012-11.bz2).


**You must download and unzip the September, November, and December comment files
from  before running any of the notebooks.

## The Notebooks 

Below are detailed descriptions of each notebook present in the repository. 

### PushShift Extract Notebook

This notebook is used as an example on how to extract data using the PushShift API. This served as a spring board that the other notebooks were built upon. If you would like to use the regular python version of the script, please do the following

```bash
python pushshift_extract.py
```

### Subreddit Network Notebook

This notebook creates the subreddit-to-subreddit networks that were described in the paper. 

### Find Political Subreddits Notebook 

This notebook is used to find "political" subreddits within a specific dataset.

### Political Subreddit Network Notebook

This notebook is identical to the Subreddit Network Notebook; however, it creates a network that is only comprised of what we deemed were "political" subreddit.

### Political User Network Notebook

This notebook is used to designate political affiliations or labels to users within a dataset. 

### Extract Data Notebook

This notebook is a helper notebook to extract data easier from locally downloaded comment data from Reddit.

### Analysis Notebook

This notebook analyzes the various subreddit-to-subreddit networks and user reply networks. It plots useful data for visualization such as the degree distribution and rank-size. 

### Create Daily Networks Notebook

This notebook seperates the extracted PushShift comment data into networks for each day in the specified months. For our analysis, we used the months September 2012, October 2012, and November 2012

### Day To Day Analysis Notebook 

This notebook allows us to see how well our political classifications are doing for each day of the month. 

### Infected Notebook 

This notebook aids in running the infection model simulation for political topic spread. 


