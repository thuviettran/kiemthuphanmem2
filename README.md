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



