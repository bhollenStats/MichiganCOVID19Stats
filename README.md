# MichiganCOVID19Stats

This is an R Markdown project that will scrape that will scrape the current daily 
reported cases of COVID-19 from http://michigan.gov/coronavirus and add them to 
a growing data frame of data stored in the project named dfCOVID19MichiganTotals.Rdata.

Three libraries are required for this project: rvest, tidyverse, and knitr.

There is currently one parameter in the markdown code that can be used to determine
if the execution should merge the new daily data with the accumulated data so far.
The parameter is named 'mergeToday' and is set to zero (0) by default to not 
add the new data to the accumulated data. A value greater than one will append
the newly collected data with the existing data accumulated before writing the 
total data back to the filesystem.

The current list of observations is also available in the file named 
'michigan_covid19_cases.csv'.
