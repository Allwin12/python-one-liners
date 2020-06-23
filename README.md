This github repo is a collection of amazing python one liners.

* [quick sort](#quick-sort)
* [sum of n consecutive numbers](#sum-of-n-consecutive-numbers)
* [swap two numbers](#swap-two-numbers)
* [fibonacci series](#fibanocci-series)
* [flat list out of list of lists](#flat-list-out-of-list-of-lists)
* [starting a http server](#starting-a-http-server)
* [reverse a list](#reverse-a-list)
* [factorial of a number](#factorial-of-a-number)
* [list comprehension](#list-comprehension)
* [set comprehension](#set-comprehension)
* [dictionary comprehension](#dictionary-comprehension)
* [if-else](#if-else)
* [check data type](#check-data-type)
* [while loop](#while-loop)
* [write to a file using print](#write-to-a-file-using-print)
* [count occurence of a character in a string](#count-occurence-of-a-character-in-a-string)
* [merge two lists](#merge-two-lists)
* [merge two dictionaries](#merge-two-dictionaries)
* [merge two sets](#merge-two-sets)
* [get timestamp](#get-timestamp)
* [repeat values in a list for n times](#repeat-values-in-a-list-for-n-time)
* [generate a random number of n digits](#generate-a-random-number-of-n-digits)
* [convert key value pair to dictionary](#convert-key-value-pair-to-dictionary)
* [get quotient and remainder](#get-quotient-and-remainder)
* [python zen](#python-zen)
* [remove duplicate elements from a list](#remove-duplicate-elements-from-a-list)

### quick sort
```python
qsort = lambda l : l if len(l)<=1 else qsort([x for x in l[1:] if x < l[0]]) + [l[0]] + qsort([x for x in l[1:] if x >= l[0]])
```

### sum of n consecutive numbers
```python
sum(range(0, n+1)
```

### swap two values
```python
a,b = b,a
```

### fibonacci series
```python
lambda x: x if x<=1 else fib(x-1) + fib(x-2)
```

### flat list out of list of lists
``` python
[item for sublist in main_list for item in sublist]
```

### starting a http server
```python
python3 -m http.server 8000
```

### reverse a list
```python
numbers[::-1]
```

### factorial of a number
```python
import math; fact_5 = math.factorial(5)
```

### list comprehension
```python
li = [num for num in range(0,100)]
# this will create a list of numbers from 0 to 99
```

### set comprehension
```python
num_set = { num for num in range(0,100)}
# this will create a set of numbers from 0 to 99
```

### dictionary comprehension
```python
dict_numbers = {x:x*x for x in range(0,5) }
```

### if else
```python
print("even") if 4%2==0 else print("odd")
```

### check data type
```python
isinstance(2, int)
isinstance("allwin", str)
isinstance([3,4,1997], list)
```

### while loop
```python
a=5
while a > 0: a = a - 1; print(a)
```

### write to a file using print
```python
print("Hello, World!", file=open('file.txt', 'w'))
```

### count occurence of a character in a string
```python
print("umbrella".count('l'))
```

### merge two lists
```python
list1.extend(list2)
# contents of list 2 will be added to the list1
```

### merge two dictionaries
```python
dict1.update(dict2)
# contents of dictionary 2 will be added to the dictionary 1 
```

### merge two sets
```python
set1.update(set2)
# contents of set2 will be copied to the set1
```

### get timestamp
```python
import time; print(time.time())
```

### repeat values in a list for n time
```python
import itertools; print(list(itertools.repeat(10,5)))
# [10, 10, 10, 10, 10] will be printed
```

### generate a random number of n digits
```python
from random import randint; print(''.join(["{}".format(randint(0, 9)) for num in range(0, n)]))
# This will print 1038496714 given the value of n=10
```

### convert key value pair to dictionary
```python
dict(name='allwin', age=23)
```

### get quotient and remainder
```python
quotient, remainder = divmod(4,5)
```

### python zen
```python
import this
```

### remove duplicate elements from a list
```python
list(set([4, 4, 5, 5, 6]))
```
