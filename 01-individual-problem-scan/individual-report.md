# 01 — Individual Problem Scan

**Học viên:** Nguyễn Hùng Mạnh — 2A202601256

Bối cảnh: AI Developer làm việc solo trên nhiều dự án song song (video/audio/dịch thuật, trading, chatbot), vận hành content đa kênh, đồng thời là học viên AI Codelabs.

## Scan rộng

Scan 10 problems, vượt mức tối thiểu 5.

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | AI có thể tốt hơn | Sau buổi họp/buổi học phải tua lại record hoặc lục tài liệu để tìm một chi tiết | Mạnh, người cần hỏi lại thông tin | 2-3 buổi dài/tuần, mỗi lần tìm 45-60 phút |
| 2 | AI có thể tốt hơn | Tiền tiêu rải qua nhiều app/ví, cuối tháng không biết tiền đi đâu | Mạnh | Chưa từng tổng hợp được lần nào |
| 3 | Tốn thời gian | Đang làm việc bị đứt mạch vì mạng xã hội và việc xen ngang | Mạnh | Không nhớ nổi bị đứt mấy lần/buổi |
| 4 | Lặp lại | Bị trừ tiền tự động cho app không còn dùng | Mạnh | Không nhớ hết đang trả những gì (YouTube, Claude, ChatGPT...) |
| 5 | AI có thể tốt hơn | Quay lại repo bỏ lâu, phải đọc lại code/docs mới nhớ đang làm dở gì | Mạnh | 45 repo trong máy, mỗi lần nối lại mạch 30 phút |
| 6 | Lặp lại | Một nội dung đăng nhiều kênh, mỗi kênh sửa caption và format riêng | Mạnh | 3 kênh đang vận hành |
| 7 | Pain từ người khác | User dùng tool hỏi lặp cùng một câu, không có FAQ nên trả lời tay | User của tool, Mạnh | Hỏi lặp nhiều, chưa có log để đếm |
| 8 | Pain từ người khác | Làm bài nhóm phải chờ thành viên gửi phần của họ mới ghép được, mỗi người một format | Cả nhóm, người ghép bài | Nhóm 5 người, bài nộp chung phải chờ đủ mới ghép |
| 9 | Tốn thời gian | Đọc tài liệu và paper kỹ thuật tiếng Anh dài, phải vừa đọc vừa tra nghĩa | Mạnh, người đọc tài liệu chuyên ngành | Đã tự xây 3 tool dịch tài liệu (BabelDOC, PolyglotPDF, DocsTranslate) — đủ đau để tự làm công cụ |
| 10 | Lặp lại | Mỗi repo mới phải dựng lại cùng một bộ cấu hình chuẩn (hướng dẫn, docs, quy ước) | Mạnh | 45 repo, lần nào cũng lặp lại cùng các bước |

## Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Tìm lại một chi tiết sau buổi họp/học | Mất nhiều thời gian nhất (45-60 phút/lần), lặp lại hằng tuần, workflow rõ | "Tìm đúng chi tiết" đủ tốt là thế nào |
| 2 | Nối lại mạch khi quay lại repo cũ | Có số thật (45 repo), workflow rõ, đo được bằng thời gian | "Nhớ ra được việc dở" đủ tốt là thế nào |
| 3 | User hỏi lặp cùng một câu về tool | Người khác cùng đau, không chỉ mình | Chưa có log nên chưa biết câu nào lặp nhiều nhất |

## Problem Card #1 — Tìm lại một chi tiết sau buổi họp/học

**Problem 1 câu:**
Sau buổi họp hoặc buổi học, khi cần dùng lại một chi tiết đã nghe thì mất 45-60 phút tua record và lục tài liệu, trong đó bước tua tìm đúng đoạn tốn nhất.

**Actor:**
Người dự buổi cần dùng lại thông tin đã nghe, và người hỏi lại thông tin đó.

**Thời điểm / bối cảnh:**
Sau các buổi dài 2-3 lần/tuần, thường là lúc bắt tay làm bài hoặc áp dụng vào việc thật.

**Current workflow:**

```text
1. Nhớ mang máng có nghe điều này ở buổi nào đó
2. Mở lại record hoặc tài liệu của buổi đó
3. Tua tìm đúng đoạn nói về nó
4. Nghe lại để xác nhận đúng chỗ cần
5. Ghi ra thông tin để dùng
```

**Bottleneck:**
Bước 3 — tua tìm đúng đoạn trong record dài, vì không biết nó nằm ở phút thứ mấy và phải nghe thử nhiều chỗ.

**Impact:**
45-60 phút mỗi lần cần tra lại, 2-3 buổi dài mỗi tuần. Tốn thời gian đến mức nhiều lần bỏ luôn không tra, chấp nhận làm theo trí nhớ mơ hồ.

**Success metric:**
Giảm thời gian tìm lại một chi tiết từ 45-60 phút xuống dưới 5 phút, và trả về được đúng đoạn nguồn để tự kiểm chứng.

**Non-AI alternative:**
Ghi note trong lúc nghe. Giúp được phần nào nhưng vừa nghe vừa ghi thì bỏ sót, và lúc đó chưa biết trước chi tiết nào sau này sẽ cần.

**AI hypothesis:**
AI tạo transcript có mốc thời gian cho mỗi buổi, cho hỏi bằng câu hỏi thường và trả về đoạn liên quan kèm mốc thời gian để người tự nghe lại xác nhận.

**Quick gut:**
Workflow.

### Draft current workflow

```text
CURRENT STATE — 45-60 phút

[1 Nhớ ra buổi nào: 5']
→ [2 Mở record/tài liệu: 5']
→ [3 Tua tìm đúng đoạn: 30']   <-- bottleneck
→ [4 Nghe lại xác nhận: 10']
→ [5 Ghi ra để dùng: 5']
```

### Draft future workflow

```text
FUTURE STATE — dưới 5 phút

[1 Hỏi bằng câu hỏi thường: 1']
→ [2 AI trả về đoạn liên quan + mốc thời gian: 1']
→ [3 Người nghe lại đúng mốc đó để xác nhận: 3']   <-- human boundary
→ [4 Dùng thông tin]

Fallback: AI trả sai đoạn hoặc không tìm thấy → tua tay như cũ.
```

## Problem Card #2 — Nối lại mạch khi quay lại repo cũ

**Problem 1 câu:**
Khi quay lại một repo đã bỏ lâu, mất khoảng 30 phút đọc lại code và docs mới nhớ được đang làm dở gì, trong đó bước tự dựng lại ngữ cảnh tốn nhất.

**Actor:**
Dev solo đang giữ 45 repo song song, không có đồng đội để hỏi lại.

**Thời điểm / bối cảnh:**
Mỗi lần chuyển sang một dự án đã không đụng tới vài tuần.

**Current workflow:**

```text
1. Mở repo, không nhớ đang dở việc gì
2. Đọc README và docs
3. Xem git log để đoán lần cuối làm gì
4. Đọc code các file liên quan
5. Chạy thử xem còn chạy được không
6. Nhớ ra việc dở, bắt đầu làm tiếp
```

**Bottleneck:**
Bước 3-4 — tự dựng lại ngữ cảnh từ code và git log, vì git log chỉ ghi việc đã xong, không ghi việc đang dở và lý do dừng.

**Impact:**
30 phút mỗi lần chuyển repo. Ngại chuyển repo nên dự án phụ bị bỏ lâu hơn, càng lâu càng khó quay lại.

**Success metric:**
Giảm thời gian nối lại mạch từ 30 phút xuống dưới 5 phút, không phải mở code ra đọc mới hiểu đang dở gì.

**Non-AI alternative:**
Ghi tay một file JOURNAL ghi việc đang dở cuối mỗi phiên. Giải được phần lớn, nhưng phụ thuộc việc nhớ ghi. Quên ghi một lần là mất luôn ngữ cảnh phiên đó.

**AI hypothesis:**
AI đọc git diff và lịch sử phiên làm việc, tự tóm tắt việc đang dở vào cuối phiên; đầu phiên sau đọc lại bản tóm tắt đó thay vì đọc code.

**Quick gut:**
Workflow.

### Draft current workflow

```text
CURRENT STATE — 30 phút

[1 Mở repo: 1']
→ [2 Đọc README/docs: 5']
→ [3 Xem git log: 5']       <-- bottleneck
→ [4 Đọc lại code: 14']     <-- bottleneck
→ [5 Chạy thử: 5']
→ [6 Làm tiếp]
```

### Draft future workflow

```text
FUTURE STATE — dưới 5 phút

[1 Mở repo: 1']
→ [2 AI tóm tắt việc dở từ git diff + note phiên trước: 1']
→ [3 Người đọc và xác nhận đúng việc: 2']   <-- human boundary
→ [4 Làm tiếp]

Fallback: tóm tắt sai hoặc thiếu → quay về đọc code như cũ.
```

## Problem Card #3 — User hỏi lặp cùng một câu về tool

**Problem 1 câu:**
User dùng tool nhắn hỏi lặp đi lặp lại cùng vài câu, mỗi người hỏi riêng nên phải gõ lại câu trả lời cũ từng lần.

**Actor:**
User của tool (người cần câu trả lời ngay) và người làm tool kiêm luôn support.

**Thời điểm / bối cảnh:**
Rải rác trong ngày, qua comment và tin nhắn ở nhiều kênh khác nhau.

**Current workflow:**

```text
1. User nhắn hỏi qua comment hoặc tin nhắn
2. Đọc câu hỏi, nhận ra câu này đã trả lời ai đó rồi
3. Tìm lại câu trả lời cũ, hoặc gõ lại từ đầu
4. Trả lời riêng cho người đó
5. Vài hôm sau người khác hỏi đúng câu đó
```

**Bottleneck:**
Bước 3-4 — gõ lại cùng một nội dung cho từng người, vì câu trả lời cũ nằm rải trong lịch sử chat, không gom về một chỗ.

**Impact:**
User phải chờ mới dùng được tool, có người bỏ luôn không dùng nữa. Người làm tool bị cắt vụn thời gian trong ngày.

**Success metric:**
Chưa có baseline. Việc đầu tiên phải làm là log lại câu hỏi trong 1-2 tuần để biết mỗi tuần bao nhiêu câu và câu nào lặp nhiều nhất, rồi mới đặt được mục tiêu.

**Non-AI alternative:**
Viết FAQ và ghim hướng dẫn ngay chỗ user hay hỏi. Rẻ và giải được phần lớn nếu đúng là chỉ lặp vài câu, nhưng vẫn có user không đọc mà hỏi thẳng.

**AI hypothesis:**
Bot đọc câu hỏi, khớp với FAQ có sẵn và trả lời ngay; câu nào không khớp thì chuyển cho người thật.

**Quick gut:**
Rule trước. Chỉ lên Workflow nếu log cho thấy câu hỏi quá đa dạng, FAQ tĩnh không phủ nổi.

### Draft current workflow

```text
CURRENT STATE — rải rác cả ngày

[1 User nhắn hỏi]
→ [2 Đọc, nhận ra câu quen]
→ [3 Tìm lại/gõ lại câu trả lời]   <-- bottleneck
→ [4 Trả lời riêng từng người]     <-- bottleneck
→ [5 Người khác lại hỏi đúng câu đó]
```

### Draft future workflow

```text
FUTURE STATE — trả lời ngay, không cần người

[1 User nhắn hỏi]
→ [2 Khớp câu hỏi với FAQ có sẵn]
→ [3a Khớp → trả lời ngay]
→ [3b Không khớp → chuyển người thật]   <-- human boundary
→ [4 Câu mới được thêm vào FAQ]

Fallback: trả lời sai hoặc user không hài lòng → chuyển ngay cho người thật.
```

## Card muốn pitch nhất

Card #1 — tìm lại một chi tiết sau buổi họp/học.

Vì sao:

```text
Đây là card tốn nhiều thời gian nhất trong ba card (45-60 phút mỗi lần cần tra
lại) và lặp lại hằng tuần, nên impact rõ nhất.

Hai card kia đều chỉ có mình tôi đau: card #2 xuất phát từ việc tôi giữ 45 repo,
card #3 thì chưa có log nên chưa chứng minh được. Card #1 thì bất kỳ ai đi học
hoặc đi họp đều gặp, nên nhóm dễ kiểm chứng và dễ mở rộng thành bài chung.
```

Câu hỏi muốn nhóm phản biện:

```text
Metric "dưới 5 phút" có phải là thứ đáng đo không, hay cái đáng đo là
có tìm ra đúng chi tiết hay không?
Nếu AI trả về sai đoạn mà mình tin luôn thì hậu quả là gì?
```
