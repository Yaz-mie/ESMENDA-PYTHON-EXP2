# Programming Assignment 2 – NumPy Essentials

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

# Create random 5x5 ndarray
X = np.random.rand(5, 5)

# Normalize X
Xmean = X.mean() 
Xstd = X.std()
Xnormalized = (X - Xmean) / Xstd

# Normalize X
Xmean = X.mean() 
Xstd = X.std()
Xnormalized = (X - Xmean) / Xstd
Computes the mean and standard deviation of the array.
