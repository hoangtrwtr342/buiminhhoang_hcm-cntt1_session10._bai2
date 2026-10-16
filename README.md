##Phần 2. Source Code Markdown hoàn chỉnh
Markdown
# Hướng dẫn cài đặt cảm biến độ ẩm cho trang trại Lan

Sử dụng lệnh `pip install sensor-lib` để cài đặt thư viện điều khiển.

## 1. Đoạn code điều khiển máy bơm (Python)

```python

import time

def control_pump(humidity):
    if humidity < 60:
        print("Độ ẩm thấp: Bật máy bơm nước.")
    else:
        print("Độ ẩm ổn định: Tắt máy bơm.")
        
```

control_pump(55)

##2. So sánh loại cảm biến
Tiêu chí	Cảm biến cũ	Cảm biến mới
Độ chính xác	Thấp (±5%)	Cao (±1%)
Kết nối	Có dây	Không dây (Wi-Fi)
Độ bền	Kém (dễ ẩm mốc)	Cao (chống nước IP67)



##3. Task List kiểm tra thiết bị
[x] Lắp đặt cảm biến vào vị trí trung tâm vườn

[x] Cấu hình kết nối Wi-Fi cho thiết bị

[ ] Kiểm tra lệnh tự động bật/tắt máy bơm

[ ] Bàn giao hệ thống cho kỹ thuật viên vận hành