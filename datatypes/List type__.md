List type**

**List type**

List is same as an array in other programming languages

examples are

scores = [2, 5, 7]

data = [1, 2, 'hello']

data2 = [1, 2, ['hi', 4]

Note: To get the number of similar items in a list, you can use count(val) functions - you can always find the right function with helper of dir/help methods

e.g

```
student_grades = [9.1, 8.8, 10.0, 7.7, 6.8, 8.0, 10.0, 8.1, 10.0, 9.9]
print(student_grades.count(10.0))
```

## slices

You can get range of values from list. The upper limit is not included 
e.g 1:3 will arr[1] && arr[2] only

```
arr = [2.3, 5.4, 6.7, 8.0, 11]
arr[1:4] == [5.4,6.7,8.0]
arr[0:2] && arr[:2] and arr[-5:-3] will return same output
arr[3:5] && arr[3:] && arr[-2:] will return same output
```

You can also negative indexing to get thee array values

### Note - 
strings also has both postive and negative indexing and you can use slicing on strings as well

```
name = 'rahul'
print(name[0]) == 'r'

arr = ['rahul', 1, 3]
print(arr[0][2]) == 'h'
```