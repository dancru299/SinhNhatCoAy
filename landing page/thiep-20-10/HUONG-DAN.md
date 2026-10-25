# Thiệp 20/10 — hướng dẫn triển khai

## 3 kiểu thiệp để người gửi chọn

Trang mặc định (link gốc) là **Hoa Mang Tên Bạn**. Lần đầu vào trang, một popup 3 slide cho người dùng chọn kiểu thiệp; lựa chọn được nhớ trên máy, lần sau không hiện lại.

**Không có link cá nhân hoá.** Người dùng nhập tên người nhận, người gửi và lời chúc ngay trên trang, rồi **xuất ảnh hoặc video** để gửi đi. Trang bỏ qua mọi tham số trên link (`?to=…`, `?m=…`…), nên không ai tạo được link hiển thị nội dung tuỳ ý trên tên miền của bạn. Tên đã nhập được giữ tạm trong trình duyệt (sessionStorage) để mang sang kiểu thiệp khác qua menu **Kiểu thiệp**, đóng tab là mất. Người nhận có thể là bất kỳ ai: mẹ, cô giáo, đồng nghiệp, bạn thân, kể cả chính mình.

| File | Kiểu | Điểm nhấn |
|---|---|---|
| `bo-hoa.html` | **Bó Hoa 20/10** (nhẹ nhàng) | Phong bì mở, bó hoa nở, bướm, 4 giao diện màu, video Story MP4 |
| `index.html` | **Hoa Mang Tên Bạn** (mặc định, tiêu bản cyanotype) | Tên → giải trình tự "DNA" → loài hoa riêng có tên Latin vui, bản vẽ thực vật nét trắng, phiếu tiêu bản lật được, "Mã gen", tập tiêu bản lưu trên máy, ảnh Story 1080×1920 |
| `thiep-exe.html` | **Thiệp.exe** (hài hước, hoài cổ) | Máy tính kiểu Windows 95 tông hồng: nút "Không" bỏ chạy, cài đặt Hạnh phúc, lỗi "quá dễ thương" gây bão cửa sổ, quét virus, thùng rác chứa nỗi buồn, mèo trợ lý kể chuyện cười, ảnh Story |

**Về bản quyền:** "Hoa Mang Tên Bạn" chỉ lấy *ý tưởng chung* (tạo hoa từ tên bằng hàm băm), là kỹ thuật phổ biến. Toàn bộ phần thể hiện là của riêng mình: phong cách cyanotype và bản vẽ thực vật, màn giải trình tự DNA, tên Latin, phiếu tiêu bản, chú thích kiểu sách khoa học, câu chữ và mã nguồn. Không dùng chữ, hình, màu hay bố cục của trang tham khảo.

## Thiệp có gì

| Xu hướng 2026 | Áp dụng trong thiệp |
|---|---|
| **Pantone 2026: Cloud Dancer** (lần đầu Pantone chọn màu trắng) | Nền giấy trắng ngà có vân giấy (grain) |
| **WGSN/Coloro 2026: Transformative Teal** | Màu chủ đạo: số "20.10", giấy gói hoa, nút mở thiệp, lá bạch đàn |
| **Adobe 2026: thiết kế giác quan, "phồng, mềm, bóp được"** | Nút mở thiệp dạng khối phồng, bị bóp khi nhấn giữ; hoa có khối 3D mềm |
| **Canva 2026: "Imperfect by Design", Notes App Chic / scrapbook** | Lời chúc trên mẩu giấy ghi chú có băng dính washi và sticker |
| **Kinetic typography + variable font** | "20.10" bật lên, nét chữ "thở" và dày lên khi rê chuột/ngón tay lại gần |
| **Motion có mục đích** | Nhấn giữ → hoa nở theo thứ tự → lời chúc hiện dần như đang gõ |
| Trend TikTok/CapCut **"Chúc bản thân 20/10"** | Có mẫu lời chúc "Chính mình" |

**Animation mới (bản 2), tham khảo thiệp phong bì, thiệp pop-up bướm & xu hướng "aura" 2026:**
- Mở phong bì: con dấu bật ra → nắp lật → lá thư trồi lên → thiệp hiện ra theo vòng tròn lan rộng.
- Bướm bay quanh bó hoa, đậu lên từng bông, chạm gần thì bướm giật mình bay đi (có cả trong video Story).
- Vầng hào quang và tia nắng xoay chậm sau bó hoa, kèm sao lấp lánh.
- Chạm đúp thả tim kiểu Instagram, chạm chữ "20.10" để chữ nhún theo sóng kèm nốt nhạc.

**4 giao diện** (nút bảng màu góc trên trái, nhớ trên máy): `cloud` Cloud Dancer · `night` Đêm Hoa Đăng (nền tối) · `blush` Hồng Pastel · `lua` Lụa Đỏ (đỏ son và vàng).

**Sửa tên ngay trên thiệp:** chạm vào tên sau chữ "Gửi" hoặc chữ ký cuối lời chúc (có biểu tượng ✎) → gõ tên mới → Enter.

**Tương tác:** nhấn giữ để mở (rung nhẹ + âm báo tăng dần), chạm khoảng trống để trồng thêm hoa, chạm vào bó hoa để lay hoa và đọc lại lời chúc, vuốt để thả cánh hoa, nhạc hộp nhạc tự tạo (không cần file nhạc), nút "Lời chúc khác" có 7 mẫu.

**Cá nhân hoá:** nút **✏️ Tạo thiệp** → điền tên, chọn 1 trong 7 mẫu lời chúc (Mọi người, Mẹ, Người yêu, Đồng nghiệp, Cô giáo, Bạn bè, Chính mình) hoặc tự viết → **Áp dụng**, **🖼️ Lưu ảnh** hoặc **🎬 Tạo video**.

## Cách gửi: chỉ bằng ảnh hoặc video

Thiệp không tạo link riêng cho từng người. Người dùng tự làm thiệp trên trang rồi gửi file:

1. **Đưa thiệp lên mạng miễn phí bằng Cloudflare Pages** (`https://thiep-20-10.pages.dev`) hoặc GitHub Pages (`https://tuanjhg.github.io/thiep-20-10/`).
2. **Gửi riêng (Messenger, Zalo):** mở trang → nhập tên người nhận → lưu ảnh hoặc video → gửi file qua tin nhắn. Trên điện thoại, nút lưu sẽ mở bảng chia sẻ để gửi thẳng file.
3. **Đăng Story Facebook:** mở thiệp trên **điện thoại** → **🎬 Video Story** → đợi 10 giây → **Chia sẻ lên Story** (hoặc **Lưu video**). Trên Facebook: Tạo tin → chọn video → thêm nhãn dán **Nhạc**. Nếu muốn bạn bè tự làm thiệp, có thể gắn nhãn dán **Liên kết** là link trang chủ (không chứa tên ai).

> Nên xuất video trên điện thoại (Chrome Android / Safari iOS) để được MP4 chuẩn. Chrome máy tính cũng xuất MP4 (đã thử: 4.8 MB, 1080×1920). Nếu máy chỉ ra WebM, dùng **Lưu ảnh** thay thế.

### Deploy bằng GitHub Pages (khoảng 1 phút)

```bash
cd thiep-20-10
git init -b main && git add *.html *.png && git commit -m "Thiep 20/10"
gh repo create thiep-20-10 --public --source=. --push
gh api -X POST repos/tuanjhg/thiep-20-10/pages -f "source[branch]=main" -f "source[path]=/"
```

Khoảng 1–2 phút sau, link `https://tuanjhg.github.io/thiep-20-10/` hoạt động. Nếu đổi tên repo hoặc dùng host khác, sửa `og:image` / `og:url` trong `index.html` cho đúng domain mới (Facebook cần URL ảnh đầy đủ). Sau đó dán link vào [Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/) và bấm "Scrape Again" để làm mới ảnh xem trước.

### Deploy bằng Cloudflare Pages (chịu tải tốt nhất)

Thiệp là trang tĩnh: mọi hiệu ứng, nhạc và video đều chạy trên máy người xem, server chỉ trả về một file HTML khoảng 90 KB và ảnh `og.png`. Cloudflare Pages gói miễn phí không giới hạn số lượt truy cập và băng thông cho file tĩnh, phục vụ qua CDN đặt tại hàng trăm thành phố. Vài chục nghìn người mở cùng lúc vẫn không sao và không tốn tiền. Phụ thuộc bên ngoài duy nhất là font Google Fonts, vốn cũng chạy trên CDN của Google.

Cách 1, kéo-thả: dash.cloudflare.com → Workers & Pages → Create → Pages → **Upload assets** → kéo thư mục `thiep-20-10` vào → tên dự án `thiep-20-10` → link `https://thiep-20-10.pages.dev`.

Cách 2, dòng lệnh:

```bash
npx wrangler pages deploy thiep-20-10 --project-name thiep-20-10
```

Sau khi có link, sửa `og:image` (và `og:url`) trong cả 3 file `index.html`, `bo-hoa.html`, `thiep-exe.html` sang domain `pages.dev` rồi deploy lại.

### Phương án khác

| Cách | Ưu | Nhược |
|---|---|---|
| **Cloudflare Pages** (khuyên dùng) | Miễn phí, không giới hạn lượt xem, CDN nhanh ở Việt Nam | Cần tài khoản Cloudflare |
| GitHub Pages | Miễn phí, đã có `gh` đăng nhập sẵn | Repo phải public; giới hạn mềm 100 GB băng thông/tháng |
| Netlify / Vercel | Kéo-thả thư mục là xong | Gói free giới hạn băng thông/tháng |
| Chỉ đăng video lên Story, không host | Nhanh nhất | Mất phần tương tác |
| Quay màn hình điện thoại khi mở thiệp | Có cả nhạc và thao tác tay thật | Phải tự cắt video, dễ lộ thanh thông báo |

## Chạy thử trên máy

```bash
python -m http.server 8020 --directory thiep-20-10
```

Mở `http://localhost:8020/`. Thêm `?og=1` để xem bố cục ảnh xem trước (dùng tên mẫu có sẵn).
