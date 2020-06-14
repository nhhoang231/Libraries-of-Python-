# Iterating
--- 
## 1. Lặp qua các phần tử 
```python
import numpy as np
vector = np.array([1,2,3])
print(vector)
for i in np.nditer(vector):
  print(i)
  
 -> [1 2 3]
    1
    2
    3
 ```

## 2. Lặp theo dòng 
```python
import numpy as np
matrix = np.array([
                    [1,2,3],
                    [4,5,6]
])
print(matrix)
for i in np.nditer(matrix, flags = ['external_loop'], order = 'F'): --lặp in ra theo cột của ma trận
  print(i)
for i in np.nditer(matrix, flags = ['external_loop'], order = 'C'): --lặp in ra tất cả phần tử ma trận thành 1 hàng
  print(i)

-> [[1 2 3]
    [4 5 6]]
    
   [1 4]
   [2 5]
   [3 6]
   
   [1 2 3 4 5 6]
```
