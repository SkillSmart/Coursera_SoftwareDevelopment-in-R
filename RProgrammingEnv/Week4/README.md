The goal of this assignment is to take datasets that are either messy or simply not tidy and to make them tidy datasets. The objective is to gain some familiarity with the functions for reading in data into R and calculating basic summary statistics on the data. In particular, we will make use of the following packages: dplyr, tidyr, readr, and readxl. You can install these packages with the install.packages() function in R, using



1
install.packages(c("dplyr", "tidyr", "readr", "readxl"))
Running install.packges() may also install a host of other packages on which these two depend so it might take a minute or two.

Before staring the quiz you will need to download the data for the quiz, which can be found in the file quiz_data.zip. The zip archive file contains two files:

daily_SPEC_2014.csv.bz2: a compressed CSV file containing daily measurements of particulate matter chemical constituents in the United States for the year 2014. Note that you should NOT have to decompress this file. The data are measured at a network of federal, state, and local monitors and assembled by the EPA. In this dataset, the "Sample.Value" column provides the level of the indicated chemical constituent and the "Parameter.Name" column provides the name of the chemical constituent. The combination of a "State.Code", a "County.Code", and a "Site.Num", uniquely identifies a monitoring site (the location of which is provided by the "Latitude" and "Longitude" columns).

aqs_sites.xlsx: An excel spreadsheet containing metadata about each of the monitoring sites in the United States where pollution measurements are made. In particular, the "Land Use" and "Location Setting" variables contain information about what kinds of areas the monitors are located in (i.e. “residential” vs. “forest”).

Once the data have been downloaded to your working directory, you can begin the quiz assignment. For this assignment, you may want to review Sections 1.2 through 1.5 of Mastering Software Development in R.