Currencies-Price-prediction

This code to import data from investing.com after I tried to use investpy, but it's seemingly not working due to connection problems

Step 1: install 
python3

and then install the necessary packages  (urllib3, time, pandas, matplotlib, numpy, statsmodels, sklearn)
by use the cond in the command prompt

pip install Pack_name

Step 2: open python and start the following codes

import urllib3
from time import time,sleep
import warnings
warnings.filterwarnings("ignore")
import pandas as pd
urllib3.disable_warnings()
import matplotlib.pyplot as plt
import numpy as np
from statsmodels.tsa.arima.model import ARIMA
from sklearn.metrics import mean_squared_error


Excecuting of the code

Step 3:

Import historical Data from website www.investing.com. In this method, you will get the last 30 days. If yor are interested in large sample size, you need to download manually in .txt file.


use the following code

w=Pred()

e=w.getData('https://www.investing.com/currencies/usd-jpy-historical-data')

ee=w.reformat(e)

et2=w.estim(ee)

examples here 

https://github.com/Fadhaa/Currencies-Price-prediction/blob/main/updated-currencies-forecasting.ipynb





































