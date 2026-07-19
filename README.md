# 🎮 Phân tích dữ liệu: Online Gaming & Anxiety
# 📌 Giới thiệu
Đây là đồ án môn học Phân tích dữ liệu, thực hiện toàn bộ bằng Google Colab.
Dataset được lấy từ Kaggle: [Online Gaming Anxiety Data](https://www.kaggle.com/datasets/divyansh22/online-gaming-anxiety-data/code)

## Mục tiêu của dự án là:
- Khám phá mối quan hệ giữa thói quen chơi game và mức độ lo âu xã hội.
- Thực hành quy trình phân tích dữ liệu từ tiền xử lý đến mô hình hóa.
- Minh họa cách sử dụng Python và thư viện phân tích dữ liệu trong môi trường Colab.

## ⚙️ Công cụ sử dụng
Google Colab: môi trường chạy code.
Python: ngôn ngữ chính.
Thư viện: pandas, numpy, matplotlib, seaborn, scikit-learn.

## 📂 Cấu trúc dự án
Preprocessing.ipynb: notebook chứa toàn bộ bước tiền xử lý dữ liệu.


## 🔄 Quy trình thực hiện
1. Thu thập dữ liệu
Dataset tải từ Kaggle và lưu trên Google Drive.
Kết nối Colab với Drive để đọc dữ liệu.

3. Khám phá dữ liệu (EDA)
Xem kích thước, kiểu dữ liệu, giá trị thiếu.
Thống kê mô tả, phân phối dữ liệu.
Trực quan hóa bằng biểu đồ.

5. Tiền xử lý dữ liệu (chi tiết trong Preprocessing.ipynb)
Loại bỏ các cột không liên quan trong phân tích
Xử lý missing values: Các cột SPIN1–SPIN17: điền bằng mode hoặc median.
Các cột số khác (Hours, streams, Narcissism, SPIN_T): điền bằng mean.
Các cột phân loại (Residence, Reference, Residence_ISO3): thay thế giá trị thiếu và không hợp lệ thành Other.
Chuẩn hóa dữ liệu: scale các biến số khi cần.
Mã hóa dữ liệu phân loại: dùng OrdinalEncoder hoặc OneHotEncoder.

7. Phân tích & mô hình hóa
Trực quan hóa mối quan hệ giữa thời gian chơi game, xem stream và điểm SPIN.
Xây dựng mô hình dự đoán mức tâm lý từ các biến hành vi.
So sánh các mô hình: Linear Regression, Random Forest, XGBoost.

9. Đánh giá kết quả

## 📊 Kết quả
Dataset được làm sạch và chuẩn hóa.
Các mô hình thử nghiệm cho thấy XGBoost có hiệu quả cao nhất trong dự đoán SPIN_T.
Kết quả minh họa rằng thói quen chơi game có liên hệ với mức độ lo âu xã hội.

## 🚀 Cách chạy dự án
Clone repo về máy hoặc mở trực tiếp trên Colab.
Tải dataset từ Kaggle và lưu vào Google Drive.
Mở notebook Preprocessing.ipynb để chạy bước tiền xử lý.
