# Broadcasting 
---
* Broadcasting(Lan truyền) là cách mà chúng ta có thể thay đổi đồng loạt giá trị nhiều phần tử của mảng.
* Numpy cung cấp cơ chế broadcasting cho phép thực hiện tính toán giữa các số và các mảng khác chiều với nhau.
---
## 1. Lan truyền mảng với số 
* Thao tác thay đổi giá trị trên vector
```python
import numpy as np
vector = np.array([1,2,3])
print(vector)
vector = vector + 3
print(vector)
vector = vector + np.array([3,3,3])
print(vector)

-> [1 2 3]
   [4 5 6]
   [7 8 9]
```
* Thao tác thay đổi giá trị trên ma trận 
```python
import numpy as np
matrix = np.array([
                     [4,5,6],
                     [7,8,9]
])
print(matrix)
matrix = matrix *2
print(matrix)

-> [[4 5 6]
    [7 8 9]]
    
   [[8  10 12]
    [14 16 18]]
```    
    
