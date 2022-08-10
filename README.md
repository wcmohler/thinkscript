# Bacon Trap

## What This Does
This thinkscript is designed to be used for option order entry rules in TOS. The script will trigger entry (or exit) criteria based on the following:
- The underlying price of a ticker
- A specified minimum amount of time after market open before becoming sctive
- Relative volume

## Inputs:
- Trigger price
- Relative volume trigger
- Contract type (calls or puts)
- Minutes after open (to avoid false triggering during volatility after market open)
![image](https://user-images.githubusercontent.com/13930961/183993082-eb964897-c5ee-423a-8995-503df3f6944c.png)

## Setup an Order Template
1. In TOS, import the script from http://tos.mx/HecjhSo
2. select an option contract, right-click and choose the `Buy custom` option, then `with OCO bracket`
3. In the order entry form, click to unlink the prices for the OCO portion (circled in blue)
![image](https://user-images.githubusercontent.com/13930961/183994542-d84e0bc6-5ee1-468c-a78d-d0993e76b36f.png)
