# Programming Assignment 2 – NumPy 

**Author:** ESMENDA, Francine Jasmine Guelle T. 

**Course:** Advanced Computer Programming and Algorithms / ECE2112  

---

## 📌 Description  

This Jupyter Notebook demonstrates beginner applications of the **NumPy library** in Python.  
It shows how to create arrays, normalize data, perform mathematical transformations, and filter values.  

The problems solved include:  
1. **Array Normalization** – Generate a 5×5 random array and normalize its values.  
2. **Integer Array Transformation** – Create a 10×10 array of integers (1–100), compute squares, and extract divisible numbers.  

---

## ⚙️ Requirements  

- Python 3 
- Jupyter Notebook  
- NumPy  

---

## ▶️ How to Run  

1. Install [Jupyter Notebook](https://jupyter.org/).  
2. Open the file ESMENDA_EXP2.ipynb.
3. Run each cell to see the outputs directly below.

## 💡 Examples w/ Explanation

**01 🎲 Random Array Normalization**

```python
#Import NumPy library
import numpy as np

#Create random 5x5 ndarray
X = np.random.rand(5, 5)
```
- import numpy as np, is needed for all numerical and array operations.
- X = np.random.rand(5, 5), generates a 5×5 array with random values between 0 and 1.
  

```python
#Normalize X
Xmean = X.mean() 
Xstd = X.std()
Xnormalized = (X - Xmean) / Xstd
```
- Computes the mean and standard deviation of the array.
- Applies normalization formula
- Ensures the data has mean = 0 and std = 1

```python
# Save the result of the normalized array
np.save('X_normalized.npy', Xnormalized)

# Print output
print(Xnormalized)
```
- np.save, saves the normalized array to a file for future use.
- print, displays the normalized 5×5 array.

**02 🔢 Integer Array Transformation**

```python
#Get the first positive integers from 1 - 100
A = np.arange(1,101) 

#Constructs a 10x10 array, then get the squares of each integer
Aarray = A.reshape(10,10) ** 2 
```
- Creates numbers 1 to 100
- Reshapes into a 10×10 matrix
- Squares every element
  
```python
# Find elements divisible by 3
divisible = A[A % 3 == 0]
```
- Filters the array to extract values divisible by 3.
  
```python
#Save to file
np.save("div_by_3.npy", divisible)
#Print output
print(divisible)
```
- np.save, this stores the divisible-by-3 results into a file
- print, shows all integers between 1 and 100 that are divisible by 3.
---

# Version History
v1.0 – Created initial notebook with NumPy import and basic array operations

v1.1 – Added element-wise addition, subtraction, multiplication, and division examples

v1.2 – Introduced mathematical functions (square root, power, mean, standard deviation)
  


 

