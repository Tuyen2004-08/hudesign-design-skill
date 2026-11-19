---
name: hudesign-design-skill
description: Bộ skill thiết kế đồ họa, bố cục, hệ thống lưới, Card UI/UX, Gradient, phối màu và Typography chuẩn hóa từ toàn bộ kênh TikTok Hủ Design (@hudesign). Dùng cho Codex khi thiết kế giao diện web/app, poster, banner, menu, infographic, card UI hoặc review thẩm mỹ Before/After.
---

# Hủ Design Visual Skill (`@hudesign`)

Skill này đóng gói hệ thống công thức thực chiến từ kênh TikTok **Hủ Design (`@hudesign`)** thành các cổng kiểm tra bắt buộc (Design Gates), bất biến thị giác (Visual Invariants), sơ đồ minh họa SVG, sổ cái video tham khảo và công thức CSS/HTML sẵn chạy cho Codex.

> Đọc nhanh trước khi viết code hoặc sinh thiết kế: [Visual Playbook](references/visual-playbook.md) · [CSS Recipes](references/css-recipes.md) · [Reference Video Ledger](references/reference-video-ledger.json) · [Visual Lab HTML](references/visual-lab.html)

## Cổng Kiểm Tra Thiết Kế 5 Bước (Design Gate — Bắt buộc cho mọi dự án)

1. **Cổng 1 — Xác định Bài toán & Khóa Bố cục (`LAY-01` đến `LAY-09`):**
   - Không bắt tay vào code hay đặt phần tử ngẫu nhiên. Mở `references/visual-playbook.md`, đối chiếu bảng **"Xem gì trước?"** để chọn đúng 1 khung bố cục (*Trung tâm + Mask, 1/3, Đường chéo, Đường cong, Khung, Đối xứng, Lặp lại, Chữ X, Hội tụ, Tỷ lệ vàng 1.618, Proximity, Infographic 7 bước* hoặc *Menu 3 tầng*).
2. **Cổng 2 — Khóa Hệ thống Lưới (`GRD-01`):**
   - Chọn rõ 1 trong 6 lưới: `RADIAL`, `MODULAR`, `AXIAL`, `COLUMN`, `HIERARCHICAL` hoặc `BASELINE`.
   - Web/Landing Page mặc định dùng `Column Grid 12 cột` + `Baseline Grid 8px`.
3. **Cổng 3 — Khóa Phân cấp Chữ & Font (`TYP-01`):**
   - Chỉnh kích thước chữ trước để diệt lỗi "chữ phẳng". Tách tối thiểu 3–4 tầng rõ rệt (Trọng tâm/Con số cực lớn → Tiêu đề phụ → Mô tả → Hotline/CTA).
   - Chọn đúng 1 trong 5 nhóm Font (*Sans Serif, Serif, Script, Display, Slab Serif*) theo đúng lĩnh vực thương hiệu.
4. **Cổng 4 — Khóa Màu sắc & Luật Gradient (`COL-01`, `COL-02`):**
   - Áp dụng 1 trong 3 công thức (*Đơn sắc, Liền kề, Bổ sung*) và tách rõ **tương phản 4 lớp UI** (Nền tổng → Thẻ Card → Khối phụ → Điểm nhấn).
   - **Bất biến Gradient:** Hai màu trong dải chuyển sắc phải nằm trong góc `<= 90°`. Nếu bắt buộc nối 2 màu đối diện `180°`, **bắt buộc chèn 1 điểm màu trung gian** để khử vùng xám xỉn (dead zone). Không dùng nền gradient cầu vồng rực rỡ lấn át sản phẩm tối giản.
5. **Cổng 5 — Nâng cấp Thẩm mỹ & Nghiệm thu QA (`POL-01..03`, `UI-01`):**
   - Chỉ chọn **1–2 kỹ thuật nâng cấp** đúng ngữ cảnh (*Watermark Numbering, Card Overflow tràn viền, Ticket Stack, Skewed Cards, Mask chiều sâu sau chủ thể, Ngắt nét chữ, Không gian âm, Speed lines, Mảng màu làm mờ nền*).
   - Rà soát đủ 10 tiêu chí QA trước khi bàn giao.

## 5 Bất Biến Cấm Vi Phạm (Hard Reject Rules)
- **KHÔNG để chữ phẳng** thiếu trọng tâm rõ trong 2 giây đầu.
- **KHÔNG để vùng xám xỉn** ở giữa dải Gradient `180°`.
- **KHÔNG rải thông tin rời rạc 4 góc** không gom nhóm theo ngữ nghĩa (vi phạm Proximity).
- **KHÔNG đặt chữ sáng trực tiếp lên vùng ảnh sáng** thiếu lớp phủ tối/mờ đảm bảo tương phản.
- **KHÔNG nhồi nhét quá 2 kỹ thuật trang trí** trên cùng một khung hình gây rối mắt.
