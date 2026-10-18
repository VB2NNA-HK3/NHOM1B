# THƯ VIỆN CÂU LỆNH — DỰ ÁN HỘP XANH

**Nhóm:** *[[ THAY — tên nhóm ]]* · **Học phần:** AI ứng dụng (06050)
**Viện Công nghệ tiên tiến và Trí tuệ nhân tạo — Trường Đại học Hùng Vương TP. Hồ Chí Minh**

> ⚠️ **Đây là tệp mẫu.** Nhóm thay toàn bộ bằng câu lệnh thật của mình. Giữ nguyên cách trình bày:
> mỗi câu lệnh phải ghi **đúng tên kỹ thuật theo chuẩn**, nêu **lý do chọn**, và **kết quả thu được**.
> Ghi các câu lệnh đã dùng để tạo ảnh, video và nội dung trên trang web. Rubric đồ án chấm ở tiêu chí *Năng lực kỹ thuật câu lệnh* (2,5 điểm): câu lệnh ảnh đủ tám lớp, video đủ bảy thành phần, có dấu vết tinh chỉnh.

---

## Cách đọc bảng dưới

| Cột | Ý nghĩa |
|---|---|
| **Kỹ thuật** | Tên chuẩn, đúng như trong đề giữa kỳ và đề chứng chỉ |
| **Vì sao chọn** | Một câu. Không viết "vì nó hay" |
| **Kết quả** | Nhận xét thật, kể cả khi kết quả tệ — lần thất bại có ghi chép vẫn được tính điểm |

---

## 01 · Zero-shot

**Kỹ thuật:** Zero-shot prompting
**Dùng ở:** Bước đầu tìm ý tưởng, Tuần 1

```
Liệt kê 10 vấn đề môi trường có thật trong khuôn viên một trường đại học
tại TP. Hồ Chí Minh mà sinh viên có thể tự giải quyết bằng một mô hình
kinh doanh nhỏ, vốn dưới 20 triệu đồng.
```

**Vì sao chọn:** Giai đoạn mở rộng ý tưởng, chưa cần ràng buộc chặt.
**Kết quả:** Ra 10 ý, nhóm chọn được 3 ý khả thi. Bốn ý bị loại vì không làm được ở quy mô sinh viên.

---

## 02 · Role prompting kèm khung R-T-C-F-E

**Kỹ thuật:** Role prompting + khung Role–Task–Context–Format–Example
**Dùng ở:** Viết phần mô tả ý tưởng trên trang chủ, Tuần 2

```
Bạn là cố vấn khởi nghiệp cho sinh viên năm nhất.
Nhiệm vụ: viết đoạn giới thiệu 60 từ cho dự án hộp đựng thức ăn dùng
nhiều lần tại căng tin trường đại học.
Bối cảnh: người đọc là sinh viên bận, lướt điện thoại, không quan tâm
thuật ngữ môi trường.
Định dạng: một đoạn duy nhất, câu ngắn, không dùng từ chuyên môn.
Ví dụ giọng điệu: "Mượn khi ăn, trả khi về. Vậy thôi."
```

**Vì sao chọn:** Bản viết trước đó quá trang trọng, sinh viên đọc không vào.
**Kết quả:** Dùng được ngay sau một lần chỉnh. Đây là bản đang nằm trên trang chủ.

---

## 03 · Few-shot

**Kỹ thuật:** Few-shot prompting
**Dùng ở:** Sinh khẩu hiệu đồng bộ giọng điệu, Tuần 2

```
Viết 5 khẩu hiệu cho dự án hộp ăn dùng nhiều lần, theo đúng nhịp của
ba ví dụ sau:
- "Mượn khi ăn, trả khi về."
- "Một chiếc hộp, năm trăm bữa cơm."
- "Rác không sinh ra, tiền không mất đi."
```

**Vì sao chọn:** Cần giữ nhịp ba tiếng–ba tiếng, mô tả bằng lời không ra được.
**Kết quả:** 5 khẩu hiệu đúng nhịp, chọn được 2 dùng cho poster.

---

## 04 · Chain-of-Thought

**Kỹ thuật:** Chain-of-Thought
**Dùng ở:** Tính điểm hoà vốn, Tuần 4

```
Hộp inox giá 85.000đ/chiếc, quay vòng được 500 lần. Chi phí rửa 1.500đ/lượt.
Căng tin đang tốn 1.200đ cho mỗi hộp xốp dùng một lần.
Hãy giải thích từng bước để tính xem sau bao nhiêu lượt sử dụng thì
mô hình hộp inox rẻ hơn hộp xốp.
```

**Vì sao chọn:** Bài toán nhiều bước, cần thấy được lập luận để tự kiểm tra.
**Kết quả:** AI bày ra từng bước nên nhóm **phát hiện nó quên chi phí hao hụt do mất hộp**. Nhóm tự bổ sung, ra con số khác.

---

## 05 · Prompt chaining

**Kỹ thuật:** Prompt chaining
**Dùng ở:** Dựng kịch bản video 90 giây, Tuần 3

```
Bước 1 — Liệt kê 5 cảnh cần có trong video 90 giây giới thiệu dự án.
Bước 2 — Với danh sách ở bước 1, viết lời thuyết minh cho từng cảnh,
         tổng không quá 160 từ.
Bước 3 — Với lời thuyết minh ở bước 2, viết mô tả hình ảnh cho từng
         cảnh để đưa vào công cụ sinh video.
```

**Vì sao chọn:** Làm một lượt thì AI ra kịch bản chung chung, không khớp thời lượng.
**Kết quả:** Ba bước tách ra cho kết quả bám đúng 90 giây. Đây là quy trình nhóm dùng chính thức.

---

## 06 · Câu lệnh sinh ảnh có mô tả đầy đủ

**Kỹ thuật:** Image prompting — chủ thể · bối cảnh · ánh sáng · góc máy · phong cách
**Dùng ở:** Poster A3, Tuần 3

```
Một chiếc hộp đựng cơm bằng inox sáng bóng đặt trên bàn gỗ căng tin,
phía sau là sinh viên đang xếp hàng mờ nhoè, ánh sáng trưa tự nhiên
từ cửa sổ bên trái, góc máy ngang tầm mắt, phong cách ảnh chụp thực tế,
tông màu xanh lá và trắng, khung dọc tỷ lệ 3:4.
```

**Vì sao chọn:** Câu lệnh đầu chỉ ghi "hộp đựng cơm thân thiện môi trường" nên ra ảnh minh hoạ vô hồn.
**Kết quả:** Đủ sáu yếu tố thì ra ảnh dùng được. Chọn 1 trong 4 ảnh sinh ra.

---

## 07 · Câu lệnh ngược — AI hỏi lại nhóm

**Kỹ thuật:** Reverse prompting, dạng AI đặt câu hỏi cho người dùng
**Dùng ở:** Làm rõ mô hình vận hành, Tuần 2

```
Tôi muốn xây dịch vụ cho mượn hộp ăn tại căng tin trường đại học.
Trước khi tư vấn, hãy hỏi tôi 7 câu hỏi mà bạn thấy cần thiết nhất
để hiểu đúng bài toán. Chỉ hỏi, chưa trả lời.
```

**Vì sao chọn:** Nhóm chưa nghĩ tới nhiều tình huống vận hành.
**Kết quả:** Câu hỏi *"ai chịu trách nhiệm khi sinh viên không trả hộp?"* làm nhóm phải thiết kế lại cơ chế đặt cọc.

---

## 08 · Câu lệnh ngược — suy ngược từ kết quả

**Kỹ thuật:** Reverse prompting, dạng suy câu lệnh từ đầu ra mẫu
**Dùng ở:** Nhân bản phong cách poster, Tuần 3

```
Đây là mô tả một poster nhóm tôi rất ưng ý: [dán mô tả poster đã chọn].
Hãy suy ra câu lệnh đầy đủ có thể đã tạo ra poster này, rồi dùng chính
câu lệnh đó viết lại cho chủ đề "thùng thu hồi hộp đặt tại sảnh B".
```

**Vì sao chọn:** Cần 4 ảnh cùng phong cách mà không phải mô tả lại từ đầu mỗi lần.
**Kết quả:** Bốn ảnh đồng bộ phong cách. Tiết kiệm được khoảng hai giờ.

---

## 09 · Generate Knowledge

**Kỹ thuật:** Generate Knowledge prompting
**Dùng ở:** Chuẩn bị phần pháp lý, Tuần 6

```
Trước khi trả lời, hãy nêu những quy định pháp luật Việt Nam liên quan
đến an toàn thực phẩm với dụng cụ chứa đựng thức ăn dùng nhiều lần.
Sau đó mới cho biết dự án của tôi cần chuẩn bị giấy tờ gì.
```

**Vì sao chọn:** Hỏi thẳng thì AI trả lời chung chung và có dấu hiệu bịa.
**Kết quả:** Có danh sách để tra cứu, nhưng **nhóm vẫn phải tự kiểm chứng từng mục** — xem bảng xác minh. Một văn bản AI nêu ra không tồn tại.

---

## 10 · Câu lệnh xác minh

**Kỹ thuật:** Verification prompting — khoá nguồn, buộc dẫn vị trí
**Dùng ở:** Rà soát toàn trang trước khi nộp, Tuần 5

```
Đây là toàn bộ nội dung trang web của nhóm tôi: [dán nội dung].
Chỉ dùng thông tin có trong văn bản trên, liệt kê mọi khẳng định mang
tính sự kiện hoặc số liệu, kèm vị trí xuất hiện. Không bổ sung kiến
thức ngoài. Đánh dấu những khẳng định không nêu nguồn.
```

**Vì sao chọn:** Cần tìm bằng hết các chỗ phải kiểm chứng, tránh sót.
**Kết quả:** Tìm ra 11 khẳng định, trong đó 3 chỗ không có nguồn. Một chỗ bị gỡ khỏi trang.

---

## Tổng hợp kỹ thuật đã dùng

| Kỹ thuật | Số câu lệnh |
|---|---|
| Zero-shot | 1 |
| Role prompting + R-T-C-F-E | 1 |
| Few-shot | 1 |
| Chain-of-Thought | 1 |
| Prompt chaining | 1 |
| Image prompting | 1 |
| Reverse prompting | 2 |
| Generate Knowledge | 1 |
| Verification prompting | 1 |
| **Tổng** | **10 câu lệnh · 9 kỹ thuật** |

---

## Ba điều nhóm rút ra

1. **Câu lệnh dài không bằng câu lệnh đủ yếu tố.** Câu lệnh sinh ảnh số 06 không dài hơn bản đầu bao nhiêu, nhưng đủ sáu yếu tố nên kết quả khác hẳn.
2. **Chain-of-Thought đáng giá vì nó để lộ chỗ sai.** Nếu AI chỉ trả về con số cuối, nhóm đã không phát hiện nó bỏ sót chi phí hao hụt.
3. **AI vẫn bịa ở phần pháp lý dù đã dùng Generate Knowledge.** Không có kỹ thuật câu lệnh nào thay được việc tự đi tra văn bản gốc.
