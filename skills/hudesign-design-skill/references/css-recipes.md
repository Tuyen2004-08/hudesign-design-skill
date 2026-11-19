# CSS & HTML Recipes — Công Thức Code Sẵn Chạy Cho Codex

Mỗi đoạn mã dưới đây ánh xạ trực tiếp từ một công thức Before/After của **Hủ Design (`@hudesign`)**.

## 1. Luật Gradient Sạch Vùng Xám (`COL-01`)
```css
/* SAI: 2 màu đối diện 180° tạo vùng xám xỉn ở giữa */
.gradient-bad-180 {
  background: linear-gradient(135deg, #8b5cf6 0%, #22c55e 100%);
}

/* CHUẨN 1: Chèn 1 điểm màu trung gian trên cung nối (Tím -> Xanh dương -> Xanh lá) */
.gradient-fixed-180 {
  background: linear-gradient(135deg, #8b5cf6 0%, #0ea5e9 50%, #22c55e 100%);
}

/* CHUẨN 2: Chọn 2 màu nằm trong góc <= 90° trên vòng màu */
.gradient-clean-90 {
  background: linear-gradient(135deg, #06b6d4 0%, #1d4ed8 100%);
}

/* CHUẨN 3: Nền tối + ánh sáng nhẹ cho sản phẩm tối giản/công nghệ */
.product-dark-stage {
  background: radial-gradient(circle at 50% 25%, rgba(56, 189, 248, 0.22), #0f172a 65%);
}
```

## 2. Tách Tương Phản 4 Lớp UI (`COL-02`)
```css
:root {
  --layer-1-canvas: #e2e8f0;  /* Nền tổng */
  --layer-2-card:   #ffffff;  /* Thẻ Card */
  --layer-3-sub:    #dbeafe;  /* Khối phụ / biểu đồ nhạt */
  --layer-4-accent: #1d4ed8;  /* Điểm nhấn chính + chữ trắng */
}
```

## 3. Card Overflow Tràn Viền Tạo Chiều Sâu 3D (`UI-01` / `POL-01`)
```css
.hudesign-overflow-card {
  position: relative;
  overflow: visible; /* Bắt buộc để sản phẩm tràn khỏi khung */
  border-radius: 20px;
  padding: 24px;
  background: linear-gradient(135deg, #dcfce7 0%, #bbf7d0 100%);
}
.hudesign-overflow-card .product-img {
  position: absolute;
  top: -28px;
  right: -18px;
  transform: rotate(-8deg);
  filter: drop-shadow(0 18px 24px rgba(15, 23, 42, 0.22));
}
```

## 4. Watermark Numbering — Số Thứ Tự Phóng To Làm Nền (`POL-01 #01`)
```css
.numbered-heading {
  position: relative;
  padding-top: 22px;
}
.numbered-heading::before {
  content: attr(data-num); /* "01", "02", "03" */
  position: absolute;
  top: -8px;
  left: -6px;
  font-size: 4.5rem;
  font-weight: 900;
  color: rgba(148, 163, 184, 0.22);
  z-index: 0;
  pointer-events: none;
}
.numbered-heading > span {
  position: relative;
  z-index: 1;
}
```

## 5. Ticket Stack UI — Vé Có Vết Khuyết 2 Bên & Đường Cắt Đứt (`UI-01 #04`)
```css
.ticket-card {
  position: relative;
  background: #ffffff;
  border-radius: 16px;
  border: 1px solid #cbd5e1;
  padding: 20px;
}
.ticket-divider {
  position: relative;
  border-top: 2px dashed #cbd5e1;
  margin: 16px -20px;
}
.ticket-divider::before,
.ticket-divider::after {
  content: "";
  position: absolute;
  top: -11px;
  width: 20px;
  height: 20px;
  border-radius: 50%;
  background: #0f172a; /* Trùng màu nền ngoài */
}
.ticket-divider::before { left: -10px; }
.ticket-divider::after  { right: -10px; }
```

## 6. Scrim Bảo Vệ Chữ Sáng Trên Ảnh Sáng (`POL-01` / `08 Mẹo P2`)
```css
.hero-photo-card {
  position: relative;
  overflow: hidden;
}
.hero-photo-card::after {
  content: "";
  position: absolute;
  inset: 0;
  background: linear-gradient(180deg, rgba(15, 23, 42, 0.1) 35%, rgba(15, 23, 42, 0.82) 100%);
}
.hero-photo-card .caption {
  position: relative;
  z-index: 1;
  color: #f8fafc;
}
```
