# Checkpoint Lab — ôn Cambridge Primary Checkpoint (Stage 6)

App web ôn thi Checkpoint cho học sinh lớp 5 hệ Cambridge, dùng trực tiếp trên điện thoại.
Toàn bộ nằm trong **một file `index.html` duy nhất**, chạy offline sau lần mở đầu tiên,
không cần cài đặt, không cần tài khoản.

## Nội dung

| Môn | Số unit | Ý chính | Câu quiz |
|---|---|---|---|
| Science | 9 | 71 | 71 |
| Mathematics | 12 | 85 | 85 |
| English (ESL) | 11 | 77 | 77 |
| **Tổng** | **32** | **233** | **233** |

Thêm 3 đề thi thử (36 câu) và 280 mục từ vựng Anh–Việt.
Mỗi unit có **số câu quiz đúng bằng số ý chính**, mỗi câu đều có lời giải thích tiếng Việt.

## Tính năng

- **Phiên ôn 15 phút/ngày**: thẻ lật → mindmap và ý chính → quiz, có đồng hồ đếm ngược.
- **Mindmap và sơ đồ** vẽ bằng SVG nội tuyến (16 sơ đồ minh hoạ: hệ tuần hoàn, chuỗi thức ăn,
  mạch điện, trạng thái vật chất, hệ toạ độ, trục thời gian thì tiếng Anh…).
- **Song ngữ có nút ẩn**: mặc định chỉ hiện tiếng Anh, chạm mới hiện tiếng Việt. Đổi được trong Cài đặt.
- **Nghe phát âm**: chạm nút loa để đọc từ và câu tiếng Anh (giọng en-GB của thiết bị).
- **Ôn lại câu sai tự động**: câu làm sai quay lại sau 1, 2, 4, 7 và 14 ngày.
- **Đề thi thử**: làm liên tục có đồng hồ, không hiện đáp án cho tới khi nộp bài.
- **Báo cáo cho bố mẹ**: số phút học 7 ngày gần nhất, điểm theo môn, unit cần kèm thêm.
- Giao diện tự đổi theo nền sáng/tối của điện thoại.

## Chạy

Mở `index.html` bằng trình duyệt bất kỳ. Trên iPhone: mở link → nút Chia sẻ →
**Thêm vào MH chính** để dùng như một app thật.

Tiến độ được lưu bằng `localStorage` ngay trên thiết bị.

## Cập nhật nội dung

Toàn bộ bài học nằm trong các khối `<script>` ở đầu file:

- `DATA` — ý chính, từ vựng và quiz của 32 unit
- `EXTRA` — câu quiz bổ sung để số câu bằng số ý chính
- `MM` — nhánh mindmap của từng unit (`"Tiếng Anh|Tiếng Việt"`)
- `DIA` — sơ đồ SVG minh hoạ
- `EXAMS` — ba đề thi thử
