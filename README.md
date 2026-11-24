# Trend Furniture – Website 3D

Website tĩnh (HTML + Three.js), chạy trực tiếp trên GitHub Pages.

## Cấu trúc
- `index.html` – toàn bộ trang (CSS + JS nằm trong file)
- `img/` – logo, ảnh sản phẩm, ảnh dự án (định dạng .webp)
- `.nojekyll` – để GitHub Pages phục vụ file nguyên trạng

## Đưa lên GitHub Pages
1. Tạo repository mới trên GitHub (Public), ví dụ `trendfurniture-website`.
2. Bấm **Add file → Upload files**, kéo thả `index.html`, `.nojekyll`, `README.md` và cả thư mục `img`, rồi **Commit changes**.
3. Vào **Settings → Pages** → Source: *Deploy from a branch* → Branch `main` / `/ (root)` → **Save**.
4. Sau 1–2 phút trang chạy tại `https://<tên-tài-khoản>.github.io/<tên-repo>/`.

## Trỏ tên miền (sau khi đã chạy được ở bước 4)
1. **Settings → Pages → Custom domain**: nhập `www.trendfurniture.com.vn` → Save (GitHub tự tạo file `CNAME`).
2. Tại nơi quản lý DNS của tên miền:
   - Bản ghi **CNAME**: `www` → `<tên-tài-khoản>.github.io`
   - Bản ghi **A** cho tên miền gốc (`@`): `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. Chờ DNS cập nhật, rồi bật **Enforce HTTPS** trong Settings → Pages.

Lưu ý: khi trỏ tên miền sang GitHub, website cũ đang chạy trên tên miền đó sẽ ngừng hiển thị.
