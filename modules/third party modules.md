third party modules

### third party modules

In the previous example we used text file and how you would read a csv of day min/max temperature and return average of it?

you would need something better than reading a text file because text file read will return all content as a string and you would to do some text procession to extract the data and do type conversion then calculate mean. 

To read the csv we can use a third party package/module called `pandas`

You can install pandas as 
`$ pip install pandas` - it will install in your python framework directory

### use panda to read csv and calc mean

```python
import os
import time
import pandas

while True:
	if os.path.exists("files/temp.csv"):
			data = pandas.read_csv("files/temp.csv")
			print(data.mean())
			print(data.mean()['col']
		else:
			print("File does not exist.")
		time.sleep(10)
```

Note: type(data) is
`pandas.code.frame.DataFrame`
its a custom datatype, you can create your own datatype.