# Numpy Array
--- 
## 1. Điểm mạnh của Numpy so với Python là có thể mô phỏng được mảng nhiều chiều 
Numpy có thể tạo ra 1 vector
```python
import numpy as np
vector = np.array([1,2,3]) 
print(vector) 
print(type(vector))
print(vector.shape)

-> [1 2 3]
   <class 'numpy.ndarray'>
   (3,) Mảng 1 chiều có 3 phần tử 
```

Numpy có thể tạo ra 1 ma trận
```python 
import numpy as np 
np_matrix = np.array([
                        [1,2,3],
                        [8,3,1]
])
print(matrix)
print(matrix.shape)

-> [[1 2,3]
    [8 3 1]]
   (2,3) Mảng 2 chiều gồm 2 hàng 3 cột
```
Numpy có thể tạo ra một hình khối 
```python
import numpy as np
cube = np.array([
                     [[1,2],[2,3],[3,4]],
                     [[4,5],[5,6],[6,7]]
])
print(cube)
print(cube.shape)

-> [[[1 2]
     [2 3]
     [3 4]]
     
    [[4,5]
     [5 6]
     [6 7]]]
    (2,3,2) Mảng 3 chiều: 2 hàng, 3 cột, 2 phần tử 1 cột 
```
> Số mở ngoặc vuông khi tạo ra 1 array tương ứng với số chiều của array đó

--- 
## 2. Zeros(), Ones(), Full()
* Dùng để tạo mảng các giá trị bằng nhau 
* Đầu vào là shape của array dưới dạng tuple

Zeros(): Tạo ra các mạng giá trị đều bằng 0 
```python
import numpy as np
vector = np.zeros((3,))
print(vector)

-> [0.0.0.]
```
Ones(): Tạo ra các mảng co giá trị bằng 1
```python
import numpy as np
vector = np.ones((3,))
print(vector)

-> [1.1.1.]
```
Full(): Tạo ra các mảng giá trị bằng nhau và bằng 1 giá trị cụ thể cho trước vào đó
```python
import numpy as np
vector = np.full((3,),10)
print(vector) 

-> [10 10 10]
```
--- 
## 3. Một số phương thức khác trong Numpy
Numpy có thể tạo ra một ma trận đơn vị
```python 
import numpy as np
matrix = np.eye((3))
print(matrix)

-> [[1.0.0.]
    [0.1.0.]
    [0.0.1.]]
```
Arange(i,j,k): Numpy có thể tạo 1 mảng chạy từ i đến j phần tử, với bước nhảy phần tử là k
```python 
import numpy as np
vector = np.arange(1,10,3)
print(vector)

-> [1 4 7]
```

Numpy có thể tự random ra một ma trận
```python 
import numpy as np
matrix = np.random.random((2,3))
print(matrix)

-> [[1 2 3]
    [4 5 6]]
```






