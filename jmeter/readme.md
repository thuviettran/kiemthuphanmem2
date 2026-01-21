# Apache JMeter Performance Test – Wikipedia

## Giới thiệu
Dự án này sử dụng **Apache JMeter 5.6.3** để thực hiện kiểm thử hiệu năng (Performance Testing) cho website **Wikipedia**.  
Test plan mô phỏng nhiều người dùng truy cập đồng thời vào các trang khác nhau và thu thập các chỉ số hiệu năng quan trọng.

---

## Công cụ sử dụng
- Apache JMeter 5.6.3  
- Giao thức: HTTP/HTTPS  
- Website kiểm thử: https://www.wikipedia.org  

---

## Cấu trúc Test Plan


```
Test Plan
├── HTTP Header Manager
├── HTTP Request Defaults
├── Thread Group 1
│   ├── GET Wikipedia Home
│   ├── View Results Tree
│   └── Summary Report
├── Thread Group 2
│   ├── GET Wikipedia Home
│   ├── GET Main Page
│   ├── View Results Tree
│   └── Summary Report
└── Thread Group 3
    ├── GET Software Testing
    ├── GET Performance Testing
    ├── View Results Tree
    └── Summary Report
```


---

## Mô tả các Thread Group

### Thread Group 1 – Wikipedia Home
- Request: `GET /`
- Mục tiêu: kiểm tra thời gian phản hồi trang chủ Wikipedia
- Kết quả:
  - 50 samples
  - Error rate: 0%
  - Throughput: ~5 requests/second

---

### Thread Group 2 – Main Page
- Requests:
  - `GET /`
  - `GET /wiki/Main_Page`
- Tổng số samples: 200
- Error rate: 0%
- Throughput: ~6.5 requests/second

---

### Thread Group 3 – Nội dung chuyên đề
- Requests:
  - `GET /wiki/Software_testing`
  - `GET /wiki/Performance_testing`
- Tổng số samples: 1192
- Error rate: 0%
- Throughput: ~19.5 requests/second

---

## Báo cáo kết quả
Sử dụng **Summary Report** để thu thập các chỉ số:
- Average Response Time
- Min Response Time
- Max Response Time
- Standard Deviation
- Throughput
- Received KB/sec
- Sent KB/sec
- Error %

Tất cả các Thread Group đều chạy thành công và không phát sinh lỗi.

---

## Cách chạy Test Plan

1. Mở Apache JMeter
2. Chọn **File → Open**
3. Mở file `Test_Plan.jmx`
4. Nhấn **Run**
5. Xem kết quả tại:
   - View Results Tree
   - Summary Report

---

## File trong repository
- `Test_Plan.jmx` – File test plan JMeter
- `README.md` – Mô tả dự án
- (Tuỳ chọn) `results/` – Lưu file kết quả `.jtl` hoặc `.csv`

---

## Kết luận
Dự án minh họa:
- Cách sử dụng nhiều Thread Group trong Apache JMeter
- Thực hiện kiểm thử hiệu năng cho website thực tế
- Phân tích kết quả bằng Summary Report

Phù hợp cho học tập và báo cáo môn Kiểm thử phần mềm / Performance Testing.
