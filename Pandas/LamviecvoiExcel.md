# Làm việc với Excel bằng thư viện Pandas
---
## 1. Đọc file excel 
```python
import pandas as pd

dataset = pd.read_excel()
print(dataset.info())  --lấy thông tin của dataset
print(dataset.head(4)) --lấy 4 dòng đầu tiên của dataset
print(dataset.tail(5)) --lấy 5 dòng cuối của dataset
print(dataset.describe()) --lấy thông tin cơ bản của dataset(Count,max,min,avg,...)
print(dataset.shape()) --hình dạng của dataset
print(dataset.drop(..., axis = ?, inplace = True)) -- xóa thông tin của dataset, axis = 1 xóa theo cột, axis = 0 xóa theo hàng
print(dataset.rename(..., inplace = True) --thay đổi cột trong dataset


