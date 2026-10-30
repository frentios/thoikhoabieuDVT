# Thời khóa biểu THPT Dương Văn Thì

Trang xem thời khóa biểu theo lớp và theo giáo viên, chạy trên GitHub Pages.

- `index.html`: toàn bộ trang (giao diện, bộ đọc PDF, trang quản trị).
- `data.json`: dữ liệu thời khóa biểu và giờ học. Trang quản trị ghi đè file này mỗi lần cập nhật.

## Cập nhật thời khóa biểu

1. Mở trang với đuôi `#quan-tri`, ví dụ `https://frentios.github.io/thoikhoabieuDVT/#quan-tri`.
2. Lần đầu trên mỗi máy: dán một fine-grained token GitHub chỉ cho repo này, quyền **Contents: Read and write**.
3. Kéo thả 3 file PDF (TKB tổng hợp lớp và giáo viên, TKB giáo viên, TKB lớp), chỉnh giờ học nếu cần, bấm **Cập nhật cho mọi người**.
4. Sau khoảng 1 đến 2 phút GitHub Pages đăng lại, mọi người mở trang sẽ thấy bản mới.

## Trang riêng cho từng lớp

- `10a1/index.html`: chỉ hiện thời khóa biểu lớp 10A1, link `https://frentios.github.io/thoikhoabieuDVT/10a1/`.
- `12a11/index.html`: chỉ hiện thời khóa biểu lớp 12A11, link `https://frentios.github.io/thoikhoabieuDVT/12a11/`.
- Trang con đọc chung `data.json` ở thư mục gốc, nên tự cập nhật khi trang quản trị lưu bản mới.
- Muốn thêm lớp khác: chép thư mục `10a1`, đổi `window.TKB_LOCK='10A1'` và tiêu đề trong file sang tên lớp mới.
