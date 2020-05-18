# anti-fragility
Data for our anti-fragility research project.

### Data from the Stock Market: 
Original source: https://www.kaggle.com/borismarjanovic/price-volume-data-for-all-us-stocks-etfs

There are daily data from 7163 symbols from the US stock market. The first date on our processed data is 1990 and the last date is between September and November 2017. There is a separate file for the data of each year, they are available here: 


### Data from the Stock Market: 
The data consisted of daily historical data (open price, market capitalization and volume) of around 1800 agents, the eldest of them starting in 2013 and up to November 2018. The full data is included in the file ```'cr_dic_glob_caf.py'``` included in this repository.  

## For reading the data run the following commands 

```
import pandas as pd
import numpy as np
import pickle

 # Create a dictionary
 
filename = 'cr_dic_glob_caf.py'   # For Stocks data change this for any of the files 'dic_glob_cafc1_201*.py', * in [0..7] 
with open(filename, 'rb') as fp:
    dic = pickle.load(fp, encoding='latin1')

 # Create a DataFrame from the dictionary
data = pd.DataFrame(dic).transpose()


# the dictionaries for the data of stocks are at:
~/antifragility/00afin/dic_glob_cafc1_2010.py
...
~/antifragility/00afin/dic_glob_cafc1_2017.py

# each of them is 81 M, I cannot upload it to github. 
```
