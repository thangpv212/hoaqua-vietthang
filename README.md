# Hoa Quả Việt Thắng 🌱

Website giới thiệu + liên hệ cho hộ kinh doanh trái cây **Hoa Quả Việt Thắng**.
Web tĩnh (HTML + CSS + JS thuần), responsive, có animation — không cần backend.

## Cấu trúc thư mục

```
website-hoaqua/
├── index.html          # Toàn bộ nội dung trang
├── css/style.css       # Giao diện — màu sắc tập trung ở :root (CSS variables)
├── js/main.js          # Menu, hiệu ứng cuộn, lightbox ảnh giấy phép
├── images/
│   ├── products/       # Ảnh 12 sản phẩm (tải từ Unsplash)
│   ├── hero/           # Ảnh banner + ảnh giới thiệu
│   └── license/        # Đặt ảnh giấy phép kinh doanh tại đây
└── README.md
```

## Cách chỉnh nội dung

### 1. Thông tin hộ kinh doanh & liên hệ
Mở `index.html`, tìm các dòng sau và thay bằng thông tin thật:
- **Địa chỉ cửa hàng** — tìm `[Điền địa chỉ cửa hàng]`.
- **Số / nơi cấp / ngày cấp giấy phép** — tìm `[Điền số GPKD]`, `[Điền nơi cấp]`, `[Điền ngày cấp]`.
- Số điện thoại, Zalo, Facebook đã được điền sẵn theo thông tin bạn cung cấp.

### 2. Đổi ảnh sản phẩm / thêm sản phẩm mới
- Ảnh sản phẩm nằm ở `images/products/`. Thay ảnh mới vào đúng tên file, hoặc đổi đường dẫn `src` trong `index.html`.
- Để **thêm 1 sản phẩm**: copy nguyên 1 khối `<article class="card">…</article>` trong `index.html`, dán thêm rồi sửa tên, giá và ảnh.
- Ảnh hiện tại là ảnh minh hoạ tải từ mạng — bạn nên thay bằng ảnh thật của cửa hàng.
- Nút **Đặt** ở mỗi sản phẩm tự **sao chép tin nhắn** (kèm tên + giá sản phẩm) rồi mở Zalo, người mua chỉ cần dán (paste). Nội dung tin nhắn soạn sẵn trong `js/main.js` (tìm `Xin chào Hoa Quả Việt Thắng`).

### 3. Thêm ảnh giấy phép kinh doanh
1. Đặt file ảnh vào `images/license/giay-phep.jpg`.
2. Trong `index.html`, ở phần `GIẤY PHÉP KINH DOANH`, bỏ comment quanh thẻ `<img class="license-img">` và xoá khối `<div class="license-empty">…</div>`.
3. Ảnh sẽ tự phóng to khi người xem bấm vào (lightbox đã cài sẵn).

### 4. Đổi màu sắc toàn site
Mở `css/style.css`, sửa các giá trị trong khối `:root` (đầu file). Toàn bộ màu chủ đạo, nền, chữ, bo góc, đổ bóng đều nằm ở đó.

## Chạy thử ở máy
Mở thẳng file `index.html` bằng trình duyệt (double-click) là xem được, không cần cài gì.

## Deploy lên GitHub Pages
1. Tạo repository trên GitHub và đẩy thư mục này lên.
2. Vào **Settings → Pages → Source: Deploy from a branch → chọn nhánh `main`, thư mục `/ (root)` → Save**.
3. Vài phút sau website sẽ có tại `https://<tên-tài-khoản>.github.io/<tên-repo>/`.

---

Ghi chú: ảnh sản phẩm đang dùng là ảnh minh hoạ từ Unsplash — vui lòng kiểm tra lại đúng loại quả trước khi đưa vào sử dụng chính thức.
