# Tra cứu vi phạm giao thông tự động

Đây là một script Python sử dụng Selenium để tự động mở trình duyệt và hỗ trợ tra cứu vi phạm phương tiện giao thông trên trang web [CSGT](https://www.csgt.vn/tra-cuu-phuong-tien-vi-pham.html). Script sẽ tự động chạy vào 6h và 12h mỗi ngày, yêu cầu người dùng nhập captcha thủ công.

## 🛠 Yêu cầu hệ thống

* Python 3.7+
* Google Chrome đã cài đặt
* ChromeDriver tương thích với phiên bản Chrome
* Các thư viện Python liệt kê trong `requirements.txt`

## 📦 Cài đặt

1. Clone hoặc tải repo này:

   ```bash
   git clone https://github.com/yourusername/auto-traffic-lookup.git
   cd auto-traffic-lookup
   ```

2. Cài đặt các thư viện cần thiết:

   ```bash
   pip install -r requirements.txt
   ```

3. Đảm bảo bạn đã cài **ChromeDriver** và thêm vào biến môi trường `PATH`.

   * Tải tại: [https://sites.google.com/chromium.org/driver/](https://sites.google.com/chromium.org/driver/)

## ▶️ Cách sử dụng

Chạy script:

```bash
python traffic_lookup.py
```

Script sẽ:

* Tự động mở trình duyệt và truy cập trang tra cứu
* Nhập sẵn biển số và loại xe
* Yêu cầu bạn nhập Captcha thủ công
* Hiển thị kết quả nếu có

## ⏰ Lịch chạy

Script sẽ kiểm tra thời gian và **tự động chạy lúc 6:00 và 12:00 mỗi ngày**.

## 📋 Ghi chú

* Captcha phải được nhập thủ công, không có xử lý tự động captcha.
* Để chạy ẩn hoặc tự động hóa hoàn toàn, cần kỹ thuật xử lý captcha nâng cao (không được hỗ trợ trong phiên bản này).

## 📄 Tệp liên quan

* `traffic_lookup.py`: Mã nguồn chính
* `requirements.txt`: Danh sách thư viện cần thiết
