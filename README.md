# WD-Lab02 — Velora Auto

## Thông tin sinh viên

- **Họ và tên:** Phan Ngọc Minh Hằng
- **MSSV:** 23110081
- **Môn học:** Thiết Kế Web
- **Bài thực hành:** WD-Lab02
- **Chủ đề:** Website E-commerce ô tô — Velora Auto

---

## Giới thiệu

**Velora Auto** là website E-commerce giới thiệu và đặt yêu cầu tư vấn các mẫu ô tô.

Project được xây dựng hoàn toàn bằng **HTML**, tập trung vào cấu trúc tài liệu, semantic HTML, liên kết giữa các trang, bảng dữ liệu, biểu mẫu và cách tổ chức tài nguyên local.

Website giữ đúng phạm vi **HTML-only**, không sử dụng CSS, JavaScript, framework hoặc backend.

---

# TỔNG QUAN MỨC HOÀN THÀNH

## Phần đã hoàn thành

- Website E-commerce HTML-only theo chủ đề **ô tô**, khác ngành hàng giày dép của StepUp Shoes.
- Hoàn thành **08 trang HTML** liên kết với nhau, gồm **05 trang bắt buộc** và **03 trang mở rộng**.
- Có **15 sản phẩm**, được định danh từ `CAR01` đến `CAR15`, vượt yêu cầu tối thiểu 10 sản phẩm.
- Sản phẩm được tổ chức thành **05 nhóm xe**:
  - City & Sedan
  - SUV & Crossover
  - Electric & Hybrid
  - Sport & Performance
  - Track & Racing
- Hình ảnh được lưu local trong thư mục `images/` và có thuộc tính `alt`.
- Relative links và fragment links dạng `#CARxx` được tổ chức nhất quán.
- Có trang chi tiết sản phẩm.
- Bảng so sánh sử dụng đầy đủ các thành phần:
  - `caption`
  - `thead`
  - `tbody`
  - `tfoot`
  - `th`
  - `scope`
  - `colspan`
  - `rowspan`
- Form HTML tĩnh sử dụng phương thức `GET`.
- Form có:
  - `label`
  - `for`
  - `id`
  - `name`
  - `required`
  - `select`
  - `radio`
  - `checkbox`
  - `textarea`
  - `button`
- Trang `xac-nhan.html` nêu đúng giới hạn của website HTML tĩnh: không lưu đơn, không thanh toán và không xử lý dữ liệu thật.
- Project đã chạy qua **XAMPP/Apache** tại localhost.
- Source code giữ đúng phạm vi **HTML-only**, không sử dụng CSS, JavaScript, framework hoặc backend.

---

## Cấu trúc sản phẩm

Website hiện có **15 mẫu xe**, được đánh mã từ:

`CAR01` → `CAR15`

Các sản phẩm được chia thành 05 nhóm chính:

| Nhóm | Nội dung |
|---|---|
| City & Sedan | Các mẫu xe đô thị và sedan |
| SUV & Crossover | Các mẫu SUV và crossover |
| Electric & Hybrid | Xe điện và xe hybrid |
| Sport & Performance | Xe thể thao và hiệu năng cao |
| Track & Racing | Xe định hướng đường đua và hiệu suất cao |

---

## Các trang của website

Project gồm tổng cộng **08 trang HTML**.

### 05 trang chính

1. `index.html` — Trang chủ
2. `chi-tiet.html` — Chi tiết sản phẩm
3. `bang-gia.html` — Bảng giá và so sánh
4. `dat-hang.html` — Form đăng ký/tư vấn
5. `xac-nhan.html` — Trang xác nhận

### 03 trang mở rộng

6. `bo-suu-tap.html` — Bộ sưu tập xe
7. `dich-vu.html` — Dịch vụ
8. `cam-nang.html` — Cẩm nang

---

## Form HTML

Form được xây dựng bằng HTML và sử dụng:

```html
<form action="xac-nhan.html" method="get">
```

Form có các thành phần nhập liệu như:

- Họ và tên
- Thông tin liên hệ
- Mẫu xe
- Phiên bản
- Màu xe
- Mục đích liên hệ
- Thời gian
- Ghi chú
- Radio button
- Checkbox
- Select
- Textarea
- Button

Các trường cần thiết sử dụng `required`, đồng thời `label`, `for`, `id` và `name` được tổ chức phù hợp.

---

## Bảng giá và so sánh

Trang bảng giá sử dụng semantic table HTML với cấu trúc:

```html
<table>
    <caption>Bảng giá và so sánh xe Velora Auto</caption>

    <thead>
        <!-- Tiêu đề bảng -->
    </thead>

    <tbody>
        <!-- Dữ liệu sản phẩm -->
    </tbody>

    <tfoot>
        <!-- Tổng hợp dữ liệu -->
    </tfoot>
</table>
```

Bảng có sử dụng `th`, `scope`, `rowspan` và `colspan` để thể hiện đúng cấu trúc dữ liệu.

---

## Liên kết và hình ảnh

Website sử dụng **relative links** để liên kết giữa các trang:

```html
<a href="chi-tiet.html">Chi tiết sản phẩm</a>
```

Fragment links được sử dụng để truy cập trực tiếp từng sản phẩm:

```html
<a href="chi-tiet.html#CAR01">Xem CAR01</a>
```

Hình ảnh được lưu local trong thư mục `images/`:

```html
<img src="images/car01.jpg" alt="Velora Auto CAR01">
```

---

# PHẦN LÀM THÊM

So với yêu cầu tối thiểu, project được mở rộng thêm:

- Tăng số lượng sản phẩm từ tối thiểu **10 lên 15 mẫu xe**.
- Tổ chức sản phẩm thành **05 nhóm xe**.
- Thêm **03 trang mở rộng**:
  - `bo-suu-tap.html`
  - `dich-vu.html`
  - `cam-nang.html`
- Bổ sung các nhóm:
  - Electric & Hybrid
  - Sport & Performance
  - Track & Racing
- Mở rộng form với:
  - Màu xe
  - Phiên bản
  - Mục đích liên hệ
  - Thời gian
  - Ghi chú
- Các phần mở rộng vẫn giữ đúng phạm vi **HTML-only**.

---

# PHẦN CẦN CHÈN TRƯỚC KHI NỘP PDF

Các minh chứng cần bổ sung vào báo cáo trước khi xuất PDF:

- Ảnh **XAMPP Control Panel** có Apache ở trạng thái `Running`.
- Ảnh website chạy trên trình duyệt bằng `localhost`.
- Đủ ảnh minh chứng **S1–S8** theo yêu cầu.
- Ảnh trang bảng giá thể hiện rõ:
  - Giá niêm yết
  - Giá ưu đãi
  - Chênh lệch
  - Phần tổng trong `tfoot`
- URL GitHub repository.
- Ảnh GitHub repository.
- Ảnh commit history.
- Ảnh kết quả `git status` với trạng thái:

```text
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```

---

## Công nghệ sử dụng

- HTML5
- XAMPP
- Apache
- Git
- GitHub
- Visual Studio Code

Không sử dụng:

- CSS
- JavaScript
- Framework
- Backend
- Database

---

## Chạy project trên localhost

Đặt thư mục project trong thư mục web server của XAMPP hoặc cấu hình thư mục phù hợp, sau đó khởi động **Apache**.

Truy cập project trên trình duyệt thông qua địa chỉ localhost tương ứng.

---

## Git & GitHub

Project được quản lý phiên bản bằng Git và lưu trữ trên GitHub.

Kiểm tra trạng thái project:

```bash
git status
```

Thêm thay đổi:

```bash
git add .
```

Tạo commit:

```bash
git commit -m "update: WD Lab02 Velora Auto"
```

Đẩy thay đổi lên GitHub:

```bash
git push
```

---

## Ghi chú

Website được xây dựng phục vụ bài thực hành **WD-Lab02** của môn **Thiết Kế Web**.

Toàn bộ chức năng đặt hàng/đăng ký trên website chỉ sử dụng **HTML tĩnh**. Website không có backend nên không thực hiện lưu đơn hàng, thanh toán hoặc xử lý dữ liệu thực tế.

---

**Sinh viên thực hiện:** Phan Ngọc Minh Hằng  
**MSSV:** 23110081
