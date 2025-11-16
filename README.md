ABC Bank – Customer Churn Prediction

Dự án phân tích & dự đoán khách hàng rời bỏ (Churn)

📌 Giới thiệu

Dự án nhằm phân tích các yếu tố khiến khách hàng rời bỏ ngân hàng ABC, đồng thời xây dựng mô hình dự đoán churn giúp ngân hàng nhận diện khách hàng có nguy cơ cao để đưa ra chiến lược giữ chân phù hợp.

🎯 Mục tiêu chính

Xác định các nhóm khách hàng có tỷ lệ rời bỏ cao.

Phân tích các yếu tố ảnh hưởng đến churn: nhân khẩu học, hành vi sử dụng sản phẩm, khu vực địa lý…

Xây dựng mô hình dự đoán churn sử dụng các thuật toán Machine Learning.

Đề xuất chiến lược giữ chân khách hàng dựa trên dữ liệu.

🧹 1. Khám phá & Tiền xử lý dữ liệu

Dữ liệu gồm 10.000+ khách hàng thuộc mảng retail banking.

Thực hiện làm sạch dữ liệu, xử lý giá trị thiếu, chuẩn hóa dữ liệu.

Một số insight quan trọng

Giới tính & Độ tuổi: nhóm nữ 50–60 tuổi có tỷ lệ churn cao nhất (~63%).

Danh mục sản phẩm: khách hàng dùng 3–4 sản phẩm có churn rate cao (82.7% – 100%).

Địa lý: khách hàng tại Đức có churn gần gấp đôi so với Pháp & Tây Ban Nha (~32% vs. ~16%).

Nhóm khách hàng có tenure ≤ 1 năm dễ rời bỏ hơn.

🤖 2. Xây dựng mô hình dự đoán

Đã thử nghiệm nhiều mô hình gồm:

Logistic Regression

Random Forest

Gradient Boosting

XGBoost

🎯 Mô hình tối ưu

Gradient Boosting

AUC = 0.86 → chính xác cao trong việc nhận diện khách hàng có rủi ro rời bỏ.

💡 3. Chiến lược giữ chân được đề xuất

Dựa trên kết quả phân tích & mô hình dự đoán:

📌 1. Cá nhân hóa dịch vụ

Tập trung nhóm nữ 50–60 tuổi: cung cấp gói tài chính – sức khỏe – bảo hiểm chuyên biệt.

Mở hotline ưu tiên, khảo sát định kỳ để nâng cao trải nghiệm.

📌 2. Cải thiện hệ sinh thái sản phẩm

Tối ưu onboarding cho nhóm sử dụng nhiều sản phẩm (3–4).

Tích hợp sản phẩm thành một ecosystem liền mạch để giảm frictions.

📌 3. Cải thiện trải nghiệm tại khu vực Đức

Đơn giản hóa quy trình đăng ký.

Miễn phí tháng đầu cho sản phẩm mới.

Follow-up sát trong 30 ngày đầu.

🛠️ 4. Công nghệ sử dụng

Ngôn ngữ: Python

Thư viện: Scikit-learn, XGBoost, Pandas, NumPy, Matplotlib

Kỹ thuật: Feature Engineering, Model Evaluation (AUC, Accuracy, Recall), Hyperparameter Tuning

📈 5. Kết quả

Nhận diện chính xác khách hàng có nguy cơ cao.

Đề xuất chiến lược giữ chân mang tính thực tiễn.

Tăng hiệu quả marketing & tối ưu chi phí chăm sóc khách hàng.
