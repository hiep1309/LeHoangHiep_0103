# Công nghệ sử dụng
---

**Thư viện sử dụng:**
- `PIL (Python Image Library)`: dùng để mở và hiển thị hình ảnh.
- `imageio`: đọc dữ liệu hình ảnh dưới dạng mảng.
- `numpy`: xử lý dữ liệu ảnh dưới dạng ma trận số học.
- `matplotlib.pyplot`: hiển thị ảnh bằng đồ họa.

# Thuật toán sử dụng
---

Trong bài này, các thuật toán xử lý ảnh cơ bản được sử dụng, bao gồm:
- Đọc ảnh từ tệp.
- Chuyển đổi ảnh sang mảng số để xử lý.
- Hiển thị ảnh.

# Giải thích cách hoạt động
---

**1. Nạp ảnh sử dụng PIL:**

```python
from PIL import Image
import numpy as np

img = Image.open('bird.png')
img.show()
Image.open(...): mở tệp ảnh.

img.show(): hiển thị ảnh sử dụng chương trình mặc định của hệ điều hành.
import numpy as np
import imageio.v2 as iio
import matplotlib.pylab as plt

data = iio.imread('bird.png')
plt.imshow(data)
plt.show()
iio.imread(...): đọc ảnh thành mảng NumPy.

plt.imshow(...): hiển thị ảnh dưới dạng đồ họa.

plt.show(): vẽ ảnh ra màn hình.