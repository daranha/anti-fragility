# anti-fragility
Data for our anti-fragility research project.

### Data from the Stock Market: 
Original source: https://www.kaggle.com/borismarjanovic/price-volume-data-for-all-us-stocks-etfs

There are daily date from 7163 symbols from the US stock market. The first date on our processed data is 1990 and the last date is between September and November 2017. 


## For reading the data run the following commands 

```
import pandas as pd
import numpy as np
import pickle

 # Create a dictionary 
with open('cr_dic_glob_caf.py', 'rb') as fp:
    dic = pickle.load(fp, encoding='latin1')

 # Create a DataFrame from the dictionary
data = pd.DataFrame(dic).transpose()


# the dictionaries for the data of stocks are at:
~/antifragility/00afin/dic_glob_cafc1_2010.py
...
~/antifragility/00afin/dic_glob_cafc1_2017.py

# each of them is 81 M, I cannot upload it to github. 
```
