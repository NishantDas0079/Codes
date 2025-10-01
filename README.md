# NUMPY BASIC CODES

```

# Import Numpy Library
import numpy as np
import warnings
warnings.filterwarnings("ignore")
from IPython.display import Image



list1 = [10,20,30,40,50,60]
list1


# Display the type of an object
type(list1)


# Convert list to Numpy Array
arr1 = np.array(list1)
arr1


# Memory address of an array object
arr1.data



# Display type of an object
type(arr1)


# Datatype of array
arr1.dtype


# Convert Integer Array to FLOAT
arr1.astype(float)


# Generate evenly spaced numbers (space =1) between 0 to 10
np.arange(0,10)


# Generate numbers between 0 to 100 with a space of 10
np.arange(0,100,10)



# Generate numbers between 10 to 100 with a space of 10 in descending order
np.arange(100, 10, -10)



# Shape of Array
arr3 = np.arange(0,10)
arr3.shape



# Size of array
arr3.size


# Bytes consumed by one element of an array object
arr3.itemsize


# Bytes consumed by an array object
arr3.nbytes


# Length of array
len(arr3)


# Generate an array of zeros
np.zeros(10)


# Generate an array of ones with given shape
np.ones(10)



# Repeat 10 five times in an array
np.repeat(10,5)



# Repeat each element in array 'a' thrice
a= np.array([10,20,30])
np.repeat(a,3)


# Generate array of Odd numbers
ar1 = np.arange(1,20)
ar1[ar1%2 ==1]


# Generate array of even numbers
ar1 = np.arange(1,20)
ar1[ar1%2 == 0]



# Create an array of random values
np.random.random(4)


# Generate an array of Random Integer numbers
np.random.randint(0,500,5)



arr2 = np.arange(1,20)
arr2


# Sum of all elements in an array
arr2.sum()

# Cumulative Sum
np.cumsum(arr2)


# Find Minimum number in an array
arr2.min()


#  Find MAX number in an array
arr2.max()


# Find mean of all numbers in an array
arr2.mean()


# Find median of all numbers present in arr2
np.median(arr2)


# Variance
np.var(arr2)

# Standard deviation
np.std(arr2)


# Calculating percentiles
np.percentile(arr2,70)


A = np.array([[1,2,3,0] , [5,6,7,22] , [10 , 11 , 1 ,13] , [14,15,16,3]])
A


# SUM of all numbers in a 2D array
A.sum()

# MAX number in a 2D array
A.max()

# Minimum
A.min()


# Enumerate for Numpy 2D Arrays
for index, value in np.ndenumerate(A):
    print(index, value)



a = np.array([7,5,3,9,0,2])


# Access first element of the array
a[0]

# Access all elements of Array except first one.
a[1:]


# Fetch 2nd , 3rd & 4th value from the Array
a[1:4]


# Get last element of the array
a[-1]


ar = np.arange(1,20)
ar


# Replace EVEN numbers with ZERO
rep1 = np.where(ar % 2 == 0, 0 , ar)
print(rep1)



# Replace 10 with value 99
rep2 = np.where(ar2 == 10, 99 , ar2)
print(rep2)
```




# PANDAS 


```

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import glob
import re
import math



# Create series from Nump Array
v = np.array([1,2,3,4,5,6,7])
s1 = pd.Series(v)
s1


# Datatype of Series
s1.dtype


# number of bytes allocated to each item
s1.itemsize



# Number of bytes consumed by Series
s1.nbytes



# Shape of the Series
s1.shape


# number of dimensions
s1.ndim

s1.size

s1.count()


# Create series from List 
s0 = pd.Series([1,2,3],index = ['a','b','c'])
s0


# Modifying index in Series
s1.index = ['a' , 'b' , 'c' , 'd' , 'e' , 'f' , 'g']
s1


# Create Series using Random and Range function
v2 = np.random.random(10)
ind2 = np.arange(0,10)
s = pd.Series(v2,ind2)
v2 , ind2 , s
```
