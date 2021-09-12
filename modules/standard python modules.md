standard python modules

### standard python modules

How would you check if a file in a directory exists or not, because if you are reading a non existent file in python program then you get an error.

you would probably looks os related commands .e.g whether path.exists?

python also provides some standard python modules which is not builtin but they exists as separate modules and get installed with python installation.

### find location of os.py modules
```python
import sys
sys.prefix

# copy the path and open that folder, you can also use terminal in mac to open folder as

$ open /Library/Frameworks/Python.framework/Versions/3.9/lib/python3.9 # here you will see all the standard modules

dir(os) # look for function that check existence of a file

e.g
os.path.exists("files/log.txt")
```

sample program:

```python
import os
import time

while True:
	if os.path.exists("files/log.txt"):
		with open("files/log.txt") as myfile:
			print(myfile.read())
		else:
			print("File does not exist.")
		time.sleep(10)
```