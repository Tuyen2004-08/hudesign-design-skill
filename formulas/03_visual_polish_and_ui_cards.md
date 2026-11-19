# 03. Nâng Cấp Thẩm Mỹ, Card UI/UX, Không Gian Âm & Chuyển Động

## A. 9 Mẹo Thiết Kế Sang Xịn Hơn (`video/7634899872566512904` • 85.1K)

| STT | Kỹ thuật | Trước (Before) | Sau (After — Công thức áp dụng) |
| :-: | :--- | :--- | :--- |
| **01** | **Phóng to số thứ tự làm nền** | Số `01.`, `02.`, `03.` nhỏ đặt ngang trước tiêu đề | Phóng cực lớn số `01, 02, 03` màu nhạt đặt chìm phía sau tiêu đề |
| **02** | **Không gian âm cho Logo** | Logo và tên thương hiệu rời rạc, khoảng trống vô nghĩa | Lồng hình phụ có ý nghĩa vào khoảng trống thân chủ thể (gấu con trong gấu mẹ) |
| **03** | **Lớp phủ mờ ảo nghệ thuật** | Ảnh nền và chữ phẳng | Thêm lớp kính mờ / hạt mưa phủ lên trên nền chữ và hình |
| **04** | **Ngắt nét chữ tại điểm nối** | Chữ tiêu đề (`NEW YEAR 2026`) liền nét bình thường | Cắt tạo khoảng hở nhỏ ở một số giao điểm nét → phá cách, vẫn dễ đọc |
| **05** | **Nghiêng chữ + Element tốc độ** | Nút `"GIAO NHANH"` chữ đứng thẳng tĩnh | Làm nghiêng chữ + thay chữ `O` bằng biểu tượng tia sét vàng |
| **06** | **Tăng chi tiết Icon UI** | Icon phẳng thiếu điểm nhấn | Dùng bộ icon 3D/gradient nhiều chi tiết cho chỉ số tương tác |
| **07** | **Tạo màu nhấn cho Menu UI** | Icon menu cài đặt đen trắng đơn sắc | Gán màu nhấn riêng có chủ đích cho từng icon |
| **08** | **Tràn viền & Góc nghiêng Card** | Sản phẩm (giày) nằm gọn cứng nhắc trong khung chữ nhật | Phóng lớn sản phẩm **tràn ra khỏi viền khung** kết hợp góc nghiêng nhẹ |
| **09** | **Mảng màu làm mờ nền Poster** | Nền poster đơn điệu | Thêm 1 mảng màu vàng cam ở cạnh dưới rồi làm mờ mạnh (`Gaussian Blur`) |

## B. 5 Mẹo Thiết Kế Card Layout Trong UI/UX (`video/7619709741140413704` • 75.6K)
1. **Bo góc thẻ & vòm nền Gradient:** Thay nền trắng trơn bằng bo góc mềm + vòm gradient phía sau sản phẩm (*Earbuds 2.5*).
2. **Sử dụng Custom Shape:** Bo cong lớn riêng 1 góc của thẻ/mảng nền.
3. **Thẻ hình khối vát nghiêng (Skewed Cards):** Thay thẻ chữ nhật đại trà bằng 4 thẻ vát nghiêng lệch nhẹ + nền gradient + icon 3D.
4. **Mô phỏng vật thể thực & xếp chồng layer:** Biến danh sách văn bản dọc thành thẻ vé máy bay (vết khuyết 2 bên, đường cắt đứt nét ngang, lưới giờ bay `09:00 → 13:00` và xếp chồng layer phần đỉnh).
5. **Đẩy chi tiết tràn khỏi khung hình (Card Overflow):** Cho bát Matcha Latte vươn ra ngoài góc trên bên phải khung thẻ để tạo chiều sâu 3D.

## C. 6 Nguyên Tắc Nền Tảng & Mẹo Tinh Tế (`video/7664239235318271250`, `video/7675723762343464210`, `video/7709495044721462536`)
1. **Trọng tâm:** Phóng cực lớn con số/yếu tố đắt giá nhất (`1K`).
2. **Phân cấp thị giác:** Chỉnh size chữ trước để tránh chữ phẳng → tách 4 tầng (Tiêu đề chính → Tiêu đề phụ → Mô tả → Hotline).
3. **Tương phản chữ sáng trên ảnh:** Thêm lớp phủ tối/mờ khi đặt chữ sáng lên ảnh nền sáng.
4. **Hiệu ứng viền dày cho chữ Sale:** Dùng viền dày (stroke) cho tiêu đề khuyến mãi (`SIÊU SALE THÁNG 8`).
5. **Làm chủ khoảng trống (Whitespace):** Giữ khoảng thở thoáng quanh chủ thể.
6. **Hệ thống lưới & Chọn Font đúng chủ đề.**

## D. Không Gian Âm (`video/7522856606074227975`) & Cảm Giác Chuyển Động (`video/7524715684501146887`)
- **Không gian âm:** (1) *Hình + Hình:* Mèo trắng + nền xanh tạo hình Chuột; Cây đen tạo mặt Khỉ đột & Sư tử; Gấu đen tạo Nốt nhạc. (2) *Chữ + Chữ:* Lồng `I`, `T` trắng vào lòng chữ `D`, `O` đỏ (`DO IT.`).
- **Cảm giác chuyển động:** (1) Làm nghiêng và sao chép lặp lại chữ mờ dần theo hướng chạy; (2) Xếp chữ dọc dứt khoát đồng trục chủ thể tốc độ (xe F1); (3) Thêm **đường tốc độ (speed lines)** ngang chuyển sắc xếp so le phía sau chủ thể.
