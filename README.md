# Thư gửi Na

Trang tĩnh (HTML/CSS/JS thuần), không cần build.

## Cấu trúc
- `index.html`  trang chính (khoá, phong bì, thư, nhạc)
- `music/o-trong-khu-rung.mp3`  file nhạc (bạn tự thêm vào)
- `vercel.json`  tắt index công cụ tìm kiếm, cache nhạc

## Tuỳ chỉnh (đầu đoạn `<script>` trong `index.html`)
- `PASSWORD`  mật khẩu mở khoá (đang là `7`)
- `START_AT`  giây bắt đầu phát nhạc (ví dụ `45` để vào thẳng đoạn bạn muốn)
- `VOLUME`    âm lượng tối đa, 0 đến 1

## Deploy lên Vercel
Cách 1, kéo thả qua CLI:
    npm i -g vercel
    cd thu-gui-na
    vercel          # lần đầu, chọn mặc định (Framework: Other)
    vercel --prod

Cách 2, qua GitHub: đẩy thư mục này lên một repo, vào vercel.com, Add New Project,
chọn repo, Framework Preset = Other, Deploy.

Sau khi deploy, mở link trên điện thoại để thử: nhập mật khẩu, chạm phong bì, nhạc sẽ tự phát.
