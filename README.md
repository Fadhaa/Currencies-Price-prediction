# Currencies-Price-prediction

#This code is to get data of last 30 days from Investing,com and apply Time series ARIMA to it to predect the future pr



w=pred()
gbpusdData=w.getData('https://www.investing.com/currencies/gbp-usd-historical-data')

print(gbpusdData)
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


warnings.filterwarnings("ignore")
forcast=w.estim(gbpusdData)


![download](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/05fdfda1-7c53-48f6-9226-4ee2b06bfca3)

w=pred()
eurusdData=w.getData('https://www.investing.com/currencies/eur-usd-historical-data')

print(eurusdData)

     Date   Price    Open    High     Low
0   01-26-2024  1.0852  1.0843  1.0885  1.0812
1   01-29-2024  1.0833  1.0849  1.0850  1.0796
2   01-30-2024  1.0840  1.0833  1.0857  1.0811
3   01-31-2024  1.0816  1.0844  1.0889  1.0795
4   02-01-2024  1.0872  1.0814  1.0876  1.0779
5   02-02-2024  1.0784  1.0873  1.0898  1.0780
6   02-05-2024  1.0741  1.0784  1.0787  1.0723
7   02-06-2024  1.0754  1.0743  1.0763  1.0723
8   02-07-2024  1.0771  1.0755  1.0784  1.0753
9   02-08-2024  1.0776  1.0772  1.0790  1.0741
10  02-09-2024  1.0782  1.0779  1.0796  1.0761
11  02-12-2024  1.0771  1.0781  1.0806  1.0755
12  02-13-2024  1.0709  1.0772  1.0796  1.0700
13  02-14-2024  1.0725  1.0710  1.0735  1.0695
14  02-15-2024  1.0771  1.0727  1.0785  1.0725
15  02-16-2024  1.0774  1.0770  1.0788  1.0732
16  02-19-2024  1.0777  1.0776  1.0790  1.0761
17  02-20-2024  1.0803  1.0779  1.0840  1.0761
18  02-21-2024  1.0817  1.0807  1.0825  1.0790
19  02-22-2024  1.0823  1.0816  1.0889  1.0802
20  02-23-2024  1.0818  1.0824  1.0841  1.0812
21  02-25-2024  1.0819  1.0826  1.0833  1.0818
22  02-26-2024  1.0852  1.0819  1.0860  1.0812


warnings.filterwarnings("ignore")
forcast=w.estim(eurusdData)

![download](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/b1aea97d-b0cf-461d-8702-92ca9643aacc)


print("The mse of the (Low, High) forcasting is")
print(forcast)

The mse of the (Low, High) forcasting is
[0.004799886196411286, 0.0032559867677543057]

















22  02-23-2024  1.2679  1.2659  1.2702  1.2648
