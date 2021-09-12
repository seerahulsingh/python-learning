string formatting

string formatting

This one will work in both python 2 and python 3

```python
user_input = input('Enter your name: ')
message = "Hello %s" % user_input 
```

Since python3.6 you can do the same as 

```python
user_input = input('Enter your name: ')
message = f"Hello {user_input}"
```

## formatting with multiuple variables

```python
name = input("Enter name: ")
surname = input("Enter surname: ")
when = "today"

message = "Hello %s %s" % (name, surname)
mesage = f"Hello {name} {surname}. What's up {when}"
```

### you can also format strings using .format() function
```python
name = "Sim"
experience_years = 1.5
print("Hi {}, you have {} years of experience".format(name, experience_years))
```