# 🧠 Sleep Disorder Prediction using Generalized Linear Models (GLM)

**Đề tài NCKH sinh viên 2024 – Dự đoán rối loạn giấc ngủ bằng GLM**  
Tác giả: **Nhật Minh – Khoa Khoa học Ứng dụng, UNETI**

---

## 🌙 Giới thiệu
Dự án này tập trung xây dựng mô hình **GLM** để dự đoán nguy cơ rối loạn giấc ngủ dựa trên các yếu tố nhân khẩu học và lối sống (ví dụ: tuổi, giới tính, giờ ngủ, mức stress, thói quen caffeine). Mục tiêu: **đánh giá yếu tố ảnh hưởng** và **xây dựng mô hình giải thích được**.

---

## 🧩 Mục tiêu
- Phân tích tương quan giữa biến độc lập và rối loạn giấc ngủ.  
- Chọn biến quan trọng bằng Random Forest & Stepwise (AIC).  
- Xây dựng GLM (binomial) và đánh giá hiệu năng (AIC, Accuracy, F1).

---
## 📊 Dữ liệu
Dữ liệu được sử dụng trong dự án này được tải từ [Kaggle](https://www.kaggle.com/...), chỉ dùng cho mục đích học tập và nghiên cứu.  
Do giới hạn bản quyền, dữ liệu **không được đính kèm trực tiếp** trong repo này.  

---
## 📂 Cấu trúc repo
sleep_disorder_glm/  
├── data/ # (private) mô tả dataset  
├── notebooks/ # notebook minh họa  
├── src/ # mã nguồn Python: tiền xử lý, mô hình  
├── results/ # biểu đồ, ảnh minh họa kết quả  
├── report/ # (không up báo cáo đầy đủ)  
├── .gitignore  
└── README.md  


---

## ⚙️ Cách chạy
Các file mã nguồn nằm trong thư mục `src/`.  
Có thể chạy trực tiếp bằng Python hoặc mở trong Jupyter Notebook.  

---

## 🧰 Công nghệ sử dụng
- Python 3.x  
- statsmodels  
- pandas, numpy  
- matplotlib, seaborn  

---

## ✨ Tác giả
**Nhật Minh**  
Khoa Khoa học Ứng dụng – Trường Đại học Kinh tế - Kỹ thuật Công nghiệp (UNETI)

## 📊 Kết quả minh họa

Một số biểu đồ và hình ảnh minh họa trong quá trình phân tích:

| Phân tích độ tuổi | Nhóm tuổi | Giới tính |
|:-----------------:|:----------:|:----------:|
| ![Age](results/age.png) | ![AgeGroup](results/agegroup.png) | ![Gender](results/gender.png) |

| Nghề nghiệp | BMI | Rối loạn giấc ngủ - BMI |
|:------------:|:----:|:-----------------------:|
| ![Occupation](results/occupation.png) | ![BMI](results/BMI.png) | ![SDBMI](results/sdbmisd.png) |

| Tương quan biến | Phân bố dữ liệu | Kết quả mô hình |
|:----------------:|:----------------:|:----------------:|
| ![Heatmap](results/heatmap.png) | ![Plot](results/plot.png) | ![Sleep Disorder](results/sd.png) |

