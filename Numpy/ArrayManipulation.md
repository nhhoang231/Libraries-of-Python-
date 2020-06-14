# Array Manipulation 
---
## 1. Thay đổi kích thước mảng trong ma trận 
```python
import numpy as np
matrix = np.array([
                    [1,2,3,4],
                    [5,6,7,8]
])
print(matrix)
print(matrix.shape)

matrix1 = matrix.reshape(4,2) --thay đổi dạng ma trận thành 4 hàng 2 cột
print(matrix1)

cube = matrix.reshape(2,2,2) --thay đổi dạng ma trận thành 1 hình khối có 2 hàng 2 cột 2 phần tử 1 đơn vị
print(cube)

-> [[1 2 3 4]
    [5 6 7 8]]
   (2,4)
   
   [[1 2]
    [3 4]
    [5 6]
    [7 8]]
   
   [[1 2]
    [3 4]]
   [[5 6]
    [7 8]]
```
   
