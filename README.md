# Trục bị cắt – Biểu đồ

Website tĩnh dành cho GitHub Pages. Bài 4 của chuỗi Excel & Phân tích dữ liệu, khối 8.

## Đưa lên GitHub Pages
1. Tạo một repository mới trên GitHub.
2. Upload `index.html` và `bieu-do-hong.png` vào thư mục gốc của repository.
3. Vào **Settings → Pages**.
4. Chọn **Deploy from a branch**.
5. Chọn nhánh **main** và thư mục **/(root)**.
6. Lưu và chờ GitHub tạo đường dẫn website.

## Điều kiện sử dụng
Học sinh mở file **LSTS_KhaoSat_K8_2026_AnDanh_Cleaned.xlsx**, sheet `Clean_Data`, vùng hàng 3 → hàng 300.
Bài 4 **vẽ biểu đồ** từ chính những bảng số đã tính ở Bài 3, không có file dữ liệu mới.

## Nội dung
- Chặng 1: Chọn đúng loại biểu đồ (cột · tròn · cột phân phối · phân tán) — chưa cần mở Excel
- Chặng 2: Biểu đồ cột và cái bẫy trục — tự đổi Format Axis → Minimum
- Chặng 3: Biểu đồ tròn và giới hạn của nó
- Chặng 4: Cột phân phối và biểu đồ phân tán
- Chặng 5: Năm thành phần bắt buộc và ba thủ thuật đánh lừa — soi một biểu đồ hỏng
- Kiểm tra cuối: 10 câu ngẫu nhiên rút từ ngân hàng 20 câu, đạt 8/10 để tải minh chứng PNG/PDF

## Đáp án các chặng (dành cho giáo viên)

| Chặng | Nội dung | Kết quả |
|---|---|---|
| 2 | Giá trị cột cao nhất (nhóm Đi bộ) | 7.82 |
| 2 | Giá trị cột thấp nhất (nhóm Xe buýt trường) | 7.14 |
| 2 | Chênh lệch cao nhất − thấp nhất | **0.68** |
| 3 | Số nhóm trong cột Mạng xã hội | 6 |
| 3 | Tỉ lệ chọn TikTok | 33.6% |
| 3 | Tỉ lệ chọn Không dùng | 5.7% |
| 4 | Số bạn ngủ 7 đến dưới 8 giờ | 112 |
| 4 | Số bạn ngủ dưới 5 giờ | 6 |
| 4 | Số bạn ngủ từ 9 giờ trở lên | 10 |
| 5 | Số thành phần bắt buộc KHÔNG đạt | **5** |
| 5 | Số thủ thuật đánh lừa đã dùng | **3** |

Chốt của cả bài: năm nhóm chênh nhau đúng **0.68 điểm** trên thang 10 — tức **6.9% chiều cao trục**.
Cắt trục từ 7.0 biến 6.9% đó thành cả một biểu đồ, trong khi **không một con số nào thay đổi**.

Biểu đồ hỏng ở chặng 5 (`bieu-do-hong.png`) sai ở 8 chỗ: tiêu đề không nói gì · thiếu nhãn trục ngang ·
thiếu nhãn trục đứng và đơn vị · không có cỡ mẫu · không có nguồn · trục cắt từ 7.2 · bỏ mất 2 trong 5 nhóm ·
hiệu ứng 3D.

## Lưu ý kỹ thuật
- Phần nhiệm vụ **không in sẵn công thức hay thao tác**. Học sinh làm sai ô nào thì ô đó tô đỏ và chỉ ô đó hiện gợi ý; câu chọn sai cũng tô đỏ riêng.
- Website không cần backend. Họ tên và lớp lưu trong `localStorage` (khóa `excelChart4Student`).
- PDF tạo từ ảnh minh chứng bằng jsPDF tải từ CDN; nếu mạng chặn CDN, học sinh vẫn tải được bản PNG.
- Ô nhập kết quả chấp nhận cả dấu phẩy và dấu chấm thập phân; hai ô tỉ lệ phần trăm chấp nhận cả dạng `33.6` lẫn `0.336`.
- Các phương án trong ô chọn được xáo trộn ngẫu nhiên mỗi lần tải trang.
