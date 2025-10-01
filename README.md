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
