This github repo is a collection of amazing python one liners.

* quick sort
* sum of n consecutive numbers

### quick sort
```python
qsort = lambda l : l if len(l)<=1 else qsort([x for x in l[1:] if x < l[0]]) + [l[0]] + qsort([x for x in l[1:] if x >= l[0]])
```
### sum of n consecutive numbers

```python
sum(range(0, n+1)
```
