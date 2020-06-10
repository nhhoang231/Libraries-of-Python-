# ***Numpy Array***
--- 
## 1. Điểm mạnh của Numpy so với Python là có thể mô phỏng được mảng nhiều chiều 
Numpy có thể tạo ra 1 vector:
```python
import numpy as np
vector = np.array([1,2,3]) 
print(vector) 
print(type(vector))
print(vector.shape)

-> [1,2,3]
   <class 'numpy.ndarray'>
   (3,) mảng 1 chiều có 3 phần tử 
```

Numpy có thể tạo ra 1 ma trận:
```python 
import numpy as np 
np_matrix = np.array([
                        [1,2,3],
                        [8,3,1]
])
print(matrix)
print(matrix.shape)

-> [[1,2,3]
    [8,3,1]]
   (2,3) mảng 2 chiều gồm 2 hàng 3 cột
```




