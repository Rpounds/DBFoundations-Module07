Rachel Pounds

5/25/2021

IT FDN 130 A

Assignment 07

Github link

# Introduction

Functions are a great way to name and store sql that can be reused to retrieve data.  This paper will discuss several kinds of functions and provide some examples. 


# Explain when a SQL UDF would be used

A User Defined Function would be used when there is a custom function the user may want to use again.  Creating the Function allows the user to retrieve it and use it another time.   They can also be used for Check constraints.  If software (like Excel) is going to be used, a UDF may not be a good idea because it’s more difficult to get other software to read the functions.  In these cases, Views may be a better option, if they are simple.


# Explain the differences between Scalar, Inline and Multi-Statement Functions

A Scalar Function returns a single value and is not treated like a table. 
An Inline Table-valued Function creates a table of data with some parameters.   When naming this kind of function DBO should be used as a prefix to the Function name.  A Select statement can be used on this type of Function, just like a View or Table.
 

![image](https://user-images.githubusercontent.com/84206447/119711839-d3fb0980-be14-11eb-8f6f-aba56a50b42f.png)

Figure 1- Inline Table-valued Function and Select statement examples


![image](https://user-images.githubusercontent.com/84206447/119711864-d8bfbd80-be14-11eb-8523-a189a554ccc9.png)

Figure 2-Snippet of results from Selecting on function


Multi-Statement  Table-Valued Functions create a pseudo table of data after some additional processing, using Select statements on various sources. 


 ![image](https://user-images.githubusercontent.com/84206447/119711929-eaa16080-be14-11eb-925e-e6785593b26b.png)

Figure 3-Multi-Statement Table-Valued Function sql example from Module 7 Demos


![image](https://user-images.githubusercontent.com/84206447/119711963-f55bf580-be14-11eb-8bf5-b3f986e45af5.png)

Figure 4- How call get results from the function from Module 7 Demo


# Summary
This paper described User Defined Functions (UDFs), including the differences between the varieties and some examples.



