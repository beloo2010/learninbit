---
title: "Python Intro"
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
  nav: "docs"
---

Python is an interpreted programming language. According to [pypl][pypl], Python is one of the most popular languages out there. This will introduce you to the basic. To run a python code, you need to install a python interpreter. It comes by default on most linux machine. Just open a terminal, type python and enter. For this, we will be using Google [colab][colab]. I have shared a [sample code][sample-code]. feel free to make a copy and follow along.

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
By default, the print statement appends a new line after every print. To avoid that, use the "end" parameter.
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

See sample below
```python
print('a', 'b') #Result -> ab
print('a' + 'b') #Result -> ab
print('a', 5) #Result -> a5
print('a'+ 5) #Result ->Error
print(5 + 5) #Result -> 10
```

#### Print and New Line
By default, print statement adds a new line after print. To remove new lines, change the end parameter
See sample below
```python
print('one')
print('two') 
# This will be printed on 2 lines. To print those on a single line
print('one', end = ' ')
print('two') # Result -> one two
```

#### Variable Naming
These are legal variable names
2myvar = "John"
my-var = "John"
my var = "John"
{: .notice--info}


These are illegal variable names
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
{: .notice--warning}

[pypl]: http://pypl.github.io/PYPL.html
[colab]:   http://colab.research.google.com/
[sample-code]: #

