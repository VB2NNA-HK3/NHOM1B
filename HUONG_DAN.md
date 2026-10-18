# 🚀 HƯỚNG DẪN TRANG WEB ĐỒ ÁN

## Học phần AI ứng dụng (06050)

**Viện Công nghệ tiên tiến và Trí tuệ nhân tạo — Trường Đại học Hùng Vương TP. Hồ Chí Minh**

Giáo viên hướng dẫn: **TS. Nguyễn Quốc Trình**

---

## Cách dùng thư mục này

Thư mục `demo_web_pro` là **một trang web hoàn chỉnh, chạy được ngay**. Nhóm dùng nó theo hai giai đoạn:

| Giai đoạn | Khi nào | Làm gì |
|---|---|---|
| **1 · Tập triển khai** | Buổi 1 | Đăng **nguyên bản mẫu**, chưa sửa một chữ nào. Mục đích là tập cho quen cách đưa một trang web lên mạng, và để nhóm có sẵn một địa chỉ |
| **2 · Hoàn thiện dự án và nộp** | Buổi 2 → hạn nộp | Nhóm **tự làm trang web cho dự án của mình**, đăng đè lên địa chỉ đã có, rồi nộp tệp zip |

> 🔑 **Một địa chỉ duy nhất suốt học kỳ.** Giai đoạn 1 nhóm tạo ra một địa chỉ web. Từ đó về sau **cập nhật đè lên chính địa chỉ đó**, không nên tạo trang mới: tạo mới mỗi lần sửa thì vừa tốn hạn mức, vừa làm địa chỉ nộp bài thay đổi liên tục.

**Hộp Xanh là ví dụ minh hoạ, không phải đề bài.** Nhóm làm chủ đề của riêng mình (ví dụ: cà phê tái chế, app gia sư, nông sản sạch, bất cứ gì).

---

## Trang mẫu có sẵn những gì

Bốn mục mà đồ án cuối kỳ yêu cầu, đã dựng sẵn đúng thứ tự:

| # | Mục | Yêu cầu tối thiểu | Điền sau buổi |
|---|---|---|---|
| **1** | Ý tưởng khởi nghiệp | Vấn đề · giải pháp · khách hàng mục tiêu. Khoảng **300 từ, viết bằng lời của nhóm** | Buổi 1–2 |
| **2** | Thông điệp và bộ nhận diện | Thông điệp chính · ảnh chủ đề · poster hoặc infographic. **Mỗi ảnh có alt-text** | Buổi 3 · TH 4 |
| **3** | Video minh họa 60–90 giây | Lời dẫn và phụ đề tiếng Việt · ít nhất hai thao tác video · có nhãn AI | Buổi 3 |
| **4** | Thông tin nhóm | Thành viên, phân công, giảng viên hướng dẫn | Trước khi nộp |

Ngoài bốn mục trên còn có **Câu hỏi thường gặp** và **nhãn nội dung AI ở chân trang**.

**Kiểm tra trước khi làm gì khác:** mở thư mục, bấm đúp vào tệp `index.html`. Trang phải hiện ra ngay trong trình duyệt. Hiện được là trang đã sẵn sàng đăng.

### Trang có những hiệu ứng gì

Ba **sân khấu ghim** — trang đứng yên còn ảnh chuyển động theo cuộn:

| # | Hiệu ứng | Ở đâu |
|---|---|---|
| **1** | Ảnh nền trôi chậm hơn chữ *(thị sai)*, chữ mờ dần khi cuộn | Đầu trang |
| **2** | Ảnh mở dần từ khung nhỏ ra tràn màn hình | Mục 1 — Ý tưởng |
| **3** | Ảnh hiện ra qua vòng tròn lớn dần, chữ đè lên tự đảo màu | Mục 3 — Video |

Cùng với đó, mỗi từ trong tiêu đề, mỗi dòng bảng, mỗi thẻ đều có độ trễ riêng khi hiện ra.

**Người nhạy cảm với chuyển động vẫn đọc được.** Ai bật *giảm chuyển động* trong hệ điều hành sẽ thấy trang tĩnh hoàn toàn, nội dung đầy đủ. Đây là một yêu cầu tiếp cận, trang nào cũng nên có.

---

# GIAI ĐOẠN 1 · TẬP TRIỂN KHAI *(Buổi 1)*

Mục tiêu buổi đầu rất hẹp: **đưa được bản mẫu lên mạng, chưa sửa gì cả.** Ai cũng làm được trong 10 phút, kể cả người chưa từng động vào HTML.

Lý do làm sớm: nếu đến tuần cuối mới đăng lần đầu, mọi lỗi vặt — sai thư mục, tài khoản chưa xác nhận, ảnh không lên — sẽ dồn vào đúng lúc không còn thời gian sửa.

## Chọn nền tảng: Netlify hay GitHub Pages

Đề cương cho phép cả hai. Trang chạy giống hệt nhau, chỉ khác cách đưa lên.

| | **Netlify** | **GitHub Pages** |
|---|---|---|
| Cách đưa lên | **Kéo thả thư mục** vào trình duyệt | Tải tệp lên kho lưu trữ |
| Thời gian lần đầu | ~5 phút | ~10 phút |
| Cần biết Git | Không | Không (dùng giao diện web) |
| Số lần đăng lại | **Giới hạn** — xem mục tiết kiệm bên dưới | Không giới hạn thực tế |
| Sửa trực tiếp trên mạng | Không — phải sửa ở máy rồi đăng lại | **Có** — sửa thẳng trong trình duyệt |
| Địa chỉ | `ten-nhom.netlify.app` | `taikhoan.github.io/ten-kho` |
| Đăng ký | Email là xong | Email là xong |

> 💡 **Nhóm chưa từng làm web thì chọn Netlify** — kéo thả là xong, ít chỗ sai nhất.
> **Nhóm biết mình sẽ sửa nhiều thì chọn GitHub Pages** — đăng lại bao nhiêu lần cũng được, và kho lưu trữ chính là thư mục `source_code/` lúc nộp.

Chọn **một** trong hai. Không cần làm cả hai.

---

## CÁCH A · NETLIFY

### Bước 1 · Tạo tài khoản

Vào **<https://app.netlify.com/signup>** → chọn **Sign up with Email** → nhập email và mật khẩu → mở hộp thư xác nhận.

**Mỗi nhóm một tài khoản riêng.** Đây là quy định ở Mục 5.5 đề cương.

### Bước 2 · Vào chỗ đăng trang

Sau khi đăng nhập, bấm **Add new site** → chọn **Deploy manually**.

Màn hình hiện một khung lớn viền đứt, đại ý *"kéo thư mục vào đây"*.

### Bước 3 · Kéo thả

Mở thư mục `demo_web_pro` trên máy. **Kéo nguyên cả thư mục** thả vào khung viền đứt.

> ⚠️ **Kéo cả thư mục, đừng mở thư mục ra rồi kéo từng tệp.** Đây là lỗi phổ biến nhất. Kéo từng tệp thì thư mục `imgs/` không lên theo, trang hiện ra nhưng **mất hết hình**.

### Bước 4 · Đợi và lấy địa chỉ

Khoảng 20–40 giây. Netlify hiện một địa chỉ ngẫu nhiên kiểu:

```
https://zesty-pika-a1b2c3.netlify.app
```

Bấm vào xem trang đã chạy chưa.

### Bước 5 · Đổi địa chỉ cho phù hợp

Vào **Site configuration** → **Change site name** → đặt theo mẫu:

```
ai06050-nhom01-tenduan
```

Địa chỉ trở thành `https://ai06050-nhom01-tenduan.netlify.app`. **Đặt theo tên dự án của nhóm, không phải "hopxanh".** Đây là địa chỉ nhóm dùng suốt học kỳ và ghi vào `Readme.md` khi nộp.

### Bước 6 · Kiểm tra bằng cửa sổ ẩn danh

Ctrl + Shift + N (Chrome, Edge) hoặc Ctrl + Shift + P (Firefox), dán địa chỉ vào. Xem được là xong giai đoạn 1.

### Đăng lại sau khi sửa nội dung

Vào site đã tạo → thẻ **Deploys** → kéo thả lại **cả thư mục** vào khung viền đứt. Bản cũ bị thay, **địa chỉ giữ nguyên**.

> ⚠️ **Đừng bấm "Add new site" lần thứ hai.** Mỗi lần bấm là một trang mới, một địa chỉ mới, và tốn thêm hạn mức. Cập nhật thì vào **Deploys** của site cũ.

### ⚠️ Quy tắc tiết kiệm của Netlify

Gói miễn phí giới hạn **khoảng 20 lần đăng mỗi tháng**. Đề cương quy định nhóm đăng **tối đa 3 lần mỗi tuần** (Mục 5.5).

Cách tiêu hết hạn mức trong một buổi chiều: sửa một chữ → đăng → xem → sửa tiếp → đăng. Cách làm đúng:

1. Sửa trang ở máy.
2. Bấm đúp mở tệp xem thử — **không tốn gì cả**.
3. Thu gọn cửa sổ trình duyệt lại cỡ điện thoại, xem lại.
4. Ưng rồi mới đăng.

*(Con số hạn mức do Netlify quy định và có thể thay đổi. Nếu tài khoản hiển thị khác, theo con số Netlify hiển thị.)*

---

## CÁCH B · GITHUB PAGES

Không cần cài phần mềm, không cần biết dòng lệnh. Làm hết bằng trình duyệt.

### Bước 1 · Tạo tài khoản GitHub

Vào **<https://github.com/signup>** → nhập email, mật khẩu, tên tài khoản → xác nhận qua hộp thư.

Tên tài khoản sẽ nằm trong địa chỉ trang, nên đặt gọn và không dấu: `nhom01ai06050` chứ đừng `banhmithapcam2007`.

### Bước 2 · Tạo kho lưu trữ

Bấm dấu **+** góc trên bên phải → **New repository**.

| Ô | Điền gì |
|---|---|
| **Repository name** | `ai06050-nhom01` *(không dấu, không khoảng trắng)* |
| **Public / Private** | Chọn **Public** — bắt buộc, gói miễn phí chỉ đăng được trang từ kho công khai |
| **Add a README file** | **Bỏ trống** |

Bấm **Create repository**.

### Bước 3 · Tải tệp lên

Trong kho vừa tạo, bấm **uploading an existing file** *(hoặc **Add file** → **Upload files**)*.

Mở thư mục `demo_web_pro`, **vào bên trong**, chọn hết *(Ctrl + A)* rồi kéo thả vào khung tải lên.

> ⚠️ **Chỗ này ngược với Netlify.** GitHub cần `index.html` nằm ngay gốc kho, nên phải kéo **nội dung bên trong** thư mục, không kéo cả thư mục. Kéo cả thư mục thì đường dẫn thành `demo_web_pro/index.html` và trang sẽ không hiện.
>
> Sau khi kéo xong, kiểm tra danh sách tệp hiện trên màn hình: phải thấy `index.html`, `imgs`, `docs`, `HUONG_DAN.md`. Thấy một mục tên `demo_web_pro` là sai — xoá đi làm lại.

Kéo xong, kéo xuống cuối trang, bấm **Commit changes**.

### Bước 4 · Bật GitHub Pages

Trong kho, bấm thẻ **Settings** *(ở thanh ngang trên cùng)* → cột trái chọn **Pages**.

Ở mục **Build and deployment**:

| Ô | Chọn |
|---|---|
| **Source** | `Deploy from a branch` |
| **Branch** | `main` · thư mục `/ (root)` |

Bấm **Save**.

### Bước 5 · Đợi và lấy địa chỉ

Khoảng 1–2 phút *(lần đầu có thể tới 5 phút)*. Tải lại trang Settings → Pages, địa chỉ hiện ở đầu trang:

```
https://nhom01ai06050.github.io/ai06050-nhom01/
```

**Đây là địa chỉ nhóm dùng suốt học kỳ và ghi vào `Readme.md` khi nộp.**

> Nếu bấm vào mà hiện **404**, đợi thêm 2 phút rồi tải lại. GitHub cần thời gian dựng trang lần đầu.

### Bước 6 · Kiểm tra bằng cửa sổ ẩn danh

Giống Netlify: Ctrl + Shift + N, dán địa chỉ, xem được là xong giai đoạn 1.

### Đăng lại sau khi sửa nội dung

Hai cách, dùng cách nào cũng được:

- **Sửa thẳng trên mạng:** vào kho → bấm vào tệp → biểu tượng **bút chì** → sửa → **Commit changes**. Tiện cho những sửa nhỏ.
- **Tải tệp mới đè lên:** **Add file** → **Upload files** → kéo tệp đã sửa ở máy vào → **Commit changes**. Tiện khi sửa nhiều, hoặc thêm ảnh.

Trang tự cập nhật sau 1–2 phút. **Không giới hạn số lần.** Vẫn dùng **cùng một kho** từ đầu đến cuối học kỳ.

### Mẹo riêng của GitHub

- Kho lưu trữ này chính là thư mục `source_code/` khi nộp — bấm **Code → Download ZIP** là có ngay bản đầy đủ.
- Lịch sử chỉnh sửa (**Commits**) cho thấy nhóm làm việc trong bao lâu, ai sửa gì. Giảng viên không chấm phần này, nhưng nó có ích khi nhóm cần đối chiếu phân công.

---

# GIAI ĐOẠN 2 · HOÀN THIỆN DỰ ÁN VÀ NỘP

Từ đây là phần được chấm. Nhóm **tự làm trang web cho dự án của mình**, rồi đăng đè lên chính địa chỉ đã tạo ở Buổi 1.

Làm cách nào là tuỳ nhóm:

- **Thay nội dung trong bản mẫu** — nhanh nhất, khung và hiệu ứng đã có sẵn.
- **Dựng trang hoàn toàn mới** — tự viết, hoặc nhờ AI sinh mã rồi nhóm đọc lại và chịu trách nhiệm về thứ mình nộp.

Đề cương không bắt phải dùng bản mẫu. Chỉ bắt trang **đạt đủ yêu cầu dưới đây**.

> 💡 Làm dần qua các buổi, đừng dồn vào tuần cuối. Mỗi buổi xong một mục là vừa sức.

## Trang phải đạt những gì

**Đủ bốn mục** — xem lại bảng ở phần *"Trang mẫu có sẵn những gì"* phía trên.

Và toàn bộ quy định kỹ thuật ở **Mục 5.5 đề cương**:

| Hạng mục | Quy định |
|---|---|
| Nền tảng | **Netlify** hoặc **GitHub Pages**, gói miễn phí. **Mỗi nhóm một tài khoản riêng** |
| Video | Tải lên YouTube ở chế độ **không công khai** rồi nhúng vào trang |
| Hình ảnh | Để trong thư mục `imgs/`; **mỗi ảnh bắt buộc có thuộc tính `alt`** |
| Số lần đăng | Netlify tối đa **3 lần mỗi tuần**; GitHub Pages không giới hạn |
| Dữ liệu cá nhân | **Không** đặt biểu mẫu thu thập thông tin cá nhân trên trang |

Thêm hai thứ nên có, vì rubric có chấm mà trang tự dựng hay thiếu:

- **Đọc được trên điện thoại** — chữ không tràn, không phải phóng to mới đọc nổi.
- **Tôn trọng tuỳ chọn *giảm chuyển động*** của hệ điều hành — ai bật thì trang hiện tĩnh, vẫn đọc đủ nội dung.

## Nhúng video YouTube

Tải video lên YouTube ở chế độ **không công khai** (Unlisted). Vào video → **Chia sẻ** → **Nhúng** → chép đoạn mã rồi dán vào trang ở Mục 3.

**Đừng tải tệp video thẳng lên Netlify hay GitHub.** Video 60–90 giây nặng vài chục đến vài trăm MB: trên Netlify ngốn hết tín dụng, trên GitHub vượt giới hạn kho. Cả hai trường hợp trang tải rất chậm.

## Lấy ảnh ở đâu cho hợp pháp

Ba ảnh trong bản mẫu lấy từ **Unsplash** — miễn phí, dùng được cả cho mục đích thương mại, không bắt buộc ghi công nhưng nên ghi.

Nguồn miễn phí khác: **Pexels**, **Pixabay**.

**Đừng lấy ảnh từ Google Images.** Phần lớn có bản quyền, và đây đúng là lỗi rubric trừ điểm — *"không dùng logo, hình ảnh, giọng nói người khác khi chưa được phép"*, trừ thẳng **2,0 điểm**.

Ảnh nhóm tự chụp hoặc do AI tạo thì tốt hơn cả — nhưng ảnh AI **phải gắn nhãn**, theo Luật Trí tuệ nhân tạo 2025.

> Nếu nhóm dùng lại bản mẫu và đã thay hết ảnh bằng ảnh của mình, nhớ sửa luôn dòng *"Ảnh: Unsplash"* ở chân trang cho đúng sự thật.

**Nén ảnh trước khi đưa lên.** Qua <https://squoosh.app>, mỗi tấm xuống dưới 400 KB — gần như không mất chất lượng nhìn thấy được, mà trang nhẹ hẳn và tiết kiệm hạn mức.

## Xem thử rồi đăng lại

Sửa xong, **bấm đúp `index.html` trên máy** để xem — không tốn hạn mức, không cần mạng *(trừ phông chữ)*. Thu gọn cửa sổ lại cỡ điện thoại để xem thử luôn.

Ưng rồi mới đăng lại, theo đúng cách đã làm ở Giai đoạn 1:

- **Netlify:** vào site cũ → thẻ **Deploys** → kéo thả lại cả thư mục.
- **GitHub:** vào kho cũ → sửa thẳng, hoặc **Add file → Upload files** đè lên.

Nhớ: **cùng một site, cùng một kho, cùng một địa chỉ** từ đầu đến cuối học kỳ.

## Nộp bài

Nộp **một tệp zip** trên LMS, đặt tên `DA_<MSSV trưởng nhóm>_<MSSV các thành viên>.zip`:

```
DA_<...>.zip
├── Readme.md        ← đường dẫn trang web, tên nhóm, thành viên, MSSV, phân công
├── source_code/     ← toàn bộ thư mục trang web đã đăng
└── docs/            ← kịch bản video và các câu lệnh đã dùng để tạo ảnh, video
```

Thư mục `docs/` trong bản mẫu đã có sẵn các tệp khung để nhóm điền:

| Tệp | Dùng làm gì |
|---|---|
| `docs/kich-ban-video.md` | Bảng phân cảnh, nguồn tư liệu, câu lệnh đã dùng cho video |
| `docs/thu-vien-cau-lenh.md` | Các câu lệnh đã dùng để tạo ảnh và nội dung |
| `docs/chinh-sach-ai.md` | *Không bắt buộc.* Giữ nếu nhóm muốn, bỏ cũng được |

> **Câu lệnh được chấm riêng 2,5 điểm.** Rubric đòi câu lệnh **có cấu trúc** — ảnh đủ tám lớp, video đủ bảy thành phần — và **cho thấy đã tinh chỉnh qua nhiều lần**. Chép mỗi câu lệnh cuối cùng vào là mất điểm; chép cả các phiên bản nháp mới đủ.

**Hạn nộp:** 3 tuần sau Buổi 6. Trang web phải truy cập được **đến hết tuần thứ 18** — đừng xoá tài khoản sau khi nộp.

## Danh mục kiểm trước khi nộp

**Nội dung**

- [ ] Đủ **bốn mục**: Ý tưởng · Nhận diện · Video · Nhóm
- [ ] Mục 1 khoảng **300 từ**, viết bằng lời của nhóm
- [ ] **Mỗi ảnh** trên trang đều có thuộc tính `alt`
- [ ] Trang mang tên và nội dung dự án của nhóm — **không còn sót chữ nào của bản mẫu Hộp Xanh**

**Video**

- [ ] Dài **60–90 giây**, nhúng vào trang và chạy được
- [ ] Có lời dẫn và phụ đề tiếng Việt, đã soát tên riêng và số liệu
- [ ] Dùng ít nhất **hai thao tác video**
- [ ] Có dòng *"Nội dung có sử dụng AI tạo sinh"*

**Pháp lý và đạo đức**

- [ ] Nhãn AI ở chân trang ghi **đúng** những khâu nhóm thực sự dùng AI
- [ ] Mọi ảnh, nhạc, video đều có quyền sử dụng; dòng ghi nguồn ảnh đúng sự thật
- [ ] Không có logo, hình ảnh, giọng nói người khác khi chưa được phép
- [ ] **Không có biểu mẫu thu thập thông tin cá nhân** trên trang
- [ ] Số liệu trong Mục 1 kiểm chứng được, không có tài liệu tham khảo bịa

**Kỹ thuật**

- [ ] Mở bằng **cửa sổ ẩn danh** — trang và video đều xem được
- [ ] Mở trên điện thoại: chữ không tràn, cuộn không giật
- [ ] Bật *giảm chuyển động* trong hệ điều hành rồi mở lại — trang vẫn đọc đủ nội dung
- [ ] Tệp zip đúng cấu trúc; `Readme.md` có đường dẫn trang và bảng phân công

---

## Lỗi hay gặp

| Hiện tượng | Nguyên nhân | Cách sửa |
|---|---|---|
| **Trang hiện nhưng mất hết ảnh** | Netlify: kéo nhầm từng tệp thay vì cả thư mục | Kéo lại **nguyên cả thư mục** |
| **Trang trắng, hoặc hiện danh sách tệp** | GitHub: kéo cả thư mục nên `index.html` không ở gốc kho | Xoá hết, kéo lại **nội dung bên trong** thư mục |
| **GitHub báo 404 sau khi bật Pages** | Chưa dựng xong | Đợi 2–5 phút rồi tải lại. Vẫn 404 thì kiểm tra kho có đúng **Public** không |
| **Sửa xong mà trang trên mạng không đổi** | Quên đăng lại, hoặc trình duyệt giữ bản cũ | Đăng lại; rồi tải lại trang bằng **Ctrl + F5** |
| **Nhóm có hai, ba địa chỉ khác nhau** | Bấm "Add new site" mỗi lần cập nhật | Chọn lấy một site, xoá các site thừa, từ nay chỉ cập nhật qua **Deploys** |
| **Ảnh hiện trên máy nhưng mất trên mạng** | Tên tệp viết hoa/thường khác nhau — máy chủ phân biệt, Windows thì không | Mở thẳng `.../imgs/ten-anh.jpg` trên trình duyệt. Báo 404 thì sửa tên trong trang cho **khớp từng chữ** với tên tệp thật |
| **Video không chạy khi người khác mở** | Để chế độ Riêng tư thay vì Không công khai | Đổi sang **Unlisted**, kiểm lại bằng cửa sổ ẩn danh |
| **Trang tải chậm, cuộn giật trên máy yếu** | Ảnh quá nặng | Nén ảnh qua <https://squoosh.app> xuống dưới 400 KB mỗi tấm |
| **Netlify báo hết tín dụng** | Đăng lại quá nhiều lần | Xem thử bằng cách mở tệp trên máy; hoặc chuyển sang GitHub Pages |

**Cách kiểm tra nhanh một tệp có lên máy chủ hay không:** mở thẳng đường dẫn tới tệp đó trên trình duyệt, ví dụ `https://ten-nhom.netlify.app/imgs/hero.jpg`. Ảnh hiện ra là tệp đã lên. Báo *Page not found* là chưa lên.
