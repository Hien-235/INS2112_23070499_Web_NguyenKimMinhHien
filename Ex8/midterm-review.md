# Midterm Review

## Mistake 1: Thứ tự thẻ `<meta charset="UTF-8">` và `<title>`
- **My answer:** Đặt thẻ `<title>` lên trước thẻ `<meta charset="UTF-8">` trong phần `<head>`.
- **Correct answer:** Đặt `<meta charset="UTF-8">` ngay đầu thẻ `<head>`, luôn đứng trước thẻ `<title>`.
- **Why:** Trình duyệt đọc mã từ trên xuống dưới, nên cần biết bảng mã UTF-8 trước khi phân tích tiêu đề để tránh lỗi hiển thị ký tự tiếng Việt trên tab.
- **Where to review:** ebook/01-html-basics.md, section HTML5 Boilerplate

## Mistake 2: Đường dẫn tương đối cho hình ảnh và CSS
- **My answer:** Dùng dấu gạch chéo ở đầu như `href="/css/style.css"` hoặc `src="../images/logo.jpg"` khi file HTML nằm ngay ở thư mục gốc `project/`.
- **Correct answer:** Dùng đường dẫn tương đối thuần túy `href="css/style.css"` và `src="images/logo.jpg"`.
- **Why:** Dấu `/` ở đầu trỏ về thư mục gốc của máy chủ (root domain) gây lỗi 404 khi mở trực tiếp file trên máy hoặc đẩy lên thư mục con, còn `../` leo ngược ra ngoài thư mục dự án.
- **Where to review:** ebook/02-file-structure.md, section Relative Paths

## Mistake 3: Nhảy cấp đề mục HTML
- **My answer:** Dùng thẻ `<h3>` ngay sau `<h1>` chỉ vì muốn cỡ chữ trông nhỏ hơn.
- **Correct answer:** Tuân thủ thứ tự phân cấp `<h1>` -> `<h2>` -> `<h3>`, và dùng CSS `font-size` để chỉnh kích thước hiển thị.
- **Why:** Thẻ đề mục thể hiện cấu trúc ngữ nghĩa cho trình đọc màn hình và công cụ tìm kiếm, không dùng để thay thế cho việc định dạng cỡ chữ.
- **Where to review:** ebook/03-text-and-images.md, section Heading Hierarchy