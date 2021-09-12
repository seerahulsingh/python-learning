List comprehensions

### List comprehensions

Task - Lets say you have a list of numbers and want to divide by 10 and save in new list, how would you do it?

basic approach -
```python
arr = [100, 200, 300]
new_arr = []

for item in arr:
	new_arr.append(item / 10)
```

but you can use list comprehension to do this in 1 line using inline for loop

```
new_arr = [item / 10 for item in arr]
```

### using if conditional
e.g divide by 10 except -9999
```python
arr = [100, 200, 300, -9999, 600]
new_arr = [item / 10 for item in arr if item != -9999]
print(new_arr) => [10, 20, 30, 60]
```

### using if-else conditional
e.g divide by 10 and replace -9999 with 0
```python
arr = [100, 200, 300, -9999, 600]
new_arr = [item / 10 if item != -9999 else 0 for item in arr]
print(new_arr) => [10, 20, 30, 0, 60]
```