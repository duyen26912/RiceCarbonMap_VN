# Dự án Phân tích OCO XCO2

## Giới thiệu
Dự án này tải xuống và trực quan hóa dữ liệu XCO2 (Carbon Dioxide trung bình theo cột) từ vệ tinh OCO-2 của NASA. Dự án tập trung vào việc phân tích nồng độ CO2 ở các khu vực cụ thể, đặc biệt là khu vực DBSH.

![OCO-2](https://upload.wikimedia.org/wikipedia/commons/3/34/Orbiting_Carbon_Observatory-2_artist_rendering_%28PIA18374%29.jpg)

## Cấu trúc dự án
```
.
├── CO2_DBSH/           # Dữ liệu CO2 cho khu vực DBSH
├── ranhGioi_DBSH/      # Dữ liệu ranh giới khu vực DBSH
├── data/               # Thư mục lưu trữ dữ liệu thô
├── images/             # Thư mục lưu trữ hình ảnh trực quan
├── Code_CO2.ipynb      # Notebook phân tích CO2
├── oco_xco2_download.ipynb    # Notebook tải dữ liệu
├── oco_xco2_analysis.ipynb    # Notebook phân tích dữ liệu
└── oco_tools.py        # Các hàm tiện ích
```

## Tính năng
- Tải dữ liệu XCO2 từ vệ tinh OCO-2 của NASA GES DISC
- Xử lý và phân tích dữ liệu nồng độ CO2
- Tạo các biểu đồ trực quan và phân tích thống kê
- Hỗ trợ phân tích cho khu vực cụ thể (DBSH)

## Yêu cầu hệ thống
- Python https://www.python.org/downloads/
- Jupyter https://jupyter.org/install
- Conda (khuyến nghị) https://docs.conda.io/en/latest/miniconda.html
- Panoply (tùy chọn) - yêu cầu JRE https://www.giss.nasa.gov/tools/panoply/download/

## Hướng dẫn sử dụng
1. Tải dữ liệu:
   - Chạy file `oco_xco2_download.ipynb` để tải dữ liệu từ OCO-2 (khoảng 20GB)
   - Dữ liệu sẽ được lưu trong thư mục `data/`

2. Phân tích:
   - Sử dụng `oco_xco2_analysis.ipynb` để phân tích tổng quan
   - Sử dụng `Code_CO2.ipynb` để phân tích CO2 chi tiết
   - Các biểu đồ được tạo sẽ được lưu trong thư mục `images/`
