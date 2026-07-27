# 02 — Group Problem Statement

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm | Phân công cụ thể |
| --- | --------- | ----------- | ------------------ | ---------------- |
| 1 | Bùi Thái Sơn | 2A202601126 | Research | Research giải pháp đã có (Zotero, Mendeley, Paperpile), tìm nguồn uy tín |
| 2 | Nguyễn Văn Trọng | 2A202601102 | Workflow | Vẽ workflow trước/sau, xác định bottleneck và AI intervention point |
| 3 | Nguyễn Hùng Mạnh | 2A202601256 | Metric | Xây dựng baseline, success metric, before/after impact table |
| 4 | Đoàn Ngọc Linh | 2A202601762 | Research | Research thêm nguồn học thuật (Semantic Scholar API, CrossRef), kiểm chứng link |
| 5 | Nguyễn Tiến Đạt | 2A202601850 | Pain point & Validation | Quick interview, mini poll, thu thập tín hiệu pain thật từ sinh viên |

---

# Phase 3 — Group Convergence

## Bước 3.1 — Trình bày top 3

Nhóm 5 người, mỗi người share top 3. Tổng cộng 15 candidates.

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh |
| --- | --- | --- | --- | --- | --- |
| 1 | Nguyễn Văn Trọng | Debug lỗi runtime/logic mất nhiều thời gian | Dev | Đọc hiểu stack trace để tìm nguyên nhân | Workflow |
| 2 | Nguyễn Văn Trọng | Viết code boilerplate CRUD lặp lại | Dev | Gõ lại pattern giống nhau cho từng entity | Rule |
| 3 | Nguyễn Văn Trọng | Viết test case / unit test lặp lại | Dev | Viết lại Arrange-Act-Assert cho từng hàm | Workflow |
| 4 | Nguyễn Hùng Mạnh | Nối lại mạch khi quay lại repo cũ | Dev solo nhiều dự án | Tự dựng lại ngữ cảnh từ code và git log | Workflow |
| 5 | Nguyễn Hùng Mạnh | Đăng một nội dung lên nhiều kênh | Người làm content | Sửa caption/format cho từng kênh | Workflow |
| 6 | Nguyễn Hùng Mạnh | Tìm lại một chi tiết sau buổi họp/học | Người dự buổi | Tua record tìm đúng đoạn | Workflow |
| 7 | Đoàn Ngọc Linh | Tạo flashcard để ôn lại bài tập | Sinh viên | Nhập tay từng thẻ | Rule |
| 8 | Đoàn Ngọc Linh | Đọc và lọc nhiều file PDF để tìm trích dẫn, số liệu | Sinh viên | Đọc quét nhiều tài liệu dài để tìm đúng đoạn | Workflow |
| 9 | Đoàn Ngọc Linh | Gom bài tập nhóm từ nhiều file rời rạc | Trưởng nhóm | Chuẩn hoá format và văn phong từ nhiều người | Rule |
| 10 | Nguyễn Tiến Đạt | Chuyển tài liệu nghiên cứu thành sản phẩm có cấu trúc | Người trình bày nghiên cứu | Rút thông tin thô thành output có logic | Workflow |
| 11 | Nguyễn Tiến Đạt | Chuyển paper/báo cáo thành slide thuyết trình | Người trình bày | Rút ý chính và sắp xếp thành slide | Workflow |
| 12 | Nguyễn Tiến Đạt | Tổng hợp và viết lại từ nhiều tài liệu | Người viết nghiên cứu | Rút ý chính rồi viết lại bằng ngôn ngữ riêng | Workflow |
| 13 | Bùi Thái Sơn | Literature review, summary paper, tóm tắt nghiên cứu | Người viết nghiên cứu | Kết nối nhiều paper thành đoạn văn mạch lạc | Workflow |
| 14 | Bùi Thái Sơn | Quản lý tham khảo và citation | Người viết bài có trích dẫn | Chuẩn hoá thông tin tham khảo cho đúng và nhất quán | Chưa biết |
| 15 | Bùi Thái Sơn | Kiểm tra citation, định dạng reference, chèn in-text citation | Người viết bài có trích dẫn | Kiểm tra và sửa thủ công khi hoàn thiện bài | Rule / Workflow |

## Bước 3.2 — Gom trùng / cluster

| Cluster | Candidates included | Pattern chung | Ghi chú |
| --- | --- | --- | --- |
| A — Code & Debug | 1, 2, 3, 4 | Lập trình viên gặp vấn đề lặp lại hoặc tốn thời gian khi code | Chỉ dev trong nhóm hiểu sâu, actor hẹp |
| B — Nội dung & Trình bày | 5, 10, 11, 12, 13 | Chuyển thông tin thô thành sản phẩm có cấu trúc | Cluster đông nhất, nhưng "output đủ tốt" khó thống nhất cách đo |
| C — Học tập & Ôn bài | 6, 7, 8, 9 | Sinh viên mất thời gian tổng hợp thông tin rời rạc | Pain thật, nhưng phạm vi rộng |
| D — Citation & Reference | 14, 15 | Kiểm tra, chuẩn hoá và chèn citation thủ công tốn thời gian, dễ sai | Đúng/sai xác định được nên dễ đo nhất |

Nhóm nhận thấy Cluster D có pain rõ nhất, actor cụ thể (sinh viên viết bài), workflow tuyến tính và metric dễ đo.

## Bước 3.3 — Shortlist

| Candidate | Vì sao vào shortlist | Rủi ro / điều chưa rõ |
| --- | --- | --- |
| Quản lý citation và reference (cluster D) | Actor rõ, workflow tuyến tính, đúng/sai đo được, cả nhóm từng làm | Zotero/Mendeley đã giải phần format — phải chỉ ra AI thêm giá trị ở đâu |
| Đọc và lọc PDF để tìm trích dẫn, số liệu (#8, cluster C) | Pain rõ và tốn nhiều thời gian nhất | Phạm vi rộng, dễ trượt thành bài toán search toàn văn |
| Tóm tắt literature review từ nhiều paper (#13, cluster B) | Workflow rõ, nhiều người trong nhóm từng làm | "Bản tóm tắt đủ tốt" mỗi người hiểu một kiểu, khó thống nhất metric |

## Bước 3.4 — Score để đồng thuận

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
| --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| Quản lý citation và reference | 5 | 5 | 5 | 4 | 5 | 5 | 5 | 34 |
| Đọc và lọc PDF tìm trích dẫn | 4 | 3 | 5 | 3 | 2 | 4 | 4 | 25 |
| Tóm tắt literature review từ nhiều paper | 4 | 4 | 3 | 2 | 4 | 3 | 4 | 24 |

Ghi chú cách chấm ở các ô thấp:

```text
- "Đọc và lọc PDF" — Làm trong lab: 2, vì phải xử lý được nhiều PDF dài, vượt
  phạm vi một buổi. Workflow rõ: 3, vì cách mỗi người tìm số liệu rất khác nhau.
- "Tóm tắt literature review" — Impact đo được: 2, vì nhóm không thống nhất được
  thế nào là bản tóm tắt đủ tốt. Pain có evidence: 3, vì trong 5 người phỏng vấn
  chỉ vài người thực sự viết literature review.
- "Quản lý citation" — Impact đo được: 4 chứ không phải 5, vì baseline 20-30 phút
  mới là ước lượng, chưa bấm giờ thật.
```

Candidate nhóm chọn:

```text
Quản lý citation và reference.
```

Vì sao chọn:

```text
- Workflow rõ ràng: tìm tài liệu → thu thập metadata → chèn citation → kiểm tra reference list.
- Pain thật: sinh viên thường mất thời gian sửa citation và reference thủ công trước khi nộp.
- Đúng/sai của một citation là xác định được, không phụ thuộc cảm nhận — nên đặt được metric chắc.
- Validate được nhanh bằng Zotero, Mendeley, Word hoặc Overleaf.
- Nhiều tool/pattern có sẵn để research và so sánh.
- Vẽ before/after workflow rất rõ.
```

Vì sao không chọn các candidate còn lại:

```text
- Đọc và lọc PDF tìm trích dẫn: impact rộng nhưng phân loại và chuẩn hoá nguồn
  phức tạp, scope quá lớn cho lab.
- Tóm tắt literature review: workflow rõ nhưng quality metric khó thống nhất
  trong thời gian lab.
- Cluster B đông candidate nhất nhưng chung đặc điểm là output mở, khó đo.
  Nhóm chọn cluster D vì ít candidate hơn nhưng đo được chắc hơn.
```

Nếu có disagreement, nhóm xử lý thế nào:

```text
Nhóm bám tiêu chí "đo được" làm trọng tài. Candidate nào không trả lời được
câu "làm sao biết là tốt hơn" thì hạ ưu tiên, kể cả khi nhiều người thấy đau.

Ban đầu nhóm nghiêng về cluster B (chuyển paper thành slide) vì nhiều người
cùng gặp, nhưng khi thử đặt metric thì không thống nhất được thế nào là
"slide tốt", nên chuyển sang cluster D.
```

---

# Phase 4 — Quick Validation + Research giải pháp

## Bước 4.1 — Quick validation

Nhóm hỏi nhanh 5 sinh viên và poll 8 người trong lớp.

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
| --- | ---: | --- | --- | --- |
| Quick interview | 5 | 4/5 người từng phải sửa citation hoặc reference thủ công trước khi nộp | 1 người đã dùng Zotero nên pain giảm nhiều | Thu hẹp problem: không phải "tự động tạo citation tổng quát", mà là "kiểm tra và chuẩn hoá citation" |
| Mini poll trong lớp | 8 | 6/8 từng gặp lỗi citation hoặc thiếu reference | Một số người dùng tool hỗ trợ nên chỉ cần kiểm tra thêm | Thêm non-AI alternative: Zotero/Mendeley + template citation |
| Log / review / ticket | 0 | Không có | Không có | Nhóm không tiếp cận được bài đã chấm hay nhận xét của giảng viên nên chưa có bằng chứng loại này |

Insight sau validation:

```text
Pain thật không nằm ở việc "copy citation". Pain nằm ở việc kiểm tra tính đúng,
nhất quán và sửa thủ công trước khi nộp.
```

Giả định còn mở (chưa kiểm chứng được):

```text
- Con số 20-30 phút/bài là ước lượng từ trải nghiệm của nhóm và người được hỏi,
  chưa bấm giờ thật trên một bài cụ thể.
- Chưa biết trung bình mỗi bài có bao nhiêu lỗi citation lọt qua khi nộp,
  vì không tiếp cận được bài đã chấm.
- Chưa kiểm chứng ngoài môi trường sinh viên (nghiên cứu sinh, người viết
  báo cáo công việc).
```

## Bước 4.2 — Research giải pháp đã có

Nhóm tìm các hướng đã có sẵn, không giả định phải tự build từ đầu.

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
| --- | --- | --- | --- | --- | --- |
| Zotero (open-source) | https://www.zotero.org | Quản lý reference, tạo citation, sync library | Miễn phí, plugin Word/Google Docs, hỗ trợ nhiều citation style (CSL) | Metadata import từ web có thể thiếu/sai, cần user kiểm tra thủ công | Dùng làm base workflow; AI nên hỗ trợ bước kiểm tra metadata mà Zotero chưa tự làm |
| Mendeley Reference Manager (Elsevier) | https://www.mendeley.com/reference-management/reference-manager | Chèn citation trong Word, quản lý PDF và reference | Tích hợp tốt với Word, auto-extract metadata từ PDF | Vẫn cần kiểm tra thủ công; bản miễn phí giới hạn storage | Pattern tốt: tool làm phần import, người dùng vẫn phải review |
| CrossRef REST API | https://api.crossref.org/swagger-ui/index.html | Tra cứu metadata chính thức của paper qua DOI | Nguồn metadata uy tín (từ nhà xuất bản), API miễn phí | Chỉ cover paper có DOI, không cover sách/web/thesis | AI có thể gọi CrossRef API để verify metadata thay vì đoán |
| Semantic Scholar API (Allen AI) | https://api.semanticscholar.org/ | Tìm paper, lấy metadata, citation graph | API miễn phí, có abstract, author, citation count | Không phủ toàn bộ ngành, metadata đôi khi trễ | Dùng như nguồn bổ sung để cross-check metadata |
| Case hallucinated citation | https://www.reuters.com/legal/new-york-lawyers-sanctioned-using-fake-chatgpt-cases-legal-brief-2023-06-22/ | Luật sư nộp hồ sơ toà với các vụ án do ChatGPT bịa ra, bị phạt | Cho thấy rủi ro rất cụ thể | Citation giả nhìn y như thật: đúng format, có tên tác giả, có số trang | Không được để AI tự sinh metadata từ trí nhớ — đây là lý do bắt buộc phải tra qua API |

Research takeaway:

```text
Không nên build agent tự làm toàn bộ citation. Hướng hợp lý: Workflow —
thu thập reference bằng Zotero/Mendeley → AI gọi CrossRef/Semantic Scholar API
kiểm tra metadata → AI gợi ý format citation → người dùng review trước khi nộp.

Điểm mấu chốt: AI chỉ được dùng metadata do API trả về, không được điền từ
trí nhớ của mô hình. Đó là ranh giới giữa "kiểm chứng" và "bịa nguồn".
```

---

# Phase 5 — Workflow + Problem Statement

## Bước 5.1 — Current workflow bản nhóm

```text
CURRENT STATE — 6 bước, 20-30 phút

[1 Thu thập paper/source: 4-6']
→ [2 Copy metadata thủ công: 4-6']
→ [3 Chọn style citation: 1-2']
→ [4 Chèn citation vào văn bản: 4-6']
→ [5 Kiểm tra reference list: 5-7']    <-- bottleneck
→ [6 Sửa lỗi thủ công: 2-3']
```

| Bước | Actor | Input | Output | Thời gian/tần suất | Ghi chú |
| --- | --- | --- | --- | --- | --- |
| 1 | Người viết | Chủ đề bài viết | Danh sách paper/source đã lưu | 4-6' · mỗi bài | Zotero/Mendeley làm được phần lớn |
| 2 | Người viết | Link/PDF nguồn | Metadata: tác giả, năm, tên bài, DOI | 4-6' · mỗi bài | Nguồn không chuẩn học thuật phải nhập tay |
| 3 | Người viết | Yêu cầu của môn/tạp chí | Chọn được style APA/IEEE/MLA | 1-2' · mỗi bài | Làm một lần, ít tốn |
| 4 | Người viết | Bản nháp + thư viện reference | Bài có in-text citation | 4-6' · mỗi bài | Handoff: từ thư viện sang bản thảo |
| 5 | Người viết | Bài đã chèn citation | Reference list đã rà | 5-7' · mỗi bài | **Bottleneck** — đối chiếu thủ công từng mục |
| 6 | Người viết | Danh sách lỗi tự phát hiện | Bản cuối để nộp | 2-3' · mỗi bài | Lỗi phát hiện muộn, sát deadline |

Bottleneck chính:

```text
Bước 5 — kiểm tra reference list. Người viết phải tự đối chiếu ba thứ cùng lúc:
citation trong bài có khớp mục trong reference list không, metadata có khớp bản
gốc không, và có mục nào thừa hoặc thiếu không.

Đây là việc đối chiếu thủ công làm sát deadline nên dễ bỏ sót. Tool hiện có
(Zotero/Mendeley) đảm bảo đúng FORMAT, nhưng không trả lời được câu
"nguồn này có thật và metadata có khớp bản gốc không".
```

## Bước 5.2 — Future workflow bản nhóm

```text
FUTURE STATE — 4 bước, 8-10 phút

[1 Import source vào Zotero/Mendeley: 2']              -- Rule/tool
→ [2 AI kiểm tra metadata qua CrossRef API: 1-2']      -- AI step
→ [3 AI gợi ý format chuẩn + kiểm tra consistency: 2'] -- AI step
→ [4 Người dùng review + xác nhận: 3-4']               <-- human boundary

Boundary:
AI chỉ được dùng metadata do CrossRef/Semantic Scholar trả về. AI không được
tự điền metadata từ trí nhớ. Nguồn nào tra không ra (sách, web, thesis không
có DOI) thì báo "không xác minh được", không đoán.

Fallback nếu AI sai:
- AI đánh dấu nhầm chỗ đúng → người bỏ qua, tốn thêm ít phút.
- AI bỏ sót → vẫn còn bước người tự rà reference list như cũ.
- AI đề xuất metadata mà không dẫn được nguồn API → coi là tín hiệu sai, bỏ ngay.

Bottleneck mới:
Bước 4 — người review và xác nhận. Chấp nhận được vì là bước kiểm soát chất lượng
và không được phép giao cho AI.
```

Before/after impact:

| Metric | Trước | Sau kỳ vọng | Ghi chú |
| --- | ---: | ---: | --- |
| Số bước | 6 | 4 | Giảm thao tác thủ công |
| Tổng thời gian | 20-30 phút | 8-10 phút | Target chính |
| Số bước thủ công | 6/6 | 2/4 | Người vẫn làm bước import và bước review |
| Bottleneck chính | Kiểm tra reference list | Review + xác nhận | Human boundary, giữ lại có chủ đích |
| Risk mới | Không có AI risk | AI gợi ý sai metadata; nguy hiểm nhất là AI tự điền metadata không tra được nguồn | Bắt buộc review trước khi nộp |

## Bước 5.3 — Problem Statement v0

| Field | Nội dung |
| --- | --- |
| **Actor** | Sinh viên, nghiên cứu sinh chịu trách nhiệm hoàn thiện bài viết và reference list. |
| **Workflow** | Thu thập paper/source → copy metadata → chọn citation style → chèn citation → kiểm tra reference list → sửa lỗi. |
| **Bottleneck** | Bước kiểm tra reference list: đối chiếu thủ công giữa citation trong bài, reference list và bản gốc; làm sát deadline nên dễ bỏ sót. |
| **Impact** | Một bài viết mất 20-30 phút cho phần citation. Sai hoặc thiếu trích dẫn bị trừ điểm; nguồn không tồn tại có thể bị xử lý như đạo văn. |
| **Success Metric** | Thời gian: 20-30 phút → 8-10 phút. Số lỗi format citation trước khi nộp: 0. Số nguồn vào bài mà chưa qua đối chiếu: 0 — nguồn có DOI đối chiếu bằng CrossRef, nguồn không có DOI (sách, web, thesis) thì người tự mở bản gốc kiểm. Cách đo: bấm giờ trên 3 bài mẫu và rà lại toàn bộ reference list sau khi nộp. |
| **Boundary** | AI chỉ kiểm tra và gợi ý; không tự nộp bài; không tự chỉnh sửa nội dung bài viết. AI không được tự điền metadata từ trí nhớ — chỉ dùng dữ liệu API trả về. Nguồn tra không ra thì báo "không xác minh được". Người phải review trước khi nộp. |

---

# Phase 6 — Rule / Workflow / Agent + Decision

## Bước 6.0 — Ma trận độ phù hợp với AI

Bài toán của nhóm nằm ở ô nào?

```text
Độ mơ hồ THẤP × Độ phức tạp CAO
→ "Workflow điều phối nhiều bước rõ ràng, chưa chắc cần Agent"
```

Vì sao?

```text
Độ mơ hồ thấp: một citation đúng hay sai là xác định được. Có chuẩn cố định
(APA/IEEE/MLA) và metadata đối chiếu được với CrossRef — không phải loại output
"mỗi lần khác nhau vẫn chấp nhận được".

Độ phức tạp cao: 6 bước nối tiếp, nhiều nguồn dữ liệu (bản nháp, thư viện
reference, API metadata), bước sau phụ thuộc kết quả bước trước.

AI không cần tự quyết định bước tiếp theo — thứ tự các bước cố định cho mọi bài.
Đó là lý do dừng ở Workflow, không lên Agent.
```

## Bước 6.1 — So sánh Rule / Workflow / Agent

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? |
| --- | --- | --- | --- | --- |
| **Rule** | Template citation style, auto-import từ Zotero/Mendeley | Đủ nếu người dùng chỉ cần format chuẩn | Không kiểm tra được metadata sai/thiếu | Không chọn làm toàn bộ, nhưng dùng cho bước import |
| **Workflow** | Import source → AI kiểm tra metadata (CrossRef API) → AI gợi ý citation → user review | Hợp vì workflow tuyến tính, AI hỗ trợ bước kiểm tra rõ ràng | AI gợi ý sai metadata khi paper không có DOI | **Chọn** |
| **Agent** | Agent tự thu thập, kiểm tra, cập nhật citation và reference list | Chỉ cần nếu workflow nhiều nhánh, tự quyết bước tiếp theo | Quá rộng; nếu agent tự tìm nguồn thì rơi đúng vào việc LLM bịa nhiều nhất | Chưa chọn |

Mức chọn:

```text
Workflow.
```

Vì sao chọn:

```text
- Thu thập dữ liệu có thể dùng rule/tool (Zotero/Mendeley).
- Kiểm tra metadata cần AI gọi API (CrossRef, Semantic Scholar) để verify.
- Người dùng vẫn review nên risk kiểm soát được.
- Chưa cần agent vì workflow không cần tự lập kế hoạch động.
```

Vì sao không chọn mức đơn giản hơn:

```text
Rule (Zotero/Mendeley + template) giải được bước thu thập và format — đó là phần
nhóm giữ nguyên, không thay bằng AI. Nhưng Rule không giải được đúng bottleneck:
nó không đọc được bản nháp nên không biết citation nào trong bài không có trong
reference list, và không đối chiếu được metadata với bản gốc.

Đó là việc đối chiếu giữa nội dung bài viết, danh sách nguồn và dữ liệu gốc —
cần đọc hiểu ngôn ngữ và gọi API, nằm ngoài khả năng của quy tắc cố định.
Vì vậy nhóm lên một mức, dừng ở Workflow, không lên Agent.
```

## Bước 6.2 — Problem Statement v1

| Field | Nội dung |
| --- | --- |
| **Actor** | Sinh viên, nghiên cứu sinh chịu trách nhiệm hoàn thiện bài viết học thuật. |
| **Workflow** | Thu thập source → kiểm tra metadata → chọn citation style → chèn citation → kiểm tra reference list → sửa lỗi. |
| **Bottleneck** | Kiểm tra reference list: đối chiếu thủ công giữa citation trong bài, reference list và bản gốc, dễ sai khi nguồn có nhiều định dạng. |
| **Impact** | 20-30 phút/bài viết; sai citation làm chậm nộp bài và giảm chất lượng học thuật; nguồn không tồn tại có thể bị xử lý như đạo văn. |
| **Success Metric** | Thời gian: 20-30 phút → 8-10 phút. Lỗi format citation trước khi nộp: 0. Nguồn vào bài mà chưa qua đối chiếu: 0 — có DOI thì dùng CrossRef, không có DOI thì người tự mở bản gốc kiểm. |
| **Boundary** | AI không tự nộp bài, không tự thay đổi nội dung, chỉ hỗ trợ kiểm tra và gợi ý citation. AI chỉ dùng metadata do API trả về, không tự điền từ trí nhớ; tra không ra thì báo "không xác minh được". |
| **AI intervention point** | Sau khi source đã được import vào tool, trước khi hoàn thiện reference list và nộp. |
| **Mức chọn** | Workflow: Zotero/Mendeley import + AI kiểm tra metadata (CrossRef API) + AI gợi ý citation + user review. |
| **Rủi ro & người thật kiểm tra** | Risk: metadata sai khi paper không có DOI; citation không đúng style; nguy hiểm nhất là AI tự điền metadata không dẫn được nguồn. Người thật: user phải review và xác nhận trước khi nộp, không nộp nguồn nào chưa tự đối chiếu. |

## Bước 6.3 — Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú |
| --- | --- | --- |
| Actor và workflow đã rõ chưa? | Yes | 6 bước, có actor, input/output và thời gian từng bước |
| Baseline và success metric đã đo được chưa? | Not Yet | 20-30 phút là ước lượng của nhóm, chưa bấm giờ thật trên bài cụ thể |
| Có data/input đủ dùng chưa? | Yes | Bản nháp và reference list là thứ người viết đã có sẵn; CrossRef API miễn phí |
| Nếu AI sai, hậu quả có chấp nhận được không? | Yes — với điều kiện giữ boundary | AI chỉ kiểm tra nên sai thì mất thêm ít thời gian. Nếu để AI tự điền metadata thì hậu quả không chấp nhận được |
| Có người review/owner vận hành không? | Yes | Chính người viết, vì họ chịu trách nhiệm bài nộp |
| Có cách non-AI đơn giản hơn không? | Yes, nhưng chưa đủ | Zotero/Mendeley giải bước thu thập và format, không giải được bước đối chiếu |

Decision:

```text
Go với scope nhỏ.
```

Lý do:

```text
Problem rõ, workflow rõ, metric rõ. Có non-AI components (Zotero/Mendeley) gánh
phần lớn quy trình. AI nằm ở bước kiểm tra metadata và gợi ý format, không ôm
toàn bộ workflow. Human review rõ ràng.

Điểm chưa chắc duy nhất là baseline thời gian chưa bấm giờ thật — nên pilot
phải đo baseline trước, không chốt con số 20-30 phút ngay.
```

Nếu Go, pilot nhỏ nhất là:

```text
1. Chọn 2-3 tài liệu mẫu từ một bài tiểu luận/báo cáo thật, bấm giờ làm lại
   phần citation theo cách cũ để có baseline thật.
2. Chạy workflow bán thủ công: import source vào Zotero → AI kiểm tra metadata
   qua CrossRef → AI gợi ý citation format → user review.
3. Đo: thời gian so với baseline, số lỗi citation phải sửa, và số nguồn AI
   báo "không xác minh được".

Exit / rollback:
- Nếu user phải sửa hơn 50% citation trong 2 lần thử → hạ xuống template +
  Zotero/Mendeley thuần.
- Nếu AI đưa ra metadata mà không dẫn được kết quả API → dừng dùng cho bước này,
  vì rủi ro nguồn giả lớn hơn lợi ích tiết kiệm thời gian.
```

Nếu Not Yet, cần validate gì trước:

```text
Không áp dụng — nhóm chốt Go. Nhưng nếu pilot cho kết quả xấu và phải quay lại
mức Not Yet, thứ cần validate trước tiên là baseline thời gian thật (bấm giờ
trên ít nhất 5 bài) và số lỗi citation thật sự lọt qua khi nộp — hai con số này
hiện vẫn là ước lượng.
```

Nếu No-Go, nên làm gì thay AI:

```text
Không áp dụng — nhóm chốt Go. Nếu sau pilot phải chuyển sang No-Go, phương án
thay thế là Rule thuần: Zotero/Mendeley lo import và format, cộng thêm một
checklist rà tay cố định trước khi nộp (mọi citation trong bài đều có trong
reference list và ngược lại; mọi nguồn đều đã tự mở bản gốc một lần).
```
