# Đố vui giơ ngón tay

Trò chơi trắc nghiệm cho học sinh tiểu học. Học sinh chọn đáp án bằng cách giơ ngón tay trước camera:

| Số ngón | Đáp án |
|---|---|
| 1 | A |
| 2 | B |
| 3 | C |
| 4 | D |

Chỉ giơ từ 1 đến 4 ngón; xòe cả 5 ngón là không hợp lệ (trò chơi sẽ đọc "Không phù hợp, mời chọn lại đáp án"). Giữ tay yên khoảng 1,5 giây để chốt đáp án.

## Tính năng
- Giao diện đổi màu và hình trang trí theo từng câu hỏi
- Giáo viên tự soạn câu hỏi (nút "Soạn câu hỏi"), lưu trên trình duyệt
- Nhận diện ngón tay bằng MediaPipe Hands, camera hiển thị trong ô tròn ở giữa màn hình
- Có thể bấm vào đáp án hoặc nhấn phím 1-4 nếu không dùng camera

## Kho câu hỏi
- `ngan-hang-cau-hoi.js`: 1000 câu lớp 2, học kì 1 (CTGDPT 2018), gồm 500 Toán và 500 Tiếng Việt, chia 3 mức Biết, Hiểu, Vận dụng.
- Toán: cộng, trừ có nhớ trong phạm vi 100. Tiếng Việt: từ chỉ sự vật, hoạt động, đặc điểm, điền khuyết chính tả, đặt câu.
- Mỗi lượt chơi lấy ngẫu nhiên 10 câu. Thanh trượt chọn tỉ lệ Toán : Tiếng Việt, nút "10 câu khác" để bốc lại.
- Nút "Câu tôi soạn" chuyển sang bộ câu hỏi giáo viên tự soạn.

## Chạy trên GitHub Pages
1. Tạo repository mới và tải cả 3 file `index.html`, `ngan-hang-cau-hoi.js`, `README.md` lên (hai file đầu phải cùng thư mục).
2. Vào **Settings > Pages**, ở mục **Branch** chọn `main` và thư mục `/ (root)`, rồi bấm **Save**.
3. Sau 1-2 phút, mở đường dẫn `https://<tên-tài-khoản>.github.io/<tên-repo>/`.

GitHub Pages dùng `https` nên trình duyệt cho phép bật camera. Máy cần có Internet để tải thư viện nhận diện tay.

## Chỉnh sửa
- Câu hỏi mẫu: biến `SAMPLE` trong `index.html`
- Thời gian giữ tay: biến `HOLD` (mili giây)
