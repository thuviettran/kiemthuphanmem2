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


