# hoanganh Auto Farm · v3.12.0

Bot hỗ trợ [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/).

- [Tải ZIP máy tính](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.12.0/hoanganh-autofarm-resource-v3.12.0.zip)
- [Tải ZIP Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.12.0/hoanganh-autofarm-mobile-v3.12.0.zip)
- [Tải userscript Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.12.0/hoanganh-autofarm-mobile.user.js)

Máy tính: giải nén, mở chrome://extensions (Edge: edge://extensions), bật Developer mode, chọn Load unpacked và chọn thư mục chứa manifest.json. Tắt bản cũ để tránh hai tool cùng điều khiển; tải lại game. Nếu cập nhật cùng thư mục, bấm Reload tiện ích. Cấu hình có thể không chuyển nếu trình duyệt cấp ID tiện ích mới.

Android: dùng Firefox và Tampermonkey, nhập hoanganh-autofarm-mobile.user.js qua Utilities → Import, xác nhận nhập, bật script rồi tải lại game. Bản thử nghiệm, cần giữ màn hình và tab game mở.

[Hỗ trợ qua Facebook](https://www.facebook.com/NguyenHoangAnh.Support)

# HoangAnh Auto Farm v3.12.0

## Auto Roll theo gen
- Mở Gacha trong game, Dừng phiên farm, vào tab Auto Roll → Đọc danh sách gen → chọn gen/khu vực và số lượt tối đa → Bắt đầu roll.
- Giới hạn tính theo số Pokémon nhận được, không phải số lần bấm. Ví dụ 20 lượt = hai gói ×10.
- Dùng vé ×10 trước, rồi vé thường. Doofcraft có thể roll đơn cho phần dư; giao diện bản gốc được hỗ trợ chỉ có gói ×10 nên dừng khi còn dưới 10 lượt. Không dùng vé rainbow, đá quý, Wish hoặc tự mua vé.
- Chờ đúng gen được chọn, chờ bảng kết quả đủ số Pokémon rồi mới tính tiến độ và roll tiếp. Dừng khi đạt giới hạn, không có nút roll phù hợp khả dụng, rời Gacha, đổi gen hoặc bạn tương tác với game.
- Không chạy cùng phiên farm; không tự tiếp tục sau tải lại trang. Khi phản hồi mất/quá 30 giây, dừng để kiểm tra thay vì bấm mua lần nữa. Lượt đã gửi trước khi bấm Dừng có thể vẫn được game xử lý.

## Donate
- Tab Donate hiển thị nguyên ảnh QR công khai do tác giả cung cấp, đóng gói trong tool.
- Techcombank · NGUYEN HOANG ANH · 207207666666.
- “Sự ủng hộ của bạn là động lực để mình tiếp tục phát triển và cải thiện tool. Cảm ơn bạn!”

## Cập nhật
Máy tính: thay tệp trong thư mục tiện ích cũ, Reload tiện ích và tải lại game. Android: nhập userscript mới vào Tampermonkey rồi tải lại game. Giữ core/cấu hình farm cũ.

Đã kiểm thử bằng giao diện mô phỏng hai bản game: chọn gen, giới hạn 11 lượt, kết quả chậm/mất, tránh roll trùng, không chạy cùng farm, và kiểm thử hồi quy farm. Chưa thực hiện roll bằng vé tài khoản thật hoặc kiểm tra trên điện thoại thật.
