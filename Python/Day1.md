# Table of Contents
- [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
    - [Origin](#origin)
    - [Why Python?](#why-python)
    - [Advantages](#advantages)
    - [Usages](#usages)
      - [Web](#web)
      - [Medical research](#medical-research)
      - [Fintech companies](#fintech-companies)
    - [Zen of Python](#zen-of-python)
    - [Python implementations](#python-implementations)
    - [Download and Install Python](#download-and-install-python)
    - [pip - package installer for python](#pip---package-installer-for-python)
    - [How to run Python code](#how-to-run-python-code)
      - [IDLE - Integrated Development and Learning Environment.](#idle---integrated-development-and-learning-environment)
    - [Hello World](#hello-world)
    - [Python Keywords](#python-keywords)
    - [Printing output](#printing-output)
- [Python 3.x program showing how to print data on a screen](#python-3x-program-showing-how-to-print-data-on-a-screen)
- [One object is passed](#one-object-is-passed)
- [Two objects are passed](#two-objects-are-passed)
- [code for disabling the softspace feature](#code-for-disabling-the-softspace-feature)
- [using end argument - does not print subsequent lines on a new line](#using-end-argument---does-not-print-subsequent-lines-on-a-new-line)
    - [Data Types in Python](#data-types-in-python)
      - [Integers](#integers)
- [define in base 2 / binary](#define-in-base-2--binary)
- [define in base 8 / octal](#define-in-base-8--octal)
- [define in base 16 / hexa](#define-in-base-16--hexa)
        - [Arithmetic Operations](#arithmetic-operations)
        - [Math Functions](#math-functions)
      - [Floating-Point](#floating-point)
      - [Boolean](#boolean)


## Introduction

### Origin
* Python was conceived in the late 1980s by Guido van Rossum at Centrum Wiskunde & Informatica (CWI) in the Netherlands as a successor to the ABC language (itself inspired by SETL), capable of exception handling and interfacing with the Amoeba operating system. Its implementation began in December 1989.
* Van Rossum shouldered sole responsibility for the project, as the lead developer, until 12 July 2018, when he announced his "permanent vacation" from his responsibilities as Python's Benevolent Dictator For Life, a title the Python community bestowed upon him to reflect his long-term commitment as the project's chief decision-maker.
* Python 2.7's end-of-life date was initially set at 2015 then postponed to 2020 out of concern that a large body of existing code could not easily be forward-ported to Python 3.

### Why Python?
The OpenStack community chose Python as the exclusive
development language for the project and requires all
new development to be in Python as well. The founders
of the community chose Python for the following reasons:
• Rapid Product Development – Leverage of a variety of
pre-existing tools and components
• Infrastructure Flexibility – Python allows for internal
infrastructure swapping of components with significantly less coding required
• Future Proof – The rapidly growing Python community
delivers a plethora of new projects to leverage for the
benefit of OpenStack
• Open Source – As an open source community, OpenStack believes in supporting other open source projects by consuming their deliverables and also giving
back

### Advantages

* Python is one of the best programming languages for current Agile era. 
* Python programs are shorter when compared to Java, C or any other high-level language => 
  - shorter development time
  - Reduced costs
  - Fewer errors
* There are many high quality solutions available standard library and thousands of additional libraries in the Python Package Index.
* Once programmed, Python applications can
run on all operating systems for which a Python interpreter
exists, significantly reducing the cost of operating-system specific applications.
  
### Usages

#### Web
* support.mozilla.com
* Firefox Sync Server
The Firefox Sync Server, which is used to synchronize bookmarks, browsing
histories, passwords, and open tabs on different computers and mobile
devices, was also written in Python.
* Google uses Python in its search functionality.
  
#### Medical research
#### Fintech companies

### Zen of Python
The principles are listed as follows:

* Beautiful is better than ugly.
* Explicit is better than implicit.
* Simple is better than complex.
* Complex is better than complicated.
* Flat is better than nested.
* Sparse is better than dense.
* Readability counts.
* Special cases aren't special enough to break the rules.
* Although practicality beats purity.
* Errors should never pass silently.
* Unless explicitly silenced.
* In the face of ambiguity, refuse the temptation to guess.
* There should be one—and preferably only one—obvious way to do it.
* Although that way may not be obvious at first unless you're Dutch.
* Now is better than never.
* Although never is often better than right now.
* If the implementation is hard to explain, it's a bad idea.
* If the implementation is easy to explain, it may be a good idea.
* Namespaces are one honking great idea—let's do more of those!

<pre> >>>import this</pre>

### Python implementations

* CPython - interpreter written in C. Most used defacto implementation.
* JPython - interpreter written in Java. This enables Python to be used in Java. All java libraries can be imported and used.
* IronPython - interpreter written in C#.

### Download and Install Python

### pip - package installer for python
<pre> pip install jupyterlab </pre>

### How to run Python code

#### IDLE - Integrated Development and Learning Environment.


* Save file as filename.py
* Command line using <pre>python filename.py</pre>
* Or, use IDLE editor.

### Hello World
<pre>
print("Hello World!")
</pre>

### Python Keywords
<pre>
  import keyword 
  print (keyword.kwlist) 
</pre>

### Printing output
<pre>Syntax: print(value(s), sep= ‘ ‘, end = ‘\n’, file=file, flush=flush)</pre>

<pre>
# Python 3.x program showing how to print data on a screen 
    
  # One object is passed 
  print("hello") 
    
  x = 5
  # Two objects are passed 
  print("x =", "10") 
    
  # code for disabling the softspace feature  
  print('a', 'b', 'c', sep ='-') 
    
  # using end argument - does not print subsequent lines on a new line
  print("Python", end = '@')   
  print("Chennai")  

  print('a','b', sep='', end='') 
  print('c') 
  #\n provides new line after printing the year 
  print('09','12', sep='-', end='-2016\n') 
</pre>

### Data Types in Python

#### Integers
* Whole numbers

* Default base used is base10, but can be converted or displayed in other bases.

* Any limit allowed up to memory limit of computer

<pre>
a = 10
b = 5
print(a, b)
print(type(a), type(b))
</pre>

* Defining different bases for integers

<pre>
# define in base 2 / binary
c = 0b00110110
print(c)
print(type(c))
# define in base 8 / octal
d = 0o452300
print(d)
print(type(d))
# define in base 16 / hexa
e = 0x234A2B
print(e)
print(type(e))
</pre>

* A given integer in base 10 decimal can be converted in to other bases using built-in functions such as bin, oct, hex, etc..

<pre>
f = 1130
print(bin(f))
print(oct(f))
print(hex(f))
</pre>

* A TypeError will be thrown when an mathematical operation is done on none integer.

<pre>
num1 = '4'
num2 = 1
print(type(num1), '|', type(num2))
print(num1 + num2)
</pre>

##### Arithmetic Operations
<pre>
  print(5 + 3)  # Addition
  print(5 * 3)  # Multiplication
  print(5 - 3)  # Subtraction
  print(5 / 3)  # Division returns quotient in decimal number
  print(5 // 3) # Division returns quotient in whole number
  print(5 % 3)  # Modulo returns Remainder
  print(5 ** 3) # Exponent
</pre>

##### Math Functions
* Built-in math functions
<pre>
x = 2.9
print(round(x))    #rounds up
print(abs(x * -1)) #asolute value
</pre>

* math module for complex mathematical functions.
<pre>
  import math
  print(math.ceil(2.9))  #ceil value
  print(math.floor(2.9)) #floor value
  print(math.factorial(3)) #factorial
</pre>


#### Floating-Point

* Any number with a decimal point.
* Division result will be a float.
* Can be defined using scientific notations (0.09 as 9 x 10^-2)
  <pre>
  print(type(0.5))  #type is float if decimal is used
  print(type(0.5 + 0.4))
  print(type(10 / 2)) #result of division is a float
  print(type(10 // 2)) #integer division
  print(9e-3 , '==>', type(9e-3)) #scientific notation

  #Beware of the precision errors that may creep up with Floating point arithmetic
  print(0.2 + 0.1)
  </pre>

#### Boolean
bool(x) -> bool Returns True when the argument x is true, False otherwise.
The builtins True and False are the only two instances of the class bool.
The class bool is a subclass of the class int, and cannot be subclassed.

<pre>
print(type('True'))
print(type(True))
</pre>