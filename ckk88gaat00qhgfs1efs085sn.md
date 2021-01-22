## Converting String to Integer (Base 2-36)

Now if you're familiar with the Python programming language and have done coding in it, you must be knowing about int() function that is used for type conversion. We generally pas one argument to it, the syntax of int is ab bit different.

First, let's see what we generally use int() with just one argument.


```python
#coded by Shashwat Raj
#To show conversion through int()

num1 = 5.6
num2 = '7'

num = int(num1)
print(num)

num = int(num2)
print(num)

``` 

**Output:**
```
5
7
``` 

In this case, we can pass a string containing digits i.e. characters from 0–9 or a floating-point value.

**Note:** *If we pass a string that has any other character other than 0–9 it will throw an error.*

The int() function can be used by passing two arguments also.

![Error](https://cdn.hashnode.com/res/hashnode/image/upload/v1611315965888/_o_JCB7RI.png "Error Output" )

> 
Syntax:
>
int('string', base)

Here the int() accepts an arbitrary base between 2 to 36 and 0. Here 0 represents the Decimal Number system ( base 10).

You must be knowing different ways of denoting an integer number i.e. Binary (base 2), Decimal (base 10), Octal (base 8), Hexadecimal (base 16).

Each base denotes how many different characters will be used to denote an integer.

For Example,


> 
Decimal has 10 characters from 0–9. This is the common number system that human use. [1, 2, 10, 13 15]
>
In the same way, Binary only has 2 characters 0 & 1.Our machine works on this number system. [0001, 0011, 1001, 1101, 1111]
>
Hexadecimal has 16 characters from 0–9 & a-f. This is also used by the machine to work with memory. [1, 2, a, d, f]

**Note:** *Here also the string should use characters that are defined for a particular base or it will throw an error.
Moreover, the characters used in the string which are alphabet (a-z) in base above 10 are not case sensitive. So you use an upper case character or a lower case character it doesn't really matter.*


```python

#Coded by Shashwat Raj
#To show the function of int()

"""
Syntax:    
       int( 'String', base)   
"""

num32 = 'shashwat131'
num16 = '123abc'
num10 = '7968'
num8 = '1257'
num2 = '010001001'

num = int (num32,32)
print(num)

num = int (num16,16)
print(num)

num = int (num10,10)
print(num)

num = int (num8,8)
print(num)

num = int (num2,2)
print(num)
``` 

**Output:**
```
104129399839163581
1194684
7968
687
137
``` 



Must be thinking what is the practical use of this function I will suggest you see this code. Here this int() function is used to generate the URL for a website to extract images.