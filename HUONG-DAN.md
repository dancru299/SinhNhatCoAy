# Hướng Dẫn Cá Nhân Hóa & Deploy Website Sinh Nhật Hoạt Hình (VOGUE TOON! × Bé Thỏ Squishy)

Bộ website gồm 2 trang liên kết trực tiếp với nhau trên cùng một domain:
1. **[`index.html`](./index.html)** (`/`): Cuốn truyện tạp chí hoạt hình **VOGUE TOON!** (Bìa Chibi, Card Hoa Hồng & Hoa Sữa Tháng 10, Máy Đo Chỉ Số Em Bé, Hộp Mù Blind Box, và Bánh Kem Thổi Nến Thật Qua Microphone).
2. **[`squishy.html`](./squishy.html)** (`/squishy` hoặc `/squishy.html`): **Món Quà Đặc Biệt Cuối Cùng** — Trang tương tác vật lý **Bé Thỏ Squishy Chậm Tăng (Slow-Rising Foam & Mochi)** sống động như ngoài đời thật.

---

## 1. Cách sửa Tên, Ngày sinh, Ảnh và Lời chúc

Mở file [`index.html`](./index.html) và tìm đến vùng cấu hình `const BIRTHDAY_CONFIG = { ... }`:

```javascript
const BIRTHDAY_CONFIG = {
  herName: "Lưu Ngân Hà",                 // Tên của cô ấy
  herTitle: "Sweet 16 • The Shining Star", // Dòng chữ phụ trên bìa tạp chí
  yourName: "Một người sắp đặc biệt",      // Tên/chữ ký của bạn ở cuối bức thư
  birthdayDate: "27 • 10",                // Ngày tháng sinh nhật trên mã vạch (27/10/2010)
  issueNumber: "SỐ ĐẶC BIỆT • SWEET 16",  // Số phát hành
  ageBadge: "Sweet 16!",                  // Chữ hiển thị trên chiếc bánh kem
  coverPhotoUrl: "",                     // Để trống sẽ hiện Nhân vật Chibi Hoạt Hình (hoặc điền link ảnh thật)
  memoryPhotos: ["", "", ""],            // 3 ảnh kỷ niệm nhỏ ở Chương Chỉ Số
  ...
};
```

---

## 2. Các Điểm Chạm Độc Nhất Vô Nhị Trên Website

1. **Bìa Tạp Chí Hoạt Hình `VOGUE TOON!` (Chương 1):**
   - Đổi 4 phong cách nhân vật Chibi (Nàng Thơ Hoa Hồng & Hoa Sữa, Công Chúa Vương Miện Dâu Tây, Thiên Thần Trà Sữa Khoai Môn, Bé Thỏ Kuromi & My Melody) hoặc dán ảnh thật lên bìa.
   - Bấm vào **Mã Vạch Siêu Thị** góc dưới để in ra **Hóa Đơn Kiểm Định Bảo Vật (Định giá: VÔ GIÁ)**.
2. **Card Hoa Đặc Biệt: Bó Hoa Hồng & Hoa Sữa Mùa Thu (Chương 2):**
   - Tương tác chạm để cắm thêm những đóa Hoa Hồng phấn/tím lilac và chùm Hoa Sữa 5 cánh trắng kem đặc trưng tháng 10, kèm hiệu ứng **Mưa Cánh Hoa Mùa Thu** bay khắp màn hình.
3. **Phòng Thí Nghiệm Chỉ Số & Thẻ Sticker Lật Mặt (Chương 3):**
   - Càng bấm đo lại thì bình năng lượng và chỉ số Đáng Yêu / Luôn Đúng càng tăng vọt lên 9,999%.
4. **Đập Hộp `BLIND BOX` Đồ Chơi Hoạt Hình (Chương 4):**
   - Chạm để lắc hộp nghe tiếng lọc cọc, sau đó kéo khóa trượt để xé hộp nhận **4 Vé Đặc Quyền (SSR / UR / SECRET 1/144)**.
5. **Thổi Tắt "Bé Lửa Nhỏ" Qua Microphone & Bức Tâm Thư Sổ Tay (Chương 5):**
   - Thổi hơi thật vào điện thoại (hoặc nhấn giữ) để thổi tắt ngọn lửa hoạt hình trên bánh kem, mở khóa bức tâm thư viết tay.
6. **Món Quà Đặc Biệt Cuối Cùng: Bé Thỏ Squishy Chậm Tăng (`/squishy` - `squishy.html`):**
   - Ở cuối trang chính có thẻ bật mí **"Khoan Đã! Vẫn Còn 1 Món Quà Đặc Biệt Nữa!"** dẫn sang trang `/squishy.html` (`/squishy`).
   - Tại đây, cô ấy có thể trực tiếp **ấn lún ngón tay lên người Bé Thỏ**, **nhấn giữ ép dẹp lép**, **véo 2 má bánh bao**, **kéo dãn đôi tai Mochi**, chọn 3 chế độ vật lý (**Chậm Tăng 3.5s**, **Siêu Chậm Tăng 6s**, **Mochi Nước Nảy Tưng Tưng**), đổi **4 mùi hương Squishy** (Kem Dâu Tây, Khoai Môn Taro, Hoa Sữa & Hoa Hồng Tháng 10, Đào Mật Ong) kèm **âm thanh ASMR bọt khí xì hơi** chân thực.

---

## 3. Cách Deploy Lên Vercel

Mở Terminal tại thư mục `d:\TestCode\SinhNhat` và chạy:
```bash
npx vercel --prod
```
Hoặc đẩy thư mục lên GitHub và Import vào [vercel.com/new](https://vercel.com/new). File [`vercel.json`](./vercel.json) đã cấu hình sẵn `cleanUrls: true` và `rewrites` để cả `/squishy` lẫn `/squishy.html` đều hoạt động mượt mà trên cùng domain!
