This github repo is a collection of amazing python one liners.

# A
* [anagram](#anagram)

# B
* [binary to decimal](#binary-to-decimal)

# C
* [check data type](#check-data-type)
* [combine strings from a list](#combine-strings-from-a-list)
* [combine two lists to dictionary](#combine-two-lists-to-dictionary)
* [common element between two lists](#common-element-between-two-lists)
* [convert decimal to binary](#convert-decimal-to-binary)
* [convert decimal to octal](#convert-decimal-to-octal)
* [convert decimal to hexadecimal](#convert-deciaml-to-hexadecimal)
* [convert a list of strings to integers](#convert-a-list-of-strings-to-integers)
* [convert key value pair to dictionary](#convert-key-value-pair-to-dictionary)
* [convert string to lower case](#convert-string-to-lower-case)
* [convert string to upper case](#convert-string-to-upper-case)
* [convert string to bytes](#convert-string-to-bytes)
* [copy files](#copy-files)
* [count occurence of a character in a string](#count-occurence-of-a-character-in-a-string)

# D
* [dictionary comprehension](#dictionary-comprehension)
* [deleting multiple elements from a list](#deleting-multiple-elements-from-a-list)

# E
* [execute strings](#execute-strings)

# F
* [fibonacci series](#fibanocci-series)
* [fizzbuzz](#fizzbuzz)
* [flat list out of list of lists](#flat-list-out-of-list-of-lists)
* [factorial of a number](#factorial-of-a-number)
* [floor division result](#floor-division-result)
* [for and if](#for-and-if)

# G
* [generate a random number of n digits](#generate-a-random-number-of-n-digits)
* [get a string of small case alphabets](#get-a-string-of-small-case-alphabets)
* [get a string of upper case alphabets](#get-a-string-of-upper-case-alphabets)
* [get a string of digits from 0 to 9](#get-a-string-of-digits-from-0-to-9)
* [get even numbers from a list](#get-even-numbers-from-a-list)
* [get individual digits from a number](#get-individual-digits-from-a-number)
* [get timestamp](#get-timestamp)
* [get quotient and remainder](#get-quotient-and-remainder)

# H
* [half pyramid](#half-pyramid)
* [hexadecimal to decimal](#hexadecimal-to-decimal)
* [hypotenuse](#hypotenuse)
* [human-readable-datetime](#human-readable-datetime)

# I
* [if-else](#if-else)
* [infinite-while-loop](#infinite-while-loop)
* [input a list of tuples](#input-a-list-of-tuples)

# L
* [lambda function with if else](#lambda-function-with-if-else)
* [longest string in a list](#longest-string-in-a-list)
* [list comprehension](#list-comprehension)

# M
* [merge two lists](#merge-two-lists)
* [merge two dictionaries](#merge-two-dictionaries)
* [merge two sets](#merge-two-sets)
* [most frequnet element in a list](#most-frequent-element-in-a-list)

# N
* [nested list comprehension](#nested-list-comprehension)

# O
* [object creation](#object-creation)
* [octal to decimal](#octal-to-decimal)

# P
* [permutation](#permutation)
* [python zen](#python-zen)

# Q
* [quick sort](#quick-sort)

# R
* [remove duplicate elements from a list](#remove-duplicate-elements-from-a-list)
* [remove numbers from string](#remove-numbers-from-string)
* [repeat values in a list for n times](#repeat-values-in-a-list-for-n-time)
* [replace words in a sentence](#replace-words-in-a-sentence)
* [rotate a list](#rotate-a-list)
* [reverse a list](#reverse-a-list)

# S
* [set comprehension](#set-comprehension)
* [sort dictionary with values](#sort-dictionary-with-values)
* [sort dictionary with key](#sort-dictionary-with-key)
* [sort list in ascending order](#sort-list-in-ascending-order)
* [sort list in descending order](#sort-list-in-descending-order)
* [substring in a string](#substring-in-a-string)
* [sum of n consecutive numbers](#sum-of-n-consecutive-numbers)
* [starting a http server](#starting-a-http-server)
* [swap two numbers](#swap-two-numbers)

# T
* [transpose matrix](#transpose-matrix)

# U
* [Unpacking elements](#unpacking-elements)

# W
* [while loop](#while-loop)
* [write to a file using print](#write-to-a-file-using-print)


### anagram
```python
from collections import Counter

s1 = 'below'
s2 = 'elbow'

print('anagram') if Counter(s1) == Counter(s2) else print('not an anagram')
```

### binary to decimal
```python
decimal = int('1010', 2)
print(decimal) #10
```
### convert decimal to binary
```python
bin(24)
```

### convert decimal to hexadecimal
```python
hex(24)
```

### convert decimal to octal
```python
oct(24)
```

### convert key value pair to dictionary
```python
dict(name='allwin', age=23)
```

### convert string to lower case
```python
"Hi my name is Allwin".lower()
# 'hi my name is allwin'
"Hi my name is Allwin".casefold()
# 'hi my name is allwin'
```

### convert string to upper case
```python
"hi my name is Allwin".upper()
# 'HI MY NAME IS ALLWIN'
```

### convert string to bytes
```python
"convert string to bytes using encode method".encode()
# b'convert string to bytes using encode method'
```

### copy files
```python
import shutil; shutil.copyfile('source.txt', 'dest.txt')
```

### deleting multiple elements from a list
```python
li = [1, 2, 3, 4, 5]
del li[0:3] 
# [4, 5]
```

### execute strings
```
exec('print("hello world!")')
# hello world!
```

### fibonacci series
```python
lambda x: x if x<=1 else fib(x-1) + fib(x-2)
```

### fizzbuzz
```python
n = 20
print('\n'.join('Fizz' * (i%3==0) + 'Buzz' * (i%5==0) or str(i) for i in range(1, n)))

1
2
Fizz
4
Buzz
Fizz
7
8
Fizz
Buzz
11
Fizz
13
14
FizzBuzz
16
17
Fizz
19
```

### half pyramid
```python
n = 5
print('\n'.join('* ' * i for i in range(1, n + 1)))

*
* *
* * *
* * * *
* * * * *
```

### quick sort
```python
qsort = lambda l : l if len(l)<=1 else qsort([x for x in l[1:] if x < l[0]]) + [l[0]] + qsort([x for x in l[1:] if x >= l[0]])
```

### sum of n consecutive numbers
```python
sum(range(0, n+1))
```

### swap two values
```python
a,b = b,a
```

### flat list out of list of lists
``` python
[item for sublist in main_list for item in sublist]
```

### starting a http server
```python
python3 -m http.server 8000
python2 -m SimpleHTTPServer
```

### reverse a list
```python
numbers[::-1]
```

### factorial of a number
```python
import math; fact_5 = math.factorial(5)
```

### floor division result
```python
print(5//2)
# 2
```

### for and if
```python
new_li = [number for number in [1, 2, 3, 4] if number % 2 == 0]
# [2, 4]
```

### lambda function with if else
```python
list(map(lambda x: x if x%2==0 else x+1, [1, 2, 3, 4]))
# [2, 2, 4, 4]
# converts only odd numbers to even numbers by adding 1 to it
```

### longest string in a list
```python
# words = ['This', 'is', 'a', 'list', 'of', 'words']
max(words, key=len)
# 'words'
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

### infinite while loop
```python
while 1:0
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

### most frequent element in a list
```python
numbers = [9, 4, 5, 4, 4, 5, 9, 5, 4]
most_frequent_element = max(set(test_list), key=test_list.count)
# 4
```
```python
from collections import Counter

numbers = [9, 4, 5, 4, 4, 5, 9, 5, 4]
print(list(Counter(numbers).most_common()))
# [(4, 4), (5, 3), (9, 2)]
```

### nested list comprehension
```python
numbers = [[num] for num in range(10)]
# [[0], [1], [2], [3], [4], [5], [6], [7], [8], [9]]
```

### object creation
```python
obj_1 = type('obj_1', (object,), {'property': 'value'})()
```

### octal to decimal
```python
print(int('30', 8)) 
# 24
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

### sort list in ascending order
```python
sorted([5, 2, 9, 1])
```

### sort list in descending order
```python
sorted([5, 2, 9, 1], reverse=True)
```

### get a string of small case alphabets
```python
import string; print(string.ascii_lowercase)
# abcdefghijklmnopqrstuvwxyz
```

### get a string of upper case alphabets
```python
import string; print(string.ascii_uppercase)
# ABCDEFGHIJKLMNOPQRSTUVWXYZ
```

### get a string of digits from 0 to 9
```python
import string; print(string.digits)
# 0123456789
```

### get individual digits from a number
```python
digits = [int(digit) for digit in str(12345)]
```

### hexadecimal to decimal
```python
print(int('da9', 16))
# 3497 
```

### hypotenuse
```python
import math; math.hypot(8, 6)
```

### human readable datetime
```python
import time; print(time.ctime())
# Thu Aug 13 20:16:23 2020
```

### convert a list of strings to integers
```python
list(map(int, ['1', '2', '3']))
# [1, 2, 3]
```

### combine strings from a list
```python
" ".join(["hello", "world"])
# "hello world"
```

### combine two lists to dictionary
```python
dict(zip([1,2,3,4], ['a','b','c','d']))
{1: 'a', 2: 'b', 3: 'c', 4: 'd'}
```

### common element between two lists
```python
list1 = [1, 2, 4, 5]
list2 = [6, 8, 4, 2]

print(set(list1) & set(list2))
print(set(list1).intersection(set(list2)))
# {2, 4}
```

### get even numbers from a list
```python
list(filter(lambda x: x%2 == 0, [1, 2, 3, 4, 5, 6] ))
# [2, 4, 6]
```

### input a list of tuples
```python
list(tuple(map(int, input().split())) for r in range(int(input('enter the no of rows:'))))
# enter the no of rows:
# 3
# 1 2
# 3 4
# 5 6
# [(1, 2), (3, 4), (5, 6)]
```

### permutation
```python
from itertools import permutations
print([''.join(perm) for perm in permutations('abc')])

# ['abc', 'acb', 'bac', 'bca', 'cab', 'cba']
```

### remove numbers from string
```python
''.join(list(filter(lambda x: x.isalpha(), 'abc123def4fg56vcg2')))
# abcdeffgvcg
```

### replace words in a sentence
```python
string = "He is a good boy"
string.replace('good', 'bad')
# returns 'he is a bad boy'
```

### rotate a list
```python
# li = [1,2,3,4,5]
# right to left
li[n:] + li[:n] # n is the no of rotations
li[2:] + li[:2]
[3, 4, 5, 1, 2]
# left to right
li[-n:] + li[:-n]
li[-1:] + li[:-1] 
[5, 1, 2, 3, 4]
```

### sort dictionary with values
```python
# x = {1: 2, 3: 4, 4: 3, 2: 1, 0: 0}
{k: v for k, v in sorted(x.items(), key=lambda item: item[1])}
# {0: 0, 2: 1, 1: 2, 4: 3, 3: 4}
```

### sort dictionary with key
```python
# {'one': 1, 'four': 4, 'eight': 8}
{key:d[key] for key in sorted(d.keys())}
# {'eight': 8, 'four': 4, 'one': 1}
```

### substring in a string
```python
'sent' in 'sentence'
# returns True
```

### transpose matrix
```python
list(list(x) for x in zip(*old_list))
# old_list = [[1, 2, 3], [3, 4, 6], [5, 6, 7]]
# [[1, 3, 5], [2, 4, 6], [3, 6, 7]]
```

### unpacking elements
```python
a, *b, c = [1, 2, 3, 4, 5]
print(a) # 1
print(b) # [2, 3, 4]
print(c) # 5
```
