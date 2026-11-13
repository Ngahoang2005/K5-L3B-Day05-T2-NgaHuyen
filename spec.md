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

### Phase 0 — làm chung (15 phút đầu)

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

## §1. Lát cắt & phạm vi
- Lát cắt (chép từ track).
- 3 việc tính năng KHÔNG làm, mỗi việc một câu vì sao.

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
