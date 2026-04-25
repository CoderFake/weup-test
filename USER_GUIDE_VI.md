# Hướng Dẫn Cấu Hình Hệ Thống

**Link demo:** [http://weup.hoangdieuit.io.vn](http://weup.hoangdieuit.io.vn)

Tài liệu hướng dẫn các bước thiết lập cơ bản để vận hành hệ thống.

---

## 1. Cài đặt API Key (Bắt buộc)
Hệ thống cần API Key của các nhà cung cấp (ChatGPT, Gemini, Anthropic) để hoạt động.

**Các bước thực hiện:**
1. Mở Cài đặt (nút **Cài đặt** trên góc màn hình / menu người dùng).
2. Chọn mục **Providers**.
3. Điền API Key vào ô tương ứng với từng nhà cung cấp (ví dụ: OpenAI, Google).
4. Bạn có thể chọn Model mặc định để sử dụng (ví dụ: `gpt-4o`).
5. Bấm **Lưu**.

---

## 2. Cấu hình Agent (Skill & Tài liệu)
Quản lý các luật dịch thuật và dữ liệu nguồn cho từng Agent (ví dụ: `translation`, `review`).

**Các bước thực hiện:**
1. Trong Cài đặt, chọn mục **Agents**.
2. Tìm Agent cần sửa và bấm biểu tượng **Sửa**. Tại đây có 2 thẻ (tab):

   - **Thẻ SKILL.md (Hướng dẫn gốc):** Chứa các lệnh, quy tắc cốt lõi bắt buộc AI làm theo.
     *Lưu ý: Viết thật ngắn gọn, rõ ý (bullet-point). Viết dài dòng sẽ khiến AI dễ bị "ảo giác" (hallucinate) làm sai lệch kết quả. Không đưa dữ liệu dài vào đây.*
     
   - **Thẻ references (Tài liệu đính kèm):** Nơi chứa nội dung (dữ liệu, bảng thuật ngữ, file mẫu) để tự động nạp (inject) cho AI đọc khi đang làm việc.
     *Lưu ý: Bất kỳ nội dung/dữ liệu dài hay ví dụ mẫu nào thì tạo file Reference ở đây, thay vì đưa vào SKILL.*
     
3. Chỉnh sửa xong nội dung, bấm **Lưu**.

---

## 3. Cấu hình Thuật ngữ (Glossary)
Khai báo các bộ từ vựng chuyên ngành để hệ thống luôn dịch đồng nhất, không bị sai lệch.

**Các bước thực hiện:**
1. Trong Cài đặt, chọn mục **Thuật ngữ** (Glossary).
2. Điền thông tin vào các ô trống:
   - **Từ khóa**: Từ gốc (tiếng Anh/nước ngoài).
   - **Nghĩa**: Nghĩa bắt buộc phải dịch sang (tiếng Việt).
3. Bấm **Lưu**.

---

## 4. Chỉnh tỷ lệ chấm điểm (Scoring)
Điều chỉnh mức độ quan trọng (trọng số) của các tiêu chí đánh giá bản dịch.

**Các bước thực hiện:**
1. Trong Cài đặt, chọn mục **Chấm điểm** (Scoring).
2. Số điểm hiện tại đang chia cho 4 tiêu chí (Độ chính xác, Trôi chảy, Văn phong, Định dạng).
3. Kéo thanh trượt để thay đổi mức độ phần trăm (%). **Lưu ý: Tổng của các thanh cộng lại phải luôn là 100%.**
4. Bấm **Lưu** để hoàn thành.
