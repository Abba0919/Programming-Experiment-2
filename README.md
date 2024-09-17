# Programming-Experiment-2

## Introduction
### In this experiment, we make a phyton program that focuses on how to use numpy and pandas. I created 2 programs that uses that uses numpy.

### NORMALIZATION PROBLEM: 
Normalization is one of the most basic preprocessing techniques in data analytics. This involves centering and scaling process. Centering means subtracting the data from the mean and scaling means dividing with its standard deviation. Mathematically, normalization can be expressed as:

in Python, element-wise mean and element-wise standard deviation can be obtained by using .mean() and .std() calls.

In this problem, create a random 5 x 5 ndarray and store it to variable X. Normalize X. Save your normalized
ndarray as X_normalized.npy

### INPUT: 
    
```python
import numpy as np
#create a random 5x5 ndarray
X = np.random.randn(5, 5)
#make a mean and standard deviation
mean = X.mean()
std = X.std()
#normalize X
X_normalized = (X - mean) / std
np.save('X_normalized.npy', X_normalized)
#Output the values
print("Original Array X:\n", X)
print("\nMean of X:")
print(mean)
print("\nStandard Deviation of X:")
print(std)
print("\nNormalized Array X_normalized:\n", X_normalized)
```

### OUTPUT:

![Screenshot 2024-09-18 013818](https://github.com/user-attachments/assets/a18adde2-eaad-4d0f-9d8c-5d0d335ea1f8)

## DIVISIBLE BY 3 PROBLEM

Create The following 10 x 10 ndarray 

![image](https://github.com/user-attachments/assets/31b40a0e-7237-4271-8ed4-e72b556e40b3)

which are the squares of the first 100 positive integers.

From this ndarray, determine all the elements that are divisible by 3. Save the result as div_by_3.npy


### INPUT:

```python
import numpy as np

# create a 10x10 ndarray with squares of the first 100 positive integers
squares = np.arange(1, 101).reshape(10, 10) ** 2

div_by_3 = squares[squares % 1 == 0]

# Print the result
print(squares)
```

### OUTPUT:

![image](https://github.com/user-attachments/assets/d37ea198-1d22-4b7e-a654-1388a6319823)





