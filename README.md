# Death Row Project
## Background, Purpose and Methodology
The Texas Department of Justice has published a dataset (mixed dataset with both continuous and categorical variables) consisting of all executed prisoners within Texas (https://www.tdcj.texas.gov/death_row/dr_executed_offenders.html). The purpose of this project is to explore this dataset and more specifically answer the following Reasearch Questions:

- Which are the main segments wihin all executed prisoners and which characteristics do these group have?
- Who are the most extreme prisoners that stick out from the rest?
- General insights through EDA.

## Methodology

- EDA: Various visualization methods inicluding Wordcloud and seaborn plots.
- Clustering: KMeans (only continuous features), KPrototypes (All features, including categorical) and Agglomerative Clustering.
- Outlier Detection: By calculating the gower distances from the KPrototypes cluster centroids.
- Dimensionality Reduction (for visualization of clusters): Reducing dimensionality from 11 to 2 with clustering and gower distances.

## How was the data acquired?
The Data was acquired through a web scraper that scraped all profiles on the webpage outlined above. Many of the profiles were in a scanned format (scanned papers) and could not be read by the scraper; these data points were tagged through a feature named "is_scanned".

## View the project nbviewer
https://nbviewer.jupyter.org/github/Kayaae/Death-Row-Project/blob/master/Deathrow.ipynb
