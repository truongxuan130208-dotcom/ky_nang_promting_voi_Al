# BÀI LÀM PHA 2 (ĐỀ LUYỆN TẬP CHỦ ĐỀ CHẠY AFFILIATE)

- **Họ tên:phạm xuân trường**
- **Lớp:cntt3**
- **Link repository Pha2:https://github.com/truongxuan130208-dotcom/ky_nang_promting_voi_Al/blob/1df2daea04d68538c8541a8fce01da6da94dd91c/bai_lam_pha2.md**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):gemini**

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
    "hang_tai_khoan": null,
    "ghi_chu": "ngồi bàn gần cửa ra vào"
  },
  {
    "ma_goi": "PRO",
    "ngay_bat_dau": null,
    "creator_chinh": 4,
    "thuc_tap_sinh": 0,
    "hang_tai_khoan": "vip",
    "ghi_chu": "mượn thêm đèn trợ sáng và phông xanh để quay mẫu"
  }
]
```

**Link trò chuyện:https://share.gemini.google/Ir7ZSLwIYqcg**

## 4.3. Báo giá gói Affiliate bằng Chain-of-Thought

**KET QUA AI**

```text
1. **Tiền Creator chính:** $4 \times 1.500.000 = 6.000.000\text{ đồng}$
2. **Tiền thực tập sinh:** $2 \times (1.500.000 \times 60\%) = 2 \times 900.000 = 1.800.000\text{ đồng}$ (bé 7 tuổi dưới 15 tuổi ngồi khu chờ được miễn phí: $0\text{ đồng}$)
3. **Tổng tiền gói:** $6.000.000 + 1.800.000 = 7.800.000\text{ đồng}$
4. **Giảm giá team:** $7.800.000 \times 10\% = 780.000\text{ đồng}$ (tiền gói sau giảm: $7.800.000 - 780.000 = 7.020.000\text{ đồng}$)
5. **Phụ thu thuê mic:** $2 \times 250.000 = 500.000\text{ đồng}$
6. **Tổng tiền:** $7.020.000 + 500.000 = 7.520.000\text{ đồng}$

[RESULT: 7.520.000 đồng]
```

**Link trò chuyện:https://share.gemini.google/0awywpR88ppH**

### b) Kiểm tra kết quả AI

kết luận của Al đã đúng

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{
  "loai_su_co": "sai_phong",
  "so_khach": 3,
  "so_ca_bi_anh_huong": 2,
  "tom_tat": "Khách nhóm 3 người bị xếp phòng thường thiếu đèn livestream và cách âm trong 2 ca thực hành."
}
```

**Link trò chuyện:https://share.gemini.google/i9OsnUg2On5G**

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
| Tiêu chí | Điểm | Minh chứng | Đề xuất sửa |
| --- | --- | --- | --- |
| **Đúng thông tin (50%)** | 0 / 5.0 | **Lỗi 1:** *"Gói TikTok Affiliate bên mình giá chỉ 1.200.000đ/người thôi"* (Sai giá chuẩn 1.500.000 đồng/Creator chính).<br>

<br>**Lỗi 2:** *"Bạn báo huỷ trước 5 ngày thì được hoàn lại đủ 100% tiền nha"* (Sai chính sách: huỷ trước 3–6 ngày chỉ hoàn 50%, không phải 100%). | *"Gói TikTok Affiliate bên mình có mức phí là 1.500.000 đồng/Creator chính ạ. Về chính sách huỷ đăng ký, nếu bạn báo huỷ trước ngày bắt đầu 5 ngày (nằm trong khoảng từ 3 đến 6 ngày), trung tâm sẽ hoàn lại 50% học phí ạ."* |
| **Đầy đủ (30%)** | 1.5 / 3.0 | **Đạt:** Đã trả lời cả hai câu hỏi về giá và chính sách huỷ của khách hàng.<br>

<br>**Lỗi thiếu thông tin:** Thiếu phần mời khách hàng cung cấp ngày đợt thực chiến và số lượng suất muốn đăng ký. | Bổ sung vào cuối câu trả lời: *"Bạn dự định tham gia đợt thực chiến vào ngày nào và muốn đăng ký bao nhiêu suất để mình hỗ trợ giữ chỗ cho bạn nhé?"* |
| **Giọng điệu (20%)** | 0 / 2.0 | **Lỗi 1:** *"Dạ hello bạn nha!"*, *"cứ chốt lẹ kẻo hết slot nè!"* (Sử dụng từ ngữ suồng sã, thiếu tính chuyên nghiệp).<br>

<br>**Lỗi 2:** *"đăng ký xong gắn link là nổ đơn hoa hồng trăm triệu luôn ạ."* (Cam kết doanh thu/hoa hồng ảo). | Thay bằng giọng điệu lịch sự, thực tế: *"Dạ chào bạn ạ!"*, bỏ cam kết thu nhập ảo và đổi lời kêu gọi thành: *"Bạn vui lòng phản hồi sớm để bên mình hỗ trợ hoàn tất thủ tục đăng ký cho bạn nhé."* |
| **Tổng điểm** | **1.5 / 10** |  |  |
```

**Link trò chuyện:**
https://share.gemini.google/tvjQfsYAXRmT
