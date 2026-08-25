# TL APP — Checkpoint Lab

App web ôn thi **Cambridge Primary Checkpoint (Stage 6)** cho học sinh lớp 5 hệ chuẩn Vinschool,
dùng trực tiếp trên điện thoại. Toàn bộ nằm trong **một file `index.html`**, chạy offline sau lần
mở đầu tiên, không cần cài đặt và không cần tài khoản.

## Bám theo sách trên lớp

Lớp 5 hệ chuẩn Vinschool học chương trình Cambridge Primary **Stage 6** — đúng với "workbook 6".
App xếp bài theo unit của sách:

| Môn | Sách | Cấu trúc trong app |
|---|---|---|
| Science | Cambridge Primary Science 6 — Learner's Book và Workbook (CUP, **2nd edition**), bản song ngữ Vinschool | **6 unit, 21 bài nhỏ kèm số trang**, mỗi bài 9 ý chính + 1 phần ôn thêm |
| Mathematics | *Cambridge Primary Mathematics 6* (CUP, 2nd edition) | **17 unit, 37 bài nhỏ** — mỗi mục nhỏ trong sách là một bài học riêng |
| English (ESL) | *Cambridge Global English 6* (CUP) | **9 unit theo chủ đề**, mỗi unit có Vocabulary và Use of English |

**Cả ba môn** đã được đối chiếu trực tiếp với ảnh chụp mục lục sách của học sinh, từng bài ghi kèm
số trang để mở sách ra so được ngay. Màn hình *"Thứ tự unit này lấy từ đâu?"* trong app ghi rõ nguồn.

## Nội dung

- **35 unit sách**, **83 bài học**, **553 ý chính**, **553 câu quiz** — mỗi bài có số câu quiz
  đúng bằng số ý chính, mỗi câu đều có lời giải thích tiếng Việt.
- **738 mục từ vựng** Anh–Việt và **3 đề thi thử** (36 câu).
- **32 bài kiểm tra cuối unit** (320 câu): Toán 17 bài, Science 6 bài, ESL 9 bài — mỗi unit một bài.
  Làm liên tục có đồng hồ, không lộ đáp án cho tới khi nộp bài, chấm xong mới hiện lời giải từng câu.
  Câu hỏi phủ kín mọi mục nhỏ của unit đó trong sách.
- Bài kiểm tra Science và ESL còn **gắn từng câu với bài học tương ứng**, nên chấm xong app chỉ ra
  đúng bài cần ôn lại và bấm thẳng vào học được ngay — con không phải tự mò xem mình yếu chỗ nào.
- **83 phần Mở rộng**: mỗi bài có 3 ý đào sâu vượt trên sách, 3 việc ứng dụng làm ngay ở nhà,
  và 1 câu hỏi thử thách.

## Hai tài khoản

Mở app lên phải chọn tài khoản:

- **Thế Lâm** — vào thẳng, học bài, làm quiz, tích điểm và xin đổi thưởng.
- **Bố mẹ** — cần **mã PIN 4 số** (lần đầu vào thì tự đặt). Duyệt đổi thưởng, xem báo cáo, đổi PIN.

Cả hai tài khoản nằm trên chính thiết bị, không cần internet và không gửi dữ liệu đi đâu.
Mã PIN chỉ để cháu không tự duyệt điểm của mình — không phải cơ chế bảo mật thật.

## Điểm thưởng

| Quy tắc | Giá trị |
|---|---|
| Mỗi bài học tối đa | 5 điểm |
| Mỗi đề thi thử tối đa | 5 điểm |
| Quy đổi | 100 điểm = 100.000đ |
| Tối đa cả chương trình | 430 điểm = 430.000đ |

Điểm mỗi bài tính theo **điểm quiz cao nhất**: đúng 100% được 5 điểm, đúng 80% được 4 điểm.
Làm lại tốt hơn thì điểm tự tăng, làm lại kém hơn không bị mất điểm, và **một bài không bao giờ
cộng quá 10 điểm** dù làm bao nhiêu lần.

Đủ 10 điểm thì cháu bấm *Xin đổi thưởng* → yêu cầu chuyển sang tài khoản Bố mẹ chờ duyệt
(điểm bị giữ tạm trong lúc chờ). Bố mẹ bấm **Duyệt · đã đưa tiền** thì điểm mới bị trừ thật
và ghi vào lịch sử.

## Tính năng

- **Phiên ôn 15 phút/ngày**: thẻ lật → mindmap và ý chính → quiz, có đồng hồ đếm ngược.
  Đặt được **mục tiêu 1, 2 hoặc 3 phiên mỗi ngày** trong Cài đặt.
- **Ôn tập định kỳ**: đề tự sinh mới mỗi lần, không cộng điểm thưởng —
  *Ôn tuần* (15 câu, lấy từ bài học trong 7 ngày gần nhất), *Ôn tháng* (25 câu),
  *Thi thử cả năm* (40 câu rút từ toàn bộ 83 bài và 32 bài kiểm tra unit).
- **Chống đoán mẹo**: vị trí bốn đáp án được xáo lại mỗi lần mở app (lệch vị trí 64% → 26%),
  và các đáp án sai được viết dài tương đương đáp án đúng (số câu lệch nặng 152 → 8). Tab **⭐ Thưởng** có bảng **Thành tích** tách rõ điểm đến từ đâu.
- **Mật mã mở app**: lần đầu vào app sẽ hỏi đặt mã 4 số (bỏ qua được, đặt lại trong Cài đặt bất cứ lúc nào).
  Mã này độc lập với mã riêng của bố mẹ dùng để duyệt đổi thưởng.
- **Mindmap cho cả 83 bài** cùng **19 sơ đồ** và **55 hình minh hoạ**: Science 43, Toán 7, ESL 5,
  tất cả vẽ bằng SVG nội tuyến nên chạy offline và tự đổi màu theo nền sáng/tối:
  quả tim bổ đôi 4 ngăn, ống máu lắng ba lớp, cách bắt mạch cổ tay, phổi và phế nang,
  đường đi của thức ăn, nhung mao ruột non, thận và bàng quang, năm nhóm động vật có xương sống,
  lưới thức ăn, gấu bắc cực và lạc đà, nước đá – nước – hơi, ba biến đổi không thuận nghịch,
  cách thu lại muối, nhiệt kế 0°C và 100°C, lực kế lò xo, dù và quả bóng rơi,
  cách tạo bóng, ống hút gãy và lăng kính, mạch điện thật, bảng kí hiệu mạch,
  ngày và đêm, tám hành tinh, các pha Mặt Trăng, bố trí thí nghiệm công bằng,
  bảng số liệu và đồ thị, rác nhựa ra biển, ba thùng phân loại rác.
- **Ứng dụng hàng ngày**: sau mỗi bài quiz app hiện 3 việc làm được ngay, tích được và lưu theo ngày.
- **Song ngữ có nút ẩn**: mặc định chỉ hiện tiếng Anh, chạm mới hiện tiếng Việt.
- **Nghe phát âm** từ và câu tiếng Anh bằng giọng en-GB của thiết bị.
- **Ôn lại câu sai tự động** sau 1, 2, 4, 7 và 14 ngày.
- **Đề thi thử** có đồng hồ, không lộ đáp án cho tới khi nộp bài.
- **Báo cáo cho bố mẹ**: số phút học 7 ngày gần nhất, điểm theo môn, unit cần kèm thêm.
- Giao diện tự đổi theo nền sáng/tối của điện thoại.

> **Lưu ý:** toàn bộ tiến độ và điểm lưu bằng `localStorage` trên **chính thiết bị và trình duyệt đó**.
> Bố mẹ duyệt thưởng trên cùng máy cháu học. Dùng máy khác thì dữ liệu bắt đầu lại từ đầu.

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
| `DIA` | sơ đồ tóm tắt của bài |
| `IMG` | 30 hình minh hoạ chi tiết môn Science |
| `EXT` | phần Mở rộng: đào sâu, ứng dụng, thử thách |
| `EXAMS` | ba đề thi thử |
| `TESTS` | 32 bài kiểm tra cuối unit của cả ba môn |
| `PROG` | **thứ tự unit theo sách** — sửa ở đây nếu lớp dạy khác thứ tự |
