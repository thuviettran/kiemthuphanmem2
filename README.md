## BÀI THỰC HÀNH KIỂM THỬ PHẦN MỀM

### Thông tin sinh viên

* **Họ và tên:** Trần Viết Thụ
* **MSSV:** BCS240041
* **Email:** tvthuwork@gmail.com
* **Môn học:** Kiểm thử phần mềm
* **Giảng viên:** Trương Anh Hoàng

---

## PHẦN 1 – BÀI THỰC HÀNH TUẦN 1: TRẢI NGHIỆM KIỂM THỬ GIAO DIỆN

### Mục tiêu bài thực hành

* Làm quen với GitHub và cách quản lý bài thực hành bằng kho lưu trữ (repository).
* Trải nghiệm và đánh giá chất lượng giao diện phần mềm.
* Nhận thức được vai trò của trải nghiệm người dùng (UX/UI) trong kiểm thử phần mềm.

### Nội dung thực hành

#### Trải nghiệm kiểm thử giao diện với Cantunsee

* Truy cập trang web: [https://cantunsee.space/](https://cantunsee.space/)
* Thực hiện các bài kiểm tra về:

  * Khả năng phân biệt màu sắc.
  * Khả năng nhận diện và đọc hiểu các thành phần giao diện người dùng.

### Minh chứng kết quả

* Ảnh chụp màn hình kết quả làm bài trên Cantunsee.
* Ảnh có dấu hiệu cá nhân (ví dụ: đang đăng nhập Chrome) để chứng minh tính xác thực.

**Hình ảnh minh chứng:**
<img width="1280" height="720" alt="Screenshot 2026-01-05 171945" src="https://github.com/user-attachments/assets/58120803-1492-4a26-ad05-28cb086a6f19" />

# Student Score Analyzer – Unit Testing with JUnit



## 1. Giới thiệu

Đây là bài tập thực hành kiểm thử đơn vị (Unit Testing) bằng Java nhằm:

- Phân tích dữ liệu điểm số học sinh

- Viết kiểm thử tự động bằng JUnit

- Thực hành quy trình làm việc với GitHub (Issues, Commit, README)



Chương trình cho phép:

- Đếm số học sinh đạt loại Giỏi (điểm >= 8.0)

- Tính điểm trung bình của các điểm hợp lệ



---



## 2. Mô tả bài toán



### Lớp `StudentAnalyzer`

Chương trình gồm lớp `StudentAnalyzer` với hai phương thức chính:



- `countExcellentStudents(List<Double> scores)`

&nbsp; - Đếm số học sinh đạt loại Giỏi (>= 8.0)

&nbsp; - Bỏ qua các điểm không hợp lệ (< 0 hoặc > 10)

&nbsp; - Nếu danh sách rỗng → trả về 0



- `calculateValidAverage(List<Double> scores)`

&nbsp; - Tính điểm trung bình của các điểm hợp lệ (0–10)

&nbsp; - Nếu không có điểm hợp lệ → trả về 0



---



## 3. Công nghệ sử dụng

- Ngôn ngữ: Java
  
- Quản lý mã nguồn: Git \& GitHub



---



## 4. Cấu trúc thư mục



```text

unit-test/

├── src/

│   └── StudentAnalyzer.java

├── test/

│   └── StudentAnalyzerTest.java

└── README.md

```

# Cypress E2E Testing – SauceDemo

## Giới thiệu
Dự án này sử dụng **Cypress** để thực hiện kiểm thử tự động End-to-End (E2E) cho website **https://www.saucedemo.com**, một trang web mô phỏng cửa hàng thương mại điện tử với các chức năng đăng nhập, danh sách sản phẩm, giỏ hàng và thanh toán.

Mục tiêu của bài tập:
- Làm quen với kiểm thử tự động E2E
- Viết test case bằng Cypress
- Tổ chức dự án kiểm thử rõ ràng
- Quản lý mã nguồn bằng GitHub

---

## Công nghệ sử dụng
- Node.js
- npm
- Cypress

---

## Các kịch bản kiểm thử

### 1. Kiểm tra đăng nhập
- Đăng nhập thành công với tài khoản hợp lệ
- Hiển thị thông báo lỗi khi đăng nhập với thông tin không hợp lệ

File: `login_spec.cy.js`

---

### 2. Kiểm tra giỏ hàng
- Thêm sản phẩm vào giỏ hàng
- Xóa sản phẩm khỏi giỏ hàng
- Kiểm tra số lượng sản phẩm hiển thị trong giỏ hàng

File: `cart_spec.cy.js`

---

### 3. Kiểm tra quy trình thanh toán
- Đăng nhập hệ thống
- Thêm sản phẩm vào giỏ hàng
- Truy cập trang thanh toán
- Nhập thông tin người dùng
- Chuyển đến trang xác nhận thanh toán

File: `checkout_spec.cy.js`

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


