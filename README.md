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

          Date   Price    Open    High     Low
0   01-24-2024  1.2723  1.2688  1.2776  1.2677
1   01-25-2024  1.2708  1.2721  1.2744  1.2680
2   01-26-2024  1.2702  1.2710  1.2759  1.2674
3   01-29-2024  1.2707  1.2697  1.2720  1.2661
4   01-30-2024  1.2697  1.2710  1.2723  1.2639
5   01-31-2024  1.2685  1.2699  1.2752  1.2657
6   02-01-2024  1.2742  1.2687  1.2757  1.2624
7   02-02-2024  1.2630  1.2744  1.2774  1.2613
8   02-05-2024  1.2532  1.2633  1.2644  1.2517
9   02-06-2024  1.2597  1.2536  1.2605  1.2529
10  02-07-2024  1.2625  1.2598  1.2643  1.2591
11  02-08-2024  1.2616  1.2626  1.2640  1.2571
12  02-09-2024  1.2619  1.2622  1.2644  1.2598
13  02-12-2024  1.2626  1.2625  1.2656  1.2605
14  02-13-2024  1.2589  1.2630  1.2685  1.2572
15  02-14-2024  1.2565  1.2590  1.2613  1.2534
16  02-15-2024  1.2600  1.2565  1.2603  1.2541
17  02-16-2024  1.2598  1.2600  1.2626  1.2550
18  02-19-2024  1.2593  1.2603  1.2631  1.2582
19  02-20-2024  1.2618  1.2591  1.2670  1.2578
20  02-21-2024  1.2634  1.2622  1.2643  1.2601
21  02-22-2024  1.2659  1.2638  1.2711  1.2610
22  02-23-2024  1.2679  1.2659  1.2702  1.2648


Step 4: 

apply time series model. In this example, we use ARIMA (1,1,1). You can also choose another model from statsmodels and tried it on to discover the differemces. The code is used for fiiting the model and for forcasting


forcast=w.estim(gbpusdData)












![download](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/ad421aec-caea-4ccb-8e38-ce6b32484709)












![download](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/abe7f429-b52c-4db2-ac4a-3b78bc6f6138)
