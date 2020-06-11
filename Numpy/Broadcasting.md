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

## 2. Lan truyền mảng với mảng
* Thao tác thay đổi giá trị cộng một ma trận mxn với một vector 
```python
import numpy as np
a = np.ones((2,3))
print(a)
b = np.arange(3)
print(b)
print(a+b)

-> [[1 1 1]
    [1 1 1]]
    
   [0 1 2]
   
  [[1 2 3]
   [1 2 3]]
```
* Thao tác thay đổi giá trị cộng ma trận hàng dọc với một vector
```python
import numpy as np
a = np.arange(3).reshape(3,1)
print(a)
b = np.arrange(3)
print(b)
print(a+b)

-> [[0]
    [1]
    [2]]
    
   [0 1 2]
   
  [[0 1 2]
   [1 2 3]
   [2 3 4]]
```
* Thao tác thay đổi giá trị cộng ma trận với ma trận 
```python 
import numpy as np
a = np.array([
               [1,2,3],
               [4,5,6]
])
print(a)
b = np.array([
               [1],
               [2]
])
print(b)
print(a+b)

-> [[1 2 3]
    [4 5 6]]
    
   [[1]
    [2]]
    
   [[2 3 4]
    [6 7 8]]
```



