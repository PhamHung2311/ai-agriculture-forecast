
# Weather Forecasting Model - Random Forest & LSTM

## Mô tả dự án
Dự án này sử dụng hai mô hình học máy để dự báo nhiệt độ và độ ẩm tại thành phố Hà Nội dựa trên dữ liệu thời tiết lịch sử:  
- **Random Forest Regressor** (một thuật toán ensemble dựa trên cây quyết định)  
- **LSTM** (Long Short-Term Memory - một loại mạng neural hồi tiếp phù hợp với dữ liệu chuỗi thời gian)

Mục tiêu chính là so sánh hiệu quả của hai mô hình trong việc dự báo chính xác nhiệt độ và độ ẩm hàng ngày.

---

## Dữ liệu
- Dữ liệu được thu thập từ [nguồn bạn sử dụng] (ví dụ Kaggle, trang thời tiết chính thức).
- Bộ dữ liệu bao gồm các cột chính: `Date`, `Temperature`, `Humidity`.
- Dữ liệu được xử lý thành các đặc trưng đầu vào dựa trên nhiệt độ và độ ẩm của một số ngày trước đó (n_lags = 3).

---

## Cách sử dụng

### Chuẩn bị môi trường
- Python >= 3.7
- Các thư viện cần thiết: `numpy`, `pandas`, `scikit-learn`, `tensorflow`, `matplotlib`

Cài đặt các thư viện:
```bash
pip install numpy pandas scikit-learn tensorflow matplotlib
