# BÀI LÀM PHA 2 (ĐỀ LUYỆN TẬP CHỦ ĐỀ CHẠY AFFILIATE)

- **Họ tên:**Nguyễn Hải Anh
- **Lớp:**CNTT3
- **Link repository Pha2:**https://github.com/haianhvotam08-creator/Luyen_tap_Affiliate
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đăng ký gói Affiliate ra JSON

**KET QUA AI**

```text
[
  {
    "ma_goi": "TT",
    "ngay_bat_dau": "2026-12-20",
    "creator_chinh": 2,
    "thuc_tap_sinh": 1,
    "hang_tai_khoan": "thuong",
    "ghi_chu": null
  },
  {
    "ma_goi": "SP",
    "ngay_bat_dau": "2027-01-08",
    "creator_chinh": 3,
    "thuc_tap_sinh": 0,
    "hang_tai_khoan": "thuong",
    "ghi_chu": "bạn đang bó bột chân cần ngồi bàn gần cửa ra vào"
  },
  {
    "ma_goi": "PRO",
    "ngay_bat_dau": null,
    "creator_chinh": 4,
    "thuc_tap_sinh": 0,
    "hang_tai_khoan": "vip",
    "ghi_chu": "cần mượn thêm đèn trợ sáng và phông xanh để quay mẫu"
  }
]
```

**Link trò chuyện:**https://share.gemini.google/qRBWYgQtvELT

## 4.3. Báo giá gói Affiliate bằng Chain-of-Thought

**KET QUA AI**

```text
Dưới góc độ kế toán, tôi xin lập bảng kê chi tiết và tính toán báo giá cho chiến dịch của team KOC theo đúng bảng giá và quy tắc hiện hành:

* **Tiền Creator chính:** Team đăng ký gói TT (1.500.000 đồng/Creator chính) với 4 Creator chính.

$$\text{Tiền Creator chính} = 4 \times 1.500.000 = 6.000.000 \text{ đồng}$$


* **Tiền thực tập sinh:** Có 2 thực tập sinh (16 tuổi và 17 tuổi, đều nằm trong độ tuổi từ 15 đến dưới 18 tuổi), mỗi người tính bằng 60% giá Creator chính. Bé 7 tuổi dưới 15 tuổi đi cùng ngồi khu chờ được miễn phí (0 đồng).

$$\text{Giá 1 thực tập sinh} = 1.500.000 \times 60\% = 900.000 \text{ đồng}$$


$$\text{Tiền thực tập sinh} = 2 \times 900.000 = 1.800.000 \text{ đồng}$$


* **Tổng tiền gói:** Cộng tiền Creator chính và tiền thực tập sinh.

$$\text{Tổng tiền gói} = 6.000.000 + 1.800.000 = 7.800.000 \text{ đồng}$$


* **Giảm giá team:** Team có 4 Creator chính (đạt điều kiện từ 4 Creator chính trở lên) nên được giảm 10% trên tổng tiền gói.

$$\text{Số tiền giảm giá} = 7.800.000 \times 10\% = 780.000 \text{ đồng}$$


$$\text{Tiền gói sau giảm} = 7.800.000 - 780.000 = 7.020.000 \text{ đồng}$$


* **Phụ thu thuê mic:** Thuê 2 bộ mic thu âm không dây với đơn giá 250.000 đồng/bộ (không áp dụng giảm giá).

$$\text{Phụ thu thuê mic} = 2 \times 250.000 = 500.000 \text{ đồng}$$


* **Tổng tiền:** Cộng tiền gói sau giảm và phụ thu thuê mic.

$$\text{Tổng tiền} = 7.020.000 + 500.000 = 7.520.000 \text{ đồng}$$



[RESULT: 7.520.000 đồng]
```

**Link trò chuyện:**https://share.gemini.google/72vxKlvvPTbI

### b) Kiểm tra kết quả AI

ĐÚNG

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{
  "loai_su_co": "sai_phong",
  "so_khach": 3,
  "so_ca_bi_anh_huong": 2,
  "tom_tat": "Khách đi team 3 người bị xếp sai phòng thiếu thiết bị livestream và bị ồn trong 2 ca thực hành."
}
```

**Link trò chuyện:**https://share.gemini.google/X2wP7pxwJgp4

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
| Tiêu chí | Điểm | Minh chứng | Đề xuất sửa |
| --- | --- | --- | --- |
| **Đúng thông tin (50%)** | 0.0 / 5.0 | **Câu bị lỗi:** "Gói TikTok Affiliate bên mình giá chỉ 1.200.000đ/người thôi..." và "Bạn báo huỷ trước 5 ngày thì được hoàn lại đủ 100% tiền nha..."<br>

<br>**Lý do sai:** Trong hồ sơ đánh giá không có dữ liệu thông tin chuẩn của trung tâm để đối chiếu xác thực mức giá và chính sách hoàn tiền khi hủy; ngoài ra câu trả lời còn gắn lời hứa hẹn thu nhập thiếu căn cứ ngay sau mức giá. | **Câu sửa đề xuất:** "Khóa học TikTok Affiliate tại trung tâm có mức học phí là [nhập mức giá chuẩn theo bảng giá trung tâm]/học viên. Về chính sách hoàn hủy, trung tâm áp dụng quy định [nhập chính sách hoàn tiền chuẩn theo quy định trung tâm]." |
| **Đầy đủ (30%)** | 0.0 / 3.0 | **Câu bị lỗi:** Không có câu nào trong phần tư vấn đề cập đến việc giải đáp đầy đủ hai câu hỏi của khách hàng hoặc mời khách hàng cung cấp thông tin đăng ký.<br>

<br>**Lý do sai:** Thiếu nội dung trả lời đầy đủ hai câu hỏi của khách hàng và không mời khách hàng cung cấp ngày đợt thực chiến cũng như số lượng suất muốn đăng ký. | **Câu sửa đề xuất:** "Để hỗ trợ anh/chị đầy đủ nhất về [nội dung câu hỏi 1] và [nội dung câu hỏi 2], trung tâm xin thông tin như sau: [nội dung giải đáp]. Anh/chị vui lòng cho biết ngày đợt thực chiến mong muốn và số lượng suất cần đăng ký để trung tâm giữ chỗ hỗ trợ mình nhé." |
| **Giọng điệu (20%)** | 0.0 / 2.0 | **Câu bị lỗi:** "Dạ hello bạn nha!"<br>

<br>**Lý do sai:** Sử dụng cách xưng hô suồng sã, thiếu tính chuyên nghiệp trong tư vấn.<br>

<br>

<br>**Câu bị lỗi:** "...đăng ký xong gắn link là nổ đơn hoa hồng trăm triệu luôn ạ."<br>

<br>**Lý do sai:** Cam kết doanh thu/hoa hồng ảo, gây hiểu lầm và thiếu khách quan.<br>

<br>

<br>**Câu bị lỗi:** "...Bạn báo huỷ trước 5 ngày thì được hoàn lại đủ 100% tiền nha, cứ chốt lẹ kẻo hết slot nè!"<br>

<br>**Lý do sai:** Dùng từ ngữ suồng sã ("nha", "chốt lẹ", "slot", "nè") và tạo áp lực thiếu chuẩn mực. | **Câu sửa đề xuất:** "Dạ chào anh/chị! Kết quả kinh doanh thực tế của học viên phụ thuộc vào năng lực triển khai, sản phẩm và chiến lược nội dung của từng cá nhân, trung tâm không cam kết mức hoa hồng cố định. Nếu anh/chị cần đăng ký tham gia, vui lòng phản hồi để trung tâm hỗ trợ chi tiết." |
| **Tổng điểm** | **0.0 / 10.0** | — | — |
```

**Link trò chuyện:**https://share.gemini.google/ac0mLr5t2nqx
