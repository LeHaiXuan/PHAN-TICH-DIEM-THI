![Banner](assets/banner.png)

# Ứng dụng Phân tích Điểm Thi THPT

**Trường: THPT Lê Quý Đôn - Long Bình Tân**  
**Tác giả triển khai: LeHaiXuan**

## 📌 Giới thiệu
Ứng dụng Streamlit giúp phân tích kết quả thi của học sinh theo:
- Kỳ thi
- Môn học
- Lớp
- Tổ chuyên môn

Hỗ trợ:
- So sánh giữa các kỳ thi
- Thống kê theo tổ chuyên môn
- Xuất báo cáo PDF nhiều trang (bảng + biểu đồ)

---

## ✅ Tính năng chính
- Tổng quan: Điểm trung bình, trung vị, độ lệch chuẩn
- Phân phối điểm theo môn: Boxplot
- Thống kê theo tổ chuyên môn: Bảng count/mean/median/std
- So sánh hai kỳ thi: Bảng pivot + biểu đồ cột
- Xuất báo cáo PDF: Tùy chỉnh tiêu đề, tải về trực tiếp

---

## 🗂 Cấu trúc dữ liệu
File dữ liệu cần các cột:
```
StudentID, HoTen, Lop, Mon, ToChuyenMon, KyThi, Diem
```
> Xem file mẫu: `data/samples/sample_scores.csv`

---

## 🚀 Cách chạy trên máy tính

### Bước 1: Cài Python
Tải Python 3.10+ từ https://www.python.org/downloads/

### Bước 2: Giải nén mã nguồn
Giải nén thư mục `ung-dung-phan-tich-diem-thi-THPT`

### Bước 3: Tạo môi trường ảo (khuyến nghị)
```bash
python -m venv .venv
# macOS/Linux
source .venv/bin/activate
# Windows (PowerShell)
.venv\Scripts\Activate.ps1
```

### Bước 4: Cài thư viện
```bash
pip install -r requirements.txt
```

### Bước 5: Chạy ứng dụng
```bash
streamlit run app.py
```
Truy cập tại: `http://localhost:8501`

---

## 🌐 Triển khai trực tuyến

### Render.com (miễn phí cơ bản)
- Build: `pip install -r requirements.txt`
- Start: `streamlit run app.py --server.port $PORT --server.headless true`

### Hugging Face Spaces
- Chọn template **Streamlit**, kéo thả mã nguồn

### GitHub Codespaces
- Mở repo → Code → Create codespace → chạy ứng dụng trực tiếp

---

## 🔍 Tùy chỉnh thêm
- Tỷ lệ đạt ≥5, ≥8; phân loại học lực
- Xếp hạng lớp theo điểm TB
- Thống kê theo giáo viên bộ môn (nếu có dữ liệu)

---

## 📜 Giấy phép
MIT License – Tự do sử dụng, chỉnh sửa, triển khai.
