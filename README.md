# 💰 ỨNG DỤNG QUẢN LÝ CHI TIÊU THÔNG MINH CHO SINH VIÊN DNU  
**Smart Expense Management App for DNU Students**

---

## 🧭 Giới thiệu chung

Trong thời đại công nghệ số hiện nay, việc **quản lý chi tiêu cá nhân** đóng vai trò cực kỳ quan trọng đối với sinh viên.  
Đặc biệt, với sinh viên Đại học Duy Tân (DNU), nhiều bạn phải sống tự lập, quản lý tài chính sinh hoạt, học tập và giải trí.  
Ứng dụng **“Quản lý Chi tiêu Thông minh cho Sinh viên DNU”** được phát triển nhằm hỗ trợ sinh viên:

- Theo dõi thu nhập và chi tiêu hàng tháng.  
- Lập kế hoạch chi tiêu hợp lý.  
- Trực quan hóa dữ liệu bằng **biểu đồ tròn sinh động**.  
- Đưa ra **cảnh báo vượt chi tiêu** giúp người dùng điều chỉnh tài chính.  

Đây là sản phẩm ứng dụng thực tế của sinh viên **Khoa Công nghệ Thông tin – Đại học Duy Tân**, được thực hiện trong học kỳ 2025.

---

## 🎯 Mục tiêu của dự án

- Xây dựng **một ứng dụng di động thân thiện, trực quan và dễ sử dụng**.  
- Hỗ trợ sinh viên quản lý tài chính cá nhân một cách **khoa học và hiệu quả**.  
- Ứng dụng kiến thức về **Flutter, SQLite, bảo mật thông tin và trực quan hóa dữ liệu** vào sản phẩm thực tế.  
- Nâng cao khả năng tư duy lập trình, phân tích hệ thống và thiết kế giao diện người dùng.

---

## 🧩 Tính năng nổi bật

| Nhóm tính năng | Mô tả chi tiết |
|-----------------|----------------|
| **1. Đăng ký / Đăng nhập** | Cho phép sinh viên tạo tài khoản và đăng nhập để quản lý dữ liệu riêng. |
| **2. Thêm thu nhập** | Lưu lại các khoản tiền sinh viên nhận được (trợ cấp, làm thêm, học bổng, v.v). |
| **3. Thêm chi tiêu** | Ghi lại chi tiết các khoản chi trong ngày theo danh mục. |
| **4. Báo cáo chi tiêu hàng tháng** | Tổng hợp và hiển thị bằng **biểu đồ tròn (Pie Chart)** qua thư viện *FlChart*. |
| **5. Cảnh báo vượt chi tiêu** | Khi chi tiêu vượt mức dự kiến, hệ thống gửi cảnh báo bằng popup hoặc notification. |
| **6. Lưu trữ dữ liệu SQLite** | Mọi dữ liệu được lưu cục bộ giúp ứng dụng hoạt động không cần Internet. |
| **7. Giao diện tối ưu cho sinh viên** | Dễ thao tác, màu sắc nhẹ nhàng, phù hợp với lứa tuổi sinh viên. |

---

## 🏗️ Kiến trúc hệ thống

Ứng dụng được xây dựng theo mô hình **MVVM (Model - View - ViewModel)** giúp tách biệt phần logic, dữ liệu và giao diện.

### 🧱 Các thành phần chính:
- **Model:** Các lớp `User`, `Expense`, `Income`, `Report`.  
- **View:** Giao diện người dùng được xây dựng bằng Flutter (Material Design).  
- **Controller (ViewModel):** Xử lý logic, kết nối dữ liệu với giao diện.  
- **Database:** SQLite để lưu dữ liệu người dùng.  
- **Storage:** SharedPreferences dùng để lưu trạng thái đăng nhập.

---

## ⚙️ Công nghệ sử dụng

| Công nghệ | Mục đích sử dụng |
|------------|------------------|
| **Flutter (Dart)** | Framework chính để phát triển ứng dụng di động đa nền tảng. |
| **SQLite** | Cơ sở dữ liệu cục bộ, nhẹ và hiệu quả. |
| **FlChart** | Vẽ biểu đồ trực quan hóa dữ liệu chi tiêu. |
| **Shared Preferences** | Lưu trạng thái người dùng (đăng nhập, cài đặt). |
| **SHA-256 Hashing** | Mã hóa mật khẩu người dùng khi đăng ký / đăng nhập. |
| **Overleaf (LaTeX)** | Soạn thảo báo cáo học thuật chuẩn IEEE. |

---

## 📂 Cấu trúc thư mục dự án

├── assets/
│ ├── images/ # Hình ảnh minh họa
│ └── icons/ # Biểu tượng giao diện
├── lib/
│ ├── main.dart # Điểm khởi đầu ứng dụng
│ ├── models/ # Các lớp dữ liệu (User, Expense, Income, Report)
│ ├── screens/ # Màn hình: Login, Dashboard, Report, Add Expense,...
│ ├── widgets/ # Thành phần giao diện tái sử dụng
│ └── database/ # Các tệp điều khiển cơ sở dữ liệu SQLite
├── report/
│ └── report.tex # Báo cáo chính trên Overleaf (IEEE format)
├── pubspec.yaml # File cấu hình thư viện Flutter
└── README.md # File mô tả dự án (file hiện tại)

---

## 🧠 Phương pháp thực hiện

1. **Phân tích yêu cầu**: Khảo sát sinh viên DNU về thói quen chi tiêu, từ đó xác định các tính năng cần thiết.  
2. **Thiết kế giao diện**: Dùng Figma để tạo layout hiện đại, dễ thao tác trên điện thoại.  
3. **Xây dựng chức năng**:  
   - Đăng ký/Đăng nhập (có mã hóa mật khẩu).  
   - Ghi thu – chi – báo cáo.  
   - Biểu đồ tròn bằng FlChart.  
4. **Kiểm thử**: Viết test case cho từng module (Add Expense, View Report...).  
5. **Đóng gói & Triển khai**: Build bản APK chạy thử nghiệm trên Android.  

---

## 📊 Kết quả đạt được

- Ứng dụng hoạt động ổn định trên nền tảng Android.  
- Giao diện thân thiện, dễ thao tác.  
- Báo cáo chi tiêu hiển thị chính xác với biểu đồ tròn sinh động.  
- Cảnh báo chi tiêu hoạt động hiệu quả giúp sinh viên cân đối tài chính.  

---

## 🚀 Hướng phát triển trong tương lai

- Tích hợp **AI** để phân tích và gợi ý chi tiêu thông minh.  
- Kết nối **Firebase** để đồng bộ dữ liệu giữa các thiết bị.  
- Bổ sung tính năng **nhắc nhở nạp tiền hoặc hạn mức chi tiêu**.  
- Phát triển thêm **phiên bản web và desktop**.  
- Nâng cấp giao diện sang **Material 3** để tăng tính hiện đại.

---

## 👨‍💻 Thành viên nhóm thực hiện

| Họ và tên | Vai trò | Công việc chính |
|------------|----------|----------------|
| **Phạm Đình Tuấn** | Trưởng nhóm | Phân tích yêu cầu, lập trình chính, hoàn thiện báo cáo Overleaf |
| **Nguyễn Văn A** | Thiết kế UI/UX | Thiết kế Figma, chỉnh sửa giao diện Flutter |
| **Trần Thị B** | Kiểm thử | Viết test case, thử nghiệm tính năng |
| **Lê Văn C** | Hỗ trợ kỹ thuật | Cấu hình môi trường, tối ưu hiệu suất ứng dụng |

---
👨‍💻 Tác giả

Phạm Đình Tuấn
Khoa Công nghệ Thông tin – Đại học Đại Nam (DNU)
📧 phamdinhtuan@dnu.edu.vn
## 📦 Cách cài đặt và chạy ứng dụng

```bash
# B1: Clone dự án từ GitHub
git clone https://github.com/<ten_tai_khoan>/<ten_du_an>.git

# B2: Di chuyển vào thư mục dự án
cd <ten_du_an>

# B3: Cài đặt các gói thư viện
flutter pub get

# B4: Chạy ứng dụng
flutter run
