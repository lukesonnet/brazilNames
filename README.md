# Brazilian Politician's Names and Sex

This repository contains the raw data from the Brazilian Electoral Tribunal's website [here](http://www.tse.jus.br/hotSites/pesquisas-eleitorais/candidatos.html). Using this raw data, I build a data set with a list of ~74,000 Brazilian first names and how often each name is used for a male or female candidates in the 2000, 2004, 2008, and 2012 municipal elections in Brazil. Thus it effectively works as a tool to classify the gender of any Brazilian (and perhaps Portuguese) name.

In total, there are 1,653,604 candidates that ran in municipal elections from 2000-2012 and the gender of 1,652,685 of those candidates was reported in the official data. I take the first characters in the reported names that precede a space and designate that as the candidate's first name. This yielded 74,650 unique first names which make up this dataset. I then record the gender of each candidate and sum how many men and women were associated with each unique first name. There are errors in the names from the source dataset and there are probably errors in the reported gender as well. However, if you are matching names from your own dataset that does NOT have errors in the name, the dataset I provide here should work fairly well to predict the gender of those in your dataset.

## To do

- Expand data source
- Cleanly document workflow in README.md
