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


Date	     Price	 Open  	High  	Low
2/26/2024	1.0852	1.0819	1.086	1.0812
2/25/2024	1.0819	1.0826	1.0833	1.0818
2/23/2024	1.0818	1.0824	1.0841	1.0812
2/22/2024	1.0823	1.0816	1.0889	1.0802
2/21/2024	1.0817	1.0807	1.0825	1.079
2/20/2024	1.0803	1.0779	1.084	1.0761
2/19/2024	1.0777	1.0776	1.079	1.0761
2/16/2024	1.0774	1.077	1.0788	1.0732
2/15/2024	1.0771	1.0727	1.0785	1.0725
2/14/2024	1.0725	1.071	1.0735	1.0695
2/13/2024	1.0709	1.0772	1.0796	1.07
2/12/2024	1.0771	1.0781	1.0806	1.0755
2/9/2024	1.0782	1.0779	1.0796	1.0761
2/8/2024	1.0776	1.0772	1.079	1.0741
2/7/2024	1.0771	1.0755	1.0784	1.0753
2/6/2024	1.0754	1.0743	1.0763	1.0723
2/5/2024	1.0741	1.0784	1.0787	1.0723
2/2/2024	1.0784	1.0873	1.0898	1.078
2/1/2024	1.0872	1.0814	1.0876	1.0779
1/31/2024	1.0816	1.0844	1.0889	1.0795
1/30/2024	1.084	1.0833	1.0857	1.0811
1/29/2024	1.0833	1.0849	1.085	1.0796
1/26/2024	1.0852	1.0843	1.0885	1.0812






![image](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/33b273b3-7690-4d8e-aa2a-1185e30a63d6)























Step 4: 

apply time series model. In this example, we use ARIMA (1,1,1). You can also choose another model from statsmodels and tried it on to discover the differemces. The code is used for fiiting the model and for forcasting


forcast=w.estim(gbpusdData)












![download](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/ad421aec-caea-4ccb-8e38-ce6b32484709)












![download](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/abe7f429-b52c-4db2-ac4a-3b78bc6f6138)
