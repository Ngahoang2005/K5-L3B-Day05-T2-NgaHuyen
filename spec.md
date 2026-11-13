# Bài nộp LAB5 — T2 Giáo dục · Nhóm NgaHuyen

**Lớp:** L3B · **Bàn / zone:** ____ · **Track:** T2 — Giáo dục (trợ lý học bài tối muộn)

| Họ và Tên | GitHub | Mã Học Viên | Việc đã làm |
|---|---|---|---|
| Nga | `Ngahoang2005` | ____ | **Người A — Kịch bản & UX khi AI sai:** §1 Lát cắt & phạm vi · §2 Kịch bản rủi ro (≥8 kịch bản, chọn 2 kịch bản đắt nhất) · §3 Khi AI sai (câu AI nói nguyên văn, HAX/PAIR, loại lỗi) · §6 Tốt là gì · chụp & đánh số ảnh prototype |
| Huyền | `duongthuyen` | ____ | **Người B — Mức tự chủ & Prototype:** §4 Mức tự chủ (4 tool, tool khó xếp nhất, thử mức trên 3 kịch bản) · §5 Prototype (`prototype/index.html`: màn học viên + màn hàng chờ TA) · lời gọi AI thật (nếu kịp) |

> Nhóm có 2 thành viên (README yêu cầu 3 — đã/ sẽ báo TA).

---

## Phân công công việc

### Nguyên tắc chia

- **Chia theo khối điểm, mỗi người là chủ khối của mình.** A giữ R1 + R2 + R3 + R6 (45đ) — *"AI nói gì khi sai"*. B giữ R4 + R5 (50đ) — *"AI được làm gì & màn hình trông ra sao"*.
- **Không sửa chung một chỗ:** A sửa trực tiếp `spec.md` §1, §2, §3, §6. B viết `drafts/s4-s5.md` và `prototype/`, cuối giờ dán §4, §5 vào `spec.md`.
- Chỉ gặp nhau ở **Phase 0 + 3 mốc sync**, còn lại làm độc lập.

### Phase 0 — làm chung (15 phút đầu) · ✅ kết quả ở mục "Kết quả làm chung (Phase 0)" và §1

Chốt 4 thứ cả hai bên đều phụ thuộc:

1. **Lát cắt + 3 việc KHÔNG làm** (gợi ý: không giải hộ / xác nhận đáp số bài đang mở · không dạy nội dung buổi chưa mở · không nhận xét năng lực học viên).
2. **2 kịch bản đắt nhất (nháp):**
   - **K1 — xin xác nhận đáp số Bài tập 3 đang mở** ("em tính trung bình 15.25, trung vị 11.5 đúng chưa ạ"). Hạn 13/11 23:59 nhưng giờ TA chỉ tới 22:00 → AI dễ xác nhận hộ hoặc `goi_y_bai_tap` quá tay.
   - **K2 — tài liệu sai:** §3.3 ghi "độ lệch chuẩn luôn nhỏ hơn phương sai" — sai khi phương sai < 1 (phương sai 0.25 → độ lệch chuẩn 0.5). AI trích như chân lý; `dang_FAQ` lan cái sai ra cả lớp.
3. **Mức tự chủ nháp cho 4 tool** — mỗi người tự xếp 5', rồi so; chỗ lệch ghi lại làm nguyên liệu "tool khó xếp nhất":
   - `tra_cuu_tai_lieu` → tự làm
   - `goi_y_bai_tap` → tự làm *chỉ bước đầu* / hay cần duyệt? (ứng viên khó xếp nhất)
   - `chuyen_TA` → tự làm, nhưng sau 22:00 phải nói rõ "TA trả lời từ 08:00"
   - `dang_FAQ` → tách "soạn nháp" (tự làm) và "đăng" (TA duyệt)
4. **Công cụ prototype:** 1 file HTML (giống `prototype-sample/`).

### Người A — Nga: Kịch bản & UX khi AI sai

| Việc | Output | Hạn |
|---|---|---|
| §1 Lát cắt, 3 việc không làm + lý do | `spec.md` §1 | phút 25 |
| §2 ≥8 kịch bản phủ ①②③④, mỗi dòng trỏ về tool / dữ liệu cụ thể. Phủ hard tests: xin giải bài 3 · xin xác nhận đáp số · §3.3 sai · "slide 12" · tự chê mình · hỏi buổi 7 p-value · hàm Excel (tài liệu không có) · hỏi đáp án bài 2 (đã hết hạn → được giải thích đầy đủ) | `spec.md` §2 + lập luận chọn 2 kịch bản đắt nhất, kịch bản suýt chọn | **phút 50 (M1)** |
| §3 Với K1, K2: câu AI nói nguyên văn · người dùng thấy gì · làm gì tiếp · ai được báo · chọn hỏi lại / trả lời kèm giới hạn / chuyển TA + phương án loại · loại lỗi (hệ thống / người dùng / ngữ cảnh) · 2–3 nguyên tắc HAX (gợi ý G2, G10, G11) · lỗi mà sửa câu chữ không cứu được | `spec.md` §3 | phút 120 |
| §6 3 tiêu chí Pass/Fail, chấm thử trên K1, K2 | `spec.md` §6 | phút 210 |
| Hỗ trợ B: chụp ảnh prototype, đánh số các chỗ | ảnh trong `prototype/` | phút 200 |

### Người B — Huyền: Mức tự chủ & Prototype

| Việc | Output | Hạn |
|---|---|---|
| §4 Mức từng tool + lý do cost-of-error (sai thì ai chịu gì · đảo được không · chờ thì mất gì) · ai duyệt / thấy gì / quá hạn thì sao · tool khó xếp nhất (Nga chọn gì, Huyền chọn gì, chốt thế nào) · thử mức trên K1, K2 + 1 ca bình thường theo 3 câu · tách `dang_FAQ` · một mức đã đổi lời hứa nào | `drafts/s4-s5.md` | **phút 125 (M2)** |
| Dựng khung prototype **từ phút 50** với placeholder câu chữ: Màn 1 học viên chat (trích §mục, nhãn độ chắc, nút "Hỏi TA", gợi ý bước 1) · Màn 2 hàng chờ TA (bonus) | `prototype/index.html` | phút 150 |
| Ráp câu chữ của A, đảm bảo thấy ≥2 mức tự chủ: tự làm có hoàn tác · cần duyệt có xác nhận · việc cấm không có nút | prototype hoàn chỉnh | **phút 200 (M3)** |
| §5 Công cụ, phần mock, bảng "số trên ảnh → nguyên tắc HAX → mức tự chủ", cách hiện khác đã nghĩ và vì sao loại | `drafts/s4-s5.md` | phút 215 |
| *(Tuỳ chọn, +3)* 1 lời gọi AI thật trả lời kèm mã mục, key để biến môi trường | log / ảnh | nếu dư giờ |

### 3 mốc sync (~5 phút mỗi lần)

1. **Phút 50 (sau M1):** A → B chốt K1, K2 để B dựng prototype đúng ca khó.
2. **Phút 120:** A → B câu chữ nguyên văn + vị trí HAX; B → A mức tự chủ đã chốt để A kiểm cột "làm gì tiếp" ở §3 cho khớp.
3. **Phút 215:** gộp `drafts/s4-s5.md` vào `spec.md`, điền mã học viên, push; kiểm repo mở được bằng cửa sổ ẩn danh. Hạn nộp **23:59 13/11/2026**.

### Demo — mỗi người một phần

- **Nga:** lát cắt (30") → 2 kịch bản đắt nhất → AI nói gì khi sai.
- **Huyền:** bấm prototype qua ca khó → một mức tự chủ và cái giá khi sai.
- **Ca lạ:** cả hai cùng trả lời. Trước demo **dạy chéo phần của nhau** — TA hỏi bất kỳ ai.

---

## Kết quả làm chung (Phase 0)

> Cả hai cùng chốt trong 15 phút đầu. Đây là **bản nháp chung** để A và B làm song song; A phát triển tiếp ở §2–§3, B ở §4–§5. Đổi gì ở đây thì báo người kia.

### 0.1 Đọc bảng tool như người thiết kế

| Tool | Đọc / thay đổi | Đảo lại được không | Ghi chú thiết kế |
|---|---|---|---|
| `tra_cuu_tai_lieu` | Chỉ đọc | — | Chỉ có tài liệu **buổi 3** (§3.1–§3.5); **không có slide đánh số**. Buổi 4–10 chỉ có tên trong đề cương |
| `goi_y_bai_tap` | Gửi nội dung cho học viên | **Không thực sự** — gợi ý quá tay thì học viên đã chép | Chỗ nguy hiểm nhất với Bài tập 3 đang mở |
| `chuyen_TA` | Tạo việc cho TA | Được | Giờ TA **08:00–22:00**; Bài 3 hạn **23:59** → sau 22:00 chuyển TA = TA trả lời sau hạn |
| `dang_FAQ` | Công khai cho cả lớp | Gỡ được, nhưng **nhiều người đã đọc** | Một câu sai nhân lên cả lớp |

**Việc người dùng sẽ đòi mà không tool nào làm được:** gia hạn nộp bài · chấm/xác nhận bài · dạy hàm Excel cụ thể (trang khoá học chỉ ghi "bảng tính", tài liệu không có hàm nào) · nói nội dung chi tiết buổi chưa mở. → AI phải nói thẳng là không làm được và chỉ đường (chuyển TA / hỏi giảng viên).

**Kiểu sai đắt nhất (một câu):** AI nói sai mà nghe như đúng, học viên tin và học sai (hoặc nộp bài chép) — không ai biết, vì lúc đó không có TA.

### 0.2 Hai kịch bản đắt nhất (nháp — A hoàn thiện lập luận ở §2)

**K1 — Xin xác nhận đáp số Bài tập 3 đang mở** · lớp ③ ngoài thẩm quyền + ④ domain
- Tin nhắn: *"22h45 rồi, em tính bài 3 ra trung bình 15.25, trung vị 11.5, đúng chưa ạ? Đúng thì em nộp luôn"*
- AI có thể sai thế nào: số của học viên **đúng** (122/8 = 15.25; (11+12)/2 = 11.5) → AI dễ nói "đúng rồi" — **đúng vì may, không vì thiết kế**, nhưng vẫn là xác nhận đáp số bài đang mở (rubric T2 #3). Hoặc gọi `goi_y_bai_tap` gửi lời giải phần (b). Sau 22:00 không còn TA → AI dễ hứa "để em báo TA kiểm tra giúp" trong khi TA trả lời sau hạn 23:59.
- Vì sao đắt: không đảo được (đã xác nhận/đã chép thì không rút lại), áp lực hạn nộp khiến học viên ép AI, và **câu trả lời trông hoàn toàn vô hại**.

**K2 — Tài liệu khoá học có câu sai (§3.3)** · lớp ① nguồn sự thật
- Tin nhắn: *"Tài liệu ghi độ lệch chuẩn luôn nhỏ hơn phương sai, vậy phương sai 0.25 thì độ lệch chuẩn bao nhiêu ạ? Em ra 0.5 mà lớn hơn, em sai ở đâu?"*
- AI có thể sai thế nào: `tra_cuu_tai_lieu` trả đúng §3.3 → AI trích nguyên văn như chân lý và bảo học viên tính sai, trong khi **tài liệu sai** (khi phương sai < 1 thì độ lệch chuẩn > phương sai; bằng nhau khi phương sai = 0 hoặc 1). Tệ hơn: `dang_FAQ` đăng câu trả lời đó cho cả lớp.
- Vì sao đắt: lỗi **âm thầm** — AI có trích nguồn nên trông rất đáng tin; học viên đúng lại bị bảo là sai (mất niềm tin vào chính mình); qua FAQ lan ra cả lớp.

**Suýt chọn (A viết lý do loại ở §2):** "slide 12 nói gì ạ" (nguồn không có — nhưng dễ chặn bằng câu "tài liệu buổi 3 không có slide đánh số") · "buổi 7 p-value là gì" (buổi chưa học — sai chỉ ở mức sửa được).

### 0.3 Mức tự chủ nháp cho 4 tool (B hoàn thiện lập luận ở §4)

| Tool | Mức nháp | Luật kèm theo | Lý do ngắn theo cost-of-error |
|---|---|---|---|
| `tra_cuu_tai_lieu` | **Tự làm** | Chỉ buổi đã mở; luôn kèm mã mục (§3.x) | Chỉ đọc, học viên tự kiểm qua mã mục; bắt chờ người thì mất luôn lý do có trợ lý lúc tối muộn |
| `goi_y_bai_tap` | **Tự làm có giới hạn** *(tool khó xếp nhất)* | Bài **đang mở**: chỉ gợi ý bước đầu, không con số cuối, không viết nhận xét hộ · Bài **đã hết hạn** (Bài 2): giải thích đầy đủ | Cấm → học viên kẹt lúc 22h không ai giúp; cần TA duyệt → sau 22:00 không ai duyệt, chờ = trễ hạn; tự làm không giới hạn → chép đáp án (K1) |
| *Xác nhận đáp số bài đang mở* | **Cấm** | Không có nút, không có tool | Không đảo được, một bước xác nhận cũng không chặn được việc đã biết đáp án |
| `chuyen_TA` | **Cần học viên bấm xác nhận** | Hiện rõ giờ TA trả lời thật (sau 22:00 → "từ 08:00 sáng mai"); AI không bao giờ nói "đã báo TA" trước khi gửi thật | Đảo được, rẻ; nhưng câu hỏi là của học viên (có thể có câu tự chê mình) → học viên quyết định gửi; một cú bấm là đủ |
| `dang_FAQ` → **tách 2 bước** | `soan_nhap_FAQ`: **tự làm** (chỉ TA thấy) · `dang_FAQ`: **TA duyệt** | Không bao giờ soạn FAQ có lời giải bài đang mở; quá hạn không ai duyệt → không đăng | Đăng sai thì cả lớp đã đọc (K2); không đăng thì chỉ mất chút tiện → chờ rẻ hơn sai |

**Lệch nhau cần ghi lại (điền khi tự xếp 5'):** Nga chọn `goi_y_bai_tap` = ____ vì ____ · Huyền chọn = ____ vì ____ · chốt: tự làm có giới hạn (như trên).

### 0.4 Công cụ prototype

Một file **HTML** tĩnh (`prototype/index.html`), dữ liệu giả, không backend — giống `prototype-sample/`. Hai màn hình: **(1)** học viên chat (ca K1 hoặc K2) · **(2)** hàng chờ TA (bonus track T2).

---

## §1. Lát cắt & phạm vi

**Lát cắt (phát sẵn, T2):** Trong **trợ lý học bài của trang khoá học (kiểu ChatGPT Study mode)**, khi **học viên** đang hỏi bài lúc tối muộn, khi không còn ai để hỏi, **AI giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng "tài liệu không có, hỏi giảng viên"**, để học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết.

| Một người dùng | Một việc | Một quyết định của AI | Một kết quả |
|---|---|---|---|
| học viên khoá "Nhập môn phân tích dữ liệu", đang học buổi 3 | hỏi bài lúc tối muộn (sau 22:00 không còn TA) | giảng kèm trích §mục · hỏi lại · gợi ý bước đầu · hay nói "tài liệu không có, hỏi giảng viên" | hiểu đúng bài, không chép đáp án, không học sai mà không biết |

**So với sản phẩm thật hôm nay:** Study mode đã hỏi ngược và gợi ý từng bước, nhưng **không có TA hay giảng viên đứng sau** và không gắn với tài liệu khoá học. Khi tích hợp vào trang khoá học, AI được thêm quyền: trích tài liệu buổi học, gửi gợi ý bài tập, chuyển TA, đăng FAQ cho cả lớp.

**Sai thì ai chịu:** học viên (học sai, hoặc chép bài mà tưởng là được giúp) · giảng viên/TA (phải gỡ hiểu sai cho cả lớp nếu lỗi lan qua FAQ). Sai theo hướng **"trả lời tự tin khi lẽ ra phải nói không chắc"** đắt hơn hướng "từ chối khi lẽ ra được giúp" — vì hướng thứ nhất âm thầm, hướng thứ hai học viên còn biết mà hỏi TA sáng hôm sau.

**3 việc tính năng KHÔNG làm:**

1. **Không đưa, không xác nhận đáp số, không viết nhận xét hộ cho bài đang mở (Bài tập 3).** Vì mục tiêu là học viên tự hiểu; đáp án đã đưa thì không rút lại được, và xác nhận "đúng rồi" cũng là đưa đáp án.
2. **Không dạy nội dung buổi chưa mở (buổi 4–10).** Vì tài liệu các buổi đó chưa có — AI chỉ có tên buổi trong đề cương, nói thêm là bịa; chỉ nói "buổi X sẽ học", tối đa một câu.
3. **Không nhận xét năng lực người học** (kể cả khi học viên tự chê "em dốt quá"). Vì AI không có căn cứ đánh giá, và một câu nhận xét lúc 23h có thể làm học viên bỏ cuộc — chỉ quay về nội dung bài.

*(Thêm, không tính vào 3 mục trên: không gia hạn nộp bài và không nói hạn nộp từ nguồn nào khác ngoài trang khoá học — không tool nào làm được.)*

**Prototype không vi phạm:** không có nút "Kiểm tra đáp án" hay "Xem lời giải" cho Bài 3; câu hỏi buổi chưa học chỉ hiện tên buổi.

## §2. Kịch bản rủi ro  (chặng 2)
- ≥8 kịch bản, mỗi lớp ①②③④ ít nhất một; mỗi kịch bản: tin người dùng · lớp · AI có thể sai thế nào · sản phẩm tốt nên làm gì · nhãn (nhẹ / sửa được / không chấp nhận được).
- Bằng chứng: cột "AI có thể sai thế nào" trỏ về một tool hoặc một dòng dữ liệu của track (hoặc chỗ dữ liệu không có).
- Quyết định: 2 kịch bản đắt nhất — vì sao đắt hơn các kịch bản còn lại; kịch bản nào suýt được chọn và vì sao không.

## §3. Khi AI sai  (chặng 3)
Với mỗi kịch bản đắt nhất:
- AI nói gì (nguyên văn) · người dùng thấy gì · làm gì tiếp · ai được báo, sau bao lâu.
- Quyết định: hỏi lại / trả lời kèm giới hạn / dừng và chuyển người — chọn cách nào, đã loại cách nào, vì sao.
- Loại lỗi (hệ thống / người dùng / ngữ cảnh) và vì sao cách nói, cách sửa đi theo loại đó.
- 2–3 nguyên tắc HAX/PAIR, mỗi cái trỏ vào một chỗ cụ thể (câu chữ hoặc chỗ trên màn hình).
- Lỗi nào sửa câu chữ không cứu được (nếu có), và thiết kế cứu nó thế nào.

## §4. Mức tự chủ  (chặng 4)
Với mỗi tool:
- Mức của nhóm (tự làm / cần người duyệt / cấm). Nếu cần người duyệt: ai duyệt · người duyệt thấy gì · quá hạn thì sao.
- Lý do theo cost-of-error: sai thì ai chịu gì · đảo lại được không · chờ người thì mất gì.
- Phương án đã cân nhắc và vì sao loại.

Thêm:
- Tool khó xếp nhất: mỗi người từng chọn gì, cái giá của mỗi phía (trỏ về kịch bản ở §2), nhóm chốt thế nào.
- Thử mức đã đặt trên 2 kịch bản đắt nhất + 1 kịch bản bình thường: cái sai có bị chặn không? còn việc nào làm khi lẽ ra phải hỏi? người dùng bình thường có phải chờ vô ích không?
- Luật thêm hoặc tool tách bước (nếu có), và vì sao.
- Một mức tự chủ đã đổi lời hứa nào với người dùng.

## §5. Prototype  (chặng 5)
- Link hoặc file · công cụ · phần nào mock · có lời gọi AI thật không.
- 1–2 ảnh có đánh số; mỗi số: thể hiện gì · nguyên tắc HAX/PAIR nào · mức tự chủ nào.
- Quyết định: cách hiện độ chắc/bằng chứng và điều khiển mức tự chủ — đã nghĩ tới cách nào khác, vì sao chọn cách này.

## §6. Tốt là gì  (chặng 6 — nhẹ, bỏ được nếu thiếu giờ)
- 3 tiêu chí Pass/Fail chấm được; thiết kế của nhóm đạt tiêu chí nào trên 2 kịch bản đắt nhất; lỗi còn lại.

## §7. Demo
- Ca lạ nhận được ở demo: prototype đã làm gì, và nhóm có đổi ý gì sau ca đó không.
