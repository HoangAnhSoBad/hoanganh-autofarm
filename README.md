# hoanganh Auto Farm · v3.11.0

Bot hỗ trợ [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/).

- [Tải ZIP máy tính](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.11.0/hoanganh-autofarm-resource-v3.11.0.zip)
- [Tải ZIP Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.11.0/hoanganh-autofarm-mobile-v3.11.0.zip)
- [Tải userscript Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.11.0/hoanganh-autofarm-mobile.user.js)

Máy tính: giải nén, mở chrome://extensions (Edge: edge://extensions), bật Developer mode, chọn Load unpacked và chọn thư mục chứa manifest.json. Tắt bản cũ để tránh hai tool cùng điều khiển; tải lại game. Nếu cập nhật cùng thư mục, bấm Reload tiện ích. Cấu hình có thể không chuyển nếu trình duyệt cấp ID tiện ích mới.

Android: dùng Firefox và Tampermonkey, nhập hoanganh-autofarm-mobile.user.js qua Utilities → Import, xác nhận nhập, bật script rồi tải lại game. Bản thử nghiệm, cần giữ màn hình và tab game mở.

[Hỗ trợ qua Facebook](https://www.facebook.com/NguyenHoangAnh.Support)

# HoangAnh Auto Farm v3.11.0

## Bond core
- Khi bảng Bond có cả chiêu sát thương và buff thuộc core, chọn chiêu sát thương trước, không phụ thuộc thứ tự nhập core.
- Khi đang dùng Bond core, giữ ô đó thay vì quay về chiêu đơn; cho phép đổi lên Bond core có nhiều thành phần hơn.
- Nếu đã thiết lập core, không tự chuyển sang Bond ngoài core. Nếu game không đưa chiêu sát thương core phù hợp, chọn phương án khả dụng để không kẹt bảng lựa chọn.

## Né boss
- Theo dõi chuyển động boss theo cả hai trục, sửa giới hạn vận tốc dọc trước đây quá thấp.
- Phát hiện boss đang lao nhanh về phía người chơi và đánh giá vùng nguy hiểm dọc quỹ đạo quan sát được để chọn hướng né.
- Khi boss nhảy vị trí lớn tới gần, không ngoại suy vận tốc sai; tạo cảnh báo tại vị trí mới trong khoảng ngắn để rút khỏi tầm cận chiến.
- Bỏ suy đoán chuyển động khi nhiều boss cùng loài không thể phân biệt chắc chắn. Giữ các chặn đường xuyên tường và né vùng báo chiêu trước đây.

## Revive đã được đồng ý bổ sung
- Nhận đúng câu hỏi hồi sinh Rift Doofcraft trong HUD tiếng Anh; chỉ gửi V/N khi có câu hỏi và đầy đủ hai lựa chọn.
- Sinh tồn: chọn dùng Revive. Farm: chọn rời Rift để giữ Revive nếu dữ liệu gần đây cho thấy boss/nguy hiểm ở sát; thiếu dữ liệu thì chọn hồi sinh.
- Dừng di chuyển trong lúc xử lý, giới hạn thử lại và chờ hộp hỏi biến mất. Không tự bấm các hộp Yes/No chung hoặc khi đang chờ người chơi khác.

## Cập nhật
Máy tính: thay tệp trong thư mục tiện ích cũ, Reload tiện ích rồi tải lại game. Android: nhập userscript mới. Giữ nguyên core và cấu hình đã lưu.

Đã qua kiểm thử logic và fixture Chrome: thứ tự Bond, giữ/nâng Bond core, cú lao dọc, thay đổi vị trí đột ngột, phân biệt boss không chắc chắn, HUD Revive hiện tại và thao tác xác nhận. Đây là phản ứng từ hình quan sát được, không biết trước vị trí dịch chuyển, không cam kết né mọi đòn hay phá đảo. Chưa đo tỷ lệ sống/thắng trên trận thực tế hoặc điện thoại thật.
