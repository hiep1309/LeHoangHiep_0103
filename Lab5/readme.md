\#2.1

-Công nghệ sử dụng

PIL: đọc ảnh

NumPy: xử lý ảnh dưới dạng mảng

Scikit-image: phân ngưỡng Otsu, gán nhãn, trích xuất thuộc tính

ImageIO: lưu ảnh

Matplotlib: hiển thị và vẽ bounding box



-Thuật toán

Đọc ảnh xám

Phân ngưỡng Otsu để nhị phân hóa ảnh

Gán nhãn các vùng liên thông

Vẽ khung bao quanh mỗi vùng



-Cách thức hoạt động

Ảnh được chuyển sang mảng và phân ngưỡng

Mỗi vùng được đánh nhãn

Duyệt từng vùng để vẽ khung chữ nhật quanh đối tượng

Hiển thị kết quả bằng imshow và Rectangle


\#2.2

-Công nghệ sử dụng

PIL: đọc ảnh

NumPy: xử lý mảng ảnh

SciPy: dịch ảnh (shift)

Matplotlib: hiển thị ảnh



-Thuật toán

Đọc ảnh xám

Dịch ảnh 1 pixel theo trục ngang

Tính sai khác tuyệt đối giữa ảnh gốc và ảnh dịch



-Cách thức hoạt động

Dùng nd.shift để dịch ảnh sang phải

Tính hiệu tuyệt đối giữa hai ảnh để phát hiện biên

Hiển thị ảnh kết quả bằng imshow



\#2.3

-Công nghệ sử dụng

PIL: đọc ảnh

SciPy: tính đạo hàm Sobel

NumPy: tính trị tuyệt đối và cộng ảnh

Matplotlib: hiển thị ảnh



-Thuật toán

Đọc ảnh

Tính đạo hàm Sobel theo trục x và y

Cộng trị tuyệt đối để làm nổi bật biên



-Cách thức hoạt động

Dùng sobel để phát hiện cạnh theo 2 chiều

Cộng kết quả để có ảnh biên tổng hợp

Hiển thị ảnh biên bằng imshow



\#2.4

\*\*-Công nghệ sử dụng\*\*

PIL: đọc ảnh

SciPy: Sobel và Gaussian filter

NumPy: tính toán ma trận

Matplotlib: hiển thị ảnh



\*\*-Thuật toán\*\*

Tính đạo hàm ảnh theo Sobel

Tạo ma trận cấu trúc (structure matrix)

Tính đáp ứng Harris để phát hiện góc



\*\*-Cách thức hoạt động\*\*

Dùng đạo hàm Sobel để lấy gradient

Tính các tích chéo và làm mịn bằng Gaussian

Tính R (Harris response) và hiển thị ảnh kết quả



\#2.5.1

-Công nghệ sử dụng

NumPy: tạo và xử lý mảng ảnh

SciPy: xử lý số liệu

Matplotlib: hiển thị kết quả



-Thuật toán

Tạo ảnh nhị phân với 1 điểm trắng

Dò theo nhiều góc để tính toán tham số đường thẳng (Hough Transform)

Tính tích lũy vào không gian Hough



-Cách thức hoạt động

Ảnh đầu vào có 1 điểm sáng

Tính các giá trị ρ (rho) theo từng góc θ

Cộng giá trị vào ma trận Hough tại (ρ, θ)

Hiển thị không gian Hough kết quả bằng imshow



\#2.5.2

-Công nghệ sử dụng

ImageIO: đọc ảnh

scikit-image: chuyển ảnh xám, phát hiện góc Harris

Matplotlib: hiển thị ảnh



-Thuật toán

Đọc ảnh màu

Chuyển sang ảnh xám

Tính đáp ứng góc bằng Harris



-Cách thức hoạt động

Dùng rgb2gray để chuyển ảnh sang xám

Áp dụng corner\_harris để phát hiện các điểm góc

Hiển thị ảnh góc bằng imshow không có trục (axis('off'))



