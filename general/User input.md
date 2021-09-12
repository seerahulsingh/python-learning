User input

User input

lets understand this with an example:

```python
def weather_condition(temprature):
	if temperature > 10;
		return 'Warm'
	else:
		return 'Cold'

user_input = float(input('Enter the temperature: '))
print(weather_condition(user_input))
```

When you run this program will stop at input line and will continue once you type any value and hit enter.

As you can see we did the datatype conversion as well because enterred value will always be treated as string.