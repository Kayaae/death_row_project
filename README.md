# Death Row Project
## Background and Purpose
The Texas Department of Justice has published a dataset (mixed dataset with both continuous and categorical variables) consisting of all executed prisoners within Texas (https://www.tdcj.texas.gov/death_row/dr_executed_offenders.html). The purpose of this project is to explore this dataset and more specifically answer the following Reasearch Questions:

- Which are the main segments wihin all executed prisoners and which characteristics do these group have?
- Which are the most extreme prisoners that stick out from the rest?
- General insights through EDA.

## Methodology

- EDA: Various visualization methods including Wordcloud and Seaborn plots.
- Clustering: KMeans (only continuous features), KPrototypes (All features, including categorical) and Agglomerative Clustering.
- Outlier Detection: By using the Gower distances from the KPrototypes cluster centroids.
- Dimensionality Reduction (for cluster visualizations): Reducing dimensionality from 11 to 2 with clustering and gower distances.

## How was the data acquired?
The data was acquired through a web scraper that scraped all profiles on the webpage outlined above. Many of the profiles were in a scanned format (scanned papers) and could not be read by the scraper; these data points were tagged through a feature named "is_scanned".

## View the project in nbviewer
https://nbviewer.jupyter.org/github/Kayaae/Death-Row-Project/blob/master/Deathrow.ipynb
