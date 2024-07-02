## Các bước để sử dụng model của mình: 
## Bước 1 : clone code của mình về máy 
```bash
! git clone https://github.com/TDThuyen/Object-Detection-Project.git
```
## Bước 2 : cài đặt các thư viện trong requirements.txt: 
```bash
%cd yolov10
! pip install -q -r requirements.txt
! pip install -e .
```
## Bước 3: khởi tạo: 
```bash
from ultralytics import YOLOv10

MODEL_PATH = [Đường dẫn đến file Helmet-Detection.pt]
model = YOLOv10 ( MODEL_PATH )
```
## Bước 4: chạy mô hình để nhận được hình ảnh: 
```bash
IMG_PATH = [Đường dẫn đến ảnh bạn muốn mô hình dự đoán]
result = model ( source = IMG_PATH ) [0]
```
## Bước 5: lưu hình ảnh về máy
```bash
result.save("[đường dẫn tới chỗ bạn muốn lưu kết quả]") 
```
