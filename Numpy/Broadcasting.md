# Broadcasting 
---
* Broadcasting(Lan truyền) là cách mà chúng ta có thể thay đổi đồng loạt giá trị nhiều phần tử của mảng.
* Numpy cung cấp cơ chế broadcasting cho phép thực hiện tính toán giữa các số và các mảng khác chiều với nhau.
---
## 1. Lan truyền mảng với số 
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

