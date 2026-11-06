# AI_LOG.md - Nhận định và Quyết định Sử dụng AI

**Sinh viên:** Lê Hoài Nam  
**MSSV:** 2071020138  
**Lớp:** 20-04  

---

## Nhật ký xử lý & Quyết định AI

### Tình huống 1: Tối ưu hóa đường dẫn tài nguyên tĩnh trên GitHub Pages
- **Hiện tượng & Dữ kiện ban đầu:** Khi deploy lên GitHub Pages, một số hình ảnh trong thư mục `assets/` bị lỗi đường dẫn tuyệt đối `/assets/` do repository dạng sub-path (`/portfolio-v7/`).
- **Nhận định trước khi hỏi AI:** Cần đổi toàn bộ đường dẫn tài nguyên sang tương đối `./assets/` hoặc `assets/` để chạy đúng cả local lẫn sub-path Pages.
- **Gợi ý từ AI:** AI đề xuất sử dụng đường dẫn tương đối `assets/image.png` thay vì `/assets/image.png`.
- **Quyết định & Lý do:** **Chấp nhận gợi ý.** Vì đường dẫn tương đối giúp tương thích hoàn toàn khi chạy ở root local và sub-folder trên GitHub Pages.
- **Kết quả thử nghiệm:** Đã commit bản sửa, chờ deploy lại và kiểm tra trên URL công khai bằng F12 Network tab. Kết quả: HTTP Status `200 OK`.

---

### Tình huống 2: Tối ưu Responsive Navigation trên thiết bị di động
- **Hiện tượng & Dữ kiện ban đầu:** Menu navigation bị vỡ khung khi xem trên màn hình điện thoại dưới 768px.
- **Nhận định trước khi hỏi AI:** Cần chèn `@media (max-width: 768px)` vào `css/style.css` để chuyển menu từ flex-direction `row` sang `column`.
- **Gợi ý từ AI:** AI gợi ý đoạn code Media Query điều chỉnh layout linh hoạt.
- **Quyết định & Lý do:** **Chấp nhận và tinh chỉnh.** Áp dụng CSS media query để giữ giao diện gọn gàng, tăng trải nghiệm người dùng trên di động.
- **Kết quả thử nghiệm:** Thử nghiệm thành công trên DevTools Responsive Mode và thiết bị thực tế.
