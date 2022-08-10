# Bacon Trap

## What this does
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

## Setup an order Template
1. In TOS, import the script from http://tos.mx/HecjhSo
2. 
