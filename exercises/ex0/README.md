# Agricultural Origination Portal

In this exercise, you will explore the "Origination Dashboard" of Agricultural Origination Portal

## Origination Dashboard

After completing the activation of your account, click on the following link

1.	Click here.
<br>![](/exercises/ex0/images/Image1.png)

2.	Insert this code.
``` abap
 DATA(params) = request->get_form_fields(  ).
 READ TABLE params REFERENCE INTO DATA(param) WITH KEY name = 'cmd'.
  IF sy-subrc <> 0.
    response->set_status( i_code = 400
                     i_reason = 'Bad request').
    RETURN.
  ENDIF.
```

## Summary

Now that you have ... 
Continue to - [Exercise 1 - Exercise 1 Description](../ex1/README.md)
