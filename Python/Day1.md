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
    - [PVM - for portability](#pvm---for-portability)
    - [Frozen Binaries](#frozen-binaries)
    - [Memory management](#memory-management)
    - [Download and Install Python](#download-and-install-python)
    - [Install useful packages](#install-useful-packages)
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
    - [Comments](#comments)
- [call functions](#call-functions)
    - [Help in Python](#help-in-python)
    - [How Python sees variables](#how-python-sees-variables)
    - [Data Types in Python](#data-types-in-python)
      - [None type](#none-type)
      - [Numeric types](#numeric-types)
        - [Integers](#integers)
- [define in base 2 / binary](#define-in-base-2--binary)
- [define in base 8 / octal](#define-in-base-8--octal)
- [define in base 16 / hexa](#define-in-base-16--hexa)
        - [Arithmetic Operations](#arithmetic-operations)
        - [Math Functions](#math-functions)
        - [Floating-Point](#floating-point)
        - [Complex numbers](#complex-numbers)
      - [Boolean](#boolean)
    - [Sequences in Python](#sequences-in-python)
      - [str](#str)
      - [bytes](#bytes)
- [create a list of numbers](#create-a-list-of-numbers)
- [convert list to bytes type array](#convert-list-to-bytes-type-array)
- [display elements from x](#display-elements-from-x)
      - [bytearray](#bytearray)
- [create a list of numbers](#create-a-list-of-numbers-1)
- [convert list to bytes type array](#convert-list-to-bytes-type-array-1)
- [display elements from x](#display-elements-from-x-1)
      - [list](#list)
      - [tuple](#tuple)
      - [range](#range)
    - [Sets](#sets)
      - [set Datatype](#set-datatype)
      - [frozenset Datatype](#frozenset-datatype)
    - [Mapping Datatypes](#mapping-datatypes)
- [can also do as follows -](#can-also-do-as-follows)
    - [Escape characters](#escape-characters)


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
* IronPython - interpreter written in C# for .NET framework.
* PyPy - written in Rpython. JIT compiler.
* RubyPython - written for Ruby applications.
* AnacondaPython - developed for large-scale data processing, predictive analysis and scientific computing.

### PVM - for portability

### Frozen Binaries 
* For final software, there are 2 ways to provide to end user.
  - Provide .pyc files to the user. User needs PVM to run the byte codes.
  - Provide .pyc files with PVM along with necessary Python library. Usually converted to an .exe file etc..that user can click and run. tese are called frozen binaries.
    * py2exe is a software that creates frozen binaries for windows.
    * pyinstaller or Freeze for Unix/Linux.

### Memory management
* Done Automatically during runtime. PVM takes care of it.
* Everything is an object in Python. All these are stored on heap memory (which is allocated during runtime). heap depends on RAM of our computer.
* Garbage collection -
  - Deletes objects which are not used in the program from memory.
  - gc / garbage collector classifies objects in to three generations. 
    - manages based on total counts of reference of objects in program and total counts of already used. when it reaches 0, gc deletes the object.
    - runs automatically based on a threshold value.  if no of allocations - no of deallocations > threshold value gc runs.
    - threshold value can be found using get_thresold() from gc module.
    - manual trigger of gc.collect() can be done based on time or event.


### Download and Install Python
* Add to PATH while installing. 
* Add a '.' at the end of the PATH to make Python run in any directory in out system.
  
### Install useful packages
* pip - package installer for python
<pre>pip install jupyterlab </pre>
<pre>pip install numpy</pre>
<pre>pip install matplotlib</pre>
<pre>pip install xlrd</pre>

* Verify modules installed using - 
<pre>>>> help('modules')</pre>


### How to run Python code

#### IDLE - Integrated Development and Learning Environment.


* Save file as filename.py
* Command line using <pre>python filename.py</pre>
* Or, use IDLE editor.

* To generate .pyc file - byte code equivalent.
<pre> python -m py_compile exp1.py </pre>

* To view byte code
<pre>python -m dis exp1.py</pre>

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

### Comments
* use '#' for comments
* use ''' or """ for multi-line comments - not in-built. this means multiline string. So memory is allocated. since these are not assigned to any variable gc deletes the object. Usually not recommended as it occupies space and wastes intrepreter's time. They have one use too.
* If written as first lines of a module or a function, they are called Docstrings and can be used to create API documentation.
  
<pre>
def add(x, y):
    '''
    This function does blah blah blah....
    '''
    print("Sum= ", (x + y))

def message():
    '''
    print("Welcome to Chennai")
    '''

# call functions
add(10, 25)
message()
</pre>

Now execute as below -
<pre> python -m pydoc -w file-name-without-extension </pre> 

-w indicates that .html file will be created



### Help in Python
* Use  help() - interactive. press enter without any input to exit interactive mode.
* Use help('print') - non-interactive. displays detais on the screen.

### How Python sees variables
* Python considers values as objects.
* While other languages has variables, Python uses them as tags to represent values.

### Data Types in Python

#### None type
* An object that does not contain any value.
* Similar to 'null' object in Java.
* Only one 'None' object is available in Python.
* One of the uses is it is used inside a function as a default value of the arguments when no value is passed while calling the function.
* 'None' object also represents 'False'

#### Numeric types

##### Integers 

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


##### Floating-Point

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

##### Complex numbers
* written in a + bj form. 
* a - real part
* b - imaginary part
* j - sq rt of -1

#### Boolean
bool(x) -> bool Returns True when the argument x is true, False otherwise.
The builtins True and False are the only two instances of the class bool.
The class bool is a subclass of the class int, and cannot be subclassed.

<pre>
print(type('True'))
print(type(True))
</pre>

### Sequences in Python
* sequence represents group of elements or items.

#### str 
* represents string datatype.
* enclosed within single quotes or double quotes.

#### bytes 
* represents group of byte numbers
* a byte number is a +ve number from 0 to 255 (inc).
* cannot be modified.
<pre>
# create a list of numbers
elements = [1, 3, 5, 7, 9]
# convert list to bytes type array
x = bytes(elements)

# display elements from x
for i in x: print(i)
</pre>

#### bytearray 
* similar to bytes, except that this can be modified.

<pre>
# create a list of numbers
elements = [1, 3, 5, 7, 9]
# convert list to bytes type array
x = bytearray(elements)

# display elements from x
for i in x: print(i)

x[0] = 0
x[1] = 9

for i in x: print(i)
</pre>

#### list
* represented by [ ] (square brackets) and elements are written in brackets as comma separated values
<pre> list1 = ['a', 1, 2, "c"] </pre>

* Similar to array in C or Java. 
Differences - 
* Can store different types of elements.
* Can grow dynamically in memory.
  

#### tuple
* Similar to Lists, but cannot be modified.
* represented by () (parantheses) with elements written as comma separated values.

<pre> tp1 = (1, 2, 3, "a", "hello") </pre>

#### range
* represents sequence of numbers. 
* non-editable.
* usually used for loops
  
<pre> 
r = range(10)
for i in r: print(i)  #displays from 0 to 9

r = range(30, 40, 2)
for i in r: print(i) 
#displays numbers from 30 to 40 with increments of 2. means 30, 32, 34, 36, 38
</pre>

### Sets
* unordered collection of elements.
* does not accept duplicate values.
  
#### set Datatype
* created using {} (curly brackets)
* Order of elements is not maintained.
* Cannot retrieve elements using indexing or slicing.
  
<pre> 
s = {1, 2, 3, 4, 5, 1, 4, 7}
print(s)  # displays only {1, 2, 3, 4, 5, 7} 
</pre>

* can use set() function convert a list to set.
<pre>
lst = [1, 2, 3, 4, 5]
s = set(lst)
print(s)
</pre>

* update() - to add elements to set
<pre>
s.update([50, 60])
print(s)
</pre>

* remove() - to remove elements from set
<pre>
s.remove(50)
print(s)
</pre>

#### frozenset Datatype
* elements cannot be modified.
  
<pre>
a = {1, 3, 5, 7, 9 }
print(a)

fa = frozenset(a)
print(fa)
</pre>

### Mapping Datatypes
* Dictionary is map datatype. All key-value elements should be enclosed in {} (curly braces).
* Key-value pairs. 
* If key is given value can be retrieved.
* Key-value separated by colon ':'

<pre>
 mp1 = {1 : 'Chennai', 2: 'Mumbai', 3: 'Delhi', 4:'Bangalore'}

# can also do as follows - 
#create empty dictionary
d1 = {}
d1[1] = 'Chennai'
</pre>

* d1[key] to fetch values for a key
* del d1[key] to delete the pair
* d1.keys() to display all keys
* d1.values() to display all values

### Escape characters
\n -> leaves a line <br>
\t -> leaves a tab space <br>
\\ -> backslash <br>
\' -> single quote <br>
\" -> double quote <br>