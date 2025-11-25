# Python Memory Allocation – Task 03

This repository contains the solution for Task-03 in the Instant D.Analysis course.

## 🔍 Search Task  
**How much memory does Python allocate for each data type?**

Python uses a dynamic memory allocation system, and the memory size varies by interpreter and system architecture. Below are typical memory sizes on a 64-bit Python interpreter:

---

## 📏 Approximate Memory Usage in Python

| Data Type | Example | Approx. Memory Usage |
|----------|----------|----------------------|
| **int** | 10 | ~28 bytes |
| **float** | 10.5 | ~24 bytes |
| **bool** | True | ~28 bytes |
| **str** | "A" | ~49 bytes + 1 byte per character |
| **list** | [1,2,3] | ~64 bytes + 8 bytes per element |
| **tuple** | (1,2,3) | ~48 bytes + 8 bytes per element |
| **dict** | {"a":1} | ~72 bytes + key/value |
| **set** | {1,2,3} | ~200+ bytes |

---

## 🧪 Checking Memory Usage in Python

```python
import sys

print(sys.getsizeof(10))         # int
print(sys.getsizeof(10.5))       # float
print(sys.getsizeof(True))       # bool
print(sys.getsizeof("Hello"))    # string
print(sys.getsizeof([1,2,3]))    # list
print(sys.getsizeof((1,2,3)))    # tuple
print(sys.getsizeof({"a": 1}))   # dict
print(sys.getsizeof({1, 2, 3}))  # set
