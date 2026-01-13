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


