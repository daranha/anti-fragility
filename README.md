# anti-fragility
Data for our anti-fragility research project 


# For reading the data run the following commands 

import pandas as pd
import numpy as np
import pickle


# Create a dictionary 
with open('cr_dic_glob_caf.py', 'rb') as fp:
    dic = pickle.load(fp, encoding='latin1')

# Create a DataFrame from the dictionary
data = pd.DataFrame(dic).transpose()
