# MLBHackathon
repo for Cristian Gamboa's MLBHackathon project

# Files description
report.pdf is the main report of for the analysis.
2015MLBPitcherlist.csv stores the results from the tests for every pitcher studied.
NLPitchers/2015 and ALPitchers/2015 contain filtered by pitcher versions of the 2015.csv dataset. They are named after the PitcherID, e.g. Mark Buehrle has the PitcherID 279824, and his pitches' information are in the 279824.csv file.
yearexp2015.m M-Files are MATLAB scripts. In particular, this one is used to compute the fastball and strike (and their complements, off-Speed and balls) for a given year.
chisqrtest2015.m This file is used to perform both chi squared test.
Maurertest2015.m This file is used to perform Maurer's Universal statistical test for random bit generators.
testing.m This file is used to test the statistical significance of the measures of randomness derived from the previous tests.

# Notes
To replicate the it's necessary to already have the 2013.csv and 2014.csv files (only relevant while using yearexp2015.m)
yearexp2015.m has to be run once for each year, and modified to load the correct source (2013.csv or 2014.csv). The weighted average was the computed by hand. 
The test for the pitchers in chisqrtest2015.m and Maurertest2015.m has to be run once for each pitcher, modifying the file to point to the correct source (a PitcherID csv file) and the result stored by hand.
testing.m has to be run once for each test, modifying the file to select the right regressors.
