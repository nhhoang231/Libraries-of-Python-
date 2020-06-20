# Làm việc với Pandas
---
## 1. Overview
1. Giới thiệu về pandas
* Pandas là một thư viện mã nguồn mở, hỗ trợ rất tốt các thao tác với dữ liệu. Nó là bộ công cụ phân tích và xử lí dữ liệu mạnh mẽ nhất của python
* Nó sử dụng một cấu trúc dữ liệu riêng là DataFrame. Pandas cung cấp chức năng xử lí và làm việc trên cấu trúc này.
2. Đặc điểm
* Đọc dữ liệu từ rất nhiều định dạng khác nhau. VD: csv,excel,sql...
* Liên kết dữ liệu và xử lí dữ liệu bị thiếu
* Tách, đánh, chỉ mục và chia nhỏ các tập dữ liệu lớn dựa trên label
* Có thể nhóm (Group By) theo các giá trị mục đích
* Lọc và thực hiện query trên dữ liệu 
---
## 2. Series on Pandas
* Pandas giúp tạo ra một series các giá trị.
VD1:
```python
import numpy as np
import pandas as pd

data = pd.Series(np.random.randint(100,size=4))
print(data)

-> 0 91
   1 97
   2 47
   3 30
   dtype: int64
```

VD2:
```python
import numpy as np
import pandas as pd

chiso = ["Kientruc","Xaydung","Dulich","CNTT"]
giatri = [317, 369, 350, 390]

data = pd.Series(giatri, chiso)
print(data)

-> Kientruc 317
   Xaydung  369
   Dulich   350
   CNTT     390
   dtype: int64
```
## 3. DataFrame
* Pandas giúp chuyển các dạng dữ liệu thành dạng dữ liệu cấu trúc dataframe. 
```python
import pandas as pd
import numpy as np

dic = [
       'a':[11,21,31,15,4]
       'b':[12.5,22.9,32.3,71.7,3.4]
       'c':['v1','v2','v3','v4','v5']
]
data = pd.dataFrame(dic)
print(data)

->    a      b  c
   0  11  12.5 v1
   1  21  22.9 v2
   2  31  32.3 v3
   3  15  71.7 v4
   4  4    3.4 v5
```
