opening files using `with`

### opening files using `with`

```python
with open('sample.txt') as myfile:
	content = myfile.read()
	
print(content)

# we dont need to close file here because of once you are out of with block it gets closed automatically
```