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
2. Select an option contract, right-click and choose the `Buy custom` option, then `with OCO bracket`
3. In the order entry form, click to unlink the prices for the OCO portion (circled in blue)

![image](https://user-images.githubusercontent.com/13930961/183994542-d84e0bc6-5ee1-468c-a78d-d0993e76b36f.png)

4. If you want the OCO orders to be based on percentages, click the `+/-` button twice, in the price column of the order entry form, then set your stop and sell percentages

![image](https://user-images.githubusercontent.com/13930961/183996392-de246549-2966-44f8-a148-d8db815622af.png)

![image](https://user-images.githubusercontent.com/13930961/183999819-30f2f1bb-bf67-4352-a361-3dd22590cf98.png)

5. Now, click on the gear icon on the right side of the entry order to bring up the Order Rules form

![image](https://user-images.githubusercontent.com/13930961/183997714-dbb5faeb-f31f-4af5-9b4e-fd8dadb972fd.png)

6. This form is where the study is put to use. Enter the underlying ticker on which the price, click `MARK` drop down the Method, select `STUDY` and `Edit...`

![image](https://user-images.githubusercontent.com/13930961/184001911-4479b1e1-6f82-4ed7-864e-2faad92b0f2d.png)

7. In the Study Order Condition window that popped up, click the `Delete` Button

![image](https://user-images.githubusercontent.com/13930961/184002715-36d04333-e1c7-41b8-bdcc-3c8fe5900fee.png)

8. Next, change the period for the Study Order Condition to 5 minutes

![image](https://user-images.githubusercontent.com/13930961/184006868-1a901435-612a-443d-a118-009a25f7027e.png)

9. Click the `Add condition` button

![image](https://user-images.githubusercontent.com/13930961/184002969-66cc6ac1-37e4-4c89-90a3-8dbe341b8c00.png)

10. Drop down `Select a condition` and select `Study`

![image](https://user-images.githubusercontent.com/13930961/184005148-4ee7c42e-aef6-4da3-a6e4-bf3f9050932b.png)

11. Start typing in `bacon` and select the `BaconTrap` study

![image](https://user-images.githubusercontent.com/13930961/184005447-0360b134-0217-4b14-ba70-cf23460733d5.png)

12. In the `Edit condition` window, select `is equal to`, then `Value`, and set the value to `1`

![image](https://user-images.githubusercontent.com/13930961/184005983-caa4365e-94f2-4e3a-af8d-33382973bd86.png)

13. Set your desired trigger price, relative volume trigger, contract type, volume periods, minutes after open and open time

![image](https://user-images.githubusercontent.com/13930961/184006353-665aefae-4782-4ab3-8593-6415cbcff2a9.png)

14. 
