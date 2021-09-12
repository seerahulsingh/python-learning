functions

functions
1. The first statement of a function can be an optional statement - the documentation string of the function or docstring.

2. The code block within every function starts with a colon (:) and is indented.

3. The statement return expression exits a function, optionally passing back an expression to the caller. A return statement with no arguments is the same as `return None`. Type of None is NoneType.

Note: None is also an object in python which means nothing

syntax:

```python
def functionname( parameters ):
   "function_docstring"
   function_suite
   return [expression]
```

* don't forget to put colon next to methodname

Note: 
1. when you print(type(mean)) it will return class `function`
2. when you print(type(sum)) it will return class `builtins_function_or_method`

Just try these in shell and see the output

### default/non-default, keyword/non-keyword function

```python
# positional/ non keyword function example
def area(a,b):
	return a * b
print(area(3,4))

# non positional / keyword function example
def area(a,b):
	return a * b
print(area(b=3,a=4)) # position of params doesnt matter because its named keyword params

# default & non default params example
def area(a,b=6):
	return a * b
print(area(3))
print(area(a=3))
print(area(3, b=3))
print(area(3,4))
```

Note: non default params should be written first then followed by default prams
e.g `def(a=1,b)` will raise syntax err

### arbitrary number of non keyword arguments

e.g `print()` function can take any number of arguments

```
def mean(*args)
		return sum(args) / len(args)
		
print(mean(3,4,56,76))

# note that when print type(args) its actually a tuple
```

### arbitrary number of keyword arguments

```python
def mean(**kwargs):
	print(type(kwargs)) # its a dict type

mean(a=1, b=3, c=6)
```