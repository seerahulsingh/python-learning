closing a file

### closing a file

When you open a file, it create an object in the memory and stays there untill the program ends

But if you wanna close the file early in the program then use .close() function on file object

```python
myfile = open('sample.txt')
content = myfile.read()
myfile.close()
```