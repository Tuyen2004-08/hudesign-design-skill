# AGENTS.md — Quy Tắc Thiết Kế Hủ Design (`@hudesign`) Dành Cho Codex

Tài liệu này là **bộ luật thiết kế bắt buộc** dành cho Codex khi tạo giao diện web/app, poster, banner, menu, infographic, card UI hoặc prompt ảnh AI dựa trên hệ thống công thức từ kênh TikTok **Hủ Design (`@hudesign`)**.

## 1. Thứ tự đọc trước khi thực thi
1. Đọc `schemas/hudesign_formulas.json` để lấy công thức chuẩn và điều kiện kích hoạt (`trigger`).
2. Tra cứu chi tiết tại `formulas/01` đến `formulas/05`.

## 2. Ma trận Quyết định Thiết kế (Decision Engine)

| Tình huống thiết kế | Công thức Hủ Design bắt buộc | Mã video `@hudesign` |
| :--- | :--- | :--- |
| Poster/Banner sản phẩm đơn lẻ | **Bố cục Trung tâm** + đặt chữ lớn phía sau chủ thể + mask tròn/bo góc + tag 4 góc | `video/7582220655031274770` |
| Poster cần nhịp chảy mềm mại | **Bố cục Đường chéo**: Tiêu đề lớn trên-trái, chủ thể giữa, chữ phụ dưới-phải | `video/7521727954192223495` |
| Poster cần lực hút cực mạnh vào tâm | **Giao điểm chữ X** (2 trục chéo + chữ nhỏ 4 góc) hoặc **Hội tụ** (tia/vật thể chỉ vào tâm) | `video/7524317963789372690` / `video/7526137835141729543` |
| Poster cần tỷ lệ kinh điển | **Tỷ lệ vàng (1.618)**: Chủ thể cung xoắn ốc lớn, tiêu đề ô trên-phải, mô tả ô dưới-phải | `video/7529573401598446866` |
| Menu / Bảng giá nhiều mục | **Proximity** (gom nhóm ngữ nghĩa) + **Menu 3 tầng** (dải màu tầng giữa + line 90°) | `video/7689793745599892754` / `video/7526475657501609224` |
| Poster/Tài liệu quá nhiều chữ | **Infographic 7 bước**: 2 cột + Ảnh neo tâm + Bar/Parabol chart + Quy trình mũi tên | `video/7531679531468442887` |
| Card UI/UX bị cứng, đại trà | **5 mẹo Card UI**: Vòm gradient, Custom Shape, thẻ vát nghiêng, vé xếp lớp, **tràn viền khung** | `video/7619709741140413704` |
| Danh sách đánh số đơn điệu | **Watermark Numbering**: Phóng to số `01, 02, 03` màu nhạt đặt chìm sau tiêu đề | `video/7634899872566512904` |
| Chủ đề tốc độ / thể thao / giao nhanh | **Cảm giác chuyển động**: Chữ nghiêng lặp mờ dần + Speed lines ngang + icon tia sét | `video/7524715684501146887` |
| Dùng Gradient cho nền / banner | **Luật Gradient <= 90°**. Nếu dùng cặp `180°` bắt buộc chèn **1 màu trung gian** khử vùng xám | `video/7671229776681585927` / `video/7539160968979401992` |

## 3. Các lỗi CẤM vi phạm (Hard Reject Rules)
1. **CẤM để chữ phẳng không phân cấp:** Phải tách tối thiểu 3 cấp độ (Trọng tâm lớn nhất → Tiêu đề phụ → Mô tả/Hotline).
2. **CẤM tạo vùng xám xỉn trong Gradient:** Không nối thẳng 2 màu đối diện `180°` (tím ↔ xanh lá, xanh dương ↔ cam) mà thiếu màu trung gian.
3. **CẤM rải thông tin rời rạc 4 góc không gom nhóm** (vi phạm Proximity).
4. **CẤM đặt chữ sáng trực tiếp lên vùng ảnh sáng** mà không có lớp phủ tối/mờ đảm bảo tương phản.
5. **CẤM dùng nền gradient cầu vồng chói** lấn át sản phẩm tối giản/công nghệ (ưu tiên nền tối hoặc gradient ánh sáng nhẹ).
