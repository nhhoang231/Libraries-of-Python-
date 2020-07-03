# Matplotlib Overview
---
## 1. Giới thiệu về Maplotlib
* Để thực hiện các thống kê, cần trực quan hóa dữ liệu thì Matplotlib là một trong các giải pháp rất tốt cho python.
* Matplotlib là một thư viện mã nguồn mở vẽ đồ thị rất mạnh mẽ và hữu ích khi làm việc với python và numpy.
* Pyplot là một module được sử dụng nhiều nhất trong matplotlib
```python 
-- We are using the inline backend 
%matplotlib inline

import matplotlib as mpl
import matplotlib.pyplot as plt
print('Matplotlib version: ', mpl._version_) 

-- How to apply a style to Matplotlib
print(plt.style.available)
mpl.style.use(['ggplot'])
```
---
## 2. Line Plot (Biêu đồ đường)
* Biểu đồ đường (Line Plot) là một loại biểu đồ hiển thị thông tin dưới dạng một loạt các điểm dữ liệu được gọi là "marker" được kết nối bởi các đoạn thẳng 
* Nó là một loại biểu đồ cơ bản phổ biến trong nhiều lĩnh vực. Sử dụng biểu đồ đường khi bạn có một bộ dữ liệu liên tục.
* Biêu đồ phù hợp nhất cho việc trực quan hóa dữ liệu dựa trên xu hướng trong một khoảng thời gian.

 

