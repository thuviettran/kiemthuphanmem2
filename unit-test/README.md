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

- Kiểm thử đơn vị: :contentReference\[oaicite:0]{index=0}

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



