# Building Energy Load Forecasting & Anomaly Detection (Green AI)

> **Môn học:** Học máy căn bản (Machine Learning) — Trường Đại học Kinh tế TP.HCM (UEH)  
> **Bộ dữ liệu:** Building Data Genome 2 (BDG2 Dataset) — 12 Tòa nhà Thương mại/Giáo dục  
> **Tác giả / Nhóm làm việc:**  
> • **Tú (Trưởng nhóm)** — *Lead & Architecture Integration*  
> • **Nguyên** — *Co-Lead & Academic Writing*  
> • **Phương & Tiên** — *Data Engineering & Visualizations*  
> • **Huy & Đức** — *Machine Learning Experiments & Code Pipeline*  

---

## 1. Giới thiệu Đề tài (Project Overview)

Dự án nghiên cứu này tập trung vào bài toán quản lý năng lượng thông minh trong các tòa nhà sử dụng dữ liệu chuỗi thời gian BDG2, hướng tới phương châm **Green AI** (cân bằng giữa độ chính xác và chi phí tính toán). Nghiên cứu được đóng gói thành **02 Bài báo khoa học**:

1. **Paper 1 (Hội nghị / Báo cáo Giữa kỳ):** *Short-Term Electrical Load Forecasting Using Lightweight Regression Models: Feature Lag and Computational Efficiency Analysis.*  
   * **Mục tiêu:** Dự báo tải điện ngắn hạn theo giờ ($t+1$) dựa trên các mô hình Hồi quy nhẹ (Linear Regression, Decision Tree, Random Forest) và đánh giá sự đóng góp của nhóm đặc trưng độ trễ (Lag Features: $t-1, t-24, t-168$).
2. **Paper 2 (Tạp chí / Báo cáo Cuối kỳ):** *Explainable Building Energy Waste Detection: Comparing Isolation Forest, Supervised Classification, and Pseudo-Labeling under Synthetic Anomaly Injection.*  
   * **Mục tiêu:** Phát hiện lãng phí năng lượng trong điều kiện thiếu nhãn bằng kỹ thuật **Chèn bất thường nhân tạo (Synthetic Anomaly Injection)** làm đối chứng (Ground Truth) và quy trình **Nhãn giả (Pseudo-Labeling)** kết hợp giữa Isolation Forest và Random Forest Classifier.

---

## 2. Phân công Nhân sự & Sub-teams

| Sub-team | Thành viên | Trách nhiệm chính |
| :--- | :--- | :--- |
| **Sub-team 1: Data & Visuals** | **Phương & Tiên** | • Lọc 12 tòa nhà BDG2 đạt chuẩn (<5% khuyết).<br>• Làm sạch dữ liệu khuyết & trích xuất đặc trưng (Lag/Weather).<br>• Thực hiện EDA, vẽ đồ thị Ablation Study, PR-AUC, ROC-AUC. |
| **Sub-team 2: ML Pipeline** | **Huy & Đức** | • Viết code huấn luyện mô hình Hồi quy & Phân loại.<br>• Viết script chèn bất thường nhân tạo (Synthetic Spikes/Night anomalies).<br>• Đo đạc chi phí tính toán (Inference time, Model size MB). |
| **Sub-team 3: Writing & Lead** | **Tú (Lead) & Nguyên** | • Quản trị chung, khởi tạo Drive/GitHub, lập tiến độ.<br>• Soạn thảo Proposal & Bài báo theo mẫu chuẩn (`PaperID 581`).<br>• Kiểm tra tính liêm chính khoa học & chuẩn hóa trích dẫn APA. |

---
