---
layout: post
title: Numbers in Python
categories: [python]
---
Python is widely known by your capacity to make mathematical operations fast. Allied  your writing power, Python is a powerful tool by scientists to make complex calculus and others data processings.

This article is to show some characteristics of numbers in Python, sometimes comparing the type across the versions 2.7 and 3:
- [The Primitive Types](#primitives);
- [The Operators in Python](#operators);
- [Conversion of Numbers](#conversion);
- [Mathematics Functions](#mathematics-functions);
- [Random Number Functions](#random-functions);
- [Trigonometric Functions](#trigonometrics-functions);
- [Mathematical Constants](#mathematics-constants);

## The Primitive Types {#primitives}
Python has supports four numerical types: *int*, *long*, *float* and *complex*.

Each one of kind this represents a set in Numbers Sets.

### Int

Represents the a subset of set ***Z*** in Numbers Sets, in others words represents the ***integers*** numbers, positives or negatives, like -1, 1000 and others. But the type ***int*** has a limitation. It is implemented using the type ***long*** in C programming language, so it use 32 bits of precision, so only can represent a little set of numbers. This limitation is present in version 2.7 of Python, but in the version 3, the limitation was removed in part, because that now is limited by the word of machine.

### Long

If you need more precision so the type which you want is ***Long***. This type represent same subset which ***int***, but expanded. In documentation it's described with unlimited size, so, can represent any number of the set ***Z***. But this normally not happen because the limitation of machine, either by size of word, processing or memory.

This type only exists until the version 2.7. In Python 3 this type and the type ***int*** are the same.

### Float

This type represent a subset ***Q***, the rational numbers. Numbers with floating point, like 0.0001 or 1156454687954.564651. In Python 2.7, it's implemented using the type ***Double*** in C language, so use 64 bits of precision. In Python 3, the precision is determined by the machine where the program is runing.

### Complex

Remember your studies in mathematics, when you was presented a number formatted with a part real and a imaginary part? Them are the complex numbers. Python is one of the few programing languages have this type of numeric representation. This is a more factor to scientists use Python.

To extract these parts from a complex number, use ```x.real``` and ```x.imag``` .

## The Operators in Python {#operators}

Almost all types of numbers in Python can support the follows operations, the only except is the complex type. The table below show compactly form the operations with use the operators +, -, * and  /.

| Operation | Result | Note |
|-------|--------|---------|
| x + y | sum of x and y |  |
| x - y | difference of x and y |  |
| x * y | product of x and y |  |
| x ** y | x to the power y |  |
| x / y | quotient of x and y | For (plain or long) integer division, the result is an integer. The result is always rounded towards minus infinity: 1/2 is 0, (-1)/2 is -1, 1/(-2) is -1, and (-1)/(-2) is 0. Note that the result is a long integer if either operand is a long integer, regardless of the numeric value. |
| x // y | (floored) quotient of x and y | Also referred to as integer division. The resultant value is a whole integer, though the result's type is not necessarily int. |
| x % y | remainder of x / y | Complex floor division operator, modulo operator, and divmod(). Deprecated since release 2.3. Instead convert to float using abs() if appropriate. |
| -x | x negated |  |
{: .table .table-striped .table-condensed}

## Conversion of Numbers {#conversion}

Python provide some functions to conversion a type of number in other type. The table below show this built-in functions:

| Operation | Result | Note |
|-------|--------|---------|
| int(x) | x converted to integer | Conversion from floating point to (long or plain) integer may round or truncate as in C; see functions floor() and ceil() in the math module for well-defined conversions. |
| long(x) | x converted to long integer | The same note as above |
| float(x) | x converted to floating point |  |
| complex(re,img) | a complex number with real part re, imaginary part img. img defaults to zero. |  |
{: .table .table-striped .table-condensed}

## Mathematics Functions {#mathematics-functions}

Such as functions to convert between number types, Python also has built-in functions to many mathematics functions. Many functions only are access through package ***math***,  first import the package with the command ```ìmport math``` and call them with ```math``` in start, like this ```math.fabs(x)```.

| Function  | Description of Return |
|---------- |-----------------------|
| abs(a)    | Return the absolute value of ***a***: the (positive) distance between ***a*** and zero |
| fabs(a)   | Return the absolute value of ***a***: not is access directly, only through package ***math*** and always return a float |
| ceil(a)   | Return the ceiling of ***a***: the smallest integer not less than ***a*** |
| floor(a)  | Return the floor of ***a***: the lagerst integer not greater than ***a*** |
| cmp(a, b)  | Compation between two numbers: return -1 if a < b, 0 if a = b and 1 if a > b |
| exp(a)    | Return exponential of a with base ***e***  |
| log(a)    | Return the natural logarithm of ***a***, for ***a*** > 0 |
| log10(a)  | Return the base 10 logarithm of ***a***, for ***a*** > 0 |
| max(a, b, ...) | Return the largest of its arguments: the value closest to positive infinite |
| min(a, b, ...) | Return the smallest of its arguments: the value closest to negative infinite |
| modf(a)   | Return the fractional and integer parts of ***a*** in a tuple. Both parts have the same sign as ***a***. The integer part is returned as a float |
| pow(a, b) | Return the value of ***a*** ** ***b*** |
| sqrt(a)   | Return the square root of ***a*** for ***a*** > 0 |
| round(a[, n]) | Return ***a*** rounded to ***n*** digits from the decimal point. Python rounds away from zero as a tie-breaker: ```round(0.5) = 1.0``` and ```round(-0.5) = -1.0```  |
{: .table .table-striped .table-condensed}

## Random Number Functions {#random-functions}

Through the package ```random```, Python offer some functions to create pseudo random sequences, or get a random number.

| Function  | Description of Return |
|---------- |-----------------------|
| choice(sequence)    | Return a random element from the sequence. The sequences can be lists, tuples or string |
| randrange([start,] stop[,step]) | Return a randomly element between the ***start*** (if defined) or zero and the ***stop***. Also you can inform the step which you want |
| random() | Return a float number ***a***, such that 0 is less than or equal to ***a*** and ***a*** is less than 1 |
| seed([a]) | Sets the integer starting value used in generating random numbers. Call this function before calling any other random module function. Returns None. |
| shuffle(list) | Randomizes the items of a list in place. Returns None
| uniform(a, b) | Return a random float ***x***, such that ***a*** is less than or equal to ***x*** and ***x*** is less than ***b*** |
{: .table .table-striped .table-condensed}

## Trigonometric Functions {#trigonometrics-functions}

The trigonometric functions not forgot by Python and someone's of them be part of language in built-in functions. Then can be access through the package ```math```.

| Function  | Description of Return |
|---------- |-----------------------|
| degrees(a)    | Converts angle ***a*** from radians to degrees |
| radians(a)    | Converts angle ***a*** from degrees to randians |
| sin(a)    | Return the sine of ***a***, in radians |
| cos(a)    | Return the cosine of ***a***, in radians |
| tan(a)    | Return the tangent of ***a***, in radians |
| acos(a)    | Return the arc cosine of ***a***, in radians |
| asin(a)    | Return the arc sine of ***a***, in radians |
| atan(a)    | Return the arc tangent of ***a***, in radians |
| atan2(a, b)    | Return the atan(a/b), in radians |
{: .table .table-striped .table-condensed}

## Mathematical Constants {#mathematics-constants}

Some mathematical constants also defined in package ```math``` in Python.

| Constant  | Description |
|---------- |-----------------------|
| ***e***    | The mathematical constant ***e*** |
| ***pi***    | The mathematical constant ***pi*** |
{: .table .table-striped .table-condensed}

If you want learn more about numbers in Python, below have the links used in this article:
- [Tutorials Point](https://www.tutorialspoint.com/python/python_numbers.htm);
- [Python 2.7 Documentation](https://docs.python.org/2/library/stdtypes.html#numeric-types-int-float-long-complex);
- [Python 3.7 Documentation](https://docs.python.org/3.7/library/stdtypes.html#numeric-types-int-float-complex);