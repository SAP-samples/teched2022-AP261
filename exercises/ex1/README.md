# Exercise 1 - Origination Portal - Contracts

In this exercise, we will review the:
1. Total Contracts Quantity
2. Total Contracts Open Quantity by Commodity
3. Contract Monitoring – Priced Quantity
4. Contract Monitoring – Delivered Quantity
5. Contract Monitoring – Settled Quantity


## Exercise 1.1 Check the Contracts information

Pre-requisite:
Valid user id and password, Business Partner assigned to your user

1. Review Total Contracts Quantity. You should be able to view open, Delivered and Unsettled, Settled and Unpaid, Paid for each commodity
<br>![](/exercises/ex1/images/Ex1_Image1.png)

2. Filter based on contract number and check the quantities for each of the types.
3. Click on the "Open" quantity bar and navigate to "Manage Contracts" application
4. Filters on the Dashboard should be passed on the "Manage Contracts" application
5. Additionally, status filter should be defaulted to "Open"
6. All the contracts with "Open" quantity for Business Partner assigned to your user.



## Exercise 1.2 Sub Exercise 2 Description

After completing these steps you will have...

1.	Enter this code.
```abap
DATA(lt_params) = request->get_form_fields(  ).
READ TABLE lt_params REFERENCE INTO DATA(lr_params) WITH KEY name = 'cmd'.
  IF sy-subrc <> 0.
    response->set_status( i_code = 400
                     i_reason = 'Bad request').
    RETURN.
  ENDIF.

```

2.	Click here.
<br>![](/exercises/ex1/images/01_02_0010.png)


## Summary

You've now ...

Continue to - [Exercise 2 - Exercise 2 Description](../ex2/README.md)

