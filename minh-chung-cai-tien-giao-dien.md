# Minh Chứng Cải Tiến Giao Diện (Buổi 5–6) - TC5a

**Sinh viên:** Lê Hoài Nam  
**MSSV:** 2071020138  
**Lớp:** 20-04  

---

## 1. Vấn đề giao diện ban đầu (Trước cải tiến)
- **Hiện tượng:** Menu điều hướng (`navbar`) và danh sách thẻ dự án (`project-card`) bị đè vạch, tràn màn hình khi thu nhỏ kích thước trình duyệt về màn hình di động (width < 768px).
- **Tiêu chí đánh giá:** Tính đáp ứng (Responsive Design) và Khả dụng (Usability / Focus State).

---

## 2. Phương án và Lý do lựa chọn cải tiến
- **Cách sửa:** 
  1. Thêm Media Query `@media (max-width: 768px)` vào `css/style.css` để chuyển đổi layout từ nằm ngang sang chiều dọc.
  2. Bổ sung trạng thái `:focus` và `:hover` rõ ràng cho các thẻ liên kết `<a>` giúp hỗ trợ truy cập phím tab tốt hơn.
- **Lý do lựa chọn:** Giữ giao diện nguyên bản chuẩn đề bài (Template gốc), không dùng thư viện ngoài nặng nề, đảm bảo tải nhanh và hiển thị đẹp trên mọi màn hình.

---

## 3. Kết quả thử nghiệm & Đối chiếu
- **Trạng thái:** Đã kiểm tra thành công trên Local, Git Repo và URL GitHub Pages.
- **Hạn chế còn lại:** Chưa có menu Toggle Hamburger bằng Javascript (giữ nguyên phạm vi thuần HTML/CSS theo yêu cầu).
