# Làm việc với file CSV bằng thư viện pandas
---
## 1. Đọc file CSV
```python 
import pandas as pd

data = pd.read_csv(url, names = name)
print(data.head())
print(data.tail())
print(data.shape)
print(data.describe())
print(data.info())
print(data.columns.values)
print(data.index.values)
---

