# Linear Algebra
---
## 1. Products
1. Tính tích vô hướng của 2 vector
```python
import numpy as np
a = np.array([1,2,3])
b = np.array([3,4,5])
print(a*b)            --tính tích vô hướng 2 vector
print(np.inner(a,b))  --tính độ dài tích vô hướng

-> [3 8 15]
   26
```
2. Tính tích vô hướng của 2 ma trận 
```python
import numpy as np
a = np.array([
               [1,2,3],
               [4,5,6]
])
b = np.array([
               [6,7,8],
               [9,10,11],
               [12,13,14]
])
print(a.dot(b))

-> [[ 60  66  62]
    [141 156 171]]
```

3. Nhân từng phần tử với nhau trên 2 ma trận
```python
import numpy as np
a = np.array([
               [1,2,3],
               [4,5,6]
])
b = np.array([
               [4,5,6],
               [6,7,8]
])
print(np.tensordot(a,b))

-> 139
```
## 2. Norm
1. L2 Norm là căn tổng bình phương của các giá trị của vector 
```python
import numpy as np
from numpy import linalg
a = np.array([1,2,3,4])
print(linalg.norm(A))

-> 5.477225575051661
```
2. L1 Norm là tổng giá trị tuyệt đối của các giá trị của vector
```python
import numpy as np
a = np.array([1,2,3,4])
print(linalg.norm(a,ord=1)

-> 10.0
```


