# ABC Bank – Customer Churn Prediction

## Giới thiệu
Dự án nhằm phân tích hành vi rời bỏ (churn) của khách hàng tại ngân hàng ABC. Thông qua việc khai thác dữ liệu nhân khẩu học, hành vi sử dụng sản phẩm và yếu tố địa lý, dự án xây dựng mô hình dự đoán churn giúp ngân hàng xác định sớm khách hàng có nguy cơ cao và đưa ra các chiến lược giữ chân phù hợp.

## Mục tiêu dự án
- Hiểu các yếu tố dẫn đến churn.
- Phát hiện nhóm khách hàng có churn rate cao.
- Xây dựng mô hình Machine Learning dự đoán churn.
- Đề xuất các giải pháp giữ chân dựa trên dữ liệu.

## Quy trình thực hiện

### 1. Thu thập và tiền xử lý dữ liệu
- Dữ liệu gồm hơn 10.000 khách hàng.
- Thực hiện:
  - Xử lý giá trị thiếu.
  - Chuẩn hóa dữ liệu.
  - Mã hóa biến phân loại.
  - Feature engineering.

### 2. Khám phá dữ liệu (EDA)
Một số insights nổi bật:
- Nhóm nữ 50–60 tuổi có churn rate cao nhất (~63%).
- Khách hàng dùng 3–4 sản phẩm có churn rate rất cao (82.7% – 100%).
- Khách hàng tại Đức có churn rate gần gấp đôi Pháp và Tây Ban Nha (~32% vs ~16%).
- Khách hàng có tenure ≤ 1 năm dễ rời bỏ hơn.

### 3. Xây dựng mô hình dự đoán
Các mô hình thử nghiệm:
- Logistic Regression
- Random Forest
- Gradient Boosting
- XGBoost

**Mô hình tối ưu:** Gradient Boosting (AUC = 0.86)

### 4. Chiến lược giữ chân khách hàng

**Nhóm nữ 50–60 tuổi**
- Xây dựng gói dịch vụ tài chính – bảo hiểm – sức khỏe.
- Hỗ trợ ưu tiên và khảo sát trải nghiệm định kỳ.

**Khách hàng dùng 3–4 sản phẩm**
- Tích hợp sản phẩm thành hệ sinh thái liền mạch.
- Tư vấn tăng gắn kết.

**Khách hàng tại Đức**
- Đơn giản hóa quy trình đăng ký.
- Ưu đãi tháng đầu, follow-up 30 ngày đầu.

## Công nghệ sử dụng
- Python
- Pandas, NumPy
- Scikit-learn, XGBoost
- Matplotlib

## Kết quả
- Mô hình Gradient Boosting đạt AUC 0.86.
- Xác định chính xác nhóm khách hàng rủi ro cao.
- Đề xuất chiến lược giữ chân theo từng phân khúc.
- Tối ưu hiệu quả marketing và chăm sóc khách hàng.

## Cấu trúc thư mục gợi ý
```
├── data/
│   ├── raw_data.csv
│   ├── cleaned_data.csv
├── notebooks/
│   ├── 01_EDA.ipynb
│   ├── 02_Modeling.ipynb
├── src/
│   ├── preprocess.py
│   ├── train_model.py
│   ├── evaluate.py
├── models/
│   ├── best_model.pkl
├── README.md
├── requirements.txt
```

## Hướng dẫn chạy dự án

### 1. Cài đặt thư viện
```
pip install -r requirements.txt
```

### 2. Chạy notebook phân tích
- `notebooks/01_EDA.ipynb`
- `notebooks/02_Modeling.ipynb`

### 3. Huấn luyện mô hình
```
python src/train_model.py
```

### 4. Đánh giá mô hình
```
python src/evaluate.py
```

## Định hướng phát triển
- Tối ưu mô hình bằng Optuna hoặc Bayesian Optimization.
- Deploy API bằng FastAPI/Flask.
- Xây dựng dashboard realtime theo dõi churn risk.
