# TL APP — Checkpoint Lab

App web ôn thi **Cambridge Primary Checkpoint (Stage 6)** cho học sinh lớp 5 hệ chuẩn Vinschool,
dùng trực tiếp trên điện thoại. Toàn bộ nằm trong **một file `index.html`**, chạy offline sau lần
mở đầu tiên, không cần cài đặt và không cần tài khoản.

## Bám theo sách trên lớp

Lớp 5 hệ chuẩn Vinschool học chương trình Cambridge Primary **Stage 6** — đúng với "workbook 6".
App xếp bài theo unit của sách:

| Môn | Sách | Cấu trúc trong app |
|---|---|---|
| Science | Cambridge Primary Science 6 Learner's Book (CUP, 1st edition), bản song ngữ Vinschool | 5 unit sách + 1 phần ôn thêm cho Checkpoint |
| Mathematics | Toán học 6 — Sách bài tập Quyển 1 (HK1) và Quyển 2 (HK2) | 12 học phần chia theo hai học kì |
| English (ESL) | Cambridge Global English 6 (CUP) | 6 phần theo kỹ năng của đề Checkpoint ESL |

Màn hình **"Thứ tự unit này lấy từ đâu?"** trong app ghi rõ phần nào đã đối chiếu được với nguồn
và phần nào còn cần xác nhận bằng mục lục sách in.

## Nội dung

- **24 unit sách**, **35 bài học**, **255 ý chính**, **255 câu quiz** — mỗi bài có số câu quiz
  đúng bằng số ý chính, mỗi câu đều có lời giải thích tiếng Việt.
- **280 mục từ vựng** Anh–Việt và **3 đề thi thử** (36 câu).
- **35 phần Mở rộng**: mỗi bài có 3 ý đào sâu vượt trên sách, 3 việc ứng dụng làm ngay ở nhà,
  và 1 câu hỏi thử thách.

## Tính năng

- **Phiên ôn 15 phút/ngày**: thẻ lật → mindmap và ý chính → quiz, có đồng hồ đếm ngược.
- **Mindmap cho cả 35 bài** cùng **19 sơ đồ minh hoạ** vẽ bằng SVG nội tuyến (hệ tuần hoàn, hô hấp,
  tiêu hoá, chuỗi thức ăn, mạch điện, trạng thái vật chất, hệ toạ độ, trục thời gian thì tiếng Anh…).
- **Ứng dụng hàng ngày**: sau mỗi bài quiz app hiện 3 việc làm được ngay, tích được và lưu theo ngày.
- **Song ngữ có nút ẩn**: mặc định chỉ hiện tiếng Anh, chạm mới hiện tiếng Việt.
- **Nghe phát âm** từ và câu tiếng Anh bằng giọng en-GB của thiết bị.
- **Ôn lại câu sai tự động** sau 1, 2, 4, 7 và 14 ngày.
- **Đề thi thử** có đồng hồ, không lộ đáp án cho tới khi nộp bài.
- **Báo cáo cho bố mẹ**: số phút học 7 ngày gần nhất, điểm theo môn, unit cần kèm thêm.
- Giao diện tự đổi theo nền sáng/tối của điện thoại.

## Chạy

Mở `index.html` bằng trình duyệt bất kỳ. Trên iPhone: mở link → nút Chia sẻ →
**Thêm vào MH chính** để dùng như một app thật. Tiến độ lưu bằng `localStorage` trên chính thiết bị.

## Sửa nội dung

Mọi thứ nằm trong các khối `<script>` của `index.html`:

| Khối | Nội dung |
|---|---|
| `DATA` | ý chính, từ vựng, quiz của 35 bài học |
| `EXTRA` | câu quiz bổ sung cho đủ bằng số ý chính |
| `MM` | nhánh mindmap từng bài (`"Tiếng Anh\|Tiếng Việt"`) |
| `DIA` | sơ đồ SVG minh hoạ |
| `EXT` | phần Mở rộng: đào sâu, ứng dụng, thử thách |
| `EXAMS` | ba đề thi thử |
| `PROG` | **thứ tự unit theo sách** — sửa ở đây nếu lớp dạy khác thứ tự |
