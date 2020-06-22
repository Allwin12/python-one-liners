This github repo is a collection of amazing python one liners.

* quick sort
* sum of n consecutive numbers
* swap two numbers
* fibonacci series
* flat list out of list of lists
* starting a http server


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
python3 -m http.server 9999
```
