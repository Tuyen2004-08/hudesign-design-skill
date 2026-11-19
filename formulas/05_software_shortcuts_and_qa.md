# 05. Checklist QA 10 Điểm & Bộ Prompt Chuẩn Cho Codex

## A. Checklist QA 10 Điểm Bắt Buộc Trước Khi Xuất Thiết Kế
- [ ] **1. Trọng tâm rõ trong 2 giây đầu:** Có 1 điểm nhấn thị giác lớn nhất (sản phẩm hoặc con số/tiêu đề chính).
- [ ] **2. Bố cục có chủ đích:** Khóa rõ 1 khung bố cục chuẩn (7 bố cục / Chữ X / Hội tụ / Tỷ lệ vàng).
- [ ] **3. Gom nhóm Proximity:** Thông tin cùng ngữ nghĩa nằm sát nhau, có khoảng thở tách biệt giữa các nhóm.
- [ ] **4. Căn lưới nhất quán:** Bám trục theo 1 trong 6 hệ thống lưới (Radial, Modular, Axial, Column, Hierarchical, Baseline).
- [ ] **5. Phân cấp chữ (Không phẳng):** Tách rõ tối thiểu 3–4 tầng kích thước & độ đậm.
- [ ] **6. Tương phản chữ trên nền ảnh:** Chữ sáng đặt trên ảnh có lớp phủ tối/mờ đảm bảo đọc rõ.
- [ ] **7. Gradient sạch vùng xám:** Góc `<= 90°` hoặc đã chèn điểm màu trung gian nếu dùng cặp `180°`.
- [ ] **8. Tách tương phản 4 lớp UI:** Nền tổng → Thẻ Card → Khối phụ → Điểm nhấn CTA.
- [ ] **9. Chọn đúng 1 trong 5 nhóm Font** phù hợp lĩnh vực thương hiệu.
- [ ] **10. Chi tiết hoàn thiện (Polish):** Chỉ áp dụng có chọn lọc 1–2 kỹ thuật nâng cấp (Watermark Numbering, Card Overflow, Mask chiều sâu, Speed lines, Mảng màu làm mờ).

## B. Prompt Mẫu Giao Việc Cho Codex
```text
Đọc AGENTS.md và schemas/hudesign_formulas.json.
Thiết kế [Landing Page / Poster / Card UI / Menu / Infographic] cho [tên dự án]:
- Áp dụng đúng bố cục, hệ thống lưới, luật Gradient <= 90°, tương phản 4 lớp và phân cấp chữ theo Hủ Design.
- Tự kiểm tra đủ 10 điểm QA trong formulas/05_software_shortcuts_and_qa.md trước khi xuất kết quả.
```
