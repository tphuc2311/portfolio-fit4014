# Portfolio cá nhân – FIT4014

Website portfolio tĩnh giới thiệu sinh viên, kỹ năng, dự án học tập và thông tin liên hệ. Dự án sử dụng **HTML5, CSS3 và JavaScript thuần**, không cần framework hoặc bước build.

## 1. Mục tiêu

- Thực hành tổ chức mã nguồn website.
- Quản lý lịch sử thay đổi bằng Git và GitHub.
- Viết tài liệu dự án và nhật ký sử dụng AI.
- Triển khai website bằng GitHub Pages.
- Kiểm tra website trên máy tính và thiết bị di động.

## 2. Công nghệ

| Công nghệ | Vai trò |
|---|---|
| HTML5 | Cấu trúc và nội dung |
| CSS3 | Giao diện, bố cục responsive, hiệu ứng |
| JavaScript | Menu trên thiết bị di động và năm hiện tại ở chân trang |
| Git | Quản lý phiên bản |
| GitHub | Lưu trữ repository |
| GitHub Pages | Xuất bản website tĩnh |

## 3. Cấu trúc thư mục

```text
portfolio-fit4014/
├── index.html
├── README.md
├── AI_LOG.md
├── RELEASE_NOTES.md
├── .nojekyll
└── assets/
    ├── css/
    │   └── style.css
    └── js/
        └── main.js
```

## 4. Chạy website ở máy local

1. Tải hoặc clone repository về máy.
2. Mở thư mục dự án.
3. Mở `index.html` bằng trình duyệt (Chrome, Edge hoặc Firefox).

Có thể dùng tiện ích Live Server trong Visual Studio Code để tự động tải lại trang khi chỉnh sửa. Website không cần cài thư viện bằng npm.

## 5. Cá nhân hóa trước khi công bố

Tìm và thay các nội dung mẫu sau trong `index.html`:

- `[HỌ VÀ TÊN]`: họ tên sinh viên.
- `[20XX–20XX]`: thời gian học tập phù hợp.
- Hai dự án có nội dung trong dấu ngoặc vuông: thay bằng bài tập/sản phẩm có thật.
- `your.email@example.com`: email liên hệ công khai (chỉ thay bằng địa chỉ bạn muốn công khai).
- Các liên kết GitHub/LinkedIn: thay bằng trang cá nhân thật hoặc bỏ nếu chưa có.

Không nên giới thiệu kỹ năng hoặc dự án mà bản thân chưa thực hiện. Sau khi sửa, kiểm tra lại toàn bộ liên kết và nội dung.

## 6. Quy trình Git và GitHub

Mở Terminal tại thư mục dự án. Repository dự kiến: `https://github.com/tphuc2311/portfolio-fit4014`.

```bash
git init
git add .
git commit -m "chore: initialize portfolio project"
git branch -M main
git remote add origin https://github.com/tphuc2311/portfolio-fit4014.git
git push -u origin main
```

Các lần cập nhật tiếp theo:

```bash
git status
git add .
git commit -m "feat: complete portfolio content"
git push
```

Gợi ý quy ước commit:
- `feat:` thêm chức năng hoặc nội dung mới.
- `fix:` sửa lỗi.
- `docs:` cập nhật tài liệu.
- `style:` chỉnh giao diện, không thay đổi logic.
- `chore:` công việc cấu hình hoặc bảo trì.

Nếu Git báo remote `origin` đã tồn tại, không chạy lặp lại lệnh `git remote add`. Kiểm tra bằng `git remote -v`; nếu URL sai thì dùng `git remote set-url origin https://github.com/tphuc2311/portfolio-fit4014.git`.

## 7. Triển khai GitHub Pages

1. Đẩy mã nguồn lên nhánh `main` của repository GitHub.
2. Mở repository → **Settings** → **Pages**.
3. Trong **Build and deployment**, chọn **Deploy from a branch**.
4. Chọn branch `main`, thư mục `/(root)`, sau đó nhấn **Save**.
5. Chờ GitHub hoàn tất triển khai. URL thường có dạng:
   `https://tphuc2311.github.io/portfolio-fit4014/`
6. Mở URL công khai để kiểm tra. Nếu chưa cập nhật, chờ workflow Pages chạy xong rồi tải lại trang.

Với repository có tên `USERNAME.github.io`, URL thường là `https://tphuc2311.github.io/`.

## 8. Kiểm thử trước khi Release

- [ ] Mở `index.html` ở local, không xuất hiện lỗi hiển thị.
- [ ] Các mục điều hướng cuộn đến đúng section.
- [ ] Menu trên điện thoại mở/đóng được.
- [ ] Bố cục không tràn ngang ở màn hình nhỏ.
- [ ] Email và liên kết ngoài đúng địa chỉ.
- [ ] Không còn nội dung `[ ... ]` chưa thay thế.
- [ ] Mở được URL GitHub Pages ở cửa sổ ẩn danh.
- [ ] Kiểm tra DevTools → Console và Network, xử lý lỗi 404 hoặc JavaScript nếu có.

## 9. Tạo Release v1.0.0

Sau khi kiểm thử và cập nhật tài liệu:

```bash
git add .
git commit -m "docs: finalize project documentation"
git push
git tag -a v1.0.0 -m "Release version 1.0.0"
git push origin v1.0.0
```

Trên GitHub: vào **Releases** → **Draft a new release** → chọn tag `v1.0.0` → đặt tiêu đề `Portfolio v1.0.0` → điền nội dung từ `RELEASE_NOTES.md` → **Publish release**.

## 10. Tác giả

- Họ tên: [HỌ VÀ TÊN]
- Lớp: [LỚP]
- Học phần: FIT4014 – Thiết kế web và triển khai hệ thống phần mềm

> Đây là dự án học tập. Hãy cá nhân hóa thông tin, kiểm thử trên tài khoản GitHub của mình và hiểu các lệnh trước khi trình bày với giảng viên.
