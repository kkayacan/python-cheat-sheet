Comment
```
# Comment line
```

Variable declaration & assignment
```
i=100
f=0.4
s="Data Science"
```

Write on terminal
```
print(s)
print(i,f,s)
```

Create list
```
list1=[10,20,30,40,50]
```

Element access in list with index
```
list1[0]=5
print(list1[0])
```

List length
```
len(list1)
```

Add element to list
```
list1.append(60)
```

Slice list
```
# Returns elements from index 1 through index 3 (not 4)
list1[1:4]

# Returns elements from start through index 2
list1[:3]

# Returns elements from index 2 through end
list1[2:]

# Returns elements from index 4 through index 8 skipping 1
list1[4:9:2]
```

Index of element in list by value
```
cities.index("London")
```

Remove element from list by index
```
cities.pop(2)
del(cities[2])
```

Remove element from list by value
```
cities.remove("London")
```

Sort list
```
sorted(list1)
sorted(list1, reverse=True)
```

Reverse current order of list
```
list1.reverse()
```

Concatenate 2 lists
```
list1+list2
```

Create tuple
```
tuple1=(3.14,2.78,5.67,78.9)
```

Element access in tuple with index
```
print(tuple1[0])
```

Assign tuple elements to variables
```
a,b,c,d=tuple1
```

Create set
```
set1=set(cities)
set2=set(tuple1)
set3={15,25,35,45,55}
```

Add single element to set
```
set1.add("Paris")
```

Add multiple elements to set
```
set3.add(list1)
```

Add multiple elements to set
```
set3.update(list1)
```

Remove element from set by value
```
set1.discard("Paris")
```

Create dictionary
```
dict1={'A': 15.7, 'B': 19.59, 'C': 25.7, 'D': 17.15, 'E': 23.45}
dict2=dict([('A', 15.7), ('B', 19.59), ('C', 25.7), ('D', 17.15), ('E', 23.45)])
```

Get keys of dictionary
```
dict1.keys()
```

Get values of dictionary
```
dict1.values()
```

Element access in dictionary with key
```
dict["B"]=19.49
print(dict["B"])
```

Add elements to dictionary
```
dict1.update(dict3)
```

Remove all elements from dictionary
```
dict1.clear()
```

Get all elements of dictionary as a list
```
dict1.items()
```

Remove last element from dictionary
```
dict1.popitem()
```

Remove element from dictionary by key
```
dict1.pop("B")
```

Get type of data structure
```
type(tuple1)
```

Branching with "if"
```
if x>y:
    print("x is greater than y")
elif x==y:
    print("x is equal to y")
else:
    print("y is greater than x")
```

Check if value is in structure
```
s="Hello World"
if("Hello" in s):
    print("Exists")

if(30 in list1):
    print("Exists")
```

for loop
```
for val in list1:
    print(val) # prints with line break

for letter in s:
    print(letter, end=" ") # prints without line break

for (key, val) in dict1.items():
    print("key is ", key, " value is ", val)
```

while loop
```
x=1
while x<11:
    print(x)
    x=x+1
```

Terminate loop
```
for val in list1:
    if val == 30:
        break # terminates the loop before printing value 30
    print(val)
```

Endless loop
```
while True:
    answer=input("Press 0 to exit")
    print("You pressed ", answer)
    if int(answer)==0:
        break
```

End current iteration in loop
```
for val in list1:
    if val == 30:
        continue # skips printing of value 30
    print(val)
```

Range
```
# prints numbers from 5 through 19
for val in list(range(5,20)):
    print(val)

# prints numbers from 5 through 19 skipping 2
for val in list(range(5,20,3)):
    print(val, end=" ")
# 5 8 11 14 17
```

Random
```
import random

#create float
random.random()

#create integer
random.randint(1,100)
```

Merge multiple tuples
```
#Creates dictionary by setting key from tuple1 and values from tuple2
dict(zip(tuple1,tuple2))
```

Import numpy library
```
import numpy as np
```

Create numpy array
```
npa1=np.array(list1)
npa2=np.array([1,2,3,4,5], dtype=np.float) # create array with type conversion
npa3=np.array([1,2,3,4],[5,6,7,8]) # multi dimension array

import random
npa4=np.random.rand(2,3) # create multi dimension array with 2 lines and 3 columns

npa5=np.aranage(10) # values 0 throguh 9
npa6=np.arange(2,10,2) # values 2 through 9 skipping 1 (2,4,6,8)
```

numpy: calculation with corresponding values in 2 lists
```
# calculates average of corresponding values
exam1=np.array(exam1)
exam2=np.array(exam2)
average=(exam1+exam2)/2
```

Slice numpy array
```
# start with index 1 through index 8 skipping 1
print(npa5[3:10:2])
# prints [2 4 6 8]

print(npa5[:10:2])
print(npa5[1::2])
print(npa5[1:10:])
```

Slice multidimension numpy array
```
print(npa4[1,2]) #prints line index 1 and column index 2
```