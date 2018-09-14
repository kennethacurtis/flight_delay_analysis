# Flight Delay Analysis

### How to view this project

The visualizations for the project were created in Tableau. For me to share the project with others on Tableau Public, the data had to be filtered by just one year, 2017. As you will see in my gathering process, I originally gathered data from 2009 to 2017 which resulted in well over 15 million rows of data, which is the limit for Tableau Public. Because of this I have provided two ways to view the project.

**To view the project for flight data in 2017 on tableau public:** [click here](https://public.tableau.com/profile/kenneth5709#!/vizhome/FlightDelayAnalysis_16/FlightsStory)

**To view the project for flight data from 2009-2017:**
* [Click here](https://drive.google.com/open?id=15U1loH4gTsSkWUpbxGPWWKsA19OOA6wA) to download the tableau workbook labeled *flights2019-2017*
* Then [click here](https://www.tableau.com/products/reader) to download the free tableau reader
* Open Tableau Reader then open the workbook

**To read the report on cleaning this data download and view on your browser:**
[Click here](https://drive.google.com/open?id=1MQcBIVftU96AEPAtSuSmZvHDlltRalo6)

### Introduction

This data comes from [The Bureau of Transportation Statistics](https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=) and tracks destinations, distance, and delay information of flights across U.S. For this project, I chose the years 2009 through 2017 resulting in 54,383,096 rows of data. To see a more detailed description of the date, click [here](https://www.transtats.bts.gov/Fields.asp?table_id=236).

### Jupyter Notebook Notes

Throughout the notebook, you'll notice that most operations are single cell, this was because my machine kept running out of usable memory. The dataset was really large and required as much memory as possible for each operation. You will see multiple cells of code that could possibly be more code efficient, but were lengthened to reduce memory errors. You will also notice that after certain blocks of code, I outputted the dataframe to a csv. Some blocks of code took more than an hour to run. So to save my progress and make sure that I would not waste time re-running previous code, I would output my progress to a csv and then read it back in. I did not include these datasets in the repository, but have kept the code in the notebook.

The BTS website did not allow users to download full years of data. I downloaded data from the BTS website month by month from 2009 to 2017 and then used `pandas` to merge the data together. If you are interested in downloading the merged data as well as the cleaned data [click here](https://drive.google.com/open?id=1L1jx_CgARXZ1fpgetbvbON9a5AAr19XO).

Finally, after the cleaning process I ended up with 53,068,460 rows resulting in keeping 97% of the data. I was also able to bring the memory usage of the dataset from 11.8 GB to 5.7 GB.
