# BÀI LÀM PHA 2 (ĐỀ LUYỆN TẬP CHỦ ĐỀ TÀI CHÍNH CÁ NHÂN)

- **Họ tên:**
- **Lớp:**
- **Link repository Pha2:**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đăng ký hội thảo ra JSON

**KET QUA AI**

```text
[
  {
    "ma_goi": "DT",
    "ngay_hoi_thao": "2026-12-20",
    "nguoi_lon": 2,
    "tre_em": 1,
    "hang_ve": "thuong",
    "ghi_chu": null
  },
  {
    "ma_goi": "CB",
    "ngay_hoi_thao": "2027-01-10",
    "nguoi_lon": 3,
    "tre_em": 0,
    "hang_ve": "thuong",
    "ghi_chu": "một người dùng xe lăn cần lối đi riêng"
  },
  {
    "ma_goi": "VIP",
    "ngay_hoi_thao": null,
    "nguoi_lon": 4,
    "tre_em": 0,
    "hang_ve": "vip",
    "ghi_chu": "một anh mắt kém cần ngồi bàn đầu gần màn hình chiếu"
  }
]
```

**Link trò chuyện:**https://share.gemini.google/h4fGWUcH5TJe

## 4.3. Báo giá vé hội thảo bằng Chain-of-Thought

**KET QUA AI**

```text
tiền người lớn: 4 × 1.500.000 = 6.000.000 đồng

tiền trẻ em: 2 trẻ (8 tuổi, 11 tuổi) × (50% × 1.500.000) + 1 bé (4 tuổi) × 0 = 2 × 750.000 + 0 = 1.500.000 đồng

tiền vé: 6.000.000 + 1.500.000 = 7.500.000 đồng

giảm giá nhóm: 10% × 7.500.000 = 750.000 đồng → tiền vé sau giảm: 7.500.000 − 750.000 = 6.750.000 đồng

phụ thu sổ tay: 2 × 200.000 = 400.000 đồng

tổng tiền: 6.750.000 + 400.000 = 7.150.000 đồng

[RESULT: 7.150.000 đồng]
```

**Link trò chuyện:**https://share.gemini.google/ciBdNroKSD9F

### b) Kiểm tra kết quả AI

(Ghi kết luận AI đúng hay sai; nếu sai, ghi bước sai đầu tiên và kết quả đúng của bước đó – xoá dòng này)

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
(Dán câu trả lời của AI vào đây (bấm nút Copy dưới câu trả lời) – xoá dòng này)
```

**Link trò chuyện:**

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
| Tiêu chí | Điểm | Minh chứng | Đề xuất sửa |
| --- | --- | --- | --- |
| **Đúng thông tin (50%)** | 0 / 5.0 | **1. Sai giá vé:**<br>

<br>- *Câu lỗi:* `"Vé gói Đầu Tư bên em giá chỉ 1.200.000đ/người thôi"`<br>

<br>- *Lý do sai:* Thông tin chuẩn của BTC là 1.500.000 đồng/người lớn.<br>

<br>

<br>**2. Sai chính sách huỷ vé:**<br>

<br>- *Câu lỗi:* `"Anh/chị báo huỷ trước 4 ngày thì bên em hoàn lại đủ 100% tiền vé nha"`<br>

<br>- *Lý do sai:* Theo quy định, huỷ trước 3 đến 6 ngày chỉ được hoàn 50% (mất 50% phí). | **1. Sửa giá vé:**<br>

<br>"Giá vé gói Đầu Tư (DT) là 1.500.000 đồng/người lớn ạ."<br>

<br>

<br>**2. Sửa chính sách huỷ vé:**<br>

<br>"Nếu anh/chị báo huỷ trước ngày hội thảo 4 ngày (thuộc mốc từ 3 đến 6 ngày), ban tổ chức sẽ hoàn lại 50% giá trị vé ạ." |
| **Đầy đủ (30%)** | 2.0 / 3.0 | **Thiếu bước khai thác nhu cầu khách hàng:**<br>

<br>- *Câu lỗi:* Toàn bộ nội dung bài làm đã đề cập đủ 2 ý hỏi (giá vé, chính sách huỷ) nhưng bỏ sót lời mời cung cấp thông tin đăng ký.<br>

<br>- *Lý do sai:* Chưa mời khách hàng cung cấp ngày hội thảo cụ thể và số lượng vé muốn đăng ký. | **Bổ sung câu mời thông tin:**<br>

<br>"Anh/chị vui lòng cho em biết ngày hội thảo cụ thể muốn tham gia và số lượng vé dự kiến đăng ký để em hỗ trợ giữ chỗ tốt nhất nhé ạ." |
| **Giọng điệu (20%)** | 0.5 / 2.0 | **1. Từ ngữ suồng sã:**<br>

<br>- *Câu lỗi:* `"Dạ chào anh/chị nha!"`, `"tiền vé nha, cứ yên tâm chốt đơn đi ạ!"`<br>

<br>- *Lý do sai:* Sử dụng từ "nha", "chốt đơn" thiếu tính chuyên nghiệp trong tư vấn hội thảo tài chính.<br>

<br>

<br>**2. Hứa hẹn lợi nhuận quá đà:**<br>

<br>- *Câu lỗi:* `"đi học về đầu tư chứng khoán lời khủng luôn ạ."`<br>

<br>- *Lý do sai:* Cam kết, thổi phồng lợi nhuận đầu tư sai quy chuẩn tư vấn. | **Điều chỉnh lời chào, kết câu và bỏ cam kết lợi nhuận:**<br>

<br>"Dạ xin chào anh/chị. Khoá học sẽ cung cấp kiến thức và phương pháp đầu tư chứng khoán bài bản, thực tế ạ. Anh/chị có thể yên tâm cân nhắc và đăng ký tham gia chương trình ạ." |
| **TỔNG ĐIỂM** | **2.5 / 10** |  |  |
```

**Link trò chuyện:** https://share.gemini.google/csPzP6KysgcH
