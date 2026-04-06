# NumPy Array Creation Functions 🚀

## 📌 Overview

This repository/document provides a comprehensive guide to commonly used **NumPy array creation functions**. These functions are essential for numerical computing, data analysis, and scientific applications in Python.

---

## 📦 Prerequisites

Make sure you have NumPy installed:

```bash
pip install numpy
```

Import NumPy:

```python
import numpy as np
```

---

# 🔢 Array Creation Functions

## 1. `np.zeros()`

### 📖 Definition

Creates an array filled with **zeros**.

### 📌 Syntax

```python
np.zeros(shape, dtype=float)
```

### ✅ Example

```python
arr = np.zeros((2, 3))
print(arr)
```

### 💡 Use Case

* Initialize arrays for computations
* Placeholder arrays

---

## 2. `np.ones()`

### 📖 Definition

Creates an array filled with **ones**.

### 📌 Syntax

```python
np.ones(shape, dtype=float)
```

### ✅ Example

```python
arr = np.ones((2, 2))
```

### 💡 Use Case

* Default weights
* Multiplicative identity initialization

---

## 3. `np.eye()`

### 📖 Definition

Creates an **identity matrix** (diagonal = 1, others = 0).

### 📌 Syntax

```python
np.eye(n, m=None)
```

### ✅ Example

```python
arr = np.eye(3)
```

### 💡 Use Case

* Linear algebra
* Matrix operations

---

## 4. `np.array()`

### 📖 Definition

Creates an array from **lists, tuples, or other sequences**.

### 📌 Syntax

```python
np.array(object)
```

### ✅ Example

```python
arr = np.array([1, 2, 3])
```

### 💡 Use Case

* Convert Python data structures into arrays

---

## 5. `np.full()`

### 📖 Definition

Creates an array filled with a **specific value**.

### 📌 Syntax

```python
np.full(shape, fill_value)
```

### ✅ Example

```python
arr = np.full((2, 2), 7)
```

### 💡 Use Case

* Constant-value initialization

---

## 🎲 Random Array Functions

## 6. `np.random`

### 📖 Definition

Module containing **random number generation functions**.

### 💡 Use Case

* Simulations
* Sampling

---

## 7. `np.random.random()`

### 📖 Definition

Generates random numbers in the range **[0, 1)**.

### 📌 Syntax

```python
np.random.random(size)
```

### ✅ Example

```python
arr = np.random.random(3)
```

---

## 8. `np.random.rand()`

### 📖 Definition

Generates random values in **[0, 1)** with given shape.

### 📌 Syntax

```python
np.random.rand(d0, d1, ...)
```

### ✅ Example

```python
arr = np.random.rand(2, 3)
```

### ⚖️ Difference from `random()`

| Feature | random() | rand()         |
| ------- | -------- | -------------- |
| Input   | tuple    | separate args  |
| Usage   | flexible | shorter syntax |

---

## 9. `np.random.seed()`

### 📖 Definition

Sets a **fixed starting point** for random number generation.

### 📌 Syntax

```python
np.random.seed(seed_value)
```

### ✅ Example

```python
np.random.seed(10)
print(np.random.rand(3))
```

### 💡 Use Case

* Reproducibility in experiments

---

## 10. `np.random.normal()`

### 📖 Definition

Generates values from a **normal (Gaussian) distribution**.

### 📌 Syntax

```python
np.random.normal(loc=0.0, scale=1.0, size=None)
```

### ✅ Example

```python
arr = np.random.normal(0, 1, (2, 2))
```

### 💡 Parameters

* `loc` → Mean
* `scale` → Standard deviation

---

## 📏 Sequence-Based Functions

## 11. `np.arange()`

### 📖 Definition

Creates values within a range with a fixed **step size**.

### 📌 Syntax

```python
np.arange(start, stop, step)
```

### ✅ Example

```python
arr = np.arange(0, 10, 2)
```

### 💡 Use Case

* Iterative sequences

---

## 12. `np.linspace()`

### 📖 Definition

Creates evenly spaced values between a range.

### 📌 Syntax

```python
np.linspace(start, stop, num)
```

### ✅ Example

```python
arr = np.linspace(0, 1, 5)
```

### ⚖️ Difference from `arange()`

| Feature   | arange() | linspace()       |
| --------- | -------- | ---------------- |
| Based on  | step     | number of points |
| Precision | less     | more             |

---

## ⚡ Memory-Based Function

## 13. `np.empty()`

### 📖 Definition

Creates an array **without initializing values** (contains garbage values).

### 📌 Syntax

```python
np.empty(shape, dtype=float)
```

### ✅ Example

```python
arr = np.empty((2, 2))
```

### ⚠️ Important

* Values are random (memory garbage)
* Faster than zeros/ones

---

# 📊 Summary Table

| Function      | Purpose            |
| ------------- | ------------------ |
| zeros         | Fill with 0        |
| ones          | Fill with 1        |
| eye           | Identity matrix    |
| array         | Create from list   |
| full          | Fill with constant |
| random        | Random module      |
| random.random | Random [0,1)       |
| random.rand   | Random shaped      |
| random.seed   | Reproducibility    |
| random.normal | Gaussian values    |
| arange        | Step-based range   |
| linspace      | Equal spacing      |
| empty         | Uninitialized      |

---

# 🎯 Conclusion

These NumPy functions are fundamental for:

* Data initialization
* Simulations
* Machine learning workflows
* Scientific computing

Mastering them will significantly improve your efficiency in handling numerical data in Python.

---

# ✍️ Author

Your Name

---
