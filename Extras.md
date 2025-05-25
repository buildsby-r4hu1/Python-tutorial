# Extras

## Contents

- [Extras](#extras)
  - [Contents](#contents)
    - [import this](#import-this)
    - [Changing case](#changing-case)
    - [Stripping Whitespaces](#stripping-whitespaces)
    - [Removing prefix](#removing-prefix)
    - [Big numbers](#big-numbers)
    - [Inerting elements in list](#inerting-elements-in-list)
    - [deleting elements from list](#deleting-elements-from-list)
    - [List sorting](#list-sorting)
    - [Using range() to make a list](#using-range-to-make-a-list)
    - [statistics with list of numbers](#statistics-with-list-of-numbers)
    - [Using get()](#using-get)

### import this

`import this`, running it, will print some set of admirable rules by Tim Peters, I'm love those rules.

### Changing case

For Capatalize `string.title()`

For Uppercase and Lowercase `string.upper()` and `string.lower()` respectively

### Stripping Whitespaces

For no extra whitespaces to right of string use `string.rstrip()`.

To left of string use `string.lstrip()`

For both sides use `string.strip()`

### Removing prefix

`string.removeprefix('prefix')` removes prefix from the string, if that prefix is at the start of string
e.g.

```python
url = 'https://github.com'
url = url.removeprefix('https://')
print(url)
```

The output is `github.com`, and prefix is removed

### Big numbers

`num = 10_000_000`, the interpreter will ignore these *underscores*, but you can use them in place of spaces

### Inerting elements in list

`append('')` adds item to last of list

For insetion we use `insert(index, 'item')` method

```python
names = ['Rahul', 'Rohan', 'Rishi']
names.inert(1,'Ravi')
print(names)
```

>['Rahul','Ravi','Rohan','Rishi']

### deleting elements from list

`pop()` method deletes item from last of list, and returns that last item

`pop(index)` does the name thing to the element that that index.

Another way is using `del`

```python
del names[1]
```

Removing using the name using `remove('item')` method

```python
names.remove('Rohan')
```

### List sorting

It's only __Alphabetical sort__

Permanent Sort

```python
list.sort()
list.sort(reverse = True)
```

Temporary sorted list

```python
sorted(list)
sorted(list).reverse()
```

### Using range() to make a list

`even-numbers = list(range(2,11,2))`

or

`even-numbers = [value*2 for value in range(1,6)]`

### statistics with list of numbers

```python
nums=[1,23,234,53,0]
min(nums) # 0
max(nums) # 234
sum(nums) # 311
```

### Using get()

if you're not sure if a key exists in dictionary, and want to access it's value if it exists, or show another value if doesn't exists, we could use get()

```python
value = list.get('key','no value assigned')
```

