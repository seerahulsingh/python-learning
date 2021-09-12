loops

# loops

### for loop examples

```python
temp = [9.1, 8.8, 7.6]
for temperature in temp:
	print(round(temperature))
	
for letter in 'Hello':
	print(letter.lower())
```

### looping through dict

```python
grades = { x: "12", y: "23", z: "21" }

for grade in grades.items():
	print(grade)
	
output will be tuple of key value pair
```
You can also loop on keys() and values() of dict.

### Dictionary Loop and String Formatting
You can combine a dictionary for loop with string formatting to create text containing information from the dictionary:

```python
phone_numbers = {"John Smith": "+37682929928", "Marry Simpons": "+423998200919"}
 
for pair in phone_numbers.items():
    print("{} has as phone number {}".format(pair[0], pair[1]))
```

Another (better) way to do it::

```python
phone_numbers = {"John Smith": "+37682929928", "Marry Simpons": "+423998200919"}
 
for key, value in phone_numbers.items():
    print("{} has as phone number {}".format(key, value))
```
In both cases the output is:

Output:

John Smith has as phone number +37682929928

Marry Simpons has as phone number +423998200919

### while loop

```python
x = 3
while x > 3:
	print("hi")
	
username = ''
while username != 'pypy':
	username = input('Enter username: ')
```

### break & continue

```python
while True:
	username = input('Enter username: ')
	if username == 'pypy':
		break;
	else:
		continue;
```