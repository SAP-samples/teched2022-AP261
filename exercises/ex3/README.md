# Exercise 2 - Available Bids

In this exercise, we will review Available Bids and convert them into a contract

## Exercise 2.1 Review "Available Bids" Card 



1. Review Available Bids Card in the Origination Dashboard
<br>![](/exercises/ex3/images/Ex_3_1_3_Image.png)

2.	You can filter Bids based on Delivery period, Commodity, and Material. You can also view the information in different Unit of Measures configured for your Business partner.
3.  Click on the card header to navigate to "Manage Bids" app to verify the Bids displayed on Dashboard.
4.  All the filters from Dashboard should be pre-populated in the app.
<br>![](/exercises/ex3/images/Ex_3_1_1_Image.png)

5. View the Bid details by clicking on the Bid.
6. CLick on "Request Contract" button on top right corner.
7. Create contract screen will appear.
<br>![](/exercises/ex3/images/Ex_3_1_2_Image.png)

8. Quantity should be editable for the contract item.
9. Provide the quantity that you intend to convert to contract.
10. Click on "Save" button at the bottom right corner.
11. Contract creation requested message should appear on screen.
12. Bid will move to "Requested" status.
13. WIthin few minutes Bid will move to approved status on the list page.
14. From personalization, select contract field to be displayed on the Bid List page.
15. Click on teh contract number and validate the data from the Bid.

## Exercise 2.2 Sub Exercise 2 Description

After completing these steps you will have...

1.	Enter this code.
```abap
DATA(lt_params) = request->get_form_fields(  ).
READ TABLE lt_params REFERENCE INTO DATA(lr_params) WITH KEY name = 'cmd'.
  IF sy-subrc = 0.
    response->set_status( i_code = 200
                     i_reason = 'Everything is fine').
    RETURN.
  ENDIF.

```

2.	Click here.
<br>![](/exercises/ex2/images/02_02_0010.png)

## Summary

You've now ...

Continue to - [Exercise 4 - Excercise 4 ](../ex4/README.md)

