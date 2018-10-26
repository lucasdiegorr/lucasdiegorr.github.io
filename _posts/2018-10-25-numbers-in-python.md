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

## <a id="primitives"></a> The Primitive Types
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

## <a id="operators"></a> The Operators in Python



## <a id="conversion"></a> Conversion of Numbers



## <a id="mathematics-functions"></a> Mathematics Functions



## <a id="random-functions"></a> Random Number Functions



## <a id="trigonometrics-functions"></a> Trigonometric Functions



## <a id="mathematics-constants"></a> Mathematical Constants
