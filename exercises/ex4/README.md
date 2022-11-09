# Exercise 4 - Origination Portal - Price Futures for Contracts

In this exercise, As a Farmer/Grower, I would want to price the Futures component of the contract based on the market prices.


## Exercise 4.1 Price Futures component of the contract

1. In Manage Contracts app click on the contract number and go to the details page.
<br>![](/exercises/ex4/images/Ex_4_2_Image.png)

2. Go to the pricing tab
<br>![](/exercises/ex4/images/Ex_4_1_1_Image.png)
3. Click on "Price Futures" button.
<br>![](/exercises/ex4/images/Ex_4_1_2_Image.png)
5. A pop-up will open with the unpriced futures quantity information. Price is fetched from the market(Source being ACM S/4HANA).There may be one or more pricing lots on the screen.
<br>![](/exercises/ex4/images/Ex_4_1_3_Image.png)
7. Futures price should already appear for the lot and quantity should be editable. Enter the quantity for which you intend to establish futures price. Perform this step for a pricing lot which already has Basis priced.
<br>![](/exercises/ex4/images/Ex_4_1_4_Image.png)
9. Click on "Save".
10. You should be redirected to the Contract item details page.
11. Navigate back to "Manage Contracts" list page and search the same contract.
12. Navigate to the details page and you should see the pricing lot with FLAT price for the quantity you just priced. 
<br>![](/exercises/ex4/images/Ex_4_1_5_Image.png)


## Exercise 4.2 Review Contract Monitoring Cards

1. From the Launchpad, navigate to Origination Dashboard and review Contract Monitoring card - Priced Quantity.
<br>![](/exercises/ex4/images/Ex_4_2_1_Image.png)

2. Filter based on Contract Number and check the Priced Quantity card
3. Priced Quantity Card should show the Flat Priced quantity against the total contract item quantity. Pricing lot quantity where basis price existed and futures was requested in previous excercise should be shown as FLAT priced here.


## Summary

You've now established Futures price for Contracts as a Farmer.

Continue to - [Exercise 5 - Exercise 5 Description](../ex5/README.md) to explore the Integration Content for Agricultural Origination Portal.
