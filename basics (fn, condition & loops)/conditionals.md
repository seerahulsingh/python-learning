conditionals

### conditionals

```python
if 1==1:
	print('hi')
else:
	print('bye')
```

as you can see if else block also starts with colon(:) and is indented

### Using "and" and "or" in a Conditional

You learned to check for one single condition:
```
x = 1
 
if x == 1:
    print("Yes")
else:
    print("No")
```
You can also check if two conditions are met at the same time using an and operator:
```
x = 1
y = 1
 
if x == 1 and y==1:
    print("Yes")
else:
    print("No")
```
That will return Yes since x == 1 and y ==1 are both True.

You can also check if one of two conditions are met using an or operator:
```
x = 1
y = 1
 
if x == 1 or y==2:
    print("Yes")
else:
    print("No")
```
That will return Yes since at least one of the conditions is True. In this case x == 1 is True.

### Check these in shell
```
type(3) == int
isinstance(3, int)
```

Both will return true but always prefer isinstance instead of type

Note: True & False also another data type in python called bool

so `type(True) == bool` is true

### elif conditional
```python
x = 3
y = 1

if x > y:
	print('x is greater than y')
elif x == y:
	print('x is equal to y')
else:
	print('x is less than y')
```