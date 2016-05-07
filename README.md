# Brazilian Politician's Names and Sex

This repository contains the raw data from the Brazilian Electoral Tribunal's website [here](http://www.tse.jus.br/hotSites/pesquisas-eleitorais/candidatos.html). Using this raw data, I build a data set with a list of ~76,500 Brazilian first names and how often each name is used for a male or female candidates in the 2000, 2004, 2008, and 2012 municipal elections in Brazil. Thus it effectively works as a tool to classify the gender of any Brazilian (and perhaps Portuguese) name.

In total, there are 1,758,134 candidates that ran in municipal and state elections from 1998-2014 and the sex of 1,652,685 of those candidates was reported in the official data. I take the first characters in the reported names that precede a space and designate that as the candidate's first name. This yielded 76,597 unique first names which make up this dataset. I then record the sex of each candidate and sum how many males and females were associated with each unique first name. There are errors in the names from the source dataset and there are probably errors in the reported sex as well. However, if you are matching names from your own dataset that does NOT have errors in the name, the dataset I provide here should work fairly well to predict the sex of those in your dataset.

## Important Caveats

- The data have not been cleaned thoroughly. If there were typos or errors in the original data uploaded by the Brazilian TSE then those errors carry forward in to this dataset with a few exceptions (leading punctuation has been removed)
- Candidates that have run more than once may be repeated in this dataset. Future work could only use one name per individual, but this may be more work than it is worth.
- Accents are maintained in their original encoding, which was ISO-8859-1.
- Due to disparities in which

## To do

- Expand data source
- Cleanly document workflow in README.md
