# Using the Bacon Trap

## What This Does
The BaconTrap study is intended to be used for "set it and forget it" type of trades, and takes advantage of trend days.
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

## Notes, Gotchas and Other Useful Information about the BaconTrap
- When choosing a contract to buy when the trap fires, find one where the premium is more than $1.00 per option. Options that are less than that are much more prone to stopping out due to the higher % moves per penny on the price.
- In the `Study Order Condition` -> `Condition Setup` window, it helps to ensure that `5m` is the selected timeframe. Any time frame larger than 5m will cause errors and you will not be able to finish setting the trap. Any time frame smaller than 5m can cause traps to fire on false breakouts.

## Set a BaconTrap
1. Select an option contract, right-click and choose the `Buy custom` option, then select the template you wish to use

![image](https://user-images.githubusercontent.com/13930961/188988948-bac0d6a5-946a-4757-962b-8b5e3477fdf4.png)

2. Click on the gear icon on the right side of the entry order to bring up the Order Rules form

![image](https://user-images.githubusercontent.com/13930961/183997714-dbb5faeb-f31f-4af5-9b4e-fd8dadb972fd.png)

3. This form is where the study is put to use. Enter the underlying ticker on which the price, click MARK drop down the Method, select STUDY and Edit...

![image](https://user-images.githubusercontent.com/13930961/184001911-4479b1e1-6f82-4ed7-864e-2faad92b0f2d.png)

4. WHen the `Oeder Rules` window opens, under "Conditions," Click the method (should already be set to "STUDY") to drop down the selections, Click "STUDY" and select "Edit..."

![image](https://user-images.githubusercontent.com/13930961/188992129-7bdb7a57-ec04-4d4d-8994-33fa451bc626.png)

5. Set your desired trigger price, relative volume trigger, contract type, volume periods, minutes after open

![image](https://user-images.githubusercontent.com/13930961/184715416-5c0dd4ed-1c9c-4e61-9004-c5d352ae21db.png)

6. Click `Save` in the lower-right of the `Edit condition` window
7. Click `OK` in the Study order condition` window
8. Click `Save` in the lower-right corner of the `Order rules` window
9. Your trap order is now ready to send

![image](https://user-images.githubusercontent.com/13930961/188992803-824e6c13-6388-412c-ad07-c96e221a27a9.png)

10. Now just wait for the traps to fire for entry then exit one way or the other. Most usually exit in the same day, but some may take a day or two
