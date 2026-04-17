Dưới đây là mã nguồn Markdown hoàn chỉnh cho file `README.md`. Bạn chỉ cần copy toàn bộ nội dung trong ô mã dưới đây và dán vào file của bạn là xong:


# 🏥 MedRisk: Hệ Thống Dự Đoán Khả Năng Tái Nhập Viện
### (Chuyên khoa: Bệnh Tiêu Hóa & Tuần Hoàn)
**Đồ án môn học:** Học Máy Ứng Dụng | **Ngành:** Trí Tuệ Nhân Tạo

---

## 🌟 Giới thiệu dự án
**MedRisk AI** là một hệ thống ứng dụng học máy nhằm dự đoán khả năng tái nhập viện của bệnh nhân mắc các bệnh về tiêu hóa và tuần hoàn. Hệ thống phân tích dữ liệu dựa trên hồ sơ y tế, thói quen sinh hoạt và lịch sử điều trị để đưa ra cảnh báo nguy cơ sớm.

Sự kết hợp giữa thuật toán học máy mạnh mẽ và giao diện **Chatbot thông minh** giúp bệnh nhân cũng như cơ sở y tế dễ dàng tương tác, giải thích kết quả dự đoán và nhận các lời khuyên y tế, chế độ dinh dưỡng cá nhân hóa.

### 🚀 Tính năng nổi bật
* **Dự đoán bằng Machine Learning:** Sử dụng thuật toán `Random Forest Classifier` (100 cây quyết định) để xử lý bài toán phân loại nhị phân nguy cơ tái nhập viện.
* **Trợ lý Y tế Ảo (Chatbot):** Tích hợp **Google Gemini API** (Gemini 1.5 Flash) giúp xử lý ngôn ngữ tự nhiên, giải thích kết quả dự đoán và tư vấn sức khỏe.
* **Tinh chỉnh xác suất thông minh:** Hệ thống thiết lập các luật nghiệp vụ y khoa để tối ưu độ chính xác (ví dụ: tăng 10% rủi ro cho bệnh nhân trên 60 tuổi, tăng 20% nếu tình trạng bệnh nền phức tạp).
* **Giao diện thân thiện:** Người dùng có thể nhập thông tin trực tiếp bằng ngôn ngữ tự nhiên hoặc tra cứu nhanh theo ID bệnh nhân.

---

## 🛠 Công nghệ sử dụng
Dự án được xây dựng tối ưu trên nền tảng Python:

| Thành phần | Công nghệ |
| :--- | :--- |
| **Ngôn ngữ** | Python 3.11.5 |
| **Backend Framework** | Flask |
| **Machine Learning** | Scikit-learn (RandomForest, LabelEncoder) |
| **Xử lý dữ liệu** | Pandas, Numpy |
| **AI API** | Google Generative AI (Gemini SDK) |
| **Frontend** | HTML5, CSS3, JavaScript |

---

## 📊 Cấu trúc dữ liệu (Dataset)
Dữ liệu được quản lý tập trung trong tệp `patient_data.csv` bao gồm:
* `ID`, `Tên bệnh nhân`, `Tuổi`.
* `Bệnh chính`, `Bệnh nền`.
* `Số lần nhập viện`.
* `Nghiêm trọng`: Đánh giá mức độ bệnh trạng (0 hoặc 1).

> **Tiền xử lý:** Các dữ liệu phân loại (Categorical) được chuyển đổi sang định dạng số nguyên thông qua `LabelEncoder` trước khi đưa vào huấn luyện mô hình.

---

## 📸 Hình ảnh dự án

### 📈 Hiệu suất mô hình
![Accuracy Score](https://github.com/user-attachments/assets/c8cb12a9-bfc4-481e-a22f-62d1782ca783)

### 💻 Giao diện người dùng
![User Interface](https://github.com/user-attachments/assets/50a89bff-44e5-43a4-9415-fd1f6590e36a)

---

## ⚙️ Hướng dẫn cài đặt và chạy

**1. Clone Repository:**
```bash
git clone [https://github.com/hanvu04012005/MedRisk_AI_Readmission_Predictor.git](https://github.com/hanvu04012005/MedRisk_AI_Readmission_Predictor.git)
cd MedRisk_AI_Readmission_Predictor
```

**2. Cài đặt môi trường:**
```bash
pip install flask pandas numpy scikit-learn google-generativeai
```

**3. Cấu hình API Key:**
Bạn cần có mã khóa API của Google Gemini để sử dụng tính năng Chatbot. Hãy thiết lập trong mã nguồn (khuyên dùng biến môi trường để bảo mật).

**4. Khởi động Server:**
```bash
python app.py
```
*Lưu ý: Mô hình Random Forest sẽ tự động được huấn luyện ngay khi server Flask khởi động.*

**5. Truy cập ứng dụng:**
Mở trình duyệt và truy cập: `http://127.0.0.1:5050`

---

## 📞 Thông tin liên hệ

Nếu bạn có bất kỳ thắc mắc nào về dự án hoặc muốn trao đổi về chuyên môn, vui lòng liên hệ:

* **Họ tên:** Nguyễn Hạn Vũ
* **Email:** [nguyenhanvu04012005@gmail.com](mailto:nguyenhanvu04012005@gmail.com)
* **GitHub:** [hanvu04012005](https://github.com/hanvu04012005)

---
*© 2026 - Dự án Học Máy Ứng Dụng*
```
