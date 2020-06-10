# Indexing và Slicing trong numpy 
---
## 1. Indexing giống như cách thao tác với list trong python 
```python
import numpy as np
matrix = np.array([
                    [1,2,3],
                    [4,5,6]
])
print(matrix)
print(matrix[0,:2]) -> In ra hàng 0, cột(0,1)
print(matrix[:,0]) -> In ra tất cả các hàng, cột 0
print(matrix[-1]) -> In ra hàng cuối cùng 
print(matrix[-1,:2]) -> In ra hàng cuối cùng, cột(0,1)
print(matrix[:1, :2]) -> In ra một ma trận hàng 0, cột(0,1)

-> [[1 2 3]
    [4 5 6]]
    
    [1 2]
    [1 4]
    [4 5 6]
    [4 5]
    [[1,2]]
```
## 2. Slicing 
```python
import numpy as np 
matrix = np.random.random((2,3))
print(matrix)
print(matrix[0:1])
print(matrix[0:1].shape)
print(matrix[0:1][-1])
print(matrix[0:1][-1].shape)

-> [[0.1 0.2 0.3]
    [0.4 0.5 0.6]]
    
   [[0.1 0.2 0.3]]
   (1,3)
   [0.1 0.2 0.3]
   (3,)
 ```
 
    
