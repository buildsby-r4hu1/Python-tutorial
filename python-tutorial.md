# Python Tutorials

## Contents

- [Python Tutorials](#python-tutorials)
  - [Contents](#contents)
    - [Printing](#printing)
    - [Concatenation](#concatenation)
    - [String Multiplication](#string-multiplication)
    - [String indexing](#string-indexing)
    - [Switch statement](#switch-statement)
    - [Ternary Operator](#ternary-operator)
    - [Multiple return](#multiple-return)
    - [random values](#random-values)
    - [Reading files](#reading-files)
    - [Writing files](#writing-files)
    - [String slicing](#string-slicing)
    - [Lambda function](#lambda-function)
    - [f string for precision](#f-string-for-precision)

### Printing

``` python
print("Hello World")
```

- `print` function adds a newline after printing on it's own.
- To prevent that we give it a parameter, `end = ' '`

    ```python
    print("hello",end=" ")
    print("World",end ='.')
    ```

    The output:

    ```python
    >>>Hello World.
    ```

- To type a multi-line string

    ```python
    print(''' 
    Your 
    Multi-line
    string
    ''')
    ```

    The output

    ```python
    Your 
    Multi-line
    String
    ```

### Concatenation

```python
one = "one"
two = "two"

print(one,two)
print(one + two)
```

The output:

```python
one two
onetwo
```

The comma adds a space, but not in concatenation

### String Multiplication

You can make a string a number of time, by multiplying it by that *integer*.

```python
tenrahul = "rahul " * 10
print(tenrahul)
```

The output:

```python
rahul rahul rahul rahul ... rahul
```

### String indexing

`name = rahul`

|character|r|a|h|u|l|
|-----|---|---|---|---|---|
|index|0|1|2|3|4|
|index|-1|-2|-3|-4|-5|

>name[-1]=name[len(name)-1]=l

### Switch statement

- Type 1

    ```python
    match argument:
        case arg1:
            code1
        case arg2:
            code2
        case_:
            code_default
    ```

- Type 2

    ```python
    match num:
        case 1 | 2:
            print('one or two')
    ```

- Type 3

    ```python
    match num:
        case num if num>0:
            print('positive')
    ```

In the 3rd type, you can match list, dict, and other data types as well like classes and not just numbers or strings

### Ternary Operator

Not much needed, yet

```python
min = "both are equal" if a==b else "a is greater" if a>b else "b is greater"

print("b is greater")[b>a]

print((lambda : "b is minimum", lambda: "a is minimum") [a<b]())

print({True: "a is minimum", False: "b is minimum"} [a<b])
```

### Multiple return

In order to return multiple items, we use commas in return statement

```python
def fun():
    #code
    return a,b,c

var1,var2,var3 = fun()
```

### random values

```python
import random
random.randint(a,b) #returns random integer in [a,b]
random.uniform(a,b) #return random float in [a,b]
```

### Reading files

`var = open('file_path','r')`

- Two arguments
- first is the file path, or the file name if exists in same directroy
- second is open mode, 'r' for read, 'w' for write, and 'a' for append
  
`content = var.read()`

- contents or file is saved in content
- You could also use `readline()` method to read line by line

### Writing files

```python
file = open('file.txt', 'w')
# 'w' or 'a' according to need
file.write('put me in the file!')
file.write('\nI am in the file now')

# very important to close the file
file.close()
```

Contents of file now :

put me in the file
I am in the file now

### String slicing

`string = 'The weather is nice today'`
`weather = string[4:11] #The last index is not included`

`last5 = strin[-5:] # leaving blank after or before colon means everything after or before respectively`

works even for list

### Lambda function

Anonymouse function

Syntax

`(lambda parameter:return_value)(argument)`

e.g. `(lambda yr:2025-yr)(2006)`

it returns your age

They're mostly used to make function factories

### f string for precision

`print(f'The value of pi is {PI:{1}.{5}}')`

{Value-to-print : {min-width}.{precision}}

>The valus of pi is 3.1416

<!--More will be added soon-->
