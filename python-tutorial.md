# Python Tutorials

### Printing

```
print("Hello World")
```

- `print` function adds a newline after printing on it's own.
- To prevent that we give it a parameter, `end = ' ' `
    ```
    print("hello",end=" ")
    print("World",end ='.')
    ```

    The output:
    ```
    >>>Hello World.
    ```
- To type a multi-line string
    ```
    print(''' 
    Your 
    Multi-line
    string
    ''')
    ```

    The output

    ```
    Your 
    Multi-line
    String
    ```

### Concatenation

```
one = "one"
two = "two"

print(one,two)
print(one + two)
```

The output:

```
one two
onetwo
```

The comma adds a space, but not in concatenation

### String Multiplication

You can make a string a number of time, by multiplying it by that *integer*.

```
10rahul = "rahul " * 10
print(10rahul)
```

The output:

```
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

    ```
    match argument:
        case arg1:
            code1
        case arg2:
            code2
        case_:
            code_default
    ```
- Type 2

    ```
    match num:
        case 1 | 2:
            print('one or two')
    ```

- Type 3

    ```
    match num:
        case num if num>0:
            print('positive')
    ```

In the 3rd type, you can match list, dict, and other data types as well like classes and not just numbers or strings

### Ternary Operator

Not much needed, yet
```
min = "both are equal" if a==b else "a is greater" if a>b else "b is greater"

print("b is greater")[b>a]

print((lambda : "b is minimum", lambda: "a is minimum") [a<b]())

print({True: "a is minimum", False: "b is minimum"} [a<b])
```

### Multiple return

In order to return multiple items, we use commas in return statement
```
def fun():
    #code
    return a,b,c

var1,var2,var3 = fun()
```

