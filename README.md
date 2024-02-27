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

w=pred()
gbpusdData=w.getData('https://www.investing.com/currencies/gbp-usd-historical-data')


print (gbpusdData)




![image](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/33b273b3-7690-4d8e-aa2a-1185e30a63d6)























Step 4: 

apply time series model. In this example, we use ARIMA (1,1,1). You can also choose another model from statsmodels and tried it on to discover the differemces. The code is used for fiiting the model and for forcasting


forcast=w.estim(gbpusdData)





![Figure_1_gbp_usd](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/4099ec59-2197-479c-a32a-86a03f396321)




We also import eur_usd data from the link


w=pred()
eurusdData=w.getData('https://www.investing.com/currencies/eur-usd-historical-data')

forcast=w.estim(eurusdData)
















![Figure_1_eur_usd](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/3e5204d6-7474-4aa1-a637-ab7ee8dbd781)



























