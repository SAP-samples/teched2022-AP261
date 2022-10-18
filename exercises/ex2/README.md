# Exercise 2 - Storage

In this exercise, we will review storage/comingled stocks

## Exercise 2.1 Review Storage/Comingled quantity information through Dashboard Card



1. Review Total Quantity in Storage Card. You should be able to view storage quantity for each commodity
<br>![](/exercises/ex2/images/Ex_2_1_Image.png)

2.	Filter based on Commodity and check the quantity.
3.  Click on the card header to navigate to "Manage Delivery Assignments" app to verify the quantity displayed on Dashboard.
4.  "Storage Indicator" filter should be auto applied in the app.
<br>![](/exercises/ex2/images/Ex_2_1_1_Image.png)


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

Continue to - [Exercise 3 - Excercise 3 ](../ex3/README.md)
