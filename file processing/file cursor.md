file cursor

### file cursor

when you create file object using open() method the cursor location will be at the top of the file

when you write myfile.read(), it read the file top to bottom and then leaves the cursor at the bottom.

so if you type myfile.read() more than 1 time, you will get output only once and then spaces for futher reads

try this

```python
myfile = open("sample.txt)
print(myfile.read())
print(myfile.read())
```