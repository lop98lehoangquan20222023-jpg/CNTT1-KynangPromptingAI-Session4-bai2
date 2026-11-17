# Bước 1: Đề xuất 2 Prompt mẫu
1. Giải pháp 1 (Đơn giản, ngắn gọn):
```
"Hãy phân loại mức độ nghiêm trọng (P1/P2/P3), tìm nguyên nhân và viết email xin lỗi cho danh sách phản hồi khách hàng sau: [Chèn dữ liệu]."
```

2. Giải pháp 2 (Chi tiết, cấu trúc hóa và nhiều ràng buộc):
```
Bạn là chuyên gia CSKH. Hãy xử lý danh sách phản hồi khách hàng theo 3 bước:
1. Đọc phản hồi của khách hàng và phân tích cảm xúc của khách hàng.
2. Đề xuất biện pháp giải quyết phản hồi của khách hàng.
3. Soạn 1 email gửi khách hàng dưới 150 từ đề xuất cách giải quyết vấn đề của khách hàng.
Quy định bắt buộc:
- Chỉ giải quyết 3 khách hàng mỗi lượt.Sau khi làm xong in ra:Đã làm tới khách hàng số: 
```
# Bước 2:
| Tiêu chí | Giải pháp 1 (Đơn giản) | Giải pháp 2 (Chi tiết) |
| :--- | :--- | :--- |
| **Độ dễ hiểu** | Cao | Trung bình |
| **Tốn token** | Ít | Nhiều hơn |
| **Chặn lỗi biên** | Trung bình | Cực tốt |
# Bước 3:
Lựa chọn phương án: Giải pháp 2 (Chi tiết, có nhiều ràng buộc).

Lý do lựa chọn: Giúp kiểm soát chặt chẽ quy trình suy luận của mô hình.
## Kết quả
```
Khách hàng số 1
Phản hồi: "Hàng Quá Hạn Sử Dụng"

Bước 1: Phân tích cảm xúc

Cảm xúc: Bực bội, thất vọng và lo lắng về vấn đề vệ sinh an toàn thực phẩm.

Bước 2: Đề xuất biện pháp giải quyết

Xin lỗi khách hàng vì sơ suất trong khâu kiểm tra hạn sử dụng trước khi xuất kho.

Đổi ngay sản phẩm mới có hạn sử dụng xa nhất (miễn phí vận chuyển) hoặc hoàn tiền 100%.

Tặng kèm voucher giảm giá cho lần mua tiếp theo để xoa dịu khách hàng.

Bước 3: Email gửi khách hàng

Tiêu đề: Thành thật xin lỗi và hỗ trợ đổi trả sản phẩm quá hạn sử dụng

Chào anh/chị,

Cửa hàng thành thật xin lỗi vì sơ suất để anh/chị nhận phải sản phẩm đã quá hạn sử dụng.

Để khắc phục, chúng tôi xin đổi ngay sản phẩm mới (miễn phí vận chuyển) hoặc hoàn tiền 100% tùy theo mong muốn của anh/chị. Cửa hàng cũng xin gửi tặng mã giảm giá 15% cho đơn hàng tiếp theo thay lời tạ lỗi.

Anh/chị vui lòng phản hồi lại email này phương án thuận tiện nhất để chúng tôi hỗ trợ ngay lập tức ạ.

Trân trọng,

Bộ phận Chăm sóc Khách hàng.

Khách hàng số 2
Phản hồi: "Ăn không như quảng cáo"

Bước 1: Phân tích cảm xúc

Cảm xúc: Hụt hẫng, mất niềm tin và cảm thấy bị lừa dối vì trải nghiệm thực tế kém xa kỳ vọng.

Bước 2: Đề xuất biện pháp giải quyết

Lắng nghe, ghi nhận đóng góp của khách hàng về hương vị/chất lượng món ăn.

Hỏi thăm chi tiết điểm chưa hài lòng (ví dụ: món bị nguội, mặn/nhạt, hay khẩu phần ít) để cải thiện bếp.

Tặng voucher giảm giá hoặc tặng kèm món miễn phí cho lần đặt sau để khách hàng có cơ hội trải nghiệm lại.

Bước 3: Email gửi khách hàng

Tiêu đề: Cảm ơn đóng góp và gửi tặng ưu đãi trải nghiệm lại dịch vụ

Chào anh/chị,

Cửa hàng rất tiếc khi hương vị món ăn chưa làm anh/chị hài lòng như kỳ vọng. Chúng tôi luôn trân trọng mọi góp ý để cải thiện chất lượng bếp mỗi ngày.

Nếu tiện, anh/chị có thể chia sẻ thêm điểm chưa ưng ý để cửa hàng rút kinh nghiệm nhé. Thay lời cảm ơn, chúng tôi xin gửi tặng anh/chị mã giảm giá 20% cho đơn hàng tới để có cơ hội phục vụ anh/chị chu đáo hơn.

Rất mong được đón tiếp anh/chị trong thời gian tới!

Trân trọng,

Bộ phận Chăm sóc Khách hàng.

Khách hàng số 3
Phản hồi: "Tôi đặt hàng online giao trễ 30p"

Bước 1: Phân tích cảm xúc

Cảm xúc: Sốt ruột, khó chịu và bực mình vì bị ảnh hưởng đến thời gian ăn uống/công việc cá nhân.

Bước 2: Đề xuất biện pháp giải quyết

Xin lỗi chân thành vì sự chậm trễ làm ảnh hưởng đến lịch trình của khách.

Giải thích ngắn gọn nguyên nhân khách quan (tắc đường, quá tải đơn giờ cao điểm) mà không đổ lỗi.

Hoàn lại phí vận chuyển của đơn hàng này hoặc tặng mã miễn phí giao hàng (Freeship) cho đơn hàng sau.

Bước 3: Email gửi khách hàng

Tiêu đề: Xin lỗi về sự chậm trễ giao hàng và quà tặng tri ân

Chào anh/chị,

Cửa hàng thành thật xin lỗi vì đơn hàng online của anh/chị đã bị giao trễ 30 phút so với dự kiến, làm ảnh hưởng đến thời gian của anh/chị.

Do lượng đơn giờ cao điểm tăng đột biến nên khâu vận chuyển chưa đảm bảo tiến độ. Để tạ lỗi, chúng tôi xin gửi tặng anh/chị mã miễn phí giao hàng (Freeship) kèm ưu đãi giảm 10% cho đơn hàng tiếp theo.

Rất mong anh/chị thông cảm và tiếp tục ủng hộ cửa hàng ạ!

Trân trọng,

Bộ phận Chăm sóc Khách hàng.

Đã làm tới khách hàng số: 3
```
