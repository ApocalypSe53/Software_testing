# Báo cáo Thực hành Tuần 1

**Môn học:** Kiểm thử phần mềm  
**Họ và tên:** Vũ Đình Anh Vũ  
**Mã sinh viên:** BCS230094  
**Lớp:** 23CS1  

---

## 1. Mục tiêu bài thực hành
- Khởi tạo `Repository` trên `GitHub` để quản lý và báo cáo kết quả học tập.
- Làm quen với `Markdown` để viết tài liệu.
- Trải nghiệm và đánh giá độ nhạy bén về UI/UX thông qua trò chơi [Can't Unsee](https://cantunsee.space/).

## 2. Kết quả trải nghiệm "Can't Unsee"

Dưới đây là kết quả điểm số cao nhất tôi đã đạt được sau khi thực hiện bài test:

<img width="3840" height="2160" alt="Screenshot (11)" src="https://github.com/user-attachments/assets/a0b23479-f60e-45c0-b04f-48889f023913" />

**Ghi chú:** - Ảnh chụp màn hình bao gồm giao diện trình duyệt có đăng nhập tài khoản cá nhân (góc trên bên phải) để xác thực chính chủ.
- Điểm số đạt được: 7680
- Mức độ đánh giá: Top 5% - PLATINUM

---

## 3. Kết luận
Qua bài thực hành này, tôi đã:
- [x] Tạo thành công Repo và file README.md.
- [x] Hiểu được sự khác biệt chi tiết trong thiết kế giao diện.
- [x] Hoàn thành việc upload ảnh minh chứng lên GitHub.


# Student Grade Analysis

Bài tập thực hành kiểm thử đơn vị với JUnit.
Chương trình phân tích danh sách điểm số học sinh để tìm ra số lượng học sinh giỏi và tính điểm trung bình hợp lệ.

## Chức năng

1.  **Đếm học sinh giỏi (`countExcellentStudents`):**
    * Input: Danh sách điểm `List<Double>`.
    * Logic: Đếm các điểm `>= 8.0`. Bỏ qua điểm `< 0` hoặc `> 10`.
2.  **Tính điểm trung bình (`calculateValidAverage`):**
    * Logic: Tính trung bình cộng các điểm trong khoảng `[0, 10]`.

## Yêu cầu hệ thống

* Java JDK 8 trở lên
* JUnit 5 (Jupiter)
* IDE: IntelliJ IDEA / Eclipse / VS Code

## Cách chạy kiểm thử

Sử dụng IDE để chạy file `StudentAnalyzerTest.java` hoặc dùng lệnh Maven/Gradle nếu có cấu hình build tool.

### Kết quả Test Case mong đợi:

| Tên Test Case | Input | Kỳ vọng | Kết quả |
| :--- | :--- | :--- | :--- |
| `testCountExcellentStudents_StandardCase` | `[9.0, 8.5, 7.0, 11.0, -1.0]` | `2` | Passed |
| `testCalculateValidAverage_StandardCase` | `[9.0, 8.5, 7.0, 11.0, -1.0]` | `8.17` | Passed |
| `testEmptyList` | `[]` | `0` | Passed |
