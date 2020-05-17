---
title: 'Python Intro'
date: 2020-05-10T15:34:30-04:00
categories:
  - python
  - introduction

tags:
  - Hello-world
  - comments
  - coding
  - beginner
sidebar:
  nav: 'docs'
---

Python is an interpreted programming language. According to [pypl][pypl], Python is one of the most popular languages out there. This will introduce you to the basic. To run a python code, you need to install a python interpreter. It comes by default on most linux machine. Just open a terminal, type python and enter. 

For this, we will be using Google [colab][colab]. I have shared a [sample code][sample-code]. feel free to make a copy and follow along.

#### Hello World
To print hello world. do this:
```python
print('Hello World')
```

#### Comments
Comments are used to desribe a fucction or leave halpful information
See sample comments below:

```python
# This is a single line comnent

'''
This is a 
multiline
comment
'''
```

#### Escape Character
Python has characters that are reserved and have special meaning. For example, python will interprete a text in a quote as a python string. Python provides the Escape (\) charater for use to print such special characters.
See sample below
```python
print('What\'s your aim of learning python\?')
``` 
The escape charater was used to make python handle the (') in what's and (?) as regular characters

#### Print and New Line
By default, the print statement appends a new line after every print. To avoid that, use the 'end' parameter.
See sample
```python
print('one')
print('two')
# This will print on two lines
print('one', end='')
print('two')
#This will print on one line
```

#### Concatenation
Concatenation is the joining of two values. This could be different depending on the type of variable involved.
To contatenate 
2 strings, use + or ,
a string and interger, use ,. + will throw an error
When + is used on integers, its sums them instead of concatenating them.

See example below
```python
print('a', 'b') #Result -> ab
print('a' + 'b') #Result -> ab
print('a', 5) #Result -> a5
print('a'+ 5) #Result ->Error
print(5 + 5) #Result -> 10
```

#### Print and New Line
By default, print statement adds a new line after print. To remove the new line, update the end parameter.
See example below
```python
print('one')
print('two') 
# This will be printed on 2 lines. To print those on a single line
print('one', end = ' ')
print('two') # Result -> one two
```
#### Variable Naming

These are legal variable names

* varname = 'belu'
* var_name = 'belu'
* _var_name = 'belu'
* varName = 'belu'
* VARNAME = 'belu'
* varname2 = 'belu'
{: .notice--info}

These are illegal variable names
* 2varname = 'John' # Cant start with numbers
* var-name = 'John' # No hyphen (-)
* var name = 'John' # No Space
{: .notice--warning}

#### Variable Assignment
Variables can be assigned:
```python
#Per element
city = 'California'

#In groups. This is called unpacking
x, y, z = 'Orange', 10, True 

print(city) # Result -> California
print(x) # Result -> Orange
print(x) # Result -> 10
print(x) # Result -> True
```

#### Type Casting
Type casting is the conversion of data type to another. See example
```python
# To know the data type of a variable, use the inbuilt type method.
x  = 1
print(type(x)) # Result -> int
y = str(x)
print(type(y)) # Result -> str
z = float(y)
print(type(z)) # Result -> float

#Know that converting a float to int would loose any decimal values
x = 1.3
y = int(x)
print(y) # Result -> 1
```

Its also possible to cast between tuple, dict and set. See example
```python
l = [1,2]
print(type(l)) # Result -> list

h = set(l)
print(h)  # Result -> {1,2}
print(type(h))  # Result -> set

t = tuple(h)
print(t)  # Result -> (1,2)
print(type(t))  # Result -> tuple

o = list(t)  # Result -> [1,2]
print(type(o))  # Result -> list
```

#Casting rules
See examples below:
```python
x = float(1)     # x will be 1.0
y = float(2.8)   # y will be 2.8
z = float('3')   # z will be 3.0
w = float('4.2') # w will be 4.2

x = str('s1') # x will be 's1'
y = str(2)    # y will be '2'
z = str(3.0)  # z will be '3.0'

x = int(1)   # x will be 1
y = int(2.8) # y will be 2
z = int('3') # z will be 3
```

#### String formating using {}
string has a .format() method  used to format methods. It uses {} as a placeholder variables
See examples
```python
# string Format using {}
print('The sum of 1 + 2 is ', 1+2)

# can also be written as
print('The sum of 1 and 2 is {}'.format(1+2)) 
# Result -> The sum of 1 and 2 is 3

# Another example
print('The product of {} and {} is {}'.format(2, 3, 2*3)) # These are positional
# Result -> The product of 2 and 3 is 6

#Can use index to change the variable positions
print('The product of {2} and {0} is {1} '.format(2*3, 2, 3)) # The position has been changed by using indexes
# Result -> The product of 2 and 3 is 6
``` 

#### Float formatting in strings
See examples
```python
# To 2 decimal places
print('{} divided by {} is {:.2f} '.format(10, 3, 10/3))
# Result -> 10 divided by 3 is 3.33
```

To learn more about python formatting, go to [pyformat.info][pyformat.info]

[pypl]: http://pypl.github.io/PYPL.html
[colab]:   http://colab.research.google.com/
[sample-code]: #
[pyformat.info]: https://pyformat.info/

