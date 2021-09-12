writing text to a file

### writing text to a file

note:
1. read looks for an existing file
2. write can create new file
3. if you use existing file in writing then new content will overwrite exiting file content

```python
with open("sample2.txt", "w") as myfile:
	myfile.write("hellow world\nhow are you")
```

define a function that takes a char and path and return number of occurance in that file

```python
def charcount(char, path):
    with open(path) as myfile:
        content = myfile.read()
        return content.count(char)
```

### append content to the existing file

to append use `a` but you can only write it but not read it

to do both read and append use `a+`

```python
with open("sample.txt", "a+") as myfile:
	myfile.write("\nhello")
	# above line already puts cursor to the last line so reading it now will return nothing
	myfile.seek(0) # use this to put cursor back to top then read the file
	content = myfile.read()
```