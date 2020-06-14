# Iterating
--- 
## 1. Lặp qua các phần tử 
```python
import numpy as np
vector = np.array([1,2,3])
print(vector)
for i in np.nditer(vector):
  print(vector)
  
 -> [1 2 3]
    1
    2
    3
 ```

