# Splunk Conf 2014 #

Analyse how was your experience at Splunk Conf 2014, also helps your on ask for company refund for some expenses.

Using **expenses** report you can control how did you used your money and how much will be refunded by your company :)

Also by using **realizations** report you can check how good was your experience and check all done things and the missing one.

### Expenses Report ###

![Expenses View 1](https://raw.githubusercontent.com/Caldas/splunkConf2014/master/Docs/PrintScreens/expenses_v1.png)
Check how many spends you did and if they are refundable* or not.

![Expenses View 2](https://raw.githubusercontent.com/Caldas/splunkConf2014/master/Docs/PrintScreens/expenses_v2.png)
You also can see your spends by day,

![Expenses View 3](https://raw.githubusercontent.com/Caldas/splunkConf2014/master/Docs/PrintScreens/expenses_v3.png)
or by money source.

![Expenses View 3](https://raw.githubusercontent.com/Caldas/splunkConf2014/master/Docs/PrintScreens/expenses_v4.png)
And sure, you can have it listed to export to your HR departament or to show your wife(husband) :)

### Realizations Report ###

![](https://raw.githubusercontent.com/Caldas/splunkConf2014/master/Docs/PrintScreens/realization_filters.png)
On realization report you can choose what to show, by filtering realization type, if it was done or not, if it was planned or just happened and also by satisfaction

![](https://raw.githubusercontent.com/Caldas/splunkConf2014/master/Docs/PrintScreens/realization_v1.png)
On overall overview you can see on stars rate how good was the selected realizations,

![](https://raw.githubusercontent.com/Caldas/splunkConf2014/master/Docs/PrintScreens/realization_v2.png)
and you can also check the done distribuction and the list of realizations registered.

#### Data ####

All app data are obtained by 2 csv files: **spends.csv** and **deeds.csv** that are located on lookup folder inside application.

**Spends Format**

| Date | Value | Type | Who | MoneySource |
|---|---|---|---|---|
| 4/10/2014 | 30.00 | Fun | Fabio | Dinheiro |
| 5/10/2014 | 10.00 | Casino | Fabio | Dinheiro |
| 9/10/2014 | 10.70 | Taxi | Fabio | Cartao de Credito |


**Deeds Format**

| Type | What | Done | Planned | Satisfaction |
|---|---|---|---|---|
| Personal | Visit Cassino MGM | yes | no | 4 |
| Personal | Buy stuff for family | yes | yes | 5 |
| Work | Know about Splunk 6.2 | yes | yes | 3 |

## Extra ##

* Refunded Spends are detected by **eventtype** *refundable* and *not_refundable*. 
