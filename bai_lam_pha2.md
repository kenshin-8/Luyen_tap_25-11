# BÀI LÀM PHA 2 (ĐỀ LUYỆN TẬP CHỦ ĐỀ CHẠY AFFILIATE)

- **Họ tên:** Hoa Việt Hoàng
- **Lớp:** CNTT3
- **Link repository Pha2:** https://github.com/kenshin-8/Luyen_tap_25-11.git
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** ChatGPT

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đăng ký gói Affiliate ra JSON

**KET QUA AI**

```text
[\
&#x20; {\
&#x20;   "ma_goi": "TT",\
&#x20;   "ngay_bat_dau": "2026-12-20",\
&#x20;   "creator_chinh": 2,\
&#x20;   "thuc_tap_sinh": 1,\
&#x20;   "hang_tai_khoan": "thuong",\
&#x20;   "ghi_chu": null\
&#x20; },\
&#x20; {\
&#x20;   "ma_goi": "SP",\
&#x20;   "ngay_bat_dau": "2027-01-08",\
&#x20;   "creator_chinh": 3,\
&#x20;   "thuc_tap_sinh": 0,\
&#x20;   "hang_tai_khoan": "thuong",\
&#x20;   "ghi_chu": "cần ngồi bàn gần cửa ra vào"\
&#x20; },\
&#x20; {\
&#x20;   "ma_goi": "PRO",\
&#x20;   "ngay_bat_dau": null,\
&#x20;   "creator_chinh": 4,\
&#x20;   "thuc_tap_sinh": 0,\
&#x20;   "hang_tai_khoan": "vip",\
&#x20;   "ghi_chu": "cần mượn thêm đèn trợ sáng và phông xanh để quay mẫu"\
&#x20; }\
]```

**Link trò chuyện:** https://chatgpt.com/share/6b070b73-b8b8-83ec-8157-63af507a7f1f

## 4.3. Báo giá gói Affiliate bằng Chain-of-Thought

**KET QUA AI**

```text
**1. Tiền Creator chính:**

- Giá gói TT: 1.500.000 đồng/Creator.
- Số lượng: 4 Creator chính.
- Thành tiền: 4 × 1.500.000 = **6.000.000 đồng**.

**2. Tiền thực tập sinh:**

- Giá mỗi thực tập sinh: 1.500.000 × 60% = 900.000 đồng.
- Số lượng: 2 thực tập sinh (16 tuổi và 17 tuổi).
- Thành tiền: 2 × 900.000 = **1.800.000 đồng**.
- Bé 7 tuổi ngồi khu chờ, không sử dụng máy nên được miễn phí: **0 đồng**.

**3. Tổng tiền gói:**

6.000.000 + 1.800.000 + 0 = **7.800.000 đồng**.

**4. Giảm giá team:**

- Team có 4 Creator chính, đủ điều kiện giảm 10%.
- Số tiền giảm: 7.800.000 × 10% = 780.000 đồng.
- Tiền gói sau giảm: 7.800.000 − 780.000 = **7.020.000 đồng**.

**5. Phụ thu thuê mic:**

- Giá thuê: 250.000 đồng/bộ.
- Số lượng: 2 bộ.
- Phụ thu: 2 × 250.000 = **500.000 đồng**.

**6. Tổng tiền:**

7.020.000 + 500.000 = **7.520.000 đồng**.

[RESULT: 7.520.000 đồng]
```

**Link trò chuyện:** https://chatgpt.com/share/6b070bbd-820c-83ec-97ac-f7c4d4ea2c31

### b) Kiểm tra kết quả AI

Đúng

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{\
&#x20; "loai_su_co": "sai_phong",\
&#x20; "so_khach": 3,\
&#x20; "so_ca_bi_anh_huong": 2,\
&#x20; "tom_tat": "3 khách bị xếp sai phòng trong 2 ca thực hành, thiếu đèn livestream và vách cách âm; nhân viên không bị khiếu nại."\
}
```

**Link trò chuyện:** https://chatgpt.com/share/6b070c21-c168-83ec-81ef-971bc2ae8ccc

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
| Tiêu chí                    | Điểm       | Minh chứng                                                                                                                                                                                                                                                                                                                                                                                        | Đề xuất sửa                                                                                                                                                                                                |
| --------------------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Đúng thông tin (50%)** | **1/5**    | **Lỗi 1:** Trích nguyên văn: “Gói TikTok Affiliate bên mình giá chỉ 1.200.000đ/người thôi”. Lý do: Giá chuẩn là 1.500.000 đồng/Creator chính, nhân viên báo sai 300.000 đồng. **Lỗi 2:** Trích nguyên văn: “Bạn báo huỷ trước 5 ngày thì được hoàn lại đủ 100% tiền nha”. Lý do: Huỷ trước 5 ngày thuộc nhóm từ 3–6 ngày, chỉ được hoàn 50%, không phải 100%.                                     | “Gói TikTok Affiliate có giá 1.500.000 đồng/Creator chính. Nếu bạn huỷ trước ngày bắt đầu 5 ngày, trung tâm sẽ hoàn lại 50% phí đăng ký theo chính sách.”                                                  |
| **2. Đầy đủ (30%)**         | **1/3**    | **Lỗi 1:** Trích nguyên văn: “Bạn báo huỷ trước 5 ngày thì được hoàn lại đủ 100% tiền nha”. Lý do: Có trả lời câu hỏi về chính sách huỷ nhưng thông tin sai. **Lỗi 2:** Toàn bộ câu trả lời không đề cập việc mời khách cung cấp ngày đợt thực chiến và số lượng suất muốn đăng ký.                                                                                                               | Bổ sung: “Bạn vui lòng cho trung tâm biết ngày đợt thực chiến dự kiến và số lượng suất muốn đăng ký để bên mình hỗ trợ tư vấn cụ thể nhé!”                                                                 |
| **3. Giọng điệu (20%)**     | **0,5/2**  | **Lỗi 1:** Trích nguyên văn: “Dạ hello bạn nha!” Lý do: Cách chào hỏi suồng sã, thiếu tính chuyên nghiệp. **Lỗi 2:** Trích nguyên văn: “gắn link là nổ đơn hoa hồng trăm triệu luôn ạ”. Lý do: Cam kết doanh thu/hoa hồng thiếu căn cứ, dễ gây hiểu nhầm cho khách hàng. **Lỗi 3:** Trích nguyên văn: “cứ chốt lẹ kẻo hết slot nè!” Lý do: Ngôn ngữ thúc ép khách hàng, thiếu tính chuyên nghiệp. | Sử dụng lời chào lịch sự: “Dạ, trung tâm xin chào bạn!” Thay lời cam kết bằng thông tin trung lập về nội dung chương trình và cơ hội thực hành. Kết thúc bằng lời mời đăng ký nhẹ nhàng, không gây áp lực. |
| **Tổng điểm**               | **2,5/10** | **Không đạt yêu cầu.** Câu trả lời sai cả giá gói và chính sách hoàn tiền, thiếu thông tin cần thu thập và sử dụng giọng điệu chưa phù hợp.                                                                                                                                                                                                                                                       | Cần chỉnh sửa toàn bộ nội dung trước khi gửi khách hàng.                                                                                                                                                   |

**Nhận xét chung:** Nhân viên cần ưu tiên kiểm tra thông tin theo chính sách chính thức của trung tâm, tuyệt đối không tự ý đưa ra cam kết doanh thu hoặc tỷ lệ hoàn tiền sai quy định.
```

**Link trò chuyện:** https://chatgpt.com/share/6b070c4c-71d0-83ec-95bc-2d26fd345486
